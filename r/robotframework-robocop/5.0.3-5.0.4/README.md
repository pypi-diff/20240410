# Comparing `tmp/robotframework-robocop-5.0.3.tar.gz` & `tmp/robotframework-robocop-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-5.0.3.tar", last modified: Fri Jan 19 09:49:05 2024, max compression
+gzip compressed data, was "robotframework-robocop-5.0.4.tar", last modified: Wed Apr 10 07:26:03 2024, max compression
```

## Comparing `robotframework-robocop-5.0.3.tar` & `robotframework-robocop-5.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.959556 robotframework-robocop-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-01-19 09:49:05.959556 robotframework-robocop-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.951556 robotframework-robocop-5.0.3/robocop/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.951556 robotframework-robocop-5.0.3/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/comments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.951556 robotframework-robocop-5.0.3/robocop/checkers/community_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/community_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/community_rules/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    32413 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (127)    58081 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56663 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    33738 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    24002 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.955556 robotframework-robocop-5.0.3/robocop/reports/
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/compare_runs_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/file_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/json_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/return_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/robocop_version_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/rules_by_id_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/rules_by_severity_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/sarif_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/time_taken_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/reports/timestamp_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.955556 robotframework-robocop-5.0.3/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/variable_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:49:05.955556 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-19 09:49:05.000000 robotframework-robocop-5.0.3/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 09:49:05.959556 robotframework-robocop-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-01-19 09:48:52.000000 robotframework-robocop-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.184041 robotframework-robocop-5.0.4/robocop/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.184041 robotframework-robocop-5.0.4/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/comments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/checkers/community_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/community_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/community_rules/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32413 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57337 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56593 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33738 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24002 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/compare_runs_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/file_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/return_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/robocop_version_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/rules_by_id_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/rules_by_severity_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/sarif_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/time_taken_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/reports/timestamp_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.188041 robotframework-robocop-5.0.4/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/variable_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 07:26:03.000000 robotframework-robocop-5.0.4/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:26:03.192041 robotframework-robocop-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 07:25:51.000000 robotframework-robocop-5.0.4/setup.py
```

### Comparing `robotframework-robocop-5.0.3/LICENSE` & `robotframework-robocop-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/PKG-INFO` & `robotframework-robocop-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 5.0.3
+Version: 5.0.4
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
@@ -31,15 +31,15 @@
 License-File: LICENSE
 Requires-Dist: jinja2<4.0,>=3.0
 Requires-Dist: robotframework>=3.2.2
 Requires-Dist: pathspec<0.13,>=0.9
 Requires-Dist: tomli>=2.0.0
 Requires-Dist: pytz>=2022.7
 Requires-Dist: python-dateutil>=2.8.2
-Requires-Dist: platformdirs<4.2.0,>=3.2.0
+Requires-Dist: platformdirs<4.3.0,>=3.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: pytest-benchmark; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `robotframework-robocop-5.0.3/README.md` & `robotframework-robocop-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/__init__.py` & `robotframework-robocop-5.0.4/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/comments.py` & `robotframework-robocop-5.0.4/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/community_rules/keywords.py` & `robotframework-robocop-5.0.4/robocop/checkers/community_rules/keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/documentation.py` & `robotframework-robocop-5.0.4/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/duplications.py` & `robotframework-robocop-5.0.4/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/errors.py` & `robotframework-robocop-5.0.4/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/lengths.py` & `robotframework-robocop-5.0.4/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/misc.py` & `robotframework-robocop-5.0.4/robocop/checkers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     get_errors,
     keyword_col,
     normalize_robot_name,
     normalize_robot_var_name,
     parse_assignment_sign_type,
     token_col,
 )
-from robocop.utils.misc import RETURN_CLASSES, find_escaped_variables
+from robocop.utils.misc import RETURN_CLASSES, _is_var_scope_local, find_escaped_variables
 from robocop.utils.variable_matcher import VariableMatches
 
 RULE_CATEGORY_ID = "09"
 
 rules = {
     "0901": Rule(
         rule_id="0901",
@@ -1198,23 +1198,39 @@
         for token in node.header.get_tokens(Token.ASSIGN):
             self.handle_assign_variable(token)
 
     def visit_LibraryImport(self, node):  # noqa
         for token in node.get_tokens(Token.NAME, Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
 
-    visit_SuiteSetup = (
+    visit_TestTags = (
+        visit_ForceTags
+    ) = (
+        visit_Metadata
+    ) = (
+        visit_DefaultTags
+    ) = (
+        visit_Variable
+    ) = (
+        visit_ReturnStatement
+    ) = (
+        visit_ReturnSetting
+    ) = (
+        visit_Teardown
+    ) = (
+        visit_Timeout
+    ) = (
+        visit_Return
+    ) = (
+        visit_SuiteSetup
+    ) = (
         visit_SuiteTeardown
-    ) = visit_TestSetup = visit_TestTeardown = visit_ResourceImport = visit_VariablesImport = visit_LibraryImport
-
-    def visit_DefaultTags(self, node):  # noqa
-        for token in node.get_tokens(Token.ARGUMENT):
-            self.find_not_nested_variable(token.value, is_var=False)
-
-    visit_TestTags = visit_ForceTags = visit_Metadata = visit_DefaultTags
+    ) = (
+        visit_TestSetup
+    ) = visit_TestTeardown = visit_Setup = visit_ResourceImport = visit_VariablesImport = visit_LibraryImport
 
     def clear_variables_after_loop(self):
         """Remove used variables after loop finishes."""
         for index, scope in enumerate(self.variables):
             self.variables[index] = {name: variable for name, variable in scope.items() if not variable.is_used}
 
     def revisit_variables_used_in_loop(self):
@@ -1287,46 +1303,23 @@
 
     def visit_KeywordCall(self, node):  # noqa
         for token in node.get_tokens(Token.ARGUMENT, Token.KEYWORD):  # argument can be used in keyword name
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.get_tokens(Token.ASSIGN):  # we first check args, then assign for used and then overwritten
             self.handle_assign_variable(token)
 
-    def visit_Variable(self, node):  # noqa
-        """Visit section variables.
-
-        We already visit and collect section variables definitions, but we revisit it to find variables that are used
-        in other variables.
-        """
-        for token in node.get_tokens(Token.ARGUMENT):
-            self.find_not_nested_variable(token.value, is_var=False)
-
-    @staticmethod
-    def _is_var_scope_local(node):
-        is_local = True
-        for option in node.get_tokens(Token.OPTION):
-            if "scope=" in option.value:
-                is_local = option.value.lower() == "scope=local"
-        return is_local
-
     def visit_Var(self, node):  # noqa
         if node.errors:  # for example invalid variable definition like $var}
             return
         for arg in node.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(arg.value, is_var=False)
         variable = node.get_token(Token.VARIABLE)
-        if variable and self._is_var_scope_local(node):
+        if variable and _is_var_scope_local(node):
             self.handle_assign_variable(variable)
 
-    def visit_Return(self, node):  # noqa
-        for token in node.get_tokens(Token.ARGUMENT):
-            self.find_not_nested_variable(token.value, is_var=False)
-
-    visit_ReturnStatement = visit_ReturnSetting = visit_Teardown = visit_Timeout = visit_Return
-
     def visit_TemplateArguments(self, node):  # noqa
         for argument in node.data_tokens:
             self.find_not_nested_variable(argument.value, is_var=False)
 
     def handle_assign_variable(self, token):
         """Check if assign does not overwrite arguments or variables.
```

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/naming.py` & `robotframework-robocop-5.0.4/robocop/checkers/naming.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     keyword_col,
     normalize_robot_name,
     normalize_robot_var_name,
     pattern_type,
     remove_robot_vars,
     token_col,
 )
-from robocop.utils.misc import remove_nested_variables
+from robocop.utils.misc import _is_var_scope_local, remove_nested_variables
 from robocop.utils.run_keywords import iterate_keyword_names
 from robocop.utils.variable_matcher import VariableMatches
 
 RULE_CATEGORY_ID = "03"
 
 rules = {
     "0301": Rule(
@@ -1073,31 +1073,23 @@
             self.report(
                 "non-local-variables-should-be-uppercase",
                 node=node,
                 col=token.col_offset + 1,
                 end_col=token.end_col_offset + 1,
             )
 
-    @staticmethod
-    def _is_var_scope_local(node):
-        is_local = True
-        for option in node.get_tokens(Token.OPTION):
-            if "scope=" in option.value:
-                is_local = option.value.lower() == "scope=local"
-        return is_local
-
     def visit_Var(self, node):  # noqa
         if node.errors:  # for example invalid variable definition like $var}
             return
         variable = node.get_token(Token.VARIABLE)
         if not variable:
             return
         self.check_for_reserved_naming_or_hyphen(variable, "Variable", is_assign=True)
         # TODO Check supported syntax for variable, ie ${{var}}?
-        if not self._is_var_scope_local(node):
+        if not _is_var_scope_local(node):
             self.check_non_local_variable(search_variable(variable.value).base, node, variable)
 
     def visit_If(self, node):  # noqa
         for token in node.header.get_tokens(Token.ASSIGN):
             self.check_for_reserved_naming_or_hyphen(token, "Variable")
         self.generic_visit(node)
 
@@ -1190,15 +1182,15 @@
     def visit_Var(self, node):  # noqa
         if node.errors:  # for example invalid variable definition like $var}
             return
         for arg in node.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(arg, arg.value, is_var=False)
         variable = node.get_token(Token.VARIABLE)
         if variable:
-            self.find_similar_variables([variable], node)
+            self.find_similar_variables([variable], node, ignore_overwriting=not _is_var_scope_local(node))
 
     def visit_If(self, node):  # noqa
         for token in node.header.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token, token.value, is_var=False)
         tokens = node.header.get_tokens(Token.ASSIGN)
         self.find_similar_variables(tokens, node)
         self.generic_visit(node)
@@ -1308,20 +1300,24 @@
             if isinstance(child, Arguments):
                 for token in child.get_tokens(Token.ARGUMENT):
                     variable_match = search_variable(token.value, ignore_errors=True)
                     name = variable_match.name
                     normalized = normalize_robot_name(variable_match.base)
                     self.assigned_variables[normalized].append(name)
 
-    def find_similar_variables(self, tokens, node):
+    def find_similar_variables(self, tokens, node, ignore_overwriting: bool = False):
         for token in tokens:
             variable_match = search_variable(token.value, ignore_errors=True)
             name = variable_match.name
             normalized = normalize_robot_name(variable_match.base)
-            if normalized in self.assigned_variables and name not in self.assigned_variables[normalized]:
+            if (
+                not ignore_overwriting
+                and normalized in self.assigned_variables
+                and name not in self.assigned_variables[normalized]
+            ):
                 self.report(
                     "possible-variable-overwriting",
                     variable_name=name,
                     block_name=self.parent_name,
                     block_type=self.parent_type,
                     node=node,
                     lineno=token.lineno,
```

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/spacing.py` & `robotframework-robocop-5.0.4/robocop/checkers/spacing.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/checkers/tags.py` & `robotframework-robocop-5.0.4/robocop/checkers/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from collections import defaultdict
 
 from robot.api import Token
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleSeverity
+from robocop.utils import variable_matcher
 
 RULE_CATEGORY_ID = "06"
 
 rules = {
     "0601": Rule(
         rule_id="0601",
         name="tag-with-space",
@@ -242,29 +243,50 @@
 
     def visit_ForceTags(self, node):  # noqa
         self.check_tags(node)
 
     visit_DefaultTags = visit_Tags = visit_KeywordTags = visit_ForceTags
 
     def visit_Documentation(self, node):  # noqa
-        if self.is_keyword:
-            *_, last_line = node.lines
-            filtered_line = filter(
-                lambda tag: tag.type not in Token.NON_DATA_TOKENS and tag.type != Token.DOCUMENTATION,
-                last_line,
-            )
-            tags = defaultdict(list)
-            for index, token in enumerate(filtered_line):
-                if index == 0 and token.value.lower() != "tags:":
-                    break
-                token.value = token.value.rstrip(",")
-                normalized_tag = token.value.lower().replace(" ", "")
-                tags[normalized_tag].append(token)
-                self.check_tag(token, node)
-            self.check_duplicates(tags)
+        """
+        Parse tags from last line of documentation.
+
+        Tags can be defined as comma separated list - Tags: tag1, tag2 .
+        """
+        if not self.is_keyword:
+            return
+        *_, last_line = node.lines
+        args = [tag for tag in last_line if tag.type == Token.ARGUMENT]
+        if not args or not args[0].value.lower().startswith("tags:"):
+            return
+        duplicates = defaultdict(list)
+        for index, token in enumerate(args):
+            tags = token.value
+            col_start = token.col_offset
+            if index == 0:
+                tags = tags[len("tags:") :]
+                col_start += len("tags:")
+            for tag in tags.split(","):
+                tag_len = len(tag)
+                tag = tag.strip()
+                if not tag:
+                    continue
+                normalized = tag.lower().replace(" ", "")
+                subtoken = self._get_new_tag_token(tag, token.lineno, col_start)
+                col_start += tag_len + 1  # 1 for ,
+                duplicates[normalized].append(subtoken)
+                self.check_tag(subtoken, node)
+        self.check_duplicates(duplicates)
+
+    def _get_new_tag_token(self, tag_value: str, lineno: int, col_offset: int) -> Token:
+        """Create new token based on tag value."""
+        subtoken = Token(Token.ARGUMENT, tag_value)
+        subtoken.lineno = lineno
+        subtoken.col_offset = col_offset
+        return subtoken
 
     def visit_Keyword(self, node):  # noqa
         self.is_keyword = True
         super().generic_visit(node)
         self.is_keyword = False
 
     def check_tags(self, node):
@@ -284,36 +306,53 @@
                     line=nodes[0].lineno,
                     column=nodes[0].col_offset + 1,
                     node=duplicate,
                     col=duplicate.col_offset + 1,
                     end_col=duplicate.end_col_offset + 1,
                 )
 
-    def check_tag(self, tag, node):
-        if " " in tag.value:
+    def check_tag(self, tag_token, node):
+        var_found = False
+        substrings = []
+        after = tag_token.value
+        for match in variable_matcher.VariableMatches(tag_token.value, ignore_errors=True):
+            substrings.append(match.before)
+            var_found = var_found or bool(match.match)
+            after = match.after
+        substrings.append(after)
+        for substring in substrings:
+            if self.check_tag_substring(substring, tag_token, node):
+                break
+        normalized = tag_token.value.lower()
+        if not var_found and normalized.startswith("robot:") and normalized not in self.reserved_tags:
             self.report(
-                "tag-with-space",
-                tag=tag.value,
+                "tag-with-reserved-word",
+                tag=tag_token.value,
                 node=node,
-                lineno=tag.lineno,
-                col=tag.col_offset + 1,
-                end_col=tag.end_col_offset + 1,
+                lineno=tag_token.lineno,
+                col=tag_token.col_offset + 1,
+                end_col=tag_token.end_col_offset,
             )
-        if "OR" in tag.value or "AND" in tag.value:
-            self.report("tag-with-or-and", tag=tag.value, node=node, lineno=tag.lineno, col=tag.col_offset + 1)
-        normalized = tag.value.lower()
-        if normalized.startswith("robot:") and normalized not in self.reserved_tags:
+
+    def check_tag_substring(self, substring, tag, node) -> bool:
+        res = False
+        if " " in substring:
             self.report(
-                "tag-with-reserved-word",
+                "tag-with-space",
                 tag=tag.value,
                 node=node,
                 lineno=tag.lineno,
                 col=tag.col_offset + 1,
-                end_col=tag.end_col_offset,
+                end_col=tag.end_col_offset + 1,
             )
+            res = True
+        if "OR" in substring or "AND" in substring:
+            self.report("tag-with-or-and", tag=tag.value, node=node, lineno=tag.lineno, col=tag.col_offset + 1)
+            res = True
+        return res
 
 
 class TagScopeChecker(VisitorChecker):
     """Checker for tag scopes."""
 
     reports = (
         "could-be-test-tags",
```

### Comparing `robotframework-robocop-5.0.3/robocop/config.py` & `robotframework-robocop-5.0.4/robocop/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/exceptions.py` & `robotframework-robocop-5.0.4/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/files.py` & `robotframework-robocop-5.0.4/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/__init__.py` & `robotframework-robocop-5.0.4/robocop/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/compare_runs_report.py` & `robotframework-robocop-5.0.4/robocop/reports/compare_runs_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/file_stats_report.py` & `robotframework-robocop-5.0.4/robocop/reports/file_stats_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/json_report.py` & `robotframework-robocop-5.0.4/robocop/reports/json_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/return_status_report.py` & `robotframework-robocop-5.0.4/robocop/reports/return_status_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/robocop_version_report.py` & `robotframework-robocop-5.0.4/robocop/reports/robocop_version_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/rules_by_id_report.py` & `robotframework-robocop-5.0.4/robocop/reports/rules_by_id_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/rules_by_severity_report.py` & `robotframework-robocop-5.0.4/robocop/reports/rules_by_severity_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/sarif_report.py` & `robotframework-robocop-5.0.4/robocop/reports/sarif_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/time_taken_report.py` & `robotframework-robocop-5.0.4/robocop/reports/time_taken_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/reports/timestamp_report.py` & `robotframework-robocop-5.0.4/robocop/reports/timestamp_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/rules.py` & `robotframework-robocop-5.0.4/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/run.py` & `robotframework-robocop-5.0.4/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/__init__.py` & `robotframework-robocop-5.0.4/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/disablers.py` & `robotframework-robocop-5.0.4/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/file_types.py` & `robotframework-robocop-5.0.4/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/misc.py` & `robotframework-robocop-5.0.4/robocop/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,7 +366,15 @@
     diff = count - prev_count
     prefix = "+" if diff >= 0 else ""
     return prefix + str(diff)
 
 
 def get_plural_form(container):
     return "" if container == 1 else "s"
+
+
+def _is_var_scope_local(node) -> bool:
+    is_local = True
+    for option in node.get_tokens(Token.OPTION):
+        if "scope=" in option.value:
+            is_local = option.value.lower() == "scope=local"
+    return is_local
```

### Comparing `robotframework-robocop-5.0.3/robocop/utils/run_keywords.py` & `robotframework-robocop-5.0.4/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/variable_matcher.py` & `robotframework-robocop-5.0.4/robocop/utils/variable_matcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robocop/utils/version_matching.py` & `robotframework-robocop-5.0.4/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-5.0.4/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 5.0.3
+Version: 5.0.4
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
@@ -31,15 +31,15 @@
 License-File: LICENSE
 Requires-Dist: jinja2<4.0,>=3.0
 Requires-Dist: robotframework>=3.2.2
 Requires-Dist: pathspec<0.13,>=0.9
 Requires-Dist: tomli>=2.0.0
 Requires-Dist: pytz>=2022.7
 Requires-Dist: python-dateutil>=2.8.2
-Requires-Dist: platformdirs<4.2.0,>=3.2.0
+Requires-Dist: platformdirs<4.3.0,>=3.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: pytest-benchmark; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `robotframework-robocop-5.0.3/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-5.0.4/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-5.0.3/setup.py` & `robotframework-robocop-5.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     install_requires=[
         "jinja2>=3.0,<4.0",
         "robotframework>=3.2.2",
         "pathspec>=0.9,<0.13",
         "tomli>=2.0.0",
         "pytz>=2022.7",
         "python-dateutil>=2.8.2",
-        "platformdirs>=3.2.0,<4.2.0",
+        "platformdirs>=3.2.0,<4.3.0",
     ],
     extras_require={
         "dev": [
             "black",
             "coverage",
             "pytest",
             "pyyaml",
```

