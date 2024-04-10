# Comparing `tmp/digitalhub-core-0.3.0.tar.gz` & `tmp/digitalhub-core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-core-0.3.0.tar", last modified: Wed Mar 27 09:37:38 2024, max compression
+gzip compressed data, was "digitalhub-core-0.3.1.tar", last modified: Wed Apr 10 08:28:29 2024, max compression
```

## Comparing `digitalhub-core-0.3.0.tar` & `digitalhub-core-0.3.1.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.456686 digitalhub-core-0.3.0/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-core-0.3.0/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14609 2024-03-27 09:37:38.456686 digitalhub-core-0.3.0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       84 2023-11-17 11:56:29.000000 digitalhub-core-0.3.0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.436686 digitalhub-core-0.3.0/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1263 2024-03-25 10:43:28.000000 digitalhub-core-0.3.0/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.436686 digitalhub-core-0.3.0/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1948 2024-02-21 12:33:19.000000 digitalhub-core-0.3.0/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.436686 digitalhub-core-0.3.0/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub-core-0.3.0/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1194 2024-03-19 15:41:29.000000 digitalhub-core-0.3.0/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8183 2024-03-22 09:44:14.000000 digitalhub-core-0.3.0/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14594 2024-03-26 12:06:44.000000 digitalhub-core-0.3.0/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.436686 digitalhub-core-0.3.0/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub-core-0.3.0/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2803 2024-03-19 15:49:55.000000 digitalhub-core-0.3.0/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.436686 digitalhub-core-0.3.0/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.440686 digitalhub-core-0.3.0/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2677 2024-03-12 16:39:31.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2403 2024-03-07 10:37:33.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1785 2024-02-15 12:11:01.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2164 2024-03-11 14:15:28.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.440686 digitalhub-core-0.3.0/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3239 2024-03-25 10:43:28.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2972 2024-03-25 10:43:28.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3173 2024-03-25 10:43:28.000000 digitalhub-core-0.3.0/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.440686 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13406 2024-03-12 16:39:31.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:13:38.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-03-07 15:14:39.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:14.000000 digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.440686 digitalhub-core-0.3.0/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16093 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:01.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1495 2024-03-19 10:59:21.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub-core-0.3.0/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.444686 digitalhub-core-0.3.0/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21687 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      866 2024-01-31 09:16:02.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub-core-0.3.0/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      710 2024-03-07 13:44:22.000000 digitalhub-core-0.3.0/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.444686 digitalhub-core-0.3.0/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14237 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      825 2024-01-31 09:16:02.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-03-22 13:57:11.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub-core-0.3.0/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.444686 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6140 2024-03-25 12:43:57.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8267 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1103 2024-02-06 10:40:16.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.448686 digitalhub-core-0.3.0/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6890 2024-03-12 16:39:31.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1106 2024-02-06 10:49:57.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub-core-0.3.0/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.448686 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5606 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10387 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      828 2024-01-31 09:16:02.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5084 2024-03-19 10:03:54.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub-core-0.3.0/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.448686 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6036 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6960 2024-03-12 16:39:31.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:02.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      373 2024-02-15 09:49:55.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub-core-0.3.0/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.452686 digitalhub-core-0.3.0/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub-core-0.3.0/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3963 2024-03-01 09:41:58.000000 digitalhub-core-0.3.0/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2233 2024-02-21 08:40:16.000000 digitalhub-core-0.3.0/digitalhub_core/runtimes/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      640 2024-02-01 10:45:50.000000 digitalhub-core-0.3.0/digitalhub_core/runtimes/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.452686 digitalhub-core-0.3.0/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-03-25 10:43:29.000000 digitalhub-core-0.3.0/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.452686 digitalhub-core-0.3.0/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-01-03 08:29:18.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-03-12 13:41:08.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-01-03 08:29:18.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-01-03 08:29:18.000000 digitalhub-core-0.3.0/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.452686 digitalhub-core-0.3.0/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.0/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub-core-0.3.0/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub-core-0.3.0/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4547 2024-03-12 16:38:39.000000 digitalhub-core-0.3.0/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2331 2024-02-15 10:46:43.000000 digitalhub-core-0.3.0/digitalhub_core/utils/import_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub-core-0.3.0/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub-core-0.3.0/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      723 2024-01-15 09:08:25.000000 digitalhub-core-0.3.0/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-03-27 09:37:38.452686 digitalhub-core-0.3.0/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14609 2024-03-27 09:37:38.000000 digitalhub-core-0.3.0/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3950 2024-03-27 09:37:38.000000 digitalhub-core-0.3.0/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-03-27 09:37:38.000000 digitalhub-core-0.3.0/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      237 2024-03-27 09:37:38.000000 digitalhub-core-0.3.0/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-03-27 09:37:38.000000 digitalhub-core-0.3.0/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1706 2024-03-27 09:35:37.000000 digitalhub-core-0.3.0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-03-27 09:37:38.456686 digitalhub-core-0.3.0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-core-0.3.1/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       84 2023-11-17 11:56:29.000000 digitalhub-core-0.3.1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.851790 digitalhub-core-0.3.1/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1263 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1948 2024-02-21 12:33:19.000000 digitalhub-core-0.3.1/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1194 2024-03-19 15:41:29.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8192 2024-04-03 11:07:40.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15046 2024-04-04 07:48:11.000000 digitalhub-core-0.3.1/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.855790 digitalhub-core-0.3.1/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub-core-0.3.1/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2803 2024-03-19 15:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3099 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2581 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1785 2024-02-15 12:11:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2164 2024-03-11 14:15:28.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3239 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2991 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3173 2024-04-10 08:00:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.859790 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13513 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:13:38.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-03-07 15:14:39.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:14.000000 digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16241 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-08 12:53:09.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub-core-0.3.1/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21767 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      866 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub-core-0.3.1/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      710 2024-03-07 13:44:22.000000 digitalhub-core-0.3.1/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.863790 digitalhub-core-0.3.1/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14263 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      825 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-03-22 13:57:11.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub-core-0.3.1/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8374 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1103 2024-02-06 10:40:16.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub-core-0.3.1/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/services/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6997 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1106 2024-02-06 10:49:57.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub-core-0.3.1/digitalhub_core/entities/services/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.867790 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5606 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10494 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      828 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5084 2024-03-19 10:03:54.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub-core-0.3.1/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6083 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7180 2024-04-10 08:26:04.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1109 2024-01-31 09:16:02.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      373 2024-02-15 09:49:55.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub-core-0.3.1/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3963 2024-03-01 09:41:58.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2233 2024-02-21 08:40:16.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      640 2024-02-01 10:45:50.000000 digitalhub-core-0.3.1/digitalhub_core/runtimes/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-10 08:00:27.000000 digitalhub-core-0.3.1/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-03-12 13:41:08.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-01-03 08:29:18.000000 digitalhub-core-0.3.1/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub-core-0.3.1/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub-core-0.3.1/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub-core-0.3.1/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub-core-0.3.1/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5341 2024-04-09 08:40:57.000000 digitalhub-core-0.3.1/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2331 2024-02-15 10:46:43.000000 digitalhub-core-0.3.1/digitalhub_core/utils/import_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub-core-0.3.1/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub-core-0.3.1/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      770 2024-04-08 13:33:46.000000 digitalhub-core-0.3.1/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:29.871790 digitalhub-core-0.3.1/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14637 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3986 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:29.000000 digitalhub-core-0.3.1/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1727 2024-04-09 13:57:43.000000 digitalhub-core-0.3.1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:28:29.875790 digitalhub-core-0.3.1/setup.cfg
```

### Comparing `digitalhub-core-0.3.0/LICENSE.txt` & `digitalhub-core-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/PKG-INFO` & `digitalhub-core-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,14 +233,15 @@
 Requires-Dist: pydantic>=1.10.8,~=1.10
 Requires-Dist: pandas<2.2,>=1.2
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pyarrow<15,>=10.0
 Requires-Dist: requests~=2.31
 Requires-Dist: PyYAML~=5.1
+Requires-Dist: GitPython>=3
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: moto; extra == "dev"
 Provides-Extra: docs
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/__init__.py` & `digitalhub-core-0.3.1/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/client/builder.py` & `digitalhub-core-0.3.1/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/client/objects/base.py` & `digitalhub-core-0.3.1/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/client/objects/dhcore.py` & `digitalhub-core-0.3.1/digitalhub_core/client/objects/dhcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                 msg = f"Backend error: {e}"
             raise BackendError(msg) from e
 
     ################################
     # Configuration methods
     ################################
 
-    def _configure(self, config: dict = None) -> None:
+    def _configure(self, config: dict | None = None) -> None:
         """
         Function to set environment variables for DHub Core config.
 
         Parameters
         ----------
         config : ClientConfig
             The client config.
@@ -284,25 +284,25 @@
 
         Returns
         -------
         tuple[str, str], str, None
             The authentication parameters.
         """
         # User for future entity ownership
-        self.user = os.getenv("DIGITALHUB_CORE_USER")
+        self._user = os.getenv("DIGITALHUB_CORE_USER")
 
         # Prioritize token over user/password
         token = os.getenv("DIGITALHUB_CORE_TOKEN")
         if token is not None:
             self._auth_type = "token"
             self._access_token = token
             return
 
         password = os.getenv("DIGITALHUB_CORE_PASSWORD")
-        if self.user is not None and password is not None:
+        if self._user is not None and password is not None:
             self._auth_type = "basic"
             self._password = password
             return
 
     @staticmethod
     def is_local() -> bool:
         """
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/client/objects/local.py` & `digitalhub-core-0.3.1/digitalhub_core/client/objects/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,29 +132,30 @@
 
                 # If the object is a project, we need to add the project spec,
                 # for example artifacts, functions, workflows, etc.
                 # Technically we have only projects that access base apis,
                 # we check entity_type just in case we add something else.
                 if entity_type == "projects":
                     obj = self._get_project_spec(obj, entity_id)
+                return obj
 
             # Context API
             #
             # GET /api/v1/-/<project-name>/runs/<entity_id>
             # GET /api/v1/-/<project-name>/artifacts/<entity_id>
             # GET /api/v1/-/<project-name>/functions/<entity_id>
             #
             # self._parse_api() should return entity_type and entity_id/version
 
             else:
                 for _, v in self._db[entity_type].items():
-                    obj = v[entity_id]
-                    break
-
-            return obj
+                    if entity_id in v:
+                        return v[entity_id]
+                else:
+                    raise KeyError
 
         except KeyError:
             msg = self._format_msg(3, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
 
     def update_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
         """
@@ -213,35 +214,46 @@
         entity_type, entity_id, context_api = self._parse_api(api)
         try:
             # Base API
             #
             # DELETE /api/v1/projects/<entity_id>
 
             if not context_api:
-                obj = self._db[entity_type].pop(entity_id)
+                self._db[entity_type].pop(entity_id)
 
             # Context API
             #
             # DELETE /api/v1/-/<project-name>/artifacts/<entity_id>
             #
             # We do not handle cascade in local client and
             # in the sdk we selectively delete objects by id,
             # not by name nor entity_type.
 
             else:
                 reset_latest = False
-                name = None
+                name = kwargs.get("params", {}).get("name")
+
+                # Delete by name
+                if entity_id is None and name is not None:
+                    self._db[entity_type].pop(name, None)
+                    return {"deleted": True}
+
+                # Delete by id
                 for _, v in self._db[entity_type].items():
-                    obj = v.pop(entity_id)
-                    # Handle latest
-                    if v["latest"]["id"] == entity_id:
-                        name = v["latest"].get("name", entity_id)
-                        v.pop("latest")
-                        reset_latest = True
-                    break
+                    if entity_id in v:
+                        v.pop(entity_id)
+
+                        # Handle latest
+                        if v["latest"]["id"] == entity_id:
+                            name = v["latest"].get("name", entity_id)
+                            v.pop("latest")
+                            reset_latest = True
+                        break
+                else:
+                    raise KeyError
 
                 if name is not None:
                     # Pop name if empty
                     if not self._db[entity_type][name]:
                         self._db[entity_type].pop(name)
 
                     # Handle latest
@@ -264,15 +276,15 @@
 
                         if latest_uuid is not None:
                             self._db[entity_type][name]["latest"] = self._db[entity_type][name][latest_uuid]
 
         except KeyError:
             msg = self._format_msg(3, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
-        return {"deleted": obj}
+        return {"deleted": True}
 
     def list_objects(self, api: str, **kwargs) -> list:
         """
         List objects.
 
         Parameters
         ----------
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/context/builder.py` & `digitalhub-core-0.3.1/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/context/context.py` & `digitalhub-core-0.3.1/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_base/base.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_base/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_base/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,34 @@
     representing a variety of objects handled by DigitalHub.
     """
 
     # Attributes to render as dict. Need to be expanded in subclasses.
     _obj_attr = ["kind", "metadata", "spec", "status"]
 
     @abstractmethod
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Entity:
         """
         Abstract save method.
         """
 
+    def _update_attributes(self, obj: dict) -> None:
+        """
+        Update attributes.
+
+        Parameters
+        ----------
+        obj : dict
+            Mapping representation of object from backend.
+        """
+        new_obj = self.from_dict(obj, validate=False)
+        self.metadata = new_obj.metadata
+        self.spec = new_obj.spec
+        self.status = new_obj.status
+        self.user = new_obj.user
+
     @abstractmethod
     def export(self, filename: str | None = None) -> None:
         """
         Abstract save method.
         """
 
     def to_dict(
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_base/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_base/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
     def __init__(
         self,
         name: str | None = None,
         source: str | None = None,
         labels: list[str] | None = None,
         embedded: bool = True,
-        created: str | None = str,
-        updated: str | None = str,
+        created: str | None = None,
+        created_by: str | None = None,
+        updated: str | None = None,
+        updated_by: str | None = None,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         name : str
@@ -35,16 +37,20 @@
             (Remote GIT) Source of the entity.
         labels : list[str]
             A list of labels to associate with the entity.
         embedded : bool
             Whether the entity specifications are embedded into a project.
         created : str
             Created date.
+        created_by : str
+            Created by.
         updated : str
             Updated date.
+        updated_by : str
+            Updated by.
         """
         self.name = name
         self.source = source
         self.labels = labels
         self.embedded = embedded
         self.created = created
         self.updated = updated
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_base/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_base/status.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_builders/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_builders/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     registry = import_registry(module_to_import, "spec_registry")
 
     # Import classes
     class_spec, class_params = _import_classes(registry, kind)
 
     # Validate arguments
     if validate:
-        kwargs = class_params(**kwargs).dict(by_alias=True)
+        kwargs = class_params(**kwargs).dict(by_alias=True, exclude_none=True)
 
     return class_spec(**kwargs)
 
 
 def _import_classes(registry: dict[str, dict[str, str]], kind: str) -> tuple[Spec, SpecParams]:
     """
     Import spec and params classes from registry.
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/_builders/status.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,37 +78,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Artifact:
         """
-        Save artifact into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Artifact from backend.
+        Artifact
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "artifacts")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "artifacts", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/artifacts/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/functions/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/functions/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/functions/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,37 +78,41 @@
         # Initialize tasks
         self._tasks: dict[str, Task] = {}
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Function:
         """
-        Save function into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         uuid : str
             Specify uuid for the function update
 
         Returns
         -------
-        dict
-            Mapping representation of Function from backend.
+        Function
+            Entity saved.
         """
         obj = self.to_dict(include_all_non_private=True)
 
         if not update:
             api = api_ctx_create(self.project, "functions")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "functions", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
@@ -466,18 +470,18 @@
         validate: bool = True,
     ) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
-        entity : str
-            Entity type.
         obj : dict
             Dictionary to parse.
+        validate : bool
+            Flag to determine if validation must be performed.
 
         Returns
         -------
         dict
             A dictionary containing the attributes of the entity instance.
         """
         project = obj.get("project")
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/functions/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/functions/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/functions/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/functions/spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,33 +22,37 @@
     """
     Source code struct.
     """
 
     def __init__(
         self,
         source: str | None = None,
+        handler: str | None = None,
         code: str | None = None,
         base64: str | None = None,
         lang: str | None = None,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         source : str
             Source reference.
+        handler : str
+            Function entrypoint.
         code : str
             Source code (plain).
         base64 : str
             Source code (base64 encoded).
         lang : str
             Source code language (hint).
         """
         self.source = source
+        self.handler = handler
         self.code = code
         self.base64 = base64
         self.lang = lang
 
     def to_dict(self) -> dict:
         """
         Convert to dictionary.
@@ -57,15 +61,18 @@
         -------
         dict
             Dictionary representation of the object.
         """
         dict_ = {}
         if self.source is not None:
             dict_["source"] = self.source
+        if self.handler is not None:
+            dict_["handler"] = self.handler
         if self.base64 is not None:
             dict_["base64"] = self.base64
         if self.lang is not None:
             dict_["lang"] = self.lang
+
         return dict_
 
     def __repr__(self) -> str:
         return str(self.to_dict())
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/projects/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/projects/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/projects/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,41 +113,45 @@
         # Set context
         set_context(self)
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Project:
         """
-        Save project and context into backend.
+        Save entity into backend.
 
         Parameters
         ----------
-        uuid : bool
-            Ignored, placed for compatibility with other objects.
+        update : bool
+            If True, the object will be updated.
 
         Returns
         -------
-        list
-            Mapping representation of Project from backend.
+        Project
+            Entity saved.
         """
         # Try to refresh project if local client
         if self._client.is_local():
             obj = self._refresh().to_dict()
         else:
             obj = self.to_dict()
 
         if not update:
             api = api_base_create("projects")
-            return self._client.create_object(api, obj)
+            new_obj = self._client.create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_base_update("projects", self.id)
-        return self._client.update_object(api, obj)
+        new_obj = self._client.update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file. If the objects are not embedded, the objects are
         exported as a YAML file.
 
         Parameters
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/projects/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/projects/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/projects/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/registries.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/runs/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/runs/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/runs/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,37 +77,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Run:
         """
-        Save run into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             If True, the object will be updated.
 
         Returns
         -------
-        dict
-            Mapping representation of Run from backend.
+        Run
+            Entity saved.
         """
         obj = self.to_dict(include_all_non_private=True)
 
         if not update:
             api = api_ctx_create(self.project, "runs")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "runs", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
@@ -182,14 +186,16 @@
             self._set_status({"state": State.RUNNING.value})
             self.spec.inputs = self.inputs(as_dict=True)
             self.save(update=True)
             status = runtime.run(self.to_dict(include_all_non_private=True))
         except Exception as err:
             status = {"state": State.ERROR.value, "message": str(err)}
 
+        # need to consider eventual run execution side effects, and update status only
+        self.refresh()
         self._set_status(status)
         self.save(update=True)
         return self
 
     def inputs(self, as_dict: bool = False) -> list[dict[str, Entity]]:
         """
         Get inputs passed in spec as objects or as dictionaries.
@@ -255,19 +261,15 @@
         Returns
         -------
         Run
             Run object.
         """
         api = api_ctx_read(self.project, "runs", self.id)
         obj = self._context().read_object(api)
-        refreshed_run = self.from_dict(obj, validate=False)
-        self.kind = refreshed_run.kind
-        self.metadata = refreshed_run.metadata
-        self.spec = refreshed_run.spec
-        self.status = refreshed_run.status
+        self._update_attributes(obj)
         return self
 
     def logs(self) -> dict:
         """
         Get object from backend.
         Returns empty dictionary if context is local.
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/runs/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/runs/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/runs/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/runs/status.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/secrets/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
 from digitalhub_core.entities.secrets.entity import secret_from_dict, secret_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
-from digitalhub_core.utils.exceptions import BackendError
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.secrets.entity import Secret
 
 
 ENTITY_TYPE = "secrets"
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/secrets/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,37 +70,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Secret:
         """
-        Save secret into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Secret from backend.
+        Secret
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "secrets")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "secrets", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/secrets/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/secrets/spec.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/services/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/services/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/services/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/services/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,37 +70,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Service:
         """
-        Save service into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Service from backend.
+        Service
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "services")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "services", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/services/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/services/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/tasks/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/tasks/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,37 +68,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Task:
         """
-        Save task into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Task from backend.
+        Task
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "tasks")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "tasks", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/tasks/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/tasks/models.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/workflows/crud.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     check_context(obj.get("project"))
     return workflow_from_dict(obj)
 
 
 def new_workflow(
     project: str,
     name: str,
+    kind: str,
     uuid: str | None = None,
     description: str | None = None,
     source: str | None = None,
     labels: list[str] | None = None,
     embedded: bool = True,
     **kwargs,
 ) -> Workflow:
@@ -88,15 +89,15 @@
     -------
     Workflow
         An instance of the created workflow.
     """
     obj = create_workflow(
         project=project,
         name=name,
-        kind="workflow",
+        kind=kind,
         uuid=uuid,
         description=description,
         source=source,
         labels=labels,
         embedded=embedded,
         **kwargs,
     )
@@ -153,14 +154,15 @@
 
     Returns
     -------
     Workflow
         Object instance.
     """
     obj: dict = read_yaml(file)
+    check_context(obj.get("project"))
     return create_workflow_from_dict(obj)
 
 
 def delete_workflow(
     project: str,
     entity_name: str | None = None,
     entity_id: str | None = None,
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/workflows/entity.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.entities.functions.crud import get_function
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
+    from digitalhub_core.entities.runs.entity import Run
     from digitalhub_core.entities.workflows.metadata import WorkflowMetadata
     from digitalhub_core.entities.workflows.spec import WorkflowSpec
     from digitalhub_core.entities.workflows.status import WorkflowStatus
 
 
 class Workflow(Entity):
     """
@@ -70,37 +72,41 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
     #  Save / Export
     #############################
 
-    def save(self, update: bool = False) -> dict:
+    def save(self, update: bool = False) -> Workflow:
         """
-        Save workflow into backend.
+        Save entity into backend.
 
         Parameters
         ----------
         update : bool
             Flag to indicate update.
 
         Returns
         -------
-        dict
-            Mapping representation of Workflow from backend.
+        Workflow
+            Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
             api = api_ctx_create(self.project, "workflows")
-            return self._context().create_object(api, obj)
+            new_obj = self._context().create_object(api, obj)
+            self._update_attributes(new_obj)
+            return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "workflows", self.id)
-        return self._context().update_object(api, obj)
+        new_obj = self._context().update_object(api, obj)
+        self._update_attributes(new_obj)
+        return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
@@ -145,32 +151,29 @@
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to parse.
+        validate : bool
+            Flag to determine if validation must be performed.
 
         Returns
         -------
         dict
             A dictionary containing the attributes of the entity instance.
         """
         project = obj.get("project")
         name = obj.get("name")
         kind = obj.get("kind")
         uuid = build_uuid(obj.get("id"))
-        metadata = build_metadata(kind, layer_digitalhub="digitalhub_core", **obj.get("metadata", {}))
-        spec = build_spec(
-            kind,
-            layer_digitalhub="digitalhub_core",
-            validate=validate,
-            **obj.get("spec", {}),
-        )
-        status = build_status(kind, layer_digitalhub="digitalhub_core", **obj.get("status", {}))
+        metadata = build_metadata(kind, framework_runtime=kind, **obj.get("metadata", {}))
+        spec = build_spec(kind, framework_runtime=kind, validate=validate, **obj.get("spec", {}))
+        status = build_status(kind, framework_runtime=kind, **obj.get("status", {}))
         return {
             "project": project,
             "name": name,
             "uuid": uuid,
             "kind": kind,
             "metadata": metadata,
             "spec": spec,
@@ -180,15 +183,15 @@
 
 def workflow_from_parameters(
     project: str,
     name: str,
     kind: str,
     uuid: str | None = None,
     description: str | None = None,
-    source: str | None = None,
+    git_source: str | None = None,
     labels: list[str] | None = None,
     embedded: bool = True,
     **kwargs,
 ) -> Workflow:
     """
     Create a new Workflow instance with the specified parameters.
 
@@ -198,15 +201,15 @@
         A string representing the project associated with this workflow.
     name : str
         The name of the workflow.
     kind : str
         Kind of the object.
     uuid : str
         ID of the object in form of UUID.
-    source : str
+    git_source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
     description : str
         A description of the workflow.
     embedded : bool
         Flag to determine if object must be embedded in project.
@@ -215,31 +218,34 @@
 
     Returns
     -------
     Workflow
         An instance of the created workflow.
     """
     uuid = build_uuid(uuid)
+    spec = build_spec(
+        kind,
+        framework_runtime=kind,
+        **kwargs,
+    )
     metadata = build_metadata(
         kind,
-        layer_digitalhub="digitalhub_core",
+        framework_runtime=kind,
         project=project,
         name=name,
         version=uuid,
         description=description,
-        source=source,
+        source=git_source,
         labels=labels,
         embedded=embedded,
     )
-    spec = build_spec(
+    status = build_status(
         kind,
-        layer_digitalhub="digitalhub_core",
-        **kwargs,
+        framework_runtime=kind,
     )
-    status = build_status(kind, layer_digitalhub="digitalhub_core")
     return Workflow(
         project=project,
         name=name,
         uuid=uuid,
         kind=kind,
         metadata=metadata,
         spec=spec,
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/entities/workflows/metadata.py` & `digitalhub-core-0.3.1/digitalhub_core/entities/workflows/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/runtimes/base.py` & `digitalhub-core-0.3.1/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/runtimes/builder.py` & `digitalhub-core-0.3.1/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/runtimes/registry.py` & `digitalhub-core-0.3.1/digitalhub_core/runtimes/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/builder.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/objects/base.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/objects/local.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/objects/remote.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/objects/s3.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/stores/objects/sql.py` & `digitalhub-core-0.3.1/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/utils/api.py` & `digitalhub-core-0.3.1/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/utils/generic_utils.py` & `digitalhub-core-0.3.1/digitalhub_core/utils/generic_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 General utilities module.
 """
 from __future__ import annotations
 
 import base64
 import os
 from datetime import datetime
-from hashlib import sha1
-from mimetypes import guess_type
 from pathlib import Path
+from urllib.parse import urlparse
 from uuid import uuid4
+from zipfile import ZipFile
 
+import boto3
+import requests
 from digitalhub_core.utils.io_utils import read_text
+from git import Repo
 
 
 def build_uuid(uuid: str | None = None) -> str:
     """
     Create a uuid if not given
 
     Parameters
@@ -158,75 +161,103 @@
         # The name and uuid are separated by a colon in the last part
         name, uuid = parts[3].split(":")
         return project, entity_type, kind, name, uuid
     except Exception as e:
         raise ValueError("Invalid key format.") from e
 
 
-def calculate_blob_hash(data_path: str) -> str:
+def clone_repository(path: Path, source: str) -> None:
     """
-    Calculate the hash of a file.
+    Clone repository.
 
     Parameters
     ----------
-    data_path : str
-        Path to the file.
+    path : Path
+        Path where to save the repository.
+    source : str
+        HTTP(S) URL of the repository.
 
     Returns
     -------
-    str
-        The hash of the file.
+    None
     """
-    with open(data_path, "rb") as f:
-        data = f.read()
-        return f"sha1_{sha1(data).hexdigest()}"
+    Repo.clone_from(source, path)
 
 
-def get_file_size(data_path: str) -> int:
+def requests_chunk_download(source: str, filename: Path) -> None:
     """
-    Get the size of a file.
+    Download a file in chunks.
 
     Parameters
     ----------
-    data_path : str
-        Path to the file.
+    source : str
+        URL to download the file.
+    filename : Path
+        Path where to save the file.
 
     Returns
     -------
-    int
-        The size of the file.
+    None
     """
-    return Path(data_path).stat().st_size
+    with requests.get(source, stream=True) as r:
+        r.raise_for_status()
+        with filename.open("wb") as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
 
 
-def get_file_mime_type(data_path: str) -> str:
+def extract_archive(path: Path, filename: Path) -> None:
     """
-    Get the mime type of a file.
+    Extract an archive.
 
     Parameters
     ----------
-    data_path : str
-        Path to the file.
+    path : Path
+        Path where to extract the archive.
+    filename : Path
+        Path to the archive.
 
     Returns
     -------
-    str
-        The mime type of the file.
+    None
     """
-    return guess_type(data_path)[0]
+    with ZipFile(filename, "r") as zip_file:
+        zip_file.extractall(path)
 
 
-def get_file_extension(data_path: str) -> str:
+def get_s3_source(bucket: str, key: str, filename: Path) -> None:
     """
-    Get the extension of a file.
+    Get S3 source.
 
     Parameters
     ----------
-    data_path : str
-        Path to the file.
+    bucket : str
+        S3 bucket name.
+    key : str
+        S3 object key.
+    filename : Path
+        Path where to save the function source.
 
     Returns
     -------
-    str
-        The extension of the file.
+    None
+    """
+    s3 = boto3.client("s3", endpoint_url=os.getenv("S3_ENDPOINT_URL"))
+    s3.download_file(bucket, key, filename)
+
+
+def get_bucket_and_key(path: str) -> tuple[str, str]:
+    """
+    Get bucket and key from path.
+
+    Parameters
+    ----------
+    path : str
+        The source path to get the key from.
+
+    Returns
+    -------
+    tuple[str, str]
+        The bucket and key.
     """
-    return Path(data_path).suffix[1:]
+    parsed = urlparse(path)
+    return parsed.netloc, parsed.path
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core/utils/import_utils.py` & `digitalhub-core-0.3.1/digitalhub_core/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/utils/io_utils.py` & `digitalhub-core-0.3.1/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-core-0.3.0/digitalhub_core/utils/uri_utils.py` & `digitalhub-core-0.3.1/digitalhub_core/utils/uri_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,8 +30,10 @@
         return "local"
     if scheme in ["http", "https", "remote"]:
         return "remote"
     if scheme in ["s3", "s3a", "s3n"]:
         return "s3"
     if scheme in ["sql", "postgresql"]:
         return "sql"
+    if scheme in ["git"]:
+        return "git"
     raise ValueError(f"Unknown scheme '{scheme}'!")
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core.egg-info/PKG-INFO` & `digitalhub-core-0.3.1/digitalhub_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,14 +233,15 @@
 Requires-Dist: pydantic>=1.10.8,~=1.10
 Requires-Dist: pandas<2.2,>=1.2
 Requires-Dist: sqlalchemy~=1.4
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pyarrow<15,>=10.0
 Requires-Dist: requests~=2.31
 Requires-Dist: PyYAML~=5.1
+Requires-Dist: GitPython>=3
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: moto; extra == "dev"
 Provides-Extra: docs
```

### Comparing `digitalhub-core-0.3.0/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub-core-0.3.1/digitalhub_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,12 +88,13 @@
 digitalhub_core/stores/objects/local.py
 digitalhub_core/stores/objects/remote.py
 digitalhub_core/stores/objects/s3.py
 digitalhub_core/stores/objects/sql.py
 digitalhub_core/utils/__init__.py
 digitalhub_core/utils/api.py
 digitalhub_core/utils/exceptions.py
+digitalhub_core/utils/file_utils.py
 digitalhub_core/utils/generic_utils.py
 digitalhub_core/utils/import_utils.py
 digitalhub_core/utils/io_utils.py
 digitalhub_core/utils/logger.py
 digitalhub_core/utils/uri_utils.py
```

### Comparing `digitalhub-core-0.3.0/pyproject.toml` & `digitalhub-core-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -24,15 +24,16 @@
     "aiobotocore",
     "pydantic~=1.10, >=1.10.8",
     "pandas>=1.2, <2.2",
     "sqlalchemy~=1.4",
     "psycopg2-binary~=2.8",
     "pyarrow>=10.0, <15",
     "requests~=2.31",
-    "PyYAML~=5.1"
+    "PyYAML~=5.1",
+    "GitPython>=3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*", "modules*"]
 
 [project.optional-dependencies]
 dev = [
@@ -60,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

