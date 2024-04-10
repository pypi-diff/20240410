# Comparing `tmp/notification_py-0.0.7.tar.gz` & `tmp/notification_py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-0.0.7.tar", max compression
+gzip compressed data, was "notification_py-0.0.8.tar", max compression
```

## Comparing `notification_py-0.0.7.tar` & `notification_py-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.7/LICENSE
--rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.7/README.md
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.7/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.7/notification_py/custom_types.py
--rw-r--r--   0        0        0     1865 2024-04-10 01:31:34.794458 notification_py-0.0.7/notification_py/main.py
--rw-r--r--   0        0        0     4614 2024-04-10 01:31:17.218473 notification_py-0.0.7/notification_py/services/discord.py
--rw-r--r--   0        0        0     2368 2024-04-10 01:31:22.262468 notification_py-0.0.7/notification_py/services/email.py
--rw-r--r--   0        0        0     3726 2024-04-10 01:31:27.349464 notification_py-0.0.7/notification_py/services/slack.py
--rw-r--r--   0        0        0      629 2024-04-10 01:33:09.143431 notification_py-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 notification_py-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-0.0.8/LICENSE
+-rw-r--r--   0        0        0      100 2024-03-30 07:03:53.459271 notification_py-0.0.8/README.md
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-0.0.8/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 23:48:03.651152 notification_py-0.0.8/notification_py/custom_types.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:31:34.794458 notification_py-0.0.8/notification_py/main.py
+-rw-r--r--   0        0        0     4614 2024-04-10 01:31:17.218473 notification_py-0.0.8/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2368 2024-04-10 01:31:22.262468 notification_py-0.0.8/notification_py/services/email.py
+-rw-r--r--   0        0        0     3726 2024-04-10 01:31:27.349464 notification_py-0.0.8/notification_py/services/slack.py
+-rw-r--r--   0        0        0      780 2024-04-10 01:38:19.443832 notification_py-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 notification_py-0.0.8/PKG-INFO
```

### Comparing `notification_py-0.0.7/LICENSE` & `notification_py-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.7/notification_py/custom_types.py` & `notification_py-0.0.8/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.7/notification_py/main.py` & `notification_py-0.0.8/notification_py/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.7/notification_py/services/discord.py` & `notification_py-0.0.8/notification_py/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.7/notification_py/services/email.py` & `notification_py-0.0.8/notification_py/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-0.0.7/notification_py/services/slack.py` & `notification_py-0.0.8/notification_py/services/slack.py`

 * *Files identical despite different names*

