# Comparing `tmp/simubox-0.2.3.tar.gz` & `tmp/simubox-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simubox-0.2.3.tar", max compression
+gzip compressed data, was "simubox-0.2.4.tar", max compression
```

## Comparing `simubox-0.2.3.tar` & `simubox-0.2.4.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.3/LICENSE
--rw-r--r--   0        0        0     1306 2024-04-08 13:52:19.103630 simubox-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.3/README.md
--rw-r--r--   0        0        0      120 2024-04-06 14:56:53.385803 simubox-0.2.3/SimuBox/__init__.py
--rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.3/SimuBox/artist/__init__.py
--rw-r--r--   0        0        0    11866 2024-04-06 14:56:53.391791 simubox-0.2.3/SimuBox/artist/compare.py
--rw-r--r--   0        0        0     7516 2024-04-06 14:56:53.403311 simubox-0.2.3/SimuBox/artist/isosurface.py
--rw-r--r--   0        0        0     9898 2024-04-06 14:56:53.407312 simubox-0.2.3/SimuBox/artist/landscape.py
--rw-r--r--   0        0        0    23670 2024-04-06 14:56:53.397800 simubox-0.2.3/SimuBox/artist/phase.py
--rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.3/SimuBox/artist/plotter.py
--rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.3/SimuBox/calculator/__init__.py
--rw-r--r--   0        0        0     4478 2024-04-03 10:55:55.752589 simubox-0.2.3/SimuBox/calculator/peak.py
--rw-r--r--   0        0        0     5484 2024-04-06 14:56:53.416335 simubox-0.2.3/SimuBox/calculator/scatter.py
--rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.3/SimuBox/calculator/topo.py
--rw-r--r--   0        0        0    11280 2024-04-06 14:56:53.412310 simubox-0.2.3/SimuBox/calculator/voronoi.py
--rw-r--r--   0        0        0       70 2024-04-03 10:11:34.170669 simubox-0.2.3/SimuBox/runner/__init__.py
--rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.3/SimuBox/runner/agents/__init__.py
--rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.3/SimuBox/runner/agents/ABC.py
--rw-r--r--   0        0        0     5250 2024-04-03 10:14:35.582991 simubox-0.2.3/SimuBox/runner/agents/ABC_ABC.py
--rw-r--r--   0        0        0     4707 2024-04-03 10:15:02.275022 simubox-0.2.3/SimuBox/runner/agents/BABCB.py
--rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.3/SimuBox/runner/agents/Mask_AB_A.py
--rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.3/SimuBox/runner/agents/Mask_AB_AB.py
--rw-r--r--   0        0        0     2125 2024-04-03 10:11:34.173663 simubox-0.2.3/SimuBox/runner/agents/MixinModel.py
--rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.3/SimuBox/runner/manager.py
--rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.3/SimuBox/runner/phases.py
--rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.3/SimuBox/schema/__init__.py
--rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.3/SimuBox/schema/enums/__init__.py
--rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.3/SimuBox/schema/enums/MixinEnums.py
--rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.3/SimuBox/schema/enums/Modes.py
--rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.3/SimuBox/schema/enums/OtherEnums.py
--rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.3/SimuBox/schema/enums/SCFTEnums.py
--rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.3/SimuBox/schema/labels.py
--rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.3/SimuBox/schema/structs/__init__.py
--rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.3/SimuBox/schema/structs/ChartElement.py
--rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.3/SimuBox/schema/structs/ComputedRes.py
--rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.3/SimuBox/schema/structs/DataFile.py
--rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.3/SimuBox/schema/structs/MixinStructs.py
--rw-r--r--   0        0        0      724 2024-04-03 13:53:56.680819 simubox-0.2.3/SimuBox/schema/structs/OtherStructs.py
--rw-r--r--   0        0        0     1428 2024-04-04 09:02:53.467218 simubox-0.2.3/SimuBox/schema/structs/SCFTStructs.py
--rw-r--r--   0        0        0      395 2024-04-03 11:46:43.830219 simubox-0.2.3/SimuBox/schema/types.py
--rw-r--r--   0        0        0    10336 2024-04-08 13:48:36.367296 simubox-0.2.3/SimuBox/script/extractor.py
--rw-r--r--   0        0        0      814 2024-04-06 15:48:07.272692 simubox-0.2.3/SimuBox/script/help.py
--rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.3/SimuBox/script/JSON/ABC_ABC.json
--rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.3/SimuBox/script/JSON/BABCB.json
--rw-r--r--   0        0        0      661 2024-04-04 10:29:51.574406 simubox-0.2.3/SimuBox/script/push_job.py
--rw-r--r--   0        0        0     1655 2024-04-06 15:49:41.998603 simubox-0.2.3/SimuBox/script/setenv.py
--rw-r--r--   0        0        0      848 2024-04-06 15:09:04.736704 simubox-0.2.3/SimuBox/script/web.py
--rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.3/SimuBox/toolkit/__init__.py
--rw-r--r--   0        0        0     3786 2024-04-03 13:52:28.451854 simubox-0.2.3/SimuBox/toolkit/function.py
--rw-r--r--   0        0        0    12058 2024-04-03 12:27:05.411475 simubox-0.2.3/SimuBox/toolkit/reader.py
--rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.3/SimuBox/toolkit/vector.py
--rw-r--r--   0        0        0     5008 2024-04-03 03:44:10.626375 simubox-0.2.3/SimuBox/toolkit/xmltrans.py
--rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.3/SimuBox/web/Homepage.py
--rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.3/SimuBox/web/pages/1_Structure.py
--rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.3/SimuBox/web/pages/2_Scatter.py
--rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.3/SimuBox/web/pages/3_Voronoi.py
--rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.3/SimuBox/web/pages/4_Curve.py
--rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.3/SimuBox/web/pages/5_Peaks.py
--rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.3/SimuBox/web/pages/6_Topology.py
--rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.3/SimuBox/web/pages/7_Landscape.py
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 simubox-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1306 2024-04-10 08:08:08.535139 simubox-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.4/README.md
+-rw-r--r--   0        0        0      120 2024-04-06 14:56:53.385803 simubox-0.2.4/SimuBox/__init__.py
+-rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.4/SimuBox/artist/__init__.py
+-rw-r--r--   0        0        0    11866 2024-04-06 14:56:53.391791 simubox-0.2.4/SimuBox/artist/compare.py
+-rw-r--r--   0        0        0     7516 2024-04-06 14:56:53.403311 simubox-0.2.4/SimuBox/artist/isosurface.py
+-rw-r--r--   0        0        0     9898 2024-04-06 14:56:53.407312 simubox-0.2.4/SimuBox/artist/landscape.py
+-rw-r--r--   0        0        0    23670 2024-04-06 14:56:53.397800 simubox-0.2.4/SimuBox/artist/phase.py
+-rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.4/SimuBox/artist/plotter.py
+-rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.4/SimuBox/calculator/__init__.py
+-rw-r--r--   0        0        0     4478 2024-04-03 10:55:55.752589 simubox-0.2.4/SimuBox/calculator/peak.py
+-rw-r--r--   0        0        0     5484 2024-04-06 14:56:53.416335 simubox-0.2.4/SimuBox/calculator/scatter.py
+-rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.4/SimuBox/calculator/topo.py
+-rw-r--r--   0        0        0    11280 2024-04-06 14:56:53.412310 simubox-0.2.4/SimuBox/calculator/voronoi.py
+-rw-r--r--   0        0        0       70 2024-04-03 10:11:34.170669 simubox-0.2.4/SimuBox/runner/__init__.py
+-rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.4/SimuBox/runner/agents/__init__.py
+-rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.4/SimuBox/runner/agents/ABC.py
+-rw-r--r--   0        0        0     5250 2024-04-03 10:14:35.582991 simubox-0.2.4/SimuBox/runner/agents/ABC_ABC.py
+-rw-r--r--   0        0        0     4707 2024-04-03 10:15:02.275022 simubox-0.2.4/SimuBox/runner/agents/BABCB.py
+-rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.4/SimuBox/runner/agents/Mask_AB_A.py
+-rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.4/SimuBox/runner/agents/Mask_AB_AB.py
+-rw-r--r--   0        0        0     2125 2024-04-03 10:11:34.173663 simubox-0.2.4/SimuBox/runner/agents/MixinModel.py
+-rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.4/SimuBox/runner/manager.py
+-rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.4/SimuBox/runner/phases.py
+-rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.4/SimuBox/schema/__init__.py
+-rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.4/SimuBox/schema/enums/__init__.py
+-rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.4/SimuBox/schema/enums/MixinEnums.py
+-rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.4/SimuBox/schema/enums/Modes.py
+-rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.4/SimuBox/schema/enums/OtherEnums.py
+-rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.4/SimuBox/schema/enums/SCFTEnums.py
+-rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.4/SimuBox/schema/labels.py
+-rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.4/SimuBox/schema/structs/__init__.py
+-rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.4/SimuBox/schema/structs/ChartElement.py
+-rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.4/SimuBox/schema/structs/ComputedRes.py
+-rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.4/SimuBox/schema/structs/DataFile.py
+-rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.4/SimuBox/schema/structs/MixinStructs.py
+-rw-r--r--   0        0        0      724 2024-04-03 13:53:56.680819 simubox-0.2.4/SimuBox/schema/structs/OtherStructs.py
+-rw-r--r--   0        0        0     1428 2024-04-04 09:02:53.467218 simubox-0.2.4/SimuBox/schema/structs/SCFTStructs.py
+-rw-r--r--   0        0        0      395 2024-04-03 11:46:43.830219 simubox-0.2.4/SimuBox/schema/types.py
+-rw-r--r--   0        0        0    10456 2024-04-10 06:16:33.540045 simubox-0.2.4/SimuBox/script/extractor.py
+-rw-r--r--   0        0        0      814 2024-04-06 15:48:07.272692 simubox-0.2.4/SimuBox/script/help.py
+-rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.4/SimuBox/script/JSON/ABC_ABC.json
+-rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.4/SimuBox/script/JSON/BABCB.json
+-rw-r--r--   0        0        0      661 2024-04-04 10:29:51.574406 simubox-0.2.4/SimuBox/script/push_job.py
+-rw-r--r--   0        0        0     1655 2024-04-06 15:49:41.998603 simubox-0.2.4/SimuBox/script/setenv.py
+-rw-r--r--   0        0        0     2077 2024-04-10 07:44:46.666366 simubox-0.2.4/SimuBox/script/stress.py
+-rw-r--r--   0        0        0     2239 2024-02-24 14:13:39.180781 simubox-0.2.4/SimuBox/script/transform_case.py
+-rw-r--r--   0        0        0      848 2024-04-06 15:09:04.736704 simubox-0.2.4/SimuBox/script/web.py
+-rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.4/SimuBox/toolkit/__init__.py
+-rw-r--r--   0        0        0     3786 2024-04-03 13:52:28.451854 simubox-0.2.4/SimuBox/toolkit/function.py
+-rw-r--r--   0        0        0    12177 2024-04-10 06:38:47.446541 simubox-0.2.4/SimuBox/toolkit/reader.py
+-rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.4/SimuBox/toolkit/vector.py
+-rw-r--r--   0        0        0     5008 2024-04-03 03:44:10.626375 simubox-0.2.4/SimuBox/toolkit/xmltrans.py
+-rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.4/SimuBox/web/Homepage.py
+-rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.4/SimuBox/web/pages/1_Structure.py
+-rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.4/SimuBox/web/pages/2_Scatter.py
+-rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.4/SimuBox/web/pages/3_Voronoi.py
+-rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.4/SimuBox/web/pages/4_Curve.py
+-rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.4/SimuBox/web/pages/5_Peaks.py
+-rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.4/SimuBox/web/pages/6_Topology.py
+-rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.4/SimuBox/web/pages/7_Landscape.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 simubox-0.2.4/PKG-INFO
```

### Comparing `simubox-0.2.3/LICENSE` & `simubox-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/pyproject.toml` & `simubox-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimuBox"
-version = "0.2.3"
+version = "0.2.4"
 description = "Free python package to do some science calculation."
 authors = ["Alkaid Yuan <kryuan@qq.com>"]
 maintainers = ["Alkaid Yuan <kryuan@qq.com>"]
 license = "./LICENSE"
 readme = "./README.md"
 repository  = "https://github.com/KangruiYuan/SimuBox"
 homepage = "https://pypi.org/project/SimuBox/"
```

### Comparing `simubox-0.2.3/README.md` & `simubox-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/artist/compare.py` & `simubox-0.2.4/SimuBox/artist/compare.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/artist/isosurface.py` & `simubox-0.2.4/SimuBox/artist/isosurface.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/artist/landscape.py` & `simubox-0.2.4/SimuBox/artist/landscape.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/artist/phase.py` & `simubox-0.2.4/SimuBox/artist/phase.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/artist/plotter.py` & `simubox-0.2.4/SimuBox/artist/plotter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/calculator/peak.py` & `simubox-0.2.4/SimuBox/calculator/peak.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/calculator/scatter.py` & `simubox-0.2.4/SimuBox/calculator/scatter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/calculator/topo.py` & `simubox-0.2.4/SimuBox/calculator/topo.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/calculator/voronoi.py` & `simubox-0.2.4/SimuBox/calculator/voronoi.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/ABC.py` & `simubox-0.2.4/SimuBox/runner/agents/ABC.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/ABC_ABC.py` & `simubox-0.2.4/SimuBox/runner/agents/ABC_ABC.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/BABCB.py` & `simubox-0.2.4/SimuBox/runner/agents/BABCB.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/Mask_AB_A.py` & `simubox-0.2.4/SimuBox/runner/agents/Mask_AB_A.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/Mask_AB_AB.py` & `simubox-0.2.4/SimuBox/runner/agents/Mask_AB_AB.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/agents/MixinModel.py` & `simubox-0.2.4/SimuBox/runner/agents/MixinModel.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/manager.py` & `simubox-0.2.4/SimuBox/runner/manager.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/runner/phases.py` & `simubox-0.2.4/SimuBox/runner/phases.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/enums/MixinEnums.py` & `simubox-0.2.4/SimuBox/schema/enums/MixinEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/enums/Modes.py` & `simubox-0.2.4/SimuBox/schema/enums/Modes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/enums/OtherEnums.py` & `simubox-0.2.4/SimuBox/schema/enums/OtherEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/enums/SCFTEnums.py` & `simubox-0.2.4/SimuBox/schema/enums/SCFTEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/labels.py` & `simubox-0.2.4/SimuBox/schema/labels.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/ChartElement.py` & `simubox-0.2.4/SimuBox/schema/structs/ChartElement.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/ComputedRes.py` & `simubox-0.2.4/SimuBox/schema/structs/ComputedRes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/DataFile.py` & `simubox-0.2.4/SimuBox/schema/structs/DataFile.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/MixinStructs.py` & `simubox-0.2.4/SimuBox/schema/structs/MixinStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/OtherStructs.py` & `simubox-0.2.4/SimuBox/schema/structs/OtherStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/schema/structs/SCFTStructs.py` & `simubox-0.2.4/SimuBox/schema/structs/SCFTStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/extractor.py` & `simubox-0.2.4/SimuBox/script/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 import subprocess as sp
 from collections import OrderedDict, defaultdict
 from itertools import combinations
 from pathlib import Path
 from typing import Any, Union, Sequence
 from tqdm import tqdm
-from ..schema.structs.SCFTStructs import Options as opts
+from SimuBox import Options as opts
 
 
 def check_files(files: list[Union[str, Path]]):
     for file in files:
         if not os.path.isfile(file):
             print(f"Absent: {file}".center(50, "*"))
             return False
@@ -30,15 +30,15 @@
 
     if round(res["freeE_dis"] - res["freeE"], 3) == 0:
         res["phase"] = "Disorder"
 
     if (res["server"] == "cpu" and res["target_comp"] < res["CompMax"]) or (
         res["server"] == "gpu" and res["target_comp"] * 1e3 < res["CompMax"]
     ):
-        print("CompMax not satisfied")
+        print("不可压缩性条件尚未满足。")
         return False
     else:
         return True
 
 
 def stats_component(inputs: dict):
     total_stats = {}
@@ -97,15 +97,15 @@
             json_data = json.load(fp, object_pairs_hook=OrderedDict)
 
         data = {}
         scripts = json_data.get("Scripts", {})
         data.update(scripts)
         stats_res = stats_component(json_data)
         data.update(stats_res)
-        server_before = scripts.get("cal_type", "cpu")
+        server_before = scripts.get("cal_type") or args.read
         data["server"] = server_before
         data["target_comp"] = json_data["Iteration"]["IncompressibilityTarget"]
         if server_before == "cpu":
             popen_freeE_MaxC = sp.Popen(
                 cmd_freeE_MaxC, shell=True, stdout=sp.PIPE, stderr=sp.PIPE
             )
             popen_freeE_MaxC.wait()
@@ -253,28 +253,29 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-n", "--name", default="", type=str)
     parser.add_argument("-t", "--terminal", default="WORKING_DIR", type=str)
     parser.add_argument("-s", "--server", default="", type=str)
     parser.add_argument("-a", "--all", action="store_true", default=False)
+    parser.add_argument("-r", "--read", default="cpu", type=str)
+    parser.add_argument('-e', "--exclude", nargs='*', default=["Density", "old"])
     args = parser.parse_args()
 
-    exclude = ("Density", "old")
     cmd_lxlylz = "tail -3 printout.txt | head -1"
     cmd_freeE_MaxC = "tail -1 printout.txt | head -1"
     lxlylz_re = re.compile("[.0-9]+(?!e)")
     freeE_re = re.compile("[.0-9e+-]+")
 
     parent_folder = Path.cwd()
     working_directory = parent_folder / args.terminal
     subdirectories = [
         item
         for item in working_directory.iterdir()
-        if item.is_dir() and item.stem not in exclude
+        if item.is_dir() and item.stem not in args.exclude
     ]
 
     output_csv_name = args.name or parent_folder.name
     output_csv_path = parent_folder / output_csv_name
     if output_csv_path.suffix != ".csv":
         output_csv_path = str(output_csv_path) + ".csv"
```

### Comparing `simubox-0.2.3/SimuBox/script/help.py` & `simubox-0.2.4/SimuBox/script/help.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/JSON/ABC_ABC.json` & `simubox-0.2.4/SimuBox/script/JSON/ABC_ABC.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/JSON/BABCB.json` & `simubox-0.2.4/SimuBox/script/JSON/BABCB.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/push_job.py` & `simubox-0.2.4/SimuBox/script/push_job.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/setenv.py` & `simubox-0.2.4/SimuBox/script/setenv.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/script/web.py` & `simubox-0.2.4/SimuBox/script/web.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/toolkit/function.py` & `simubox-0.2.4/SimuBox/toolkit/function.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/toolkit/reader.py` & `simubox-0.2.4/SimuBox/toolkit/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,18 @@
     def _validate(vec: np.ndarray):
         return any(vec > 1000) or any(vec <= 0)
 
     skip = 0
     offset = 0
     if parse_N:
         if text:
-            NxNyNz = np.array(list(map(int, content[skip].strip().split(" "))))
+            NxNyNz = list(map(int, content[skip].strip().split(" ")))
+            if len(NxNyNz) < 3:
+                NxNyNz = [1]*(3 - len(NxNyNz)) + NxNyNz
+            NxNyNz = np.array(NxNyNz)
         else:
             # int32 for scft
             NxNyNz = bin_read_function(content, dtype=np.int32, count=3)
             if _validate(NxNyNz):
                 # int64 for tops
                 NxNyNz = bin_read_function(content, dtype=np.int64, count=3)
                 if _validate(NxNyNz):
```

### Comparing `simubox-0.2.3/SimuBox/toolkit/vector.py` & `simubox-0.2.4/SimuBox/toolkit/vector.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/toolkit/xmltrans.py` & `simubox-0.2.4/SimuBox/toolkit/xmltrans.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/Homepage.py` & `simubox-0.2.4/SimuBox/web/Homepage.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/1_Structure.py` & `simubox-0.2.4/SimuBox/web/pages/1_Structure.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/2_Scatter.py` & `simubox-0.2.4/SimuBox/web/pages/2_Scatter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/3_Voronoi.py` & `simubox-0.2.4/SimuBox/web/pages/3_Voronoi.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/4_Curve.py` & `simubox-0.2.4/SimuBox/web/pages/4_Curve.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/5_Peaks.py` & `simubox-0.2.4/SimuBox/web/pages/5_Peaks.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/6_Topology.py` & `simubox-0.2.4/SimuBox/web/pages/6_Topology.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/SimuBox/web/pages/7_Landscape.py` & `simubox-0.2.4/SimuBox/web/pages/7_Landscape.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.3/PKG-INFO` & `simubox-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuBox
-Version: 0.2.3
+Version: 0.2.4
 Summary: Free python package to do some science calculation.
 Home-page: https://pypi.org/project/SimuBox/
 License: ./LICENSE
 Author: Alkaid Yuan
 Author-email: kryuan@qq.com
 Maintainer: Alkaid Yuan
 Maintainer-email: kryuan@qq.com
```

