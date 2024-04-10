# Comparing `tmp/tsk_monster-0.0.0.tar.gz` & `tmp/tsk_monster-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.0.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.1.tar", max compression
```

## Comparing `tsk_monster-0.0.0.tar` & `tsk_monster-0.0.1.tar`

### file list

```diff
@@ -1,6 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-09 06:29:21.335344 tsk_monster-0.0.0/README.md
--rw-r--r--   0        0        0      442 2024-04-10 12:17:57.781541 tsk_monster-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1430 2024-04-10 12:19:39.365187 tsk_monster-0.0.0/tsk_monster/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-10 12:19:31.461547 tsk_monster-0.0.0/tsk_monster/tsks.py
--rw-r--r--   0        0        0      481 2024-04-10 12:19:20.110513 tsk_monster-0.0.0/tsk_monster/util.py
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 tsk_monster-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 06:29:21.335344 tsk_monster-0.0.1/README.md
+-rw-r--r--   0        0        0      442 2024-04-10 13:36:08.875801 tsk_monster-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2719 2024-04-10 13:31:58.772870 tsk_monster-0.0.1/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 tsk_monster-0.0.1/PKG-INFO
```

