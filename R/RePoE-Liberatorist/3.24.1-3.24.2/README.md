# Comparing `tmp/RePoE-Liberatorist-3.24.1.tar.gz` & `tmp/RePoE-Liberatorist-3.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RePoE-Liberatorist-3.24.1.tar", last modified: Tue Apr  9 11:24:08 2024, max compression
+gzip compressed data, was "RePoE-Liberatorist-3.24.2.tar", last modified: Tue Apr  9 18:11:36 2024, max compression
```

## Comparing `RePoE-Liberatorist-3.24.1.tar` & `RePoE-Liberatorist-3.24.2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.1/LICENSE.md
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)     4135 2024-04-09 09:19:35.000000 RePoE-Liberatorist-3.24.1/README.md
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.417429 RePoE-Liberatorist-3.24.1/RePoE/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     2061 2024-04-09 11:20:12.000000 RePoE-Liberatorist-3.24.1/RePoE/__init__.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/RePoE/data/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/active_skill_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   567679 2024-04-09 11:21:33.000000 RePoE-Liberatorist-3.24.1/RePoE/data/atlas_tree.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 11:21:32.000000 RePoE-Liberatorist-3.24.1/RePoE/data/base_items.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/characters.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewel_notables.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewels.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cost_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/crafting_bench_options.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/default_monster_stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 11:20:35.000000 RePoE-Liberatorist-3.24.1/RePoE/data/essences.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 11:20:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/flavour.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/fossils.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/gem_tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 11:20:42.000000 RePoE-Liberatorist-3.24.1/RePoE/data/gems.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/item_classes.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 11:20:27.000000 RePoE-Liberatorist-3.24.1/RePoE/data/mod_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 11:21:29.000000 RePoE-Liberatorist-3.24.1/RePoE/data/mods.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2160399 2024-04-09 11:21:33.000000 RePoE-Liberatorist-3.24.1/RePoE/data/skill_tree.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 11:21:07.000000 RePoE-Liberatorist-3.24.1/RePoE/data/stat_translations.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 11:20:42.000000 RePoE-Liberatorist-3.24.1/RePoE/data/stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 11:20:35.000000 RePoE-Liberatorist-3.24.1/RePoE/data/tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    10346 2024-04-09 11:18:38.000000 RePoE-Liberatorist-3.24.1/RePoE/poe_types.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)      922 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/SOURCES.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/dependency_links.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/top_level.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.1/pyproject.toml
--rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/setup.cfg
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1138 2024-04-09 11:22:49.000000 RePoE-Liberatorist-3.24.1/setup.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.2/LICENSE.md
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     4324 2024-04-09 11:28:40.000000 RePoE-Liberatorist-3.24.2/README.md
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.269074 RePoE-Liberatorist-3.24.2/RePoE/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     2249 2024-04-09 18:06:30.000000 RePoE-Liberatorist-3.24.2/RePoE/__init__.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/RePoE/data/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/active_skill_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    55428 2024-04-09 18:09:28.000000 RePoE-Liberatorist-3.24.2/RePoE/data/areas.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   567679 2024-04-09 18:09:02.000000 RePoE-Liberatorist-3.24.2/RePoE/data/atlas_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 18:09:00.000000 RePoE-Liberatorist-3.24.2/RePoE/data/base_items.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/characters.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewel_notables.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewels.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cost_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/crafting_bench_options.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/default_monster_stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.2/RePoE/data/essences.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.2/RePoE/data/flavour.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/fossils.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/gem_tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/gems.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/item_classes.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.2/RePoE/data/mod_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 18:08:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/mods.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2160399 2024-04-09 18:09:01.000000 RePoE-Liberatorist-3.24.2/RePoE/data/skill_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 18:08:31.000000 RePoE-Liberatorist-3.24.2/RePoE/data/stat_translations.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.2/RePoE/data/tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   721113 2024-04-09 18:09:08.000000 RePoE-Liberatorist-3.24.2/RePoE/data/unique_items.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   532028 2024-04-09 18:09:25.000000 RePoE-Liberatorist-3.24.2/RePoE/data/unique_monsters.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    10629 2024-04-09 18:05:35.000000 RePoE-Liberatorist-3.24.2/RePoE/poe_types.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1017 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/top_level.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.2/pyproject.toml
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/setup.cfg
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1138 2024-04-09 18:10:59.000000 RePoE-Liberatorist-3.24.2/setup.py
```

### Comparing `RePoE-Liberatorist-3.24.1/LICENSE.md` & `RePoE-Liberatorist-3.24.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/README.md` & `RePoE-Liberatorist-3.24.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 ```
 python3 RePoE/run_parser.py all -f {POE_PATH}
 ```
 
 where {POE_PATH} is the path where the PoE ggpk file is located
 For me working in WSL this is POE_PATH="/mnt/c/Program Files (x86)/Grinding Gear Games/Path of Exile"
 
+## How upload this to pypi
+
+After running the parser, change the version in setup.py and run
+
+```
+python3 -m build
+python3 -m twine upload dist/*
+```
+
+and enter pypi api-key when prompted
+
 ## Files
 
 The [RePoE/data](RePoE/data) folder contains the generated data in Json format. Each file has a
 formatted and a compact version. The formatted versions complement their descriptions
 in the [RePoE/docs](RePoE/docs) folder.
 
 Note that the file formats are not final, they may change at any time, e.g. when the format
```

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/__init__.py` & `RePoE-Liberatorist-3.24.2/RePoE/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,7 +41,10 @@
 tags: List[str] = load_json("tags.min.json")
 cluster_jewels: Dict[str, ClusterJewel] = load_json("cluster_jewels.min.json")
 cluster_jewel_notables: List[ClusterJewelNotable] = load_json(
     "cluster_jewel_notables.min.json")
 cost_types: Dict[str, CostType] = load_json("cost_types.min.json")
 skill_tree: SkillTree = load_json("skill_tree.min.json")
 atlas_tree: AtlasTree = load_json("atlas_tree.min.json")
+unique_items: List[UniqueItem] = load_json("unique_items.min.json")
+unique_monsters: Dict[str, str] = load_json("unique_monsters.min.json")
+areas: List[Area] = load_json("areas.min.json")
```

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/active_skill_types.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/active_skill_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/atlas_tree.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/atlas_tree.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/base_items.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/base_items.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/characters.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/characters.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewel_notables.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewel_notables.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewels.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewels.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/cost_types.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/cost_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/crafting_bench_options.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/crafting_bench_options.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/default_monster_stats.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/default_monster_stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/essences.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/essences.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/flavour.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/flavour.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/fossils.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/fossils.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/gem_tags.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/gem_tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/gems.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/gems.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/item_classes.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/item_classes.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/mod_types.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/mod_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/mods.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/mods.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/skill_tree.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/skill_tree.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/stat_translations.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/stat_translations.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/stats.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/data/tags.min.json` & `RePoE-Liberatorist-3.24.2/RePoE/data/tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.1/RePoE/poe_types.py` & `RePoE-Liberatorist-3.24.2/RePoE/poe_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     item_class: str
     inventory_width: int
     inventory_height: int
     drop_level: int
     implicits: list[str]
     tags: list[str]
     visual_identity: VisualIdentity
-    properties: Dict[str, Union[int, str, BaseItemProperty]]
+    properties: Dict[str, dict]
     release_state: str
     requirements: NotRequired[Requirements]
     grants_buff: NotRequired[FlaskBuff]
 
 
 class Unarmed(TypedDict):
     attack_time: float
@@ -453,7 +453,21 @@
     min_x: int
     min_y: int
     nodes: Dict[str, SkillTreeNode]
     points: SkillTreePoints
     sprites: dict
     tree: Literal["Atlas"]
 
+class UniqueItem(TypedDict):
+    name: str
+    class_id: str
+    base_item: str
+    is_drop_restricted: bool
+    drop_enabled: bool
+    drop_monsters: List[str]
+    explicit_stat_text: List[str]
+
+class Area(TypedDict):
+    name: str
+    area_levels: List[int]
+    boss_monster_ids: List[str]
+    tags: List[str]
```

### Comparing `RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/SOURCES.txt` & `RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
 RePoE/__init__.py
 RePoE/poe_types.py
 RePoE/data/active_skill_types.min.json
+RePoE/data/areas.min.json
 RePoE/data/atlas_tree.min.json
 RePoE/data/base_items.min.json
 RePoE/data/characters.min.json
 RePoE/data/cluster_jewel_notables.min.json
 RePoE/data/cluster_jewels.min.json
 RePoE/data/cost_types.min.json
 RePoE/data/crafting_bench_options.min.json
@@ -21,11 +22,13 @@
 RePoE/data/item_classes.min.json
 RePoE/data/mod_types.min.json
 RePoE/data/mods.min.json
 RePoE/data/skill_tree.min.json
 RePoE/data/stat_translations.min.json
 RePoE/data/stats.min.json
 RePoE/data/tags.min.json
+RePoE/data/unique_items.min.json
+RePoE/data/unique_monsters.min.json
 RePoE_Liberatorist.egg-info/PKG-INFO
 RePoE_Liberatorist.egg-info/SOURCES.txt
 RePoE_Liberatorist.egg-info/dependency_links.txt
 RePoE_Liberatorist.egg-info/top_level.txt
```

### Comparing `RePoE-Liberatorist-3.24.1/setup.py` & `RePoE-Liberatorist-3.24.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Package meta-data.
 NAME = "RePoE-Liberatorist"
 DESCRIPTION = "Repository of Path of Exile resources for tool developers"
 URL = "https://github.com/Liberatorist/RePoE"
 EMAIL = ""
 AUTHOR = "Liberatorist"
 REQUIRES_PYTHON = ">=3.11.0"
-VERSION = "3.24.1"
+VERSION = "3.24.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

