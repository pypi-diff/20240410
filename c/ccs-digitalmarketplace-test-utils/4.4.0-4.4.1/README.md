# Comparing `tmp/ccs-digitalmarketplace-test-utils-4.4.0.tar.gz` & `tmp/ccs-digitalmarketplace-test-utils-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-test-utils-4.4.0.tar", last modified: Mon Apr  8 13:19:06 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-test-utils-4.4.1.tar", last modified: Wed Apr 10 10:11:45 2024, max compression
```

## Comparing `ccs-digitalmarketplace-test-utils-4.4.0.tar` & `ccs-digitalmarketplace-test-utils-4.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.325380 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 13:19:06.000000 ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.325380 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/audit_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/lot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:19:06.329380 ccs-digitalmarketplace-test-utils-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 13:18:57.000000 ccs-digitalmarketplace-test-utils-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:11:45.943889 ccs-digitalmarketplace-test-utils-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 10:11:45.943889 ccs-digitalmarketplace-test-utils-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:11:45.939888 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 10:11:45.000000 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 10:11:45.000000 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:11:45.000000 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 10:11:45.000000 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 10:11:45.000000 ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:11:45.943889 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:11:45.943889 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/audit_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/brief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/framework_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/lot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/supplier_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:11:45.943889 ccs-digitalmarketplace-test-utils-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-10 10:11:33.000000 ccs-digitalmarketplace-test-utils-4.4.1/setup.py
```

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/LICENCE` & `ccs-digitalmarketplace-test-utils-4.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/README.md` & `ccs-digitalmarketplace-test-utils-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-test-utils-4.4.1/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/__init__.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/audit_event.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/audit_event.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/base.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/brief.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/brief_response.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/brief_response.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/communication.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,33 @@
     supplier_user = {
         'id': 456,
         'email': 'test+456@digital.gov.uk'
     }
     default_data = {
         'id': 1234,
         'subject': 'Communication Subject',
+        'notificationEmails': [
+            'test+1@email.com',
+            'test+2@email.com',
+        ],
         'supplierId': 1234,
         'supplierName': "My Little Company",
         'frameworkSlug': 'g-cloud-14',
         'frameworkFramework': 'g-cloud',
         'frameworkFamily': 'g-cloud',
         'frameworkName': 'G-Cloud 14',
         'frameworkStatus': 'pending',
         'createdAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
         'updatedAt': DEFAULT_TIME.strftime(DATETIME_FORMAT),
         'links': {},
         'messages': [],
     }
     optional_keys = [
         ('supplierName', 'supplier_name'),
+        ('notificationEmails', 'notification_emails')
     ]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         if kwargs.get('archived'):
             self.response_data.update(**{
```

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/framework_agreement.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/framework_agreement.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/lot.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/lot.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/services.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/services.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/supplier.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/api_model_stubs/supplier_framework.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/api_model_stubs/supplier_framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/comparisons.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/comparisons.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/fixtures.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/fixtures.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/login.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/login.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/dmtestutils/mocking.py` & `ccs-digitalmarketplace-test-utils-4.4.1/dmtestutils/mocking.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-4.4.0/setup.py` & `ccs-digitalmarketplace-test-utils-4.4.1/setup.py`

 * *Files identical despite different names*

