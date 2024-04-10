# Comparing `tmp/tahrir_messages-1.0.1.tar.gz` & `tmp/tahrir_messages-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir_messages-1.0.1.tar", max compression
+gzip compressed data, was "tahrir_messages-1.0.2.tar", max compression
```

## Comparing `tahrir_messages-1.0.1.tar` & `tahrir_messages-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,7 @@
-drwxr-xr-x   0        0        0        0 2024-04-09 10:06:10.247183 tahrir_messages-1.0.1/LICENSES/
--rw-r--r--   0        0        0      486 2024-04-08 23:18:48.843306 tahrir_messages-1.0.1/README.md
--rw-r--r--   0        0        0     2118 2024-04-10 05:40:08.971931 tahrir_messages-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3965 2024-04-10 05:38:56.629373 tahrir_messages-1.0.1/tahrir_messages/__init__.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 tahrir_messages-1.0.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/LICENSES/
+-rw-r--r--   0        0        0    34674 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0    42098 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0      486 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/README.md
+-rw-r--r--   0        0        0     2118 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3959 2024-04-10 20:03:31.263480 tahrir_messages-1.0.2/tahrir_messages/__init__.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 tahrir_messages-1.0.2/PKG-INFO
```

### Comparing `tahrir_messages-1.0.1/pyproject.toml` & `tahrir_messages-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2024 Contributors to the Fedora Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 [tool.poetry]
 name = "tahrir-messages"
-version = "1.0.1"
+version = "1.0.2"
 description = "A schema package for messages sent by tahrir"
 authors = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "http://github.com/fedora-infra/tahrir-messages"
 repository = "http://github.com/fedora-infra/tahrir-messages"
 keywords = ["fedora-messaging"]
```

### Comparing `tahrir_messages-1.0.1/tahrir_messages/__init__.py` & `tahrir_messages-1.0.2/tahrir_messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             "badge_id": {"type": "string"},
             "description": {"type": "string"},
             "image_url": {"type": "string"},
             "name": {"type": "string"},
         },
     }
 
-    topic = "person.login.first"
+    topic = "badge.award"
     body_schema: typing.ClassVar = {
         "id": "http://fedoraproject.org/message-schema/tahrir",
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "The message sent when a user logs into tahrir for the first time",
         "type": "object",
         "required": ["user", "badge"],
         "properties": {
@@ -124,15 +124,15 @@
             "id": {"type": "integer"},
             "nickname": {"type": "string"},
             "rank": {"type": "integer"},
             "website": {"type": ["string", "null"]},
         },
     }
 
-    topic = "person.login.first"
+    topic = "person.rank.advance"
     body_schema: typing.ClassVar = {
         "id": "http://fedoraproject.org/message-schema/tahrir",
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "The message sent when a user's rank changes",
         "type": "object",
         "required": ["old_rank", "person"],
         "properties": {
```

### Comparing `tahrir_messages-1.0.1/PKG-INFO` & `tahrir_messages-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir-messages
-Version: 1.0.1
+Version: 1.0.2
 Summary: A schema package for messages sent by tahrir
 Home-page: http://github.com/fedora-infra/tahrir-messages
 License: LGPL-3.0-or-later
 Keywords: fedora-messaging
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fedora-messaging (>=3.3.0,<4.0.0)
 Project-URL: Repository, http://github.com/fedora-infra/tahrir-messages
 Description-Content-Type: text/markdown
 
 # tahrir messages
```

