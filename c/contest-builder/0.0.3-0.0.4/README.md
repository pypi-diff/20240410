# Comparing `tmp/contest-builder-0.0.3.tar.gz` & `tmp/contest-builder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contest-builder-0.0.3.tar", last modified: Tue Apr  9 14:15:36 2024, max compression
+gzip compressed data, was "contest-builder-0.0.4.tar", last modified: Tue Apr  9 14:34:50 2024, max compression
```

## Comparing `contest-builder-0.0.3.tar` & `contest-builder-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1077 2023-08-17 14:07:48.000000 contest-builder-0.0.3/LICENSE
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      249 2024-04-09 14:14:51.000000 contest-builder-0.0.3/MANIFEST.in
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 14:15:36.699047 contest-builder-0.0.3/PKG-INFO
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.3/README.md
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      891 2024-04-09 14:15:30.000000 contest-builder-0.0.3/pyproject.toml
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2024-04-09 14:15:36.699047 contest-builder-0.0.3/setup.cfg
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.3/src/contest_builder/README.md
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:37:21.000000 contest-builder-0.0.3/src/contest_builder/__init__.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1475 2024-04-09 13:46:30.000000 contest-builder-0.0.3/src/contest_builder/__main__.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/configs/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       53 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/configs/main.json
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:38:07.000000 contest-builder-0.0.3/src/contest_builder/py.typed
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/actions/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      993 2024-04-09 13:46:56.000000 contest-builder-0.0.3/src/contest_builder/src/actions/problem_actions.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/executors/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1496 2024-04-09 13:47:24.000000 contest-builder-0.0.3/src/contest_builder/src/executors/cpp_executor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1337 2024-04-09 13:48:11.000000 contest-builder-0.0.3/src/contest_builder/src/executors/executor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      709 2024-04-09 13:48:09.000000 contest-builder-0.0.3/src/contest_builder/src/executors/program_excecutor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1000 2024-04-09 13:48:07.000000 contest-builder-0.0.3/src/contest_builder/src/executors/python_executor.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/generators/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2088 2024-04-09 13:48:00.000000 contest-builder-0.0.3/src/contest_builder/src/generators/contest_generator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1549 2024-04-09 13:48:04.000000 contest-builder-0.0.3/src/contest_builder/src/generators/problem_generator.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/command/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      412 2024-04-09 13:48:20.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/command/command_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/config/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      246 2024-04-09 14:06:02.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/config/config.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1544 2024-04-09 13:48:43.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/config/local_config.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      226 2024-04-08 13:18:04.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/config/templates.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/file/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1994 2024-04-09 13:49:30.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/file/file_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/folder/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      294 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/folder/folder_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/model/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/model/finders/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:48.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/model/finders/language_finder.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:58.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/model/finders/provider_finder.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      345 2024-04-09 13:50:04.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/model/language_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      162 2024-04-08 11:53:02.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/model/model_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1153 2024-04-09 13:50:12.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/model/problem_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1502 2024-04-09 13:31:59.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/arg_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      363 2024-04-09 13:50:31.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/cat_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      930 2023-09-12 13:44:59.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/single_process.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/helpers/utils/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      259 2023-09-12 12:23:28.000000 contest-builder-0.0.3/src/contest_builder/src/helpers/utils/timer.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.695047 contest-builder-0.0.3/src/contest_builder/src/mediators/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1090 2024-04-09 13:50:46.000000 contest-builder-0.0.3/src/contest_builder/src/mediators/contest_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1316 2024-04-09 13:50:50.000000 contest-builder-0.0.3/src/contest_builder/src/mediators/execution_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      995 2024-04-09 13:50:55.000000 contest-builder-0.0.3/src/contest_builder/src/mediators/init_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1204 2024-04-09 13:50:59.000000 contest-builder-0.0.3/src/contest_builder/src/mediators/problem_mediator.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder/src/models/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1945 2024-04-09 13:51:05.000000 contest-builder-0.0.3/src/contest_builder/src/models/contest.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1358 2024-04-08 14:41:19.000000 contest-builder-0.0.3/src/contest_builder/src/models/language.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1995 2024-04-09 13:51:12.000000 contest-builder-0.0.3/src/contest_builder/src/models/problem.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      639 2024-04-08 14:42:03.000000 contest-builder-0.0.3/src/contest_builder/src/models/provider.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder/src/types/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)       86 2023-09-11 19:49:53.000000 contest-builder-0.0.3/src/contest_builder/src/types/languages.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      129 2023-08-30 01:48:44.000000 contest-builder-0.0.3/src/contest_builder/src/types/name_types.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      123 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/src/types/providers.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder/templates/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder/templates/codeforces/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2522 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/templates/codeforces/template.cpp
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1161 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/templates/codeforces/template.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder/templates/leetcode/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2686 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/templates/leetcode/template.cpp
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      856 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/templates/leetcode/template.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2354 2023-10-22 17:06:27.000000 contest-builder-0.0.3/src/contest_builder/templates/template.json
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:15:36.699047 contest-builder-0.0.3/src/contest_builder.egg-info/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/PKG-INFO
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2436 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       66 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/entry_points.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       33 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/requires.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2024-04-09 14:15:36.000000 contest-builder-0.0.3/src/contest_builder.egg-info/top_level.txt
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.146805 contest-builder-0.0.4/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1077 2023-08-17 14:07:48.000000 contest-builder-0.0.4/LICENSE
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      249 2024-04-09 14:14:51.000000 contest-builder-0.0.4/MANIFEST.in
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     6104 2024-04-09 14:34:50.146805 contest-builder-0.0.4/PKG-INFO
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     4191 2024-04-09 14:33:27.000000 contest-builder-0.0.4/README.md
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      891 2024-04-09 14:34:33.000000 contest-builder-0.0.4/pyproject.toml
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2024-04-09 14:34:50.146805 contest-builder-0.0.4/setup.cfg
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     4191 2024-04-09 14:33:27.000000 contest-builder-0.0.4/src/contest_builder/README.md
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:37:21.000000 contest-builder-0.0.4/src/contest_builder/__init__.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1475 2024-04-09 13:46:30.000000 contest-builder-0.0.4/src/contest_builder/__main__.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/configs/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       53 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/configs/main.json
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:38:07.000000 contest-builder-0.0.4/src/contest_builder/py.typed
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/actions/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      993 2024-04-09 13:46:56.000000 contest-builder-0.0.4/src/contest_builder/src/actions/problem_actions.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/executors/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1496 2024-04-09 13:47:24.000000 contest-builder-0.0.4/src/contest_builder/src/executors/cpp_executor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1337 2024-04-09 13:48:11.000000 contest-builder-0.0.4/src/contest_builder/src/executors/executor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      709 2024-04-09 13:48:09.000000 contest-builder-0.0.4/src/contest_builder/src/executors/program_excecutor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1000 2024-04-09 13:48:07.000000 contest-builder-0.0.4/src/contest_builder/src/executors/python_executor.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/generators/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2088 2024-04-09 13:48:00.000000 contest-builder-0.0.4/src/contest_builder/src/generators/contest_generator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1549 2024-04-09 13:48:04.000000 contest-builder-0.0.4/src/contest_builder/src/generators/problem_generator.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/command/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      412 2024-04-09 13:48:20.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/command/command_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/config/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      246 2024-04-09 14:06:02.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/config/config.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1544 2024-04-09 13:48:43.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/config/local_config.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      226 2024-04-08 13:18:04.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/config/templates.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/file/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1994 2024-04-09 13:49:30.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/file/file_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/folder/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      294 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/folder/folder_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/model/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/model/finders/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:48.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/model/finders/language_finder.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:58.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/model/finders/provider_finder.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      345 2024-04-09 13:50:04.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/model/language_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      162 2024-04-08 11:53:02.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/model/model_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1153 2024-04-09 13:50:12.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/model/problem_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1502 2024-04-09 13:31:59.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/arg_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      363 2024-04-09 13:50:31.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/cat_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      930 2023-09-12 13:44:59.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/single_process.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/helpers/utils/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      259 2023-09-12 12:23:28.000000 contest-builder-0.0.4/src/contest_builder/src/helpers/utils/timer.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/mediators/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1090 2024-04-09 13:50:46.000000 contest-builder-0.0.4/src/contest_builder/src/mediators/contest_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1316 2024-04-09 13:50:50.000000 contest-builder-0.0.4/src/contest_builder/src/mediators/execution_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      995 2024-04-09 13:50:55.000000 contest-builder-0.0.4/src/contest_builder/src/mediators/init_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1204 2024-04-09 13:50:59.000000 contest-builder-0.0.4/src/contest_builder/src/mediators/problem_mediator.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/models/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1945 2024-04-09 13:51:05.000000 contest-builder-0.0.4/src/contest_builder/src/models/contest.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1358 2024-04-08 14:41:19.000000 contest-builder-0.0.4/src/contest_builder/src/models/language.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1995 2024-04-09 13:51:12.000000 contest-builder-0.0.4/src/contest_builder/src/models/problem.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      639 2024-04-08 14:42:03.000000 contest-builder-0.0.4/src/contest_builder/src/models/provider.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/src/types/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)       86 2023-09-11 19:49:53.000000 contest-builder-0.0.4/src/contest_builder/src/types/languages.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      129 2023-08-30 01:48:44.000000 contest-builder-0.0.4/src/contest_builder/src/types/name_types.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      123 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/src/types/providers.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/templates/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/templates/codeforces/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2522 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/templates/codeforces/template.cpp
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1161 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/templates/codeforces/template.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder/templates/leetcode/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2686 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/templates/leetcode/template.cpp
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      856 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/templates/leetcode/template.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2354 2023-10-22 17:06:27.000000 contest-builder-0.0.4/src/contest_builder/templates/template.json
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:34:50.142805 contest-builder-0.0.4/src/contest_builder.egg-info/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     6104 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2436 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       66 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       33 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/requires.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2024-04-09 14:34:50.000000 contest-builder-0.0.4/src/contest_builder.egg-info/top_level.txt
```

### Comparing `contest-builder-0.0.3/LICENSE` & `contest-builder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/PKG-INFO` & `contest-builder-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contest-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Competetive Programming Management Tool
 Author-email: shamir0xe <shamir0xe@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Amirhossein Shapoori
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 License-File: LICENSE
 Requires-Dist: pylib-0xe>=0.0.5
 Provides-Extra: dev
 Requires-Dist: unittest; extra == "dev"
 
 # Contest Builder
 
-![Python](https://img.shields.io/badge/Python-3.6%2B-blue)
+![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 Contest Builder is a Python tool designed to simplify the process of managing programming contest solutions by providing a structured workflow for organizing, compiling, and testing code.
 
 ## Features
 
 - Quickly generate the folder and file structure for a contest's problems.
@@ -56,14 +56,15 @@
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Configuration](#configuration)
 * [Contributing](#contributing)
+* [License](#license)
 
 <!-- vim-markdown-toc -->
 
 ## Installation
 
 You can install Contest Builder via pip:
 
@@ -103,40 +104,67 @@
 - `--problem_cnt <problem_count>`
   Specify the number of problems.
 - `--language <programming_language>`
   Specify the language you are using at this contest if it differs from the default value.
 - `--name_type <folders_name_type>`
   It can be `alphabetical`, `numerical`, or `roman`.
 
+For example you want to create a codeforces contest with 8 problems, using python language. in order to do this, you
+can simply write:
+
+```bash
+contest-builder --name "Codeforces Round 938 (Div. 3)" --problem_cnt 8 --language py --provider cf
+```
+
+You can set your desired abbreviations for languages and contest providers in the `cb-config`.
+
 2. Compiling and Running Solutions
 
 To compile and run a solution for a specific problem, use the contest-builder command with the --run option:
 
 ```bash
 contest-builder --run <problem_name>
 ```
 
-This will compile and execute the solution file for the specified problem. Also if you are located in the
-problem's folder, you can discard the `<problem_name>` and just pass the `--run` option to compile and execute the code.
+This will detect the language you've chosen to write the code, and then
+compiles and executes the solution based on the way it's provided in the
+`cb-config`. If you are located in the
+problem's folder, you can discard the `<problem_name>` and just pass the `--run` option.
+
+Example:
+
+```bash
+contest-builder --run a
+```
 
 3. Creating Structure for Single Problem
 
    You can also create the folder and file structure for a single problem using the contest-builder command with the `--problem` option:
 
 ```bash
-contest-builder --problem <problem_name>
+contest-builder --problem --name <problem_name>
 ```
 
 This will generate the necessary files and directories for the specified problem.
 
+Example:
+
+```bash
+contest-builder --problem --name "Random Problem" --language seepp --provider lc
+```
+
+it will generate `leetcode/problemset/random-problem/random-problem.cpp` and it's
+corresponding input as well.
+
 ## Configuration
 
 Contest Builder allows you to customize templates for generating solution files. You can modify these templates according to your preferences by editing the template files located in the templates directory.
 
 Also you need to edit the `compile` and `run` sections in the config file as you want to be done.
 
 ## Contributing
 
 Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.
 
-License
-Contest Builder is licensed under the MIT License. See the LICENSE file for details.
+## License
+
+Contest Builder is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `contest-builder-0.0.3/README.md` & `contest-builder-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Contest Builder
 
-![Python](https://img.shields.io/badge/Python-3.6%2B-blue)
+![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 Contest Builder is a Python tool designed to simplify the process of managing programming contest solutions by providing a structured workflow for organizing, compiling, and testing code.
 
 ## Features
 
 - Quickly generate the folder and file structure for a contest's problems.
@@ -16,14 +16,15 @@
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Configuration](#configuration)
 * [Contributing](#contributing)
+* [License](#license)
 
 <!-- vim-markdown-toc -->
 
 ## Installation
 
 You can install Contest Builder via pip:
 
@@ -63,40 +64,67 @@
 - `--problem_cnt <problem_count>`
   Specify the number of problems.
 - `--language <programming_language>`
   Specify the language you are using at this contest if it differs from the default value.
 - `--name_type <folders_name_type>`
   It can be `alphabetical`, `numerical`, or `roman`.
 
+For example you want to create a codeforces contest with 8 problems, using python language. in order to do this, you
+can simply write:
+
+```bash
+contest-builder --name "Codeforces Round 938 (Div. 3)" --problem_cnt 8 --language py --provider cf
+```
+
+You can set your desired abbreviations for languages and contest providers in the `cb-config`.
+
 2. Compiling and Running Solutions
 
 To compile and run a solution for a specific problem, use the contest-builder command with the --run option:
 
 ```bash
 contest-builder --run <problem_name>
 ```
 
-This will compile and execute the solution file for the specified problem. Also if you are located in the
-problem's folder, you can discard the `<problem_name>` and just pass the `--run` option to compile and execute the code.
+This will detect the language you've chosen to write the code, and then
+compiles and executes the solution based on the way it's provided in the
+`cb-config`. If you are located in the
+problem's folder, you can discard the `<problem_name>` and just pass the `--run` option.
+
+Example:
+
+```bash
+contest-builder --run a
+```
 
 3. Creating Structure for Single Problem
 
    You can also create the folder and file structure for a single problem using the contest-builder command with the `--problem` option:
 
 ```bash
-contest-builder --problem <problem_name>
+contest-builder --problem --name <problem_name>
 ```
 
 This will generate the necessary files and directories for the specified problem.
 
+Example:
+
+```bash
+contest-builder --problem --name "Random Problem" --language seepp --provider lc
+```
+
+it will generate `leetcode/problemset/random-problem/random-problem.cpp` and it's
+corresponding input as well.
+
 ## Configuration
 
 Contest Builder allows you to customize templates for generating solution files. You can modify these templates according to your preferences by editing the template files located in the templates directory.
 
 Also you need to edit the `compile` and `run` sections in the config file as you want to be done.
 
 ## Contributing
 
 Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.
 
-License
-Contest Builder is licensed under the MIT License. See the LICENSE file for details.
+## License
+
+Contest Builder is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `contest-builder-0.0.3/pyproject.toml` & `contest-builder-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "contest-builder"
-version = "0.0.3"
+version = "0.0.4"
 description = "Competetive Programming Management Tool"
 readme = "README.md"
 authors = [{ name = "shamir0xe", email = "shamir0xe@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `contest-builder-0.0.3/src/contest_builder/README.md` & `contest-builder-0.0.4/src/contest_builder/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Contest Builder
 
-![Python](https://img.shields.io/badge/Python-3.6%2B-blue)
+![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 Contest Builder is a Python tool designed to simplify the process of managing programming contest solutions by providing a structured workflow for organizing, compiling, and testing code.
 
 ## Features
 
 - Quickly generate the folder and file structure for a contest's problems.
@@ -16,14 +16,15 @@
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Configuration](#configuration)
 * [Contributing](#contributing)
+* [License](#license)
 
 <!-- vim-markdown-toc -->
 
 ## Installation
 
 You can install Contest Builder via pip:
 
@@ -63,40 +64,67 @@
 - `--problem_cnt <problem_count>`
   Specify the number of problems.
 - `--language <programming_language>`
   Specify the language you are using at this contest if it differs from the default value.
 - `--name_type <folders_name_type>`
   It can be `alphabetical`, `numerical`, or `roman`.
 
+For example you want to create a codeforces contest with 8 problems, using python language. in order to do this, you
+can simply write:
+
+```bash
+contest-builder --name "Codeforces Round 938 (Div. 3)" --problem_cnt 8 --language py --provider cf
+```
+
+You can set your desired abbreviations for languages and contest providers in the `cb-config`.
+
 2. Compiling and Running Solutions
 
 To compile and run a solution for a specific problem, use the contest-builder command with the --run option:
 
 ```bash
 contest-builder --run <problem_name>
 ```
 
-This will compile and execute the solution file for the specified problem. Also if you are located in the
-problem's folder, you can discard the `<problem_name>` and just pass the `--run` option to compile and execute the code.
+This will detect the language you've chosen to write the code, and then
+compiles and executes the solution based on the way it's provided in the
+`cb-config`. If you are located in the
+problem's folder, you can discard the `<problem_name>` and just pass the `--run` option.
+
+Example:
+
+```bash
+contest-builder --run a
+```
 
 3. Creating Structure for Single Problem
 
    You can also create the folder and file structure for a single problem using the contest-builder command with the `--problem` option:
 
 ```bash
-contest-builder --problem <problem_name>
+contest-builder --problem --name <problem_name>
 ```
 
 This will generate the necessary files and directories for the specified problem.
 
+Example:
+
+```bash
+contest-builder --problem --name "Random Problem" --language seepp --provider lc
+```
+
+it will generate `leetcode/problemset/random-problem/random-problem.cpp` and it's
+corresponding input as well.
+
 ## Configuration
 
 Contest Builder allows you to customize templates for generating solution files. You can modify these templates according to your preferences by editing the template files located in the templates directory.
 
 Also you need to edit the `compile` and `run` sections in the config file as you want to be done.
 
 ## Contributing
 
 Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.
 
-License
-Contest Builder is licensed under the MIT License. See the LICENSE file for details.
+## License
+
+Contest Builder is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `contest-builder-0.0.3/src/contest_builder/__main__.py` & `contest-builder-0.0.4/src/contest_builder/__main__.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/actions/problem_actions.py` & `contest-builder-0.0.4/src/contest_builder/src/actions/problem_actions.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/executors/cpp_executor.py` & `contest-builder-0.0.4/src/contest_builder/src/executors/cpp_executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/executors/executor.py` & `contest-builder-0.0.4/src/contest_builder/src/executors/executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/executors/program_excecutor.py` & `contest-builder-0.0.4/src/contest_builder/src/executors/program_excecutor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/executors/python_executor.py` & `contest-builder-0.0.4/src/contest_builder/src/executors/python_executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/generators/contest_generator.py` & `contest-builder-0.0.4/src/contest_builder/src/generators/contest_generator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/generators/problem_generator.py` & `contest-builder-0.0.4/src/contest_builder/src/generators/problem_generator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/config/local_config.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/config/local_config.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/file/file_helper.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/file/file_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/model/finders/language_finder.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/model/finders/language_finder.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/model/finders/provider_finder.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/model/finders/provider_finder.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/model/problem_helper.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/model/problem_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/arg_helper.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/arg_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/helpers/terminal/single_process.py` & `contest-builder-0.0.4/src/contest_builder/src/helpers/terminal/single_process.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/mediators/contest_mediator.py` & `contest-builder-0.0.4/src/contest_builder/src/mediators/contest_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/mediators/execution_mediator.py` & `contest-builder-0.0.4/src/contest_builder/src/mediators/execution_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/mediators/init_mediator.py` & `contest-builder-0.0.4/src/contest_builder/src/mediators/init_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/mediators/problem_mediator.py` & `contest-builder-0.0.4/src/contest_builder/src/mediators/problem_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/models/contest.py` & `contest-builder-0.0.4/src/contest_builder/src/models/contest.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/models/language.py` & `contest-builder-0.0.4/src/contest_builder/src/models/language.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/models/problem.py` & `contest-builder-0.0.4/src/contest_builder/src/models/problem.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/src/models/provider.py` & `contest-builder-0.0.4/src/contest_builder/src/models/provider.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/templates/codeforces/template.cpp` & `contest-builder-0.0.4/src/contest_builder/templates/codeforces/template.cpp`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/templates/codeforces/template.py` & `contest-builder-0.0.4/src/contest_builder/templates/codeforces/template.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/templates/leetcode/template.cpp` & `contest-builder-0.0.4/src/contest_builder/templates/leetcode/template.cpp`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/templates/leetcode/template.py` & `contest-builder-0.0.4/src/contest_builder/templates/leetcode/template.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder/templates/template.json` & `contest-builder-0.0.4/src/contest_builder/templates/template.json`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.3/src/contest_builder.egg-info/PKG-INFO` & `contest-builder-0.0.4/src/contest_builder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contest-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Competetive Programming Management Tool
 Author-email: shamir0xe <shamir0xe@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Amirhossein Shapoori
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 License-File: LICENSE
 Requires-Dist: pylib-0xe>=0.0.5
 Provides-Extra: dev
 Requires-Dist: unittest; extra == "dev"
 
 # Contest Builder
 
-![Python](https://img.shields.io/badge/Python-3.6%2B-blue)
+![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 Contest Builder is a Python tool designed to simplify the process of managing programming contest solutions by providing a structured workflow for organizing, compiling, and testing code.
 
 ## Features
 
 - Quickly generate the folder and file structure for a contest's problems.
@@ -56,14 +56,15 @@
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Configuration](#configuration)
 * [Contributing](#contributing)
+* [License](#license)
 
 <!-- vim-markdown-toc -->
 
 ## Installation
 
 You can install Contest Builder via pip:
 
@@ -103,40 +104,67 @@
 - `--problem_cnt <problem_count>`
   Specify the number of problems.
 - `--language <programming_language>`
   Specify the language you are using at this contest if it differs from the default value.
 - `--name_type <folders_name_type>`
   It can be `alphabetical`, `numerical`, or `roman`.
 
+For example you want to create a codeforces contest with 8 problems, using python language. in order to do this, you
+can simply write:
+
+```bash
+contest-builder --name "Codeforces Round 938 (Div. 3)" --problem_cnt 8 --language py --provider cf
+```
+
+You can set your desired abbreviations for languages and contest providers in the `cb-config`.
+
 2. Compiling and Running Solutions
 
 To compile and run a solution for a specific problem, use the contest-builder command with the --run option:
 
 ```bash
 contest-builder --run <problem_name>
 ```
 
-This will compile and execute the solution file for the specified problem. Also if you are located in the
-problem's folder, you can discard the `<problem_name>` and just pass the `--run` option to compile and execute the code.
+This will detect the language you've chosen to write the code, and then
+compiles and executes the solution based on the way it's provided in the
+`cb-config`. If you are located in the
+problem's folder, you can discard the `<problem_name>` and just pass the `--run` option.
+
+Example:
+
+```bash
+contest-builder --run a
+```
 
 3. Creating Structure for Single Problem
 
    You can also create the folder and file structure for a single problem using the contest-builder command with the `--problem` option:
 
 ```bash
-contest-builder --problem <problem_name>
+contest-builder --problem --name <problem_name>
 ```
 
 This will generate the necessary files and directories for the specified problem.
 
+Example:
+
+```bash
+contest-builder --problem --name "Random Problem" --language seepp --provider lc
+```
+
+it will generate `leetcode/problemset/random-problem/random-problem.cpp` and it's
+corresponding input as well.
+
 ## Configuration
 
 Contest Builder allows you to customize templates for generating solution files. You can modify these templates according to your preferences by editing the template files located in the templates directory.
 
 Also you need to edit the `compile` and `run` sections in the config file as you want to be done.
 
 ## Contributing
 
 Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.
 
-License
-Contest Builder is licensed under the MIT License. See the LICENSE file for details.
+## License
+
+Contest Builder is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `contest-builder-0.0.3/src/contest_builder.egg-info/SOURCES.txt` & `contest-builder-0.0.4/src/contest_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

