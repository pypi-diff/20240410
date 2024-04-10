# Comparing `tmp/igz_mgmt-0.1.2.tar.gz` & `tmp/igz_mgmt-0.1.3.tar.gz`

## Comparing `igz_mgmt-0.1.2.tar` & `igz_mgmt-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/client.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/constants.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/operations.py
--rw-r--r--   0        0        0    90402 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/schemas/events.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/README.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/client.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    90860 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/events.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/README.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/PKG-INFO
```

### Comparing `igz_mgmt-0.1.2/igz_mgmt/__init__.py` & `igz_mgmt-0.1.3/igz_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/__version__.py` & `igz_mgmt-0.1.3/igz_mgmt/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 # x.y.zrcN
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `igz_mgmt-0.1.2/igz_mgmt/client.py` & `igz_mgmt-0.1.3/igz_mgmt/client.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/constants.py` & `igz_mgmt-0.1.3/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/cruds.py` & `igz_mgmt-0.1.3/igz_mgmt/cruds.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/exceptions.py` & `igz_mgmt-0.1.3/igz_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/operations.py` & `igz_mgmt-0.1.3/igz_mgmt/operations.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/resources.py` & `igz_mgmt-0.1.3/igz_mgmt/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,14 +749,23 @@
             user.relationships["user_groups"]["data"].append(
                 {"id": group_id, "type": "user_group"}
             )
             return True
 
         return False
 
+    def _fields_to_attributes(self, exclude_unset=True):
+        attributes = super()._fields_to_attributes(exclude_unset)
+
+        # set raw password and not SecretStr or else we hit json encoding issues
+        # anyway, we need to dump the password as a string when client tries to change it.
+        if self.password:
+            attributes["password"] = self.password.get_secret_value()
+        return attributes
+
 
 class Group(BaseResource, ProjectMembershipResource):
     """Group resource represents user group in the system."""
 
     type: str = "user_group"
     name: str = ""
     description: str = None
@@ -2267,15 +2276,15 @@
 
 class Event(BaseResource):
     """Event resource represents events in the system.
 
     Events are used to notify about changes in the system.
     """
 
-    type: str = "event"
+    type: typing.Optional[str] = "event"
 
     source: str = pydantic.Field(
         description="The originator of the event, in the form of a service ID (e.g. igz0.vn.3)",
         default="",
     )
     kind: str = pydantic.Field(
         description="A string in dot notation representing which event occurred",
@@ -2397,15 +2406,15 @@
 class AuditEvent(Event):
     """AuditEvent resource represents audit events in the system.
 
     Audit events are used to represent user and system actions within the system
 
     """
 
-    type = "audit_event"
+    type: typing.Optional[str] = "audit_event"
 
     @classmethod
     def delete_all(cls, http_client: igz_mgmt.client.APIClient):
         """Deleting audit events are not supported."""
         raise igz_mgmt.exceptions.ResourceDeleteException
 
     def emit(self, http_client, **kwargs):
```

### Comparing `igz_mgmt-0.1.2/igz_mgmt/common/__init__.py` & `igz_mgmt-0.1.3/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/common/helpers.py` & `igz_mgmt-0.1.3/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.1.3/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/logger/logger.py` & `igz_mgmt-0.1.3/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.1.3/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.1.3/igz_mgmt/schemas/app_services.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/schemas/events.py` & `igz_mgmt-0.1.3/igz_mgmt/schemas/events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.1.3/igz_mgmt/schemas/manual_events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/LICENSE` & `igz_mgmt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/pyproject.toml` & `igz_mgmt-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.2/PKG-INFO` & `igz_mgmt-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: igz-mgmt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

