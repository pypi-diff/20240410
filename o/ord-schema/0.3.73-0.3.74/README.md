# Comparing `tmp/ord-schema-0.3.73.tar.gz` & `tmp/ord-schema-0.3.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.73.tar", last modified: Wed Feb 21 22:16:31 2024, max compression
+gzip compressed data, was "ord-schema-0.3.74.tar", last modified: Wed Apr 10 14:44:49 2024, max compression
```

## Comparing `ord-schema-0.3.73.tar` & `ord-schema-0.3.74.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.475485 ord-schema-0.3.73/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-21 22:16:14.000000 ord-schema-0.3.73/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-21 22:16:14.000000 ord-schema-0.3.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-21 22:16:14.000000 ord-schema-0.3.73/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-21 22:16:31.475485 ord-schema-0.3.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-21 22:16:14.000000 ord-schema-0.3.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.463485 ord-schema-0.3.73/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.467485 ord-schema-0.3.73/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.467485 ord-schema-0.3.73/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.471485 ord-schema-0.3.73/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    91519 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/reaction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.471485 ord-schema-0.3.73/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    47179 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-02-21 22:16:14.000000 ord-schema-0.3.73/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.471485 ord-schema-0.3.73/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-21 22:16:31.000000 ord-schema-0.3.73/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-02-21 22:16:31.000000 ord-schema-0.3.73/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 22:16:31.000000 ord-schema-0.3.73/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 22:16:31.000000 ord-schema-0.3.73/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-21 22:16:31.000000 ord-schema-0.3.73/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:16:31.471485 ord-schema-0.3.73/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-21 22:16:14.000000 ord-schema-0.3.73/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (127)    46965 2024-02-21 22:16:14.000000 ord-schema-0.3.73/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-21 22:16:14.000000 ord-schema-0.3.73/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-21 22:16:14.000000 ord-schema-0.3.73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 22:16:31.475485 ord-schema-0.3.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-21 22:16:16.000000 ord-schema-0.3.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.192983 ord-schema-0.3.74/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 14:44:33.000000 ord-schema-0.3.74/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:44:33.000000 ord-schema-0.3.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 14:44:33.000000 ord-schema-0.3.74/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 14:44:49.192983 ord-schema-0.3.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-10 14:44:33.000000 ord-schema-0.3.74/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.180983 ord-schema-0.3.74/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.180983 ord-schema-0.3.74/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.184983 ord-schema-0.3.74/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.184983 ord-schema-0.3.74/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91519 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47179 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    46965 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 14:44:33.000000 ord-schema-0.3.74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:44:49.192983 ord-schema-0.3.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 14:44:36.000000 ord-schema-0.3.74/setup.py
```

### Comparing `ord-schema-0.3.73/LICENSE` & `ord-schema-0.3.74/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/PKG-INFO` & `ord-schema-0.3.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.73
+Version: 0.3.74
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.73/README.md` & `ord-schema-0.3.74/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/__init__.py` & `ord-schema-0.3.74/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/frozen_message.py` & `ord-schema-0.3.74/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/frozen_message_test.py` & `ord-schema-0.3.74/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/logging.py` & `ord-schema-0.3.74/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/macros/__init__.py` & `ord-schema-0.3.74/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/macros/solutions.py` & `ord-schema-0.3.74/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.74/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/macros/workups.py` & `ord-schema-0.3.74/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/message_helpers.py` & `ord-schema-0.3.74/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/message_helpers_test.py` & `ord-schema-0.3.74/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/__init__.py` & `ord-schema-0.3.74/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/conftest.py` & `ord-schema-0.3.74/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/database.py` & `ord-schema-0.3.74/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/database_test.py` & `ord-schema-0.3.74/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/mappers.py` & `ord-schema-0.3.74/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.74/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.74/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.74/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/__init__.py` & `ord-schema-0.3.74/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.74/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/dataset_pb2.pyi` & `ord-schema-0.3.74/ord_schema/proto/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.74/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.74/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/reaction_pb2.pyi` & `ord-schema-0.3.74/ord_schema/proto/reaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.74/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.74/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/resolvers.py` & `ord-schema-0.3.74/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/resolvers_test.py` & `ord-schema-0.3.74/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/__init__.py` & `ord-schema-0.3.74/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.74/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.74/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.74/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.74/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.74/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.74/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.74/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.74/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.74/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/templating.py` & `ord-schema-0.3.74/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/templating_test.py` & `ord-schema-0.3.74/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/units.py` & `ord-schema-0.3.74/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/units_test.py` & `ord-schema-0.3.74/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/updates.py` & `ord-schema-0.3.74/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/updates_test.py` & `ord-schema-0.3.74/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/validations.py` & `ord-schema-0.3.74/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema/validations_test.py` & `ord-schema-0.3.74/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.74/ord_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.73
+Version: 0.3.74
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.73/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.74/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.74/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/proto/dataset.proto` & `ord-schema-0.3.74/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/proto/reaction.proto` & `ord-schema-0.3.74/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/proto/test.proto` & `ord-schema-0.3.74/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.73/setup.py` & `ord-schema-0.3.74/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.73",
+    version="0.3.74",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

