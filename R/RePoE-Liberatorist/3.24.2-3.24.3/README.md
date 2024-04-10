# Comparing `tmp/RePoE-Liberatorist-3.24.2.tar.gz` & `tmp/RePoE-Liberatorist-3.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RePoE-Liberatorist-3.24.2.tar", last modified: Tue Apr  9 18:11:36 2024, max compression
+gzip compressed data, was "RePoE-Liberatorist-3.24.3.tar", last modified: Tue Apr  9 18:34:30 2024, max compression
```

## Comparing `RePoE-Liberatorist-3.24.2.tar` & `RePoE-Liberatorist-3.24.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.2/LICENSE.md
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)     4324 2024-04-09 11:28:40.000000 RePoE-Liberatorist-3.24.2/README.md
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.269074 RePoE-Liberatorist-3.24.2/RePoE/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     2249 2024-04-09 18:06:30.000000 RePoE-Liberatorist-3.24.2/RePoE/__init__.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/RePoE/data/
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/active_skill_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    55428 2024-04-09 18:09:28.000000 RePoE-Liberatorist-3.24.2/RePoE/data/areas.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   567679 2024-04-09 18:09:02.000000 RePoE-Liberatorist-3.24.2/RePoE/data/atlas_tree.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 18:09:00.000000 RePoE-Liberatorist-3.24.2/RePoE/data/base_items.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/characters.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewel_notables.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewels.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/cost_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.2/RePoE/data/crafting_bench_options.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/default_monster_stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.2/RePoE/data/essences.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.2/RePoE/data/flavour.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/fossils.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/gem_tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/gems.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.2/RePoE/data/item_classes.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.2/RePoE/data/mod_types.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 18:08:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/mods.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2160399 2024-04-09 18:09:01.000000 RePoE-Liberatorist-3.24.2/RePoE/data/skill_tree.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 18:08:31.000000 RePoE-Liberatorist-3.24.2/RePoE/data/stat_translations.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.2/RePoE/data/stats.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.2/RePoE/data/tags.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   721113 2024-04-09 18:09:08.000000 RePoE-Liberatorist-3.24.2/RePoE/data/unique_items.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)   532028 2024-04-09 18:09:25.000000 RePoE-Liberatorist-3.24.2/RePoE/data/unique_monsters.min.json
--rw-r--r--   0 fabian    (1000) fabian    (1000)    10629 2024-04-09 18:05:35.000000 RePoE-Liberatorist-3.24.2/RePoE/poe_types.py
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/
--rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1017 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/SOURCES.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/dependency_links.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 18:11:36.000000 RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/top_level.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.2/pyproject.toml
--rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 18:11:36.312407 RePoE-Liberatorist-3.24.2/setup.cfg
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1138 2024-04-09 18:10:59.000000 RePoE-Liberatorist-3.24.2/setup.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:34:30.964768 RePoE-Liberatorist-3.24.3/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1333 2024-04-08 15:41:04.000000 RePoE-Liberatorist-3.24.3/LICENSE.md
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:34:30.964768 RePoE-Liberatorist-3.24.3/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     4324 2024-04-09 11:28:40.000000 RePoE-Liberatorist-3.24.3/README.md
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:34:30.921435 RePoE-Liberatorist-3.24.3/RePoE/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     2249 2024-04-09 18:06:30.000000 RePoE-Liberatorist-3.24.3/RePoE/__init__.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:34:30.964768 RePoE-Liberatorist-3.24.3/RePoE/data/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1858 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.3/RePoE/data/active_skill_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    55428 2024-04-09 18:34:09.000000 RePoE-Liberatorist-3.24.3/RePoE/data/areas.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   567679 2024-04-09 18:09:02.000000 RePoE-Liberatorist-3.24.3/RePoE/data/atlas_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2097542 2024-04-09 18:09:00.000000 RePoE-Liberatorist-3.24.3/RePoE/data/base_items.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1762 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.3/RePoE/data/characters.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    37559 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.3/RePoE/data/cluster_jewel_notables.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     8919 2024-04-09 18:07:58.000000 RePoE-Liberatorist-3.24.3/RePoE/data/cluster_jewels.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1055 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.3/RePoE/data/cost_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   215310 2024-04-09 18:07:59.000000 RePoE-Liberatorist-3.24.3/RePoE/data/crafting_bench_options.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    11283 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.3/RePoE/data/default_monster_stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   113821 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.3/RePoE/data/essences.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   318851 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.3/RePoE/data/flavour.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   227752 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.3/RePoE/data/fossils.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      930 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.3/RePoE/data/gem_tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  4656860 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.3/RePoE/data/gems.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     3489 2024-04-09 18:08:53.000000 RePoE-Liberatorist-3.24.3/RePoE/data/item_classes.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   793808 2024-04-09 18:07:39.000000 RePoE-Liberatorist-3.24.3/RePoE/data/mod_types.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000) 18478894 2024-04-09 18:08:57.000000 RePoE-Liberatorist-3.24.3/RePoE/data/mods.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2160399 2024-04-09 18:09:01.000000 RePoE-Liberatorist-3.24.3/RePoE/data/skill_tree.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  2577009 2024-04-09 18:08:31.000000 RePoE-Liberatorist-3.24.3/RePoE/data/stat_translations.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)  1898551 2024-04-09 18:07:57.000000 RePoE-Liberatorist-3.24.3/RePoE/data/stats.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    21236 2024-04-09 18:07:49.000000 RePoE-Liberatorist-3.24.3/RePoE/data/tags.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   721113 2024-04-09 18:33:49.000000 RePoE-Liberatorist-3.24.3/RePoE/data/unique_items.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   380608 2024-04-09 18:34:06.000000 RePoE-Liberatorist-3.24.3/RePoE/data/unique_monsters.min.json
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    10629 2024-04-09 18:05:35.000000 RePoE-Liberatorist-3.24.3/RePoE/poe_types.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2024-04-09 18:34:30.964768 RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      287 2024-04-09 18:34:30.000000 RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1017 2024-04-09 18:34:30.000000 RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2024-04-09 18:34:30.000000 RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        6 2024-04-09 18:34:30.000000 RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/top_level.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      118 2024-04-09 06:48:30.000000 RePoE-Liberatorist-3.24.3/pyproject.toml
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2024-04-09 18:34:30.964768 RePoE-Liberatorist-3.24.3/setup.cfg
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1138 2024-04-09 18:34:10.000000 RePoE-Liberatorist-3.24.3/setup.py
```

### Comparing `RePoE-Liberatorist-3.24.2/LICENSE.md` & `RePoE-Liberatorist-3.24.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/README.md` & `RePoE-Liberatorist-3.24.3/README.md`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/__init__.py` & `RePoE-Liberatorist-3.24.3/RePoE/__init__.py`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/active_skill_types.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/active_skill_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/areas.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/areas.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/atlas_tree.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/atlas_tree.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/base_items.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/base_items.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/characters.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/characters.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewel_notables.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/cluster_jewel_notables.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/cluster_jewels.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/cluster_jewels.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/cost_types.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/cost_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/crafting_bench_options.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/crafting_bench_options.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/default_monster_stats.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/default_monster_stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/essences.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/essences.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/flavour.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/flavour.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/fossils.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/fossils.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/gem_tags.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/gem_tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/gems.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/gems.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/item_classes.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/item_classes.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/mod_types.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/mod_types.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/mods.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/mods.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/skill_tree.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/skill_tree.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/stat_translations.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/stat_translations.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/stats.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/stats.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/tags.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/tags.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/data/unique_items.min.json` & `RePoE-Liberatorist-3.24.3/RePoE/data/unique_items.min.json`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE/poe_types.py` & `RePoE-Liberatorist-3.24.3/RePoE/poe_types.py`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/RePoE_Liberatorist.egg-info/SOURCES.txt` & `RePoE-Liberatorist-3.24.3/RePoE_Liberatorist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RePoE-Liberatorist-3.24.2/setup.py` & `RePoE-Liberatorist-3.24.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Package meta-data.
 NAME = "RePoE-Liberatorist"
 DESCRIPTION = "Repository of Path of Exile resources for tool developers"
 URL = "https://github.com/Liberatorist/RePoE"
 EMAIL = ""
 AUTHOR = "Liberatorist"
 REQUIRES_PYTHON = ">=3.11.0"
-VERSION = "3.24.2"
+VERSION = "3.24.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

