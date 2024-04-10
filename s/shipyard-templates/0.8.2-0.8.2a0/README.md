# Comparing `tmp/shipyard_templates-0.8.2.tar.gz` & `tmp/shipyard_templates-0.8.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.8.2.tar", max compression
+gzip compressed data, was "shipyard_templates-0.8.2a0.tar", max compression
```

## Comparing `shipyard_templates-0.8.2.tar` & `shipyard_templates-0.8.2a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.8.2/README.md
--rw-r--r--   0        0        0      343 2024-04-10 20:14:55.344199 shipyard_templates-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      481 2024-01-17 00:03:52.913226 shipyard_templates-0.8.2/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      712 2024-03-14 04:10:25.264195 shipyard_templates-0.8.2/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0      920 2024-02-05 15:18:12.454746 shipyard_templates-0.8.2/shipyard_templates/crm.py
--rw-r--r--   0        0        0     4161 2024-03-27 16:08:43.657214 shipyard_templates-0.8.2/shipyard_templates/database.py
--rw-r--r--   0        0        0      346 2024-02-05 15:18:12.455141 shipyard_templates-0.8.2/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     2449 2024-04-04 19:39:49.109168 shipyard_templates-0.8.2/shipyard_templates/etl.py
--rw-r--r--   0        0        0      598 2023-09-26 17:06:16.596503 shipyard_templates-0.8.2/shipyard_templates/exit_code_exception.py
--rw-r--r--   0        0        0     2648 2024-02-20 16:15:01.174516 shipyard_templates-0.8.2/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      116 2024-02-05 15:18:12.456666 shipyard_templates-0.8.2/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      937 2024-03-14 04:10:25.265265 shipyard_templates-0.8.2/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0     1881 2024-02-12 21:39:56.699411 shipyard_templates-0.8.2/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      575 2024-02-07 15:09:08.394166 shipyard_templates-0.8.2/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 shipyard_templates-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.8.2a0/README.md
+-rw-r--r--   0        0        0      345 2024-04-04 19:39:49.108707 shipyard_templates-0.8.2a0/pyproject.toml
+-rw-r--r--   0        0        0      481 2024-01-17 00:03:52.913226 shipyard_templates-0.8.2a0/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      712 2024-03-14 04:10:25.264195 shipyard_templates-0.8.2a0/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0      920 2024-02-05 15:18:12.454746 shipyard_templates-0.8.2a0/shipyard_templates/crm.py
+-rw-r--r--   0        0        0     4161 2024-03-27 16:08:43.657214 shipyard_templates-0.8.2a0/shipyard_templates/database.py
+-rw-r--r--   0        0        0      346 2024-02-05 15:18:12.455141 shipyard_templates-0.8.2a0/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     2449 2024-04-04 19:39:49.109168 shipyard_templates-0.8.2a0/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      598 2023-09-26 17:06:16.596503 shipyard_templates-0.8.2a0/shipyard_templates/exit_code_exception.py
+-rw-r--r--   0        0        0     2648 2024-02-20 16:15:01.174516 shipyard_templates-0.8.2a0/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      116 2024-02-05 15:18:12.456666 shipyard_templates-0.8.2a0/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      937 2024-03-14 04:10:25.265265 shipyard_templates-0.8.2a0/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0     1881 2024-02-12 21:39:56.699411 shipyard_templates-0.8.2a0/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      575 2024-02-07 15:09:08.394166 shipyard_templates-0.8.2a0/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 shipyard_templates-0.8.2a0/PKG-INFO
```

### Comparing `shipyard_templates-0.8.2/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.8.2a0/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/crm.py` & `shipyard_templates-0.8.2a0/shipyard_templates/crm.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/database.py` & `shipyard_templates-0.8.2a0/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/etl.py` & `shipyard_templates-0.8.2a0/shipyard_templates/etl.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/exit_code_exception.py` & `shipyard_templates-0.8.2a0/shipyard_templates/exit_code_exception.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/messaging.py` & `shipyard_templates-0.8.2a0/shipyard_templates/messaging.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/projectmanagement.py` & `shipyard_templates-0.8.2a0/shipyard_templates/projectmanagement.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.8.2a0/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.8.2/shipyard_templates/spreadsheets.py` & `shipyard_templates-0.8.2a0/shipyard_templates/spreadsheets.py`

 * *Files identical despite different names*

