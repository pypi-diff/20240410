# Comparing `tmp/Quid-2.6.1.tar.gz` & `tmp/Quid-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quid-2.6.1.tar", last modified: Thu Feb 22 17:04:27 2024, max compression
+gzip compressed data, was "Quid-2.6.2.tar", last modified: Wed Apr 10 10:38:25 2024, max compression
```

## Comparing `Quid-2.6.1.tar` & `Quid-2.6.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-02-21 19:06:48.000000 Quid-2.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13207 2024-02-22 17:04:27.180779 Quid-2.6.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/Quid.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13207 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-02-22 17:04:27.000000 Quid-2.6.1/Quid.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    12352 2024-02-21 19:06:48.000000 Quid-2.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-02-21 19:06:48.000000 Quid-2.6.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.176779 Quid-2.6.1/quid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.176779 Quid-2.6.1/quid/cli/
--rw-rw-rw-   0 root         (0) root         (0)    29334 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/cli/QuidCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.176779 Quid-2.6.1/quid/core/
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/BestMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/InternalMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/InternalMatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)    18157 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/Quid.py
--rw-rw-rw-   0 root         (0) root         (0)    18592 2024-02-22 17:02:55.000000 Quid-2.6.1/quid/core/QuidMatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    14310 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/QuidMerger.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/Text.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/core/Token.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/quid/helper/
--rw-rw-rw-   0 root         (0) root         (0)     1736 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/helper/Decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/helper/Loader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/quid/match/
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/match/Match.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/match/MatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/quid/passager/
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/AnalyzedWork.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/CitationSource.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/CitationSourceLink.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/Location.py
--rw-rw-rw-   0 root         (0) root         (0)    28856 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/Passager.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/SourceSegment.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TargetLocation.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TargetLocationSelection.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TargetMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TargetText.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TargetTextLocationLink.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/passager/TextWithMatches.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/passager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 17:04:27.180779 Quid-2.6.1/quid/visualization/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/Info.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/Markup.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/MarkupSpan.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/TargetHtml.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/TargetTextWithContent.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/Visualization.py
--rw-rw-rw-   0 root         (0) root         (0)    12916 2024-02-21 19:06:48.000000 Quid-2.6.1/quid/visualization/Visualizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 17:04:10.000000 Quid-2.6.1/quid/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-02-22 17:04:27.184779 Quid-2.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.428470 Quid-2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 13:24:44.000000 Quid-2.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6817 2024-04-10 10:38:25.428470 Quid-2.6.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/Quid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6817 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5962 2024-04-09 13:52:32.000000 Quid-2.6.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-09 13:24:44.000000 Quid-2.6.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.420470 Quid-2.6.2/quid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    29334 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/cli/QuidCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/core/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/BestMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/InternalMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/InternalMatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)    18157 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Quid.py
+-rw-rw-rw-   0 root         (0) root         (0)    18592 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/QuidMatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    14310 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/QuidMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Text.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Token.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/helper/
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/helper/Decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/helper/Loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/match/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/match/Match.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/match/MatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/passager/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/AnalyzedWork.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/CitationSource.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/CitationSourceLink.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/Location.py
+-rw-rw-rw-   0 root         (0) root         (0)    28856 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/Passager.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/SourceSegment.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetLocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetLocationSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetText.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetTextLocationLink.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TextWithMatches.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/passager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Info.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/MarkupSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/TargetHtml.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/TargetTextWithContent.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12916 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Visualizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/visualization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-10 10:38:25.428470 Quid-2.6.2/setup.cfg
```

### Comparing `Quid-2.6.1/LICENSE` & `Quid-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/Quid.egg-info/SOURCES.txt` & `Quid-2.6.2/Quid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/cli/QuidCLI.py` & `Quid-2.6.2/quid/cli/QuidCLI.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/core/Quid.py` & `Quid-2.6.2/quid/core/Quid.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/core/QuidMatcher.py` & `Quid-2.6.2/quid/core/QuidMatcher.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/core/QuidMerger.py` & `Quid-2.6.2/quid/core/QuidMerger.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/helper/Decoder.py` & `Quid-2.6.2/quid/helper/Decoder.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/helper/Loader.py` & `Quid-2.6.2/quid/helper/Loader.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/passager/AnalyzedWork.py` & `Quid-2.6.2/quid/passager/AnalyzedWork.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/passager/CitationSource.py` & `Quid-2.6.2/quid/passager/CitationSource.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/passager/Passager.py` & `Quid-2.6.2/quid/passager/Passager.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/passager/SourceSegment.py` & `Quid-2.6.2/quid/passager/SourceSegment.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/passager/TargetText.py` & `Quid-2.6.2/quid/passager/TargetText.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/quid/visualization/Visualizer.py` & `Quid-2.6.2/quid/visualization/Visualizer.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.1/setup.cfg` & `Quid-2.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Quid
-version = 2.6.1
+version = 2.6.2
 author = Frederik Arnold
 author_email = frederik.arnold@hu-berlin.de
 description = Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = quotation detection, quotation identification, literal citation extraction, key passages, natural language processing, nlp, text reuse
 url = https://hu.berlin/quid
```

