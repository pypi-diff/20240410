# Comparing `tmp/djangoldp_resource-3.1.2.tar.gz` & `tmp/djangoldp_resource-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_resource-3.1.2.tar", last modified: Wed Feb  7 14:50:20 2024, max compression
+gzip compressed data, was "djangoldp_resource-3.1.3.tar", last modified: Wed Apr 10 11:05:11 2024, max compression
```

## Comparing `djangoldp_resource-3.1.2.tar` & `djangoldp_resource-3.1.3.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:50:20.789969 djangoldp_resource-3.1.2/
--rw-r--r--   0 root         (0) root         (0)      270 2024-02-07 14:50:20.789969 djangoldp_resource-3.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:50:20.785968 djangoldp_resource-3.1.2/djangoldp_resource/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-07 14:50:18.000000 djangoldp_resource-3.1.2/djangoldp_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:50:20.789969 djangoldp_resource-3.1.2/djangoldp_resource/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2661 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0002_auto_20200426_1902.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0002_resource_user.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0003_auto_20200616_0957.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0003_resource_conversations.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0004_merge_20200616_1011.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0005_merge_20200616_1030.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0006_auto_20200617_1458.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0007_auto_20200709_1411.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0008_auto_20200812_1446.py
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0009_auto_20200812_1459.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0010_auto_20200923_1017.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0011_auto_20210525_1018.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0012_auto_20210525_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0013_auto_20221012_1503.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0014_auto_20221027_0958.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/0015_alter_keyword_options_alter_resource_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/models.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/djangoldp_resource/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:50:20.785968 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/
--rw-r--r--   0 root         (0) root         (0)      270 2024-02-07 14:50:20.000000 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1512 2024-02-07 14:50:20.000000 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 14:50:20.000000 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-02-07 14:50:20.000000 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-02-07 14:50:20.000000 djangoldp_resource-3.1.2/djangoldp_resource.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-02-07 14:50:20.789969 djangoldp_resource-3.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-07 14:49:59.000000 djangoldp_resource-3.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.525947 djangoldp_resource-3.1.3/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-10 11:05:11.525947 djangoldp_resource-3.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.521947 djangoldp_resource-3.1.3/djangoldp_resource/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-10 11:05:08.000000 djangoldp_resource-3.1.3/djangoldp_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.525947 djangoldp_resource-3.1.3/djangoldp_resource/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0002_auto_20200426_1902.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0002_resource_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0003_auto_20200616_0957.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0003_resource_conversations.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0004_merge_20200616_1011.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0005_merge_20200616_1030.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0006_auto_20200617_1458.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0007_auto_20200709_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0008_auto_20200812_1446.py
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0009_auto_20200812_1459.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0010_auto_20200923_1017.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0011_auto_20210525_1018.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0012_auto_20210525_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0013_auto_20221012_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0014_auto_20221027_0958.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/0015_alter_keyword_options_alter_resource_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/djangoldp_resource/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.521947 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-10 11:05:11.000000 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-04-10 11:05:11.000000 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:05:11.000000 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-10 11:05:11.000000 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 11:05:11.000000 djangoldp_resource-3.1.3/djangoldp_resource.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-04-10 11:05:11.525947 djangoldp_resource-3.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-10 11:04:50.000000 djangoldp_resource-3.1.3/setup.py
```

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/admin.py` & `djangoldp_resource-3.1.3/djangoldp_resource/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0001_initial.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0002_auto_20200426_1902.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0002_auto_20200426_1902.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0002_resource_user.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0002_resource_user.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0003_auto_20200616_0957.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0003_auto_20200616_0957.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0003_resource_conversations.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0003_resource_conversations.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0006_auto_20200617_1458.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0006_auto_20200617_1458.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0007_auto_20200709_1411.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0007_auto_20200709_1411.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0008_auto_20200812_1446.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0008_auto_20200812_1446.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0009_auto_20200812_1459.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0009_auto_20200812_1459.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0010_auto_20200923_1017.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0010_auto_20200923_1017.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0011_auto_20210525_1018.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0011_auto_20210525_1018.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0012_auto_20210525_1022.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0012_auto_20210525_1022.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/migrations/0015_alter_keyword_options_alter_resource_options_and_more.py` & `djangoldp_resource-3.1.3/djangoldp_resource/migrations/0015_alter_keyword_options_alter_resource_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource/models.py` & `djangoldp_resource-3.1.3/djangoldp_resource/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.conf import settings
 from django.db import models
 from djangoldp_conversation.models import Conversation, Message
 from djangoldp.models import Model
 from djangoldp_circle.models import Circle
 from django.contrib.auth import get_user_model
-from djangoldp_resource.permissions import ResourcePermissions
-from djangoldp.permissions import AuthenticatedOnly
+from djangoldp.permissions import AuthenticatedOnly, AnonymousReadOnly, ReadAndCreate, ACLPermissions, InheritPermissions
 
 
 class Type (Model):
     name = models.CharField(max_length=50, null=True, blank=True, verbose_name="Resource type")
 
     class Meta(Model.Meta):
         permission_classes = [AuthenticatedOnly]
@@ -46,13 +45,14 @@
 
     class Meta(Model.Meta):
         serializer_fields = ["@id", "name", "shortdesc", "longdesc", "type", "img", "document",\
                            "link", "keywords", "conversations", "circle", "creationDate"]
         auto_author = 'user'
         owner_field = 'user'
         container_path = 'resources/'
-        rdf_type = 'hd:resource'
-        permission_classes = [ResourcePermissions]
+        rdf_type = 'sib:resource'
+        permission_classes = [AuthenticatedOnly, ReadAndCreate|ACLPermissions, InheritPermissions]
+        inherit_permissions = ['circle']
         nested_fields = ['keywords', 'conversations', 'circle', 'type']
-        
+
     def __str__(self):
         return self.name
```

### Comparing `djangoldp_resource-3.1.2/djangoldp_resource.egg-info/SOURCES.txt` & `djangoldp_resource-3.1.3/djangoldp_resource.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 README.md
 setup.cfg
 setup.py
 djangoldp_resource/__init__.py
 djangoldp_resource/admin.py
 djangoldp_resource/apps.py
 djangoldp_resource/factories.py
-djangoldp_resource/filters.py
 djangoldp_resource/models.py
-djangoldp_resource/permissions.py
 djangoldp_resource/views.py
 djangoldp_resource.egg-info/PKG-INFO
 djangoldp_resource.egg-info/SOURCES.txt
 djangoldp_resource.egg-info/dependency_links.txt
 djangoldp_resource.egg-info/requires.txt
 djangoldp_resource.egg-info/top_level.txt
 djangoldp_resource/migrations/0001_initial.py
```

### Comparing `djangoldp_resource-3.1.2/setup.cfg` & `djangoldp_resource-3.1.3/setup.cfg`

 * *Files identical despite different names*

