# Comparing `tmp/hubrdvmairie-3.2.0.tar.gz` & `tmp/hubrdvmairie-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubrdvmairie-3.2.0.tar", last modified: Tue Mar 26 16:03:08 2024, max compression
+gzip compressed data, was "hubrdvmairie-3.3.0.tar", last modified: Wed Apr 10 13:39:32 2024, max compression
```

## Comparing `hubrdvmairie-3.2.0.tar` & `hubrdvmairie-3.3.0.tar`

### file list

```diff
@@ -1,78 +1,86 @@
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.635196 hubrdvmairie-3.2.0/
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1091 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/LICENSE
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2786 2024-03-26 16:03:08.635196 hubrdvmairie-3.2.0/PKG-INFO
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1416 2024-03-26 16:01:31.000000 hubrdvmairie-3.2.0/pyproject.toml
--rw-r--r--   0 w137219   (1000) w137219   (1000)       38 2024-03-26 16:03:08.635196 hubrdvmairie-3.2.0/setup.cfg
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/hubrdvmairie/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/__init__.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      516 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/controller.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/dependencies/
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1809 2023-12-15 14:38:00.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/dependencies/auth_token.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     4351 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/data.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)    11393 2024-03-15 15:03:36.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/external.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)    15294 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/internal.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     5788 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/time_slots.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     6543 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/websocket.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.615196 hubrdvmairie-3.2.0/src/hubrdvmairie/core/
--rw-r--r--   0 w137219   (1000) w137219   (1000)      142 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/core/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      903 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/core/config.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/core/errors.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.625196 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     3441 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/base.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1968 2024-01-17 14:01:53.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1196 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_editor_panorama.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2725 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_meeting_point.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1827 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_token_ants_to_editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1752 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_token_editor_to_ants.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.625196 hubrdvmairie-3.2.0/src/hubrdvmairie/db/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/db/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      892 2024-02-14 08:15:45.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/db/postgresdb.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      346 2024-02-14 08:15:45.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/db/postgresdb_utils.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2405 2024-02-14 08:15:45.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/db/schemas.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     6358 2024-02-14 08:15:45.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/db/utils.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.625196 hubrdvmairie-3.2.0/src/hubrdvmairie/logging/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/logging/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     3068 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/logging/app_logger.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1507 2024-01-17 14:00:43.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/logging/app_logger_formatter.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.625196 hubrdvmairie-3.2.0/src/hubrdvmairie/models/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      121 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/announcement.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      184 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/application.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      145 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/available_time_slot.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)    22012 2024-03-05 16:51:51.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2031 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor_model.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      656 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor_panorama.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      660 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/meeting_point.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1068 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/municipality.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      950 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/token_ants_to_editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      997 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/models/token_editor_to_ants.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.625196 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      422 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      693 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/editor_panorama.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      508 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/meeting_point.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      659 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/token_ants_to_editor.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      639 2024-01-17 14:00:11.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/token_editor_to_ants.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.635196 hubrdvmairie-3.2.0/src/hubrdvmairie/services/
--rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/__init__.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2310 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/data_validator.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      609 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/excel_helper.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2547 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/meeting_point_service.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     7647 2024-03-15 11:16:34.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/mock_data.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)      423 2024-02-14 08:15:45.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/panorama_service.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     1170 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/scheduled_functions.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2903 2024-01-31 14:32:39.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_meeting_points.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     4762 2023-09-26 10:45:56.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_meetings.py
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2632 2024-03-05 16:51:51.000000 hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_time_slots.py
-drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-03-26 16:03:08.635196 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2786 2024-03-26 16:03:08.000000 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/PKG-INFO
--rw-r--r--   0 w137219   (1000) w137219   (1000)     2523 2024-03-26 16:03:08.000000 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/SOURCES.txt
--rw-r--r--   0 w137219   (1000) w137219   (1000)        1 2024-03-26 16:03:08.000000 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/dependency_links.txt
--rw-r--r--   0 w137219   (1000) w137219   (1000)      415 2024-03-26 16:03:08.000000 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/requires.txt
--rw-r--r--   0 w137219   (1000) w137219   (1000)       13 2024-03-26 16:03:08.000000 hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/top_level.txt
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1091 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/LICENSE
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2786 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/PKG-INFO
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1416 2024-04-10 13:38:05.000000 hubrdvmairie-3.3.0/pyproject.toml
+-rw-r--r--   0 w137219   (1000) w137219   (1000)       38 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/setup.cfg
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.535657 hubrdvmairie-3.3.0/src/
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/__init__.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      516 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/controller.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/dependencies/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1809 2023-12-15 14:38:00.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/dependencies/auth_token.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)    12442 2024-04-10 13:08:33.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/data.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)    11393 2024-03-15 15:03:36.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/external.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)    15285 2024-04-04 11:46:38.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/internal.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     5788 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/time_slots.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     6543 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/websocket.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/core/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      142 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/core/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      903 2024-04-02 07:01:49.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/core/config.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/core/errors.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     3441 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/base.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2216 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_certified_municipality.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1968 2024-01-17 14:01:53.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1196 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_editor_panorama.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2725 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_meeting_point.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1827 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_token_ants_to_editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1752 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_token_editor_to_ants.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/db/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/db/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      892 2024-02-14 08:15:45.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/db/postgresdb.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      346 2024-02-14 08:15:45.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/db/postgresdb_utils.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2405 2024-02-14 08:15:45.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/db/schemas.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     6358 2024-02-14 08:15:45.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/db/utils.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.545657 hubrdvmairie-3.3.0/src/hubrdvmairie/logging/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/logging/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     3068 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/logging/app_logger.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1507 2024-01-17 14:00:43.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/logging/app_logger_formatter.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/src/hubrdvmairie/models/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      121 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/announcement.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      184 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/application.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      145 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/available_time_slot.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1411 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/certified_municipality.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)    22241 2024-04-04 11:46:38.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2031 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor_model.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      656 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor_panorama.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      660 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/meeting_point.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1068 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/municipality.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      950 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/token_ants_to_editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      997 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/models/token_editor_to_ants.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      730 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/certified_municipality.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      422 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      693 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/editor_panorama.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      508 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/meeting_point.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      659 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/token_ants_to_editor.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      639 2024-01-17 14:00:11.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/token_editor_to_ants.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/src/hubrdvmairie/services/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     3999 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/certified_municipality_service.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2310 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/data_validator.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      609 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/excel_helper.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2547 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/meeting_point_service.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     7647 2024-03-15 11:16:34.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/mock_data.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      423 2024-02-14 08:15:45.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/panorama_service.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     1170 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/scheduled_functions.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2903 2024-01-31 14:32:39.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_meeting_points.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     4762 2023-09-26 10:45:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_meetings.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2632 2024-03-05 16:51:51.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_time_slots.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/src/hubrdvmairie/utils/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        0 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/utils/__init__.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     3200 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/utils/departments.py
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      836 2024-04-10 12:37:56.000000 hubrdvmairie-3.3.0/src/hubrdvmairie/utils/utils.py
+drwxr-xr-x   0 w137219   (1000) w137219   (1000)        0 2024-04-10 13:39:32.555657 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2786 2024-04-10 13:39:32.000000 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/PKG-INFO
+-rw-r--r--   0 w137219   (1000) w137219   (1000)     2842 2024-04-10 13:39:32.000000 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/SOURCES.txt
+-rw-r--r--   0 w137219   (1000) w137219   (1000)        1 2024-04-10 13:39:32.000000 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/dependency_links.txt
+-rw-r--r--   0 w137219   (1000) w137219   (1000)      415 2024-04-10 13:39:32.000000 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/requires.txt
+-rw-r--r--   0 w137219   (1000) w137219   (1000)       13 2024-04-10 13:39:32.000000 hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/top_level.txt
```

### Comparing `hubrdvmairie-3.2.0/LICENSE` & `hubrdvmairie-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/PKG-INFO` & `hubrdvmairie-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubrdvmairie
-Version: 3.2.0
+Version: 3.3.0
 Summary: API de la plateforme de recherche de rendez-vous mairies
 Author-email: ANTS <ants-rdvmairie@interieur.gouv.fr>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hubrdvmairie-3.2.0/pyproject.toml` & `hubrdvmairie-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hubrdvmairie"
-version = "3.2.0"
+version = "3.3.0"
 description = "API de la plateforme de recherche de rendez-vous mairies"
 readme = "README.md"
 authors = [{ name = "ANTS", email = "ants-rdvmairie@interieur.gouv.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/controller.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/dependencies/auth_token.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/dependencies/auth_token.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/external.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/external.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/internal.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     elif name == "paris":
         for point in all_points:
             if point["name"] == "Service titres d'identité de Paris  Centre":
                 city = point
                 return city
     elif name == "marseille":
         for point in all_points:
-            if point["website"] == "https://troov.com/bmdp-desiree-clary/rendez-vous":
+            if point["name"] == "Mairie de Marseille : BMdP Désirée Clary":
                 city = point
                 return city
     else:
         for point in all_points:
             if point["decoded_city_name"] == name:
                 city = point
                 return city
```

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/time_slots.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/time_slots.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/controllers/routes/websocket.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/controllers/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/core/config.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/core/config.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/base.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/base.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_editor.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_editor.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_editor_panorama.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_editor_panorama.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_meeting_point.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_meeting_point.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_token_ants_to_editor.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_token_ants_to_editor.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/crud/crud_token_editor_to_ants.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/crud/crud_token_editor_to_ants.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/db/postgresdb.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/db/postgresdb.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/db/schemas.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/db/schemas.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/db/utils.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/db/utils.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/logging/app_logger.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/logging/app_logger.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/logging/app_logger_formatter.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/logging/app_logger_formatter.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,25 @@
                         raise Exception(
                             f"Status code not handled : {response.status_code}"
                         )
             except Exception as get_meeting_points_e:
                 if self.status:
                     self.status = False
                     self.api_down_datetime = datetime.now(tz=FRA_TZ)
-
                 _logger.error(
-                    "Error while getting meeting points for %s : %s",
-                    self.name,
-                    str(get_meeting_points_e),
-                    extra={"extra_info": {"type": "app", "editor_name": self.name}},
+                    "Error while getting meeting points",
+                    extra={
+                        "extra_info": {
+                            "type": "app",
+                            "editor_name": self.name,
+                            "category": "external_service",
+                            "endpoint": "getManagedMeetingPoints",
+                            "error": str(get_meeting_points_e),
+                        }
+                    },
                 )
 
                 retry_thread = [
                     th
                     for th in threading.enumerate()
                     if th.name == f"retry-get-managed-{self.name}"
                 ]
```

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor_model.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor_model.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/editor_panorama.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/editor_panorama.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/meeting_point.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/meeting_point.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/municipality.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/municipality.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/token_ants_to_editor.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/token_ants_to_editor.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/models/token_editor_to_ants.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/models/token_editor_to_ants.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/editor_panorama.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/editor_panorama.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/token_ants_to_editor.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/token_ants_to_editor.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/schemas/token_editor_to_ants.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/schemas/token_editor_to_ants.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/data_validator.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/data_validator.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/excel_helper.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/excel_helper.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/meeting_point_service.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/meeting_point_service.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/mock_data.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/mock_data.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/scheduled_functions.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/scheduled_functions.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_meeting_points.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_meeting_points.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_meetings.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_meetings.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie/services/search_time_slots.py` & `hubrdvmairie-3.3.0/src/hubrdvmairie/services/search_time_slots.py`

 * *Files identical despite different names*

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/PKG-INFO` & `hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubrdvmairie
-Version: 3.2.0
+Version: 3.3.0
 Summary: API de la plateforme de recherche de rendez-vous mairies
 Author-email: ANTS <ants-rdvmairie@interieur.gouv.fr>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hubrdvmairie-3.2.0/src/hubrdvmairie.egg-info/SOURCES.txt` & `hubrdvmairie-3.3.0/src/hubrdvmairie.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/hubrdvmairie/controllers/routes/time_slots.py
 src/hubrdvmairie/controllers/routes/websocket.py
 src/hubrdvmairie/core/__init__.py
 src/hubrdvmairie/core/config.py
 src/hubrdvmairie/core/errors.py
 src/hubrdvmairie/crud/__init__.py
 src/hubrdvmairie/crud/base.py
+src/hubrdvmairie/crud/crud_certified_municipality.py
 src/hubrdvmairie/crud/crud_editor.py
 src/hubrdvmairie/crud/crud_editor_panorama.py
 src/hubrdvmairie/crud/crud_meeting_point.py
 src/hubrdvmairie/crud/crud_token_ants_to_editor.py
 src/hubrdvmairie/crud/crud_token_editor_to_ants.py
 src/hubrdvmairie/db/__init__.py
 src/hubrdvmairie/db/postgresdb.py
@@ -33,30 +34,36 @@
 src/hubrdvmairie/logging/__init__.py
 src/hubrdvmairie/logging/app_logger.py
 src/hubrdvmairie/logging/app_logger_formatter.py
 src/hubrdvmairie/models/__init__.py
 src/hubrdvmairie/models/announcement.py
 src/hubrdvmairie/models/application.py
 src/hubrdvmairie/models/available_time_slot.py
+src/hubrdvmairie/models/certified_municipality.py
 src/hubrdvmairie/models/editor.py
 src/hubrdvmairie/models/editor_model.py
 src/hubrdvmairie/models/editor_panorama.py
 src/hubrdvmairie/models/meeting_point.py
 src/hubrdvmairie/models/municipality.py
 src/hubrdvmairie/models/token_ants_to_editor.py
 src/hubrdvmairie/models/token_editor_to_ants.py
 src/hubrdvmairie/schemas/__init__.py
+src/hubrdvmairie/schemas/certified_municipality.py
 src/hubrdvmairie/schemas/editor.py
 src/hubrdvmairie/schemas/editor_panorama.py
 src/hubrdvmairie/schemas/meeting_point.py
 src/hubrdvmairie/schemas/token_ants_to_editor.py
 src/hubrdvmairie/schemas/token_editor_to_ants.py
 src/hubrdvmairie/services/__init__.py
+src/hubrdvmairie/services/certified_municipality_service.py
 src/hubrdvmairie/services/data_validator.py
 src/hubrdvmairie/services/excel_helper.py
 src/hubrdvmairie/services/meeting_point_service.py
 src/hubrdvmairie/services/mock_data.py
 src/hubrdvmairie/services/panorama_service.py
 src/hubrdvmairie/services/scheduled_functions.py
 src/hubrdvmairie/services/search_meeting_points.py
 src/hubrdvmairie/services/search_meetings.py
-src/hubrdvmairie/services/search_time_slots.py
+src/hubrdvmairie/services/search_time_slots.py
+src/hubrdvmairie/utils/__init__.py
+src/hubrdvmairie/utils/departments.py
+src/hubrdvmairie/utils/utils.py
```

