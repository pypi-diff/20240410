# Comparing `tmp/djangoldp_event-3.1.2.tar.gz` & `tmp/djangoldp_event-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_event-3.1.2.tar", last modified: Wed Feb  7 14:49:50 2024, max compression
+gzip compressed data, was "djangoldp_event-3.1.3.tar", last modified: Wed Apr 10 11:05:11 2024, max compression
```

## Comparing `djangoldp_event-3.1.2.tar` & `djangoldp_event-3.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.980782 djangoldp_event-3.1.2/
--rw-r--r--   0 root         (0) root         (0)      258 2024-02-07 14:49:50.980782 djangoldp_event-3.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.976782 djangoldp_event-3.1.2/djangoldp_event/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-07 14:49:48.000000 djangoldp_event-3.1.2/djangoldp_event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.976782 djangoldp_event-3.1.2/djangoldp_event/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.976782 djangoldp_event-3.1.2/djangoldp_event/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/management/commands/mock_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.980782 djangoldp_event-3.1.2/djangoldp_event/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3506 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0002_auto_20200202_1639.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0003_auto_20200202_1644.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0004_auto_20200202_2110.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0004_auto_20200426_1603.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0005_auto_20200617_1458.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0006_auto_20200709_1411.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0007_merge_20200812_0928.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0008_merge_20200812_1009.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0009_auto_20200812_1446.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0010_auto_20200812_1459.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0011_auto_20200923_1017.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0012_event_author.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0013_auto_20210525_1018.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0014_auto_20210525_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0015_event_visible.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0016_auto_20210527_1612.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0017_auto_20221012_1503.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/0018_alter_event_options_alter_locationevent_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3451 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/models.py
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/djangoldp_event/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:49:50.976782 djangoldp_event-3.1.2/djangoldp_event.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2024-02-07 14:49:50.000000 djangoldp_event-3.1.2/djangoldp_event.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1635 2024-02-07 14:49:50.000000 djangoldp_event-3.1.2/djangoldp_event.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 14:49:50.000000 djangoldp_event-3.1.2/djangoldp_event.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-02-07 14:49:50.000000 djangoldp_event-3.1.2/djangoldp_event.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-07 14:49:50.000000 djangoldp_event-3.1.2/djangoldp_event.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-07 14:49:50.980782 djangoldp_event-3.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-07 14:49:29.000000 djangoldp_event-3.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.513947 djangoldp_event-3.1.3/
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-10 11:05:11.513947 djangoldp_event-3.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.509947 djangoldp_event-3.1.3/djangoldp_event/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-10 11:05:08.000000 djangoldp_event-3.1.3/djangoldp_event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.509947 djangoldp_event-3.1.3/djangoldp_event/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.513947 djangoldp_event-3.1.3/djangoldp_event/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/management/commands/mock_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.513947 djangoldp_event-3.1.3/djangoldp_event/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3506 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0002_auto_20200202_1639.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0003_auto_20200202_1644.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0004_auto_20200202_2110.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0004_auto_20200426_1603.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0005_auto_20200617_1458.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0006_auto_20200709_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0007_merge_20200812_0928.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0008_merge_20200812_1009.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0009_auto_20200812_1446.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0010_auto_20200812_1459.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0011_auto_20200923_1017.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0012_event_author.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0013_auto_20210525_1018.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0014_auto_20210525_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0015_event_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0016_auto_20210527_1612.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0017_auto_20221012_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/0018_alter_event_options_alter_locationevent_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/djangoldp_event/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:05:11.509947 djangoldp_event-3.1.3/djangoldp_event.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-10 11:05:11.000000 djangoldp_event-3.1.3/djangoldp_event.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-04-10 11:05:11.000000 djangoldp_event-3.1.3/djangoldp_event.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:05:11.000000 djangoldp_event-3.1.3/djangoldp_event.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-10 11:05:11.000000 djangoldp_event-3.1.3/djangoldp_event.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-10 11:05:11.000000 djangoldp_event-3.1.3/djangoldp_event.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-04-10 11:05:11.513947 djangoldp_event-3.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-10 11:04:50.000000 djangoldp_event-3.1.3/setup.py
```

### Comparing `djangoldp_event-3.1.2/djangoldp_event/admin.py` & `djangoldp_event-3.1.3/djangoldp_event/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0001_initial.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0002_auto_20200202_1639.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0002_auto_20200202_1639.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0004_auto_20200202_2110.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0004_auto_20200202_2110.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0005_auto_20200617_1458.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0005_auto_20200617_1458.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0006_auto_20200709_1411.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0006_auto_20200709_1411.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0009_auto_20200812_1446.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0009_auto_20200812_1446.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0010_auto_20200812_1459.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0010_auto_20200812_1459.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0011_auto_20200923_1017.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0011_auto_20200923_1017.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0012_event_author.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0012_event_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0013_auto_20210525_1018.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0013_auto_20210525_1018.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0014_auto_20210525_1022.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0014_auto_20210525_1022.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0016_auto_20210527_1612.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0016_auto_20210527_1612.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/migrations/0018_alter_event_options_alter_locationevent_options_and_more.py` & `djangoldp_event-3.1.3/djangoldp_event/migrations/0018_alter_event_options_alter_locationevent_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/djangoldp_event/models.py` & `djangoldp_event-3.1.3/djangoldp_event/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
 from djangoldp_circle.models import Circle
-from djangoldp.permissions import AuthenticatedOnly, AnonymousReadOnly, ReadAndCreate, ACLPermissions
+from djangoldp.permissions import AuthenticatedOnly, AnonymousReadOnly, ReadAndCreate, ACLPermissions, InheritPermissions
 
 
 class Typeevent (Model):
     name = models.CharField(max_length=50, blank=True, null=True, verbose_name="Type d'évènement")
 
     class Meta(Model.Meta):
         permission_classes = [AuthenticatedOnly]
@@ -57,12 +57,13 @@
     visible = models.BooleanField(verbose_name="Visible sur le site", blank=True, null=True,  default=True)
 
     class Meta(Model.Meta):
         nested_fields = ['type', 'circle', 'author', 'location']
         ordering = ['startDate']
         auto_author = 'author'
         owner_field = 'author'
-        permission_classes = [AuthenticatedOnly, ReadAndCreate|ACLPermissions]
+        permission_classes = [AuthenticatedOnly, ReadAndCreate|ACLPermissions, InheritPermissions]
+        inherit_permissions = ['circle']
         rdf_type = 'sib:event'
 
     def __str__(self):
         return self.name
```

### Comparing `djangoldp_event-3.1.2/djangoldp_event.egg-info/SOURCES.txt` & `djangoldp_event-3.1.3/djangoldp_event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.1.2/setup.cfg` & `djangoldp_event-3.1.3/setup.cfg`

 * *Files identical despite different names*

