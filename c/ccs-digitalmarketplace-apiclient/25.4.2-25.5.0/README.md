# Comparing `tmp/ccs-digitalmarketplace-apiclient-25.4.2.tar.gz` & `tmp/ccs-digitalmarketplace-apiclient-25.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.4.2.tar", last modified: Fri Mar 22 12:12:33 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-apiclient-25.5.0.tar", last modified: Wed Apr 10 10:56:30 2024, max compression
```

## Comparing `ccs-digitalmarketplace-apiclient-25.4.2.tar` & `ccs-digitalmarketplace-apiclient-25.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:33.029007 ccs-digitalmarketplace-apiclient-25.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-22 12:12:33.029007 ccs-digitalmarketplace-apiclient-25.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:33.029007 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-22 12:12:32.000000 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-22 12:12:32.000000 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:12:32.000000 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 12:12:32.000000 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-22 12:12:32.000000 ccs-digitalmarketplace-apiclient-25.4.2/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:33.029007 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/antivirus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    46927 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/search.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 12:12:33.029007 ccs-digitalmarketplace-apiclient-25.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-22 12:12:24.000000 ccs-digitalmarketplace-apiclient-25.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:56:30.533310 ccs-digitalmarketplace-apiclient-25.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 10:56:30.533310 ccs-digitalmarketplace-apiclient-25.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:56:30.533310 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 10:56:30.000000 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-10 10:56:30.000000 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:56:30.000000 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 10:56:30.000000 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 10:56:30.000000 ccs-digitalmarketplace-apiclient-25.5.0/ccs_digitalmarketplace_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:56:30.533310 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/antivirus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47082 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 10:56:30.537310 ccs-digitalmarketplace-apiclient-25.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-10 10:56:21.000000 ccs-digitalmarketplace-apiclient-25.5.0/setup.py
```

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/LICENCE` & `ccs-digitalmarketplace-apiclient-25.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/README.md` & `ccs-digitalmarketplace-apiclient-25.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/antivirus.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/antivirus.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/audit.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     create_outcome = "create_outcome"
     complete_outcome = "complete_outcome"
     update_outcome = "update_outcome"
 
     # Mailing list actions
     mailing_list_subscription = "mailing_list_subscription"
 
-    # Conversations
+    # Communications
     create_communication = "create_communication"
     archive_communication = "archive_communication"
     send_communication_message = "send_communication_message"
     read_communication_message = "read_communication_message"
 
     @staticmethod
     def is_valid_audit_type(test_audit_type):
```

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/base.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/data.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1294,15 +1294,15 @@
                 "completed": completed,
             },
         )
 
     find_outcomes_iter = make_iter_method("find_outcomes", "outcomes")
     find_outcomes_iter.__name__ = str("find_outcomes_iter")
 
-    # Conversations
+    # Communications
 
     def find_communications(self, framework, supplier_id=None, latest_message_target=None, archived=None, page=None):
         warnings.warn(
             "The output of 'find_communications' is paginated. Use 'find_communications_iter' instead.",
             DeprecationWarning
         )
 
@@ -1346,23 +1346,33 @@
             "/communications/{}/messages".format(communication_id),
             data={
                 "communicationMessages": message,
             },
             user=user,
         )
 
-    def create_communication(self, supplier_id, framework_slug, subject, message, attachments=None, user=None):
+    def create_communication(
+        self,
+        supplier_id,
+        framework_slug,
+        subject,
+        notification_emails,
+        message,
+        attachments=None,
+        user=None
+    ):
         if attachments is not None:
             message["attachments"] = attachments
 
         return self._post_with_updated_by(
             "/communications",
             data={
                 "communications": {
                     "supplierId": supplier_id,
                     "frameworkSlug": framework_slug,
                     "subject": subject,
+                    "notificationEmails": notification_emails,
                     "messages": message
                 },
             },
             user=user,
         )
```

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/errors.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/dmapiclient/search.py` & `ccs-digitalmarketplace-apiclient-25.5.0/dmapiclient/search.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-apiclient-25.4.2/setup.py` & `ccs-digitalmarketplace-apiclient-25.5.0/setup.py`

 * *Files identical despite different names*

