# Comparing `tmp/diaspora-event-sdk-0.2.1.tar.gz` & `tmp/diaspora-event-sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.1.tar", last modified: Mon Apr  8 03:54:06 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.2.tar", last modified: Wed Apr 10 18:50:28 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.1.tar` & `diaspora-event-sdk-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158544 diaspora-event-sdk-0.2.1/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-08 03:54:06.158436 diaspora-event-sdk-0.2.1/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.153341 diaspora-event-sdk-0.2.1/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.155040 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     6964 2024-04-08 03:10:38.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.157044 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.157408 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     3724 2024-04-08 02:59:36.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-08 03:30:12.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.153857 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-08 03:54:06.000000 diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-08 03:54:06.158585 diaspora-event-sdk-0.2.1/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158056 diaspora-event-sdk-0.2.1/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.1/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-08 03:54:06.158147 diaspora-event-sdk-0.2.1/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.1/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.1/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499890 diaspora-event-sdk-0.2.2/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-10 18:50:28.499773 diaspora-event-sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.496796 diaspora-event-sdk-0.2.2/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.498102 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7503 2024-04-10 18:49:14.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499063 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499252 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3679 2024-04-10 18:01:19.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-10 18:49:26.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.497355 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-10 18:50:28.499939 diaspora-event-sdk-0.2.2/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499371 diaspora-event-sdk-0.2.2/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499452 diaspora-event-sdk-0.2.2/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.2/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.2/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.1/LICENSE` & `diaspora-event-sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/PKG-INFO` & `diaspora-event-sdk-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.1/README.md` & `diaspora-event-sdk-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def logout(self):
         """Remove credentials from your local system"""
         self.login_manager.logout()
 
     @requires_login
     def create_key(self):
         """
-        Invalidate previous keys (if any) and generate a new one
+        Revokes existing keys, generates a new key, and updates the token storage with the newly created key and the Diaspora endpoint.
         """
         resp = self.web_client.create_key(self.subject_openid)
         if resp["status"] == "error":
             raise Exception("should not happen")
         tokens = self.login_manager._token_storage.get_token_data(
             DIASPORA_RESOURCE_SERVER
         )
@@ -66,15 +66,15 @@
             "secret_key": tokens["secret_key"],
             "endpoint": tokens["endpoint"],
         }
 
     @requires_login
     def retrieve_key(self):
         """
-        Attempt to retrieve the key from local token storage, and call create_key if local key is not found
+        Retrieves the key from local token storage, and calls create_key() if the local key is not found.
         """
         tokens = self.login_manager._token_storage.get_token_data(
             DIASPORA_RESOURCE_SERVER
         )
         if (
             tokens is None
             or "endpoint" not in tokens
@@ -110,89 +110,89 @@
                 ],
             )
             self.login_manager._token_storage._connection.commit()
 
     @requires_login
     def list_topics(self):
         """
-        Retrieves the list of topics associated with the user's OpenID.
+        Returns a list of topics currently registered under the user's account.
         """
         return self.web_client.list_topics(self.subject_openid)
 
     @requires_login
     def register_topic(self, topic):
         """
-        Registers a new topic under the user's OpenID.
+        Registers a new topic the user's account with permissions to read, write, and describe the topic.
         """
         return self.web_client.register_topic(self.subject_openid, topic, "register")
 
     @requires_login
     def unregister_topic(self, topic):
         """
-        Unregisters a topic from the user's OpenID.
+        Unregisters a topic from a user's account, but all existing events within the topic are unaffected.
         """
         return self.web_client.register_topic(self.subject_openid, topic, "unregister")
 
     @requires_login
     def get_topic_configs(self, topic):
         """
-        Get topic configurations.
+        Retrieves the current configurations for a registered topic.
         """
         return self.web_client.get_topic_configs(self.subject_openid, topic)
 
     @requires_login
     def update_topic_configs(self, topic, configs):
         """
-        Set topic configurations.
+        Updates the configurations for a registered topic.
         """
         return self.web_client.update_topic_configs(self.subject_openid, topic, configs)
 
     @requires_login
     def update_topic_partitions(self, topic, new_partitions):
         """
-        Adjust topic number of partitions
+        Increases the number of partitions for a given topic to the specified new partition count.
         """
         return self.web_client.update_topic_partitions(self.subject_openid, topic, new_partitions)
 
     @requires_login
     def grant_user_access(self, topic, user):
         """
-        Registers a new topic under the user's OpenID.
+        Authorizes another user to access a registered topic under the invoker's account.
         """
         return self.web_client.grant_user_access(self.subject_openid, topic, user, "grant")
 
     @requires_login
     def revoke_user_access(self, topic, user):
         """
-        Unregisters a topic from the user's OpenID.
+        Removes access permissions for another user from a registered topic under the invoker's account.
         """
         return self.web_client.grant_user_access(self.subject_openid, topic, user, "revoke")
 
     @requires_login
     def list_triggers(self):
         """
-        Retrieves the list of functions associated with the user's OpenID.
+        Retrieves a list of triggers associated created under the user's account, showing each trigger's configurations and UUID.
         """
         return self.web_client.list_triggers(self.subject_openid)
 
     @requires_login
     def create_trigger(self, topic, function, function_configs, trigger_configs):
         """
-        Registers a new functions under the user's OpenID.
+        Creates a new trigger under the user's account with specific function and invocation configurations. 
         """
-        return self.web_client.create_trigger(self.subject_openid, topic, function, "create",
-                                              function_configs, trigger_configs)
+        return self.web_client.create_trigger(
+            self.subject_openid, topic, function, "create", function_configs, trigger_configs)
 
     @requires_login
     def delete_trigger(self, topic, function):
         """
-        Unregisters a functions from the user's OpenID.
+        Deletes a trigger and related AWS resources, while the associated topic remains unaffected.
         """
-        return self.web_client.create_trigger(self.subject_openid, topic, function, "delete",
-                                              {}, {})
+        return self.web_client.create_trigger(
+            self.subject_openid, topic, function, "delete", {}, {})
 
     @requires_login
     def update_trigger(self, trigger_uuid, trigger_configs):
         """
-        Update a functions's trigger'.
+        Updates invocation configurations of an existing trigger, identified by its unique trigger UUID.
         """
         return self.web_client.update_trigger(self.subject_openid, trigger_uuid, trigger_configs)
```

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/web_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     def list_topics(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/api/v2/topics", headers={"Subject": str(subject)})
 
     def register_topic(
         self, subject: UUID_LIKE_T, topic: str, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.put(
-            f"/api/v2/topic/{topic}", headers={"Subject": str(subject), "Action": action}
+            f"/api/v2/topic/{topic}",
+            headers={"Subject": str(subject), "Action": action}
         )
 
     def get_topic_configs(
         self, subject: UUID_LIKE_T, topic: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(
             f"/api/v2/topic/{topic}",
-            headers={"Subject": str(subject), "Topic": topic},
-            # data=json.dumps(configs).encode("utf-8")
+            headers={"Subject": str(subject), "Topic": topic}
         )
 
     def update_topic_configs(
         self, subject: UUID_LIKE_T, topic: str, configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}",
@@ -57,15 +57,15 @@
 
     def update_topic_partitions(
         self, subject: UUID_LIKE_T, topic: str, new_partitions: int
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/partitions",
             headers={"Subject": str(subject), "Topic": topic,
-                     "NewPartitions": str(new_partitions)},
+                     "NewPartitions": str(new_partitions)}
         )
 
     def grant_user_access(
         self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/topic/{topic}/user",
```

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.1/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/setup.py` & `diaspora-event-sdk-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.1/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.2/tests/unit/test_client.py`

 * *Files identical despite different names*

