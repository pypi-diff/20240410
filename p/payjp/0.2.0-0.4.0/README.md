# Comparing `tmp/payjp-0.2.0.tar.gz` & `tmp/payjp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payjp-0.2.0.tar", last modified: Mon Sep 26 09:59:06 2022, max compression
+gzip compressed data, was "payjp-0.4.0.tar", last modified: Wed Apr 10 02:25:12 2024, max compression
```

## Comparing `payjp-0.2.0.tar` & `payjp-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 09:59:06.342783 payjp-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-09-26 09:58:57.000000 payjp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-26 09:59:06.342783 payjp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-09-26 09:58:57.000000 payjp-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 09:59:06.338783 payjp-0.2.0/payjp/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13859 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 09:59:06.342783 payjp-0.2.0/payjp/test/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    15493 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/test_requestor.py
--rw-r--r--   0 runner    (1001) docker     (121)    30589 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-26 09:58:57.000000 payjp-0.2.0/payjp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 09:59:06.338783 payjp-0.2.0/payjp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-26 09:59:06.000000 payjp-0.2.0/payjp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-26 09:59:06.000000 payjp-0.2.0/payjp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 09:59:06.000000 payjp-0.2.0/payjp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-26 09:59:06.000000 payjp-0.2.0/payjp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-26 09:59:06.000000 payjp-0.2.0/payjp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-26 09:59:06.342783 payjp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-09-26 09:58:57.000000 payjp-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 02:25:03.000000 payjp-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 02:25:12.427127 payjp-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 02:25:03.000000 payjp-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 02:25:03.000000 payjp-0.4.0/payjp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:25:12.427127 payjp-0.4.0/payjp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 02:25:12.000000 payjp-0.4.0/payjp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:25:12.427127 payjp-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 02:25:03.000000 payjp-0.4.0/setup.py
```

### Comparing `payjp-0.2.0/LICENSE` & `payjp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/README.md` & `payjp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/api_requestor.py` & `payjp-0.4.0/payjp/api_requestor.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/error.py` & `payjp-0.4.0/payjp/error.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/http_client.py` & `payjp-0.4.0/payjp/http_client.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/resource.py` & `payjp-0.4.0/payjp/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 logger = logging.getLogger('payjp')
 
 def convert_to_payjp_object(resp, api_key, account, api_base=None):
     types = {'account': Account, 'card': Card,
              'charge': Charge, 'customer': Customer,
              'event': Event, 'plan': Plan,
              'subscription': Subscription, 'token': Token,
-             'transfer': Transfer, 'list': ListObject}
+             'transfer': Transfer, 'statement': Statement, 'list': ListObject, 'term': Term, 'balance': Balance}
 
     if isinstance(resp, list):
         return [convert_to_payjp_object(i, api_key, account, api_base) for i in resp]
     elif isinstance(resp, dict) and not isinstance(resp, PayjpObject):
         resp = resp.copy()
         klass_name = resp.get('object')
         if isinstance(klass_name, string_types):
@@ -418,7 +418,22 @@
         self.refresh_from(self.request('post', url, kwargs))
         return self
 
 
 class Transfer(ListableAPIResource):
     pass
 
+
+class Statement(ListableAPIResource):
+
+    def statement_urls(self, **kwargs):
+        url = self.instance_url() + '/statement_urls'
+        self.refresh_from(self.request('post', url, kwargs))
+        return self
+
+
+class Term(ListableAPIResource):
+    pass
+
+
+class Balance(ListableAPIResource):
+    pass
```

### Comparing `payjp-0.2.0/payjp/test/helper.py` & `payjp-0.4.0/payjp/test/helper.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/test/test_http_client.py` & `payjp-0.4.0/payjp/test/test_http_client.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/test/test_integration.py` & `payjp-0.4.0/payjp/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/test/test_requestor.py` & `payjp-0.4.0/payjp/test/test_requestor.py`

 * *Files identical despite different names*

### Comparing `payjp-0.2.0/payjp/test/test_resources.py` & `payjp-0.4.0/payjp/test/test_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # coding: utf-8
 
-import json
 import pickle
 import sys
-import time
-import datetime
 import unittest
 
 import payjp
 import payjp.resource
 
 from payjp.test.helper import (
     PayjpUnitTestCase, PayjpApiTestCase,
@@ -664,18 +661,19 @@
         self.assertTrue(obj is obj.delete())
 
         self.assertEqual(True, obj.deleted)
         self.assertEqual('mid', obj.id)
 
 
 class PayjpResourceTest(PayjpApiTestCase):
+    response = {}
 
     def setUp(self):
         super(PayjpResourceTest, self).setUp()
-        self.mock_response({})
+        self.mock_response(self.response)
 
 
 class ChargeTest(PayjpResourceTest):
 
     def test_charge_list_all(self):
         payjp.Charge.all(created={'lt': NOW})
 
@@ -1117,9 +1115,101 @@
             '/v1/charges/ch_foo',
             {
                 'metadata': {'whole': None},
             },
             None
         )
 
+
+class StatementTest(PayjpResourceTest):
+    response = {
+        'object': 'statement',
+        "id": "st_xxx",
+    }
+
+    def test_statement_urls(self):
+        statement = payjp.Statement.retrieve('st_xxx')
+        self.requestor_mock.request.assert_called_with(
+            'get', '/v1/statements/st_xxx', {}, None)
+        self.assertTrue(isinstance(statement, payjp.Statement))
+
+        statement.statement_urls(platformer=True)
+        self.requestor_mock.request.assert_called_with(
+            'post',
+            '/v1/statements/st_xxx/statement_urls',
+            {
+                'platformer': True,
+            },
+            None
+        )
+
+
+class TermTest(PayjpResourceTest):
+
+    def test_list_terms(self):
+        payjp.Term.all()
+        self.requestor_mock.request.assert_called_with(
+            'get',
+            '/v1/terms',
+            {}
+        )
+
+    def test_retrieve_term(self):
+        payjp.Term.retrieve('term_foo')
+        self.requestor_mock.request.assert_called_with(
+            'get',
+            '/v1/terms/term_foo',
+            {},
+            None
+        )
+
+
+class BalanceTest(PayjpResourceTest):
+    response = {
+        "created": 1438354800,
+        "id": "ba_xxx",
+        "livemode": False,
+        "net": 1000,
+        "object": "balance",
+        "state": "collecting",
+        "statements": [{
+            "balance_id": "ba_xxx",
+            "created": 1438354800,
+            "id": "st_xxx",
+            "object": "statement",
+        }],
+        "closed": False,
+        "due_date": None,
+        "bank_info": None,
+        "tenant_id": None
+    }
+
+    def test_list_balances(self):
+        payjp.Balance.all()
+        self.requestor_mock.request.assert_called_with(
+            'get',
+            '/v1/balances',
+            {}
+        )
+
+    def test_retrieve_balance(self):
+        balance = payjp.Balance.retrieve('balance_foo')
+        self.requestor_mock.request.assert_called_with(
+            'get',
+            '/v1/balances/balance_foo',
+            {},
+            None
+        )
+        self.assertTrue(isinstance(balance, payjp.Balance))
+        self.assertEqual(balance.id, 'ba_xxx')
+        self.assertTrue(isinstance(balance.statements[0], payjp.Statement))
+        balance.statements[0].statement_urls()
+        self.requestor_mock.request.assert_called_with(
+            'post',
+            '/v1/statements/st_xxx/statement_urls',
+            {},
+            None
+        )
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `payjp-0.2.0/setup.py` & `payjp-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     raise DeprecationWarning('Python 2.6 and older are no longer supported by PAY.JP. ')
 
 install_requires.append('requests >= 2.7.0')
 install_requires.append('six >= 1.9.0')
 
 setup(
     name="payjp",
-    version="0.2.0",
+    version="0.4.0",
     description='PAY.JP python bindings',
     author="PAY.JP",
     author_email='support@pay.jp',
     packages=['payjp', 'payjp.test'],
     url='https://github.com/payjp/payjp-python',
     install_requires=install_requires,
     tests_require=[
```

