# Comparing `tmp/RePoE-Liberatorist-3.24.0.tar.gz` & `tmp/RePoE-Liberatorist-3.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RePoE-Liberatorist-3.24.0.tar", last modified: Tue Apr  9 09:22:08 2024, max compression
+gzip compressed data, was "RePoE-Liberatorist-3.24.1.tar", last modified: Tue Apr  9 11:24:08 2024, max compression
```

## Comparing `RePoE-Liberatorist-3.24.0.tar` & `RePoE-Liberatorist-3.24.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 09:22:08.757335 RePoE-Liberatorist-3.24.0/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.0/LICENSE.md
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 09:22:08.757335 RePoE-Liberatorist-3.24.0/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)     4135 2024-04-09 09:19:35.000000 RePoE-Liberatorist-3.24.0/README.md
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 09:22:08.703168 RePoE-Liberatorist-3.24.0/RePoE/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1943 2024-04-09 06:45:22.000000 RePoE-Liberatorist-3.24.0/RePoE/__init__.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 09:22:08.757335 RePoE-Liberatorist-3.24.0/RePoE/data/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 06:35:57.000000 RePoE-Liberatorist-3.24.0/RePoE/data/active_skill_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 06:36:55.000000 RePoE-Liberatorist-3.24.0/RePoE/data/base_items.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 06:35:58.000000 RePoE-Liberatorist-3.24.0/RePoE/data/characters.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 06:35:57.000000 RePoE-Liberatorist-3.24.0/RePoE/data/cluster_jewel_notables.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 06:35:57.000000 RePoE-Liberatorist-3.24.0/RePoE/data/cluster_jewels.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 06:35:58.000000 RePoE-Liberatorist-3.24.0/RePoE/data/cost_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 06:35:58.000000 RePoE-Liberatorist-3.24.0/RePoE/data/crafting_bench_options.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 06:36:48.000000 RePoE-Liberatorist-3.24.0/RePoE/data/default_monster_stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 06:35:48.000000 RePoE-Liberatorist-3.24.0/RePoE/data/essences.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 06:35:38.000000 RePoE-Liberatorist-3.24.0/RePoE/data/flavour.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 06:35:56.000000 RePoE-Liberatorist-3.24.0/RePoE/data/fossils.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 06:36:48.000000 RePoE-Liberatorist-3.24.0/RePoE/data/gem_tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 06:35:56.000000 RePoE-Liberatorist-3.24.0/RePoE/data/gems.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 06:36:48.000000 RePoE-Liberatorist-3.24.0/RePoE/data/item_classes.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 06:35:39.000000 RePoE-Liberatorist-3.24.0/RePoE/data/mod_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 06:36:52.000000 RePoE-Liberatorist-3.24.0/RePoE/data/mods.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 06:36:25.000000 RePoE-Liberatorist-3.24.0/RePoE/data/stat_translations.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 06:35:56.000000 RePoE-Liberatorist-3.24.0/RePoE/data/stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 06:35:48.000000 RePoE-Liberatorist-3.24.0/RePoE/data/tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     7355 2024-04-09 09:09:33.000000 RePoE-Liberatorist-3.24.0/RePoE/types.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 09:22:08.757335 RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 09:22:08.000000 RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)      856 2024-04-09 09:22:08.000000 RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/SOURCES.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 09:22:08.000000 RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/dependency_links.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 09:22:08.000000 RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/top_level.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.0/pyproject.toml
--rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 09:22:08.757335 RePoE-Liberatorist-3.24.0/setup.cfg
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1134 2024-04-09 09:08:49.000000 RePoE-Liberatorist-3.24.0/setup.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.1/LICENSE.md
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     4135 2024-04-09 09:19:35.000000 RePoE-Liberatorist-3.24.1/README.md
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.417429 RePoE-Liberatorist-3.24.1/RePoE/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     2061 2024-04-09 11:20:12.000000 RePoE-Liberatorist-3.24.1/RePoE/__init__.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/RePoE/data/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/active_skill_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   567679 2024-04-09 11:21:33.000000 RePoE-Liberatorist-3.24.1/RePoE/data/atlas_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 11:21:32.000000 RePoE-Liberatorist-3.24.1/RePoE/data/base_items.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/characters.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewel_notables.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewels.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/cost_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 11:20:44.000000 RePoE-Liberatorist-3.24.1/RePoE/data/crafting_bench_options.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/default_monster_stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 11:20:35.000000 RePoE-Liberatorist-3.24.1/RePoE/data/essences.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 11:20:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/flavour.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 11:20:43.000000 RePoE-Liberatorist-3.24.1/RePoE/data/fossils.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/gem_tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 11:20:42.000000 RePoE-Liberatorist-3.24.1/RePoE/data/gems.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 11:21:26.000000 RePoE-Liberatorist-3.24.1/RePoE/data/item_classes.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 11:20:27.000000 RePoE-Liberatorist-3.24.1/RePoE/data/mod_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 11:21:29.000000 RePoE-Liberatorist-3.24.1/RePoE/data/mods.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2160399 2024-04-09 11:21:33.000000 RePoE-Liberatorist-3.24.1/RePoE/data/skill_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 11:21:07.000000 RePoE-Liberatorist-3.24.1/RePoE/data/stat_translations.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 11:20:42.000000 RePoE-Liberatorist-3.24.1/RePoE/data/stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 11:20:35.000000 RePoE-Liberatorist-3.24.1/RePoE/data/tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    10346 2024-04-09 11:18:38.000000 RePoE-Liberatorist-3.24.1/RePoE/poe_types.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      922 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 11:24:08.000000 RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/top_level.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.1/pyproject.toml
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 11:24:08.460762 RePoE-Liberatorist-3.24.1/setup.cfg
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1138 2024-04-09 11:22:49.000000 RePoE-Liberatorist-3.24.1/setup.py
```

### Comparing `RePoE-Liberatorist-3.24.0/LICENSE.md` & `RePoE-Liberatorist-3.24.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/README.md` & `RePoE-Liberatorist-3.24.1/README.md`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/__init__.py` & `RePoE-Liberatorist-3.24.1/RePoE/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 from typing import Dict, List, Optional
 
-from RePoE.types import *
+from RePoE.poe_types import *
 # directory that this __init__ file lives in
 __REPOE_DIR__, _ = os.path.split(__file__)
 
 # full path to ./data
 __DATA_PATH__ = os.path.join(__REPOE_DIR__, "data", "")
 
 
@@ -39,7 +39,9 @@
 stat_translations: List[StatTranslation] = load_json(
     "stat_translations.min.json")
 tags: List[str] = load_json("tags.min.json")
 cluster_jewels: Dict[str, ClusterJewel] = load_json("cluster_jewels.min.json")
 cluster_jewel_notables: List[ClusterJewelNotable] = load_json(
     "cluster_jewel_notables.min.json")
 cost_types: Dict[str, CostType] = load_json("cost_types.min.json")
+skill_tree: SkillTree = load_json("skill_tree.min.json")
+atlas_tree: AtlasTree = load_json("atlas_tree.min.json")
```

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/active_skill_types.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/active_skill_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/base_items.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/base_items.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/characters.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/characters.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/cluster_jewel_notables.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewel_notables.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/cluster_jewels.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/cluster_jewels.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/cost_types.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/cost_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/crafting_bench_options.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/crafting_bench_options.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/default_monster_stats.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/default_monster_stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/essences.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/essences.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/flavour.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/flavour.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/fossils.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/fossils.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/gem_tags.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/gem_tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/gems.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/gems.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/item_classes.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/item_classes.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/mod_types.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/mod_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/mods.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/mods.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/stat_translations.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/stat_translations.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/stats.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/data/tags.min.json` & `RePoE-Liberatorist-3.24.1/RePoE/data/tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.0/RePoE/types.py` & `RePoE-Liberatorist-3.24.1/RePoE/poe_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-from enum import Enum
 from typing import Dict, List, Literal, NotRequired, TypedDict, Union
 
 
-class Format(Enum):
-    DICT = 0
-    LIST = 1
-
-
 class Requirements(TypedDict):
     strength: int
     dexterity: int
     intelligence: int
     level: int
 
 
@@ -310,14 +304,20 @@
 
 
 class ClusterJewelNotable(TypedDict):
     id: str
     jewel_stat: str
     name: str
 
+class Rect(TypedDict):
+    height: int
+    width: int
+    x: int
+    y: int
+
 
 class ClusterJewelPassiveSkill(TypedDict):
     id: str
     name: str
     stats: Dict[str, int]
     tag: str
 
@@ -333,7 +333,127 @@
     socket_indices: List[int]
     total_indices: int
 
 
 class CostType(TypedDict):
     format_text: str
     stat: str
+
+
+class Ascendancy(TypedDict):
+    flavourText: str
+    flavourTextColour: str
+    flavourTextRect: Rect
+    id: str
+    name: str
+
+class PoEClass(TypedDict):
+    ascendancies: List[Ascendancy]
+    base_dex: int
+    base_int: int
+    base_str: int
+    name: str
+
+class SkillTreeConstants(TypedDict):
+    PSSCentreInnerRadius: int
+    characterAttributes: Dict[str, int]
+    classes: Dict[str, int]
+    orbitRadii: List[int]
+    skillsPerOrbit: List[int]
+
+class SkillTreeExtraImage(TypedDict):
+        image: str
+        x: float
+        y: float
+class SkillTreeBackground(TypedDict):
+    image: str
+    isHalfImage: bool
+
+class SkillTreeGroup(TypedDict):
+    background: SkillTreeBackground
+    nodes: List[str]
+    orbits: List[int]
+    x: float
+    y: float
+
+class MasteryEffect(TypedDict):
+    effect: int
+    stats: List[str]    
+    reminderText: NotRequired[List[str]]
+
+class SkillTreeNode(TypedDict):
+    group: int
+    icon: str
+    in_: List[str]
+    out: List[str]
+    name: str
+    orbit: int
+    orbitIndex: int
+    out: List[str]
+    reminderText: List[str]
+    skill: int
+    stats: List[str]
+    activeIcon: NotRequired[str]
+    activeEffectImage: NotRequired[str]
+    inactiveIcon: NotRequired[str]
+    recipe: NotRequired[List[str]]
+    isNotable: NotRequired[bool]
+    isBlighted: NotRequired[bool]
+    isKeystone: NotRequired[bool]
+    isJewelSocket: NotRequired[bool]
+    isProxy: NotRequired[bool]
+    isMastery: NotRequired[bool]
+    isAscendancyStart: NotRequired[bool]
+    masteryEffects: NotRequired[List[MasteryEffect]]
+    grantedPassivePoints: NotRequired[int]
+    grantedIntelligence: NotRequired[int]
+    grantedDexterity: NotRequired[int]
+    grantedStrength: NotRequired[int]
+    classStartIndex: NotRequired[int]
+    ascendancyName: NotRequired[str]
+    ascendancyClassName: NotRequired[str]
+    ascendancyClass: NotRequired[str]
+    isMultipleChoice: NotRequired[bool]
+    isMultipleChoiceOption: NotRequired[bool]
+    expansionJewel: NotRequired[bool]
+    grantedSkills: NotRequired[List[str]]
+    grantedNotable: NotRequired[str]
+    isJewelSocketActive: NotRequired[bool]
+    activeIcon: NotRequired[str]
+
+
+class SkillTreePoints(TypedDict):
+    ascendancyPoints: int
+    totalPoints: int
+
+
+class SkillTree(TypedDict):
+    alternate_ascendancies: List[Ascendancy]
+    classes: List[PoEClass]
+    constants: SkillTreeConstants
+    extra_images: Dict[str, SkillTreeExtraImage]
+    groups: Dict[str, SkillTreeGroup]
+    imageZoomLevels: List[float]
+    jewelSlots: List[int]
+    max_x: int
+    max_y: int
+    min_x: int
+    min_y: int
+    nodes: Dict[str, SkillTreeNode]
+    points: SkillTreePoints
+    sprites: dict
+    tree: Literal["default"]
+
+
+class AtlasTree(TypedDict):
+    constants: SkillTreeConstants
+    groups: Dict[str, SkillTreeGroup]
+    imageZoomLevels: List[float]
+    max_x: int
+    max_y: int
+    min_x: int
+    min_y: int
+    nodes: Dict[str, SkillTreeNode]
+    points: SkillTreePoints
+    sprites: dict
+    tree: Literal["Atlas"]
+
```

### Comparing `RePoE-Liberatorist-3.24.0/RePoE_Liberatorist.egg-info/SOURCES.txt` & `RePoE-Liberatorist-3.24.1/RePoE_Liberatorist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
 RePoE/__init__.py
-RePoE/types.py
+RePoE/poe_types.py
 RePoE/data/active_skill_types.min.json
+RePoE/data/atlas_tree.min.json
 RePoE/data/base_items.min.json
 RePoE/data/characters.min.json
 RePoE/data/cluster_jewel_notables.min.json
 RePoE/data/cluster_jewels.min.json
 RePoE/data/cost_types.min.json
 RePoE/data/crafting_bench_options.min.json
 RePoE/data/default_monster_stats.min.json
@@ -16,14 +17,15 @@
 RePoE/data/flavour.min.json
 RePoE/data/fossils.min.json
 RePoE/data/gem_tags.min.json
 RePoE/data/gems.min.json
 RePoE/data/item_classes.min.json
 RePoE/data/mod_types.min.json
 RePoE/data/mods.min.json
+RePoE/data/skill_tree.min.json
 RePoE/data/stat_translations.min.json
 RePoE/data/stats.min.json
 RePoE/data/tags.min.json
 RePoE_Liberatorist.egg-info/PKG-INFO
 RePoE_Liberatorist.egg-info/SOURCES.txt
 RePoE_Liberatorist.egg-info/dependency_links.txt
 RePoE_Liberatorist.egg-info/top_level.txt
```

### Comparing `RePoE-Liberatorist-3.24.0/setup.py` & `RePoE-Liberatorist-3.24.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Package meta-data.
 NAME = "RePoE-Liberatorist"
 DESCRIPTION = "Repository of Path of Exile resources for tool developers"
 URL = "https://github.com/Liberatorist/RePoE"
 EMAIL = ""
 AUTHOR = "Liberatorist"
 REQUIRES_PYTHON = ">=3.11.0"
-VERSION = "3.24.0"
+VERSION = "3.24.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
@@ -32,15 +32,15 @@
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    py_modules=["RePoE.types"],
+    py_modules=["RePoE.poe_types"],
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     license="proprietary",
 
     data_files=[
         (directory, data_files),
     ]
```

