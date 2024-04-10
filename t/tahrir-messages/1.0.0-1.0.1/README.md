# Comparing `tmp/tahrir_messages-1.0.0.tar.gz` & `tmp/tahrir_messages-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir_messages-1.0.0.tar", max compression
+gzip compressed data, was "tahrir_messages-1.0.1.tar", max compression
```

## Comparing `tahrir_messages-1.0.0.tar` & `tahrir_messages-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0        0        0        0 2024-04-09 10:06:10.247183 tahrir_messages-1.0.0/LICENSES/
--rw-r--r--   0        0        0      486 2024-04-08 23:18:48.843306 tahrir_messages-1.0.0/README.md
--rw-r--r--   0        0        0     2118 2024-04-09 09:27:54.451479 tahrir_messages-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3955 2024-04-09 10:03:19.706933 tahrir_messages-1.0.0/tahrir_messages/__init__.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 tahrir_messages-1.0.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-04-09 10:06:10.247183 tahrir_messages-1.0.1/LICENSES/
+-rw-r--r--   0        0        0      486 2024-04-08 23:18:48.843306 tahrir_messages-1.0.1/README.md
+-rw-r--r--   0        0        0     2118 2024-04-10 05:40:08.971931 tahrir_messages-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3965 2024-04-10 05:38:56.629373 tahrir_messages-1.0.1/tahrir_messages/__init__.py
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 tahrir_messages-1.0.1/PKG-INFO
```

### Comparing `tahrir_messages-1.0.0/pyproject.toml` & `tahrir_messages-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2024 Contributors to the Fedora Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 [tool.poetry]
 name = "tahrir-messages"
-version = "1.0.0"
+version = "1.0.1"
 description = "A schema package for messages sent by tahrir"
 authors = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "http://github.com/fedora-infra/tahrir-messages"
 repository = "http://github.com/fedora-infra/tahrir-messages"
 keywords = ["fedora-messaging"]
```

### Comparing `tahrir_messages-1.0.0/tahrir_messages/__init__.py` & `tahrir_messages-1.0.1/tahrir_messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,11 +132,11 @@
     body_schema: typing.ClassVar = {
         "id": "http://fedoraproject.org/message-schema/tahrir",
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "The message sent when a user's rank changes",
         "type": "object",
         "required": ["old_rank", "person"],
         "properties": {
-            "old_rank": {"type": "integer"},
+            "old_rank": {"type": ["integer", "null"]},
             "person": person_schema,
         },
     }
```

### Comparing `tahrir_messages-1.0.0/PKG-INFO` & `tahrir_messages-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir-messages
-Version: 1.0.0
+Version: 1.0.1
 Summary: A schema package for messages sent by tahrir
 Home-page: http://github.com/fedora-infra/tahrir-messages
 License: LGPL-3.0-or-later
 Keywords: fedora-messaging
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.8,<4.0
```

