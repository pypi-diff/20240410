# Comparing `tmp/payload-api-0.4.7.tar.gz` & `tmp/payload-api-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payload-api-0.4.7.tar", last modified: Tue Jul 25 19:58:42 2023, max compression
+gzip compressed data, was "payload-api-0.4.8.tar", last modified: Wed Apr 10 03:18:33 2024, max compression
```

## Comparing `payload-api-0.4.7.tar` & `payload-api-0.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.7/LICENSE
--rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/__init__.py
--rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/attr.py
--rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/object.py
--rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.7/payload/arm/request.py
--rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/session.py
--rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/exceptions.py
--rw-r--r--   0        0        0     2255 2023-07-25 19:27:28.628182 payload-api-0.4.7/payload/objects.py
--rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/utils.py
--rw-r--r--   0        0        0      495 2023-07-18 16:01:06.820588 payload-api-0.4.7/payload/version.py
--rw-r--r--   0        0        0      766 2023-07-25 19:47:22.165762 payload-api-0.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0     4760 2023-07-25 19:52:34.456622 payload-api-0.4.7/tests/fixtures.py
--rw-r--r--   0        0        0      430 2023-07-25 19:53:17.275924 payload-api-0.4.7/tests/test_access_token.py
--rw-r--r--   0        0        0     3252 2023-07-25 19:51:47.197393 payload-api-0.4.7/tests/test_account.py
--rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_billing.py
--rw-r--r--   0        0        0     1660 2023-07-25 19:53:03.976140 payload-api-0.4.7/tests/test_invoice.py
--rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_payment_link.py
--rw-r--r--   0        0        0     3552 2023-07-25 19:53:31.039700 payload-api-0.4.7/tests/test_payment_method.py
--rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_request.py
--rw-r--r--   0        0        0     3515 2023-07-25 19:51:47.201393 payload-api-0.4.7/tests/test_session.py
--rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.7/tests/test_transaction.py
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-10 03:18:24.723776 payload-api-0.4.8/LICENSE
+-rw-r--r--   0        0        0      673 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/__init__.py
+-rw-r--r--   0        0        0     2104 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/attr.py
+-rw-r--r--   0        0        0     3930 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/object.py
+-rw-r--r--   0        0        0     7240 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/request.py
+-rw-r--r--   0        0        0      989 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/session.py
+-rw-r--r--   0        0        0     1282 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/exceptions.py
+-rw-r--r--   0        0        0     2356 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/objects.py
+-rw-r--r--   0        0        0     2782 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/utils.py
+-rw-r--r--   0        0        0      495 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/version.py
+-rw-r--r--   0        0        0      767 2024-04-10 03:18:24.727776 payload-api-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0     4866 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/fixtures.py
+-rw-r--r--   0        0        0      430 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_access_token.py
+-rw-r--r--   0        0        0     3252 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_account.py
+-rw-r--r--   0        0        0     1419 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_billing.py
+-rw-r--r--   0        0        0     1660 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_invoice.py
+-rw-r--r--   0        0        0     1416 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_payment_link.py
+-rw-r--r--   0        0        0     3655 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_payment_method.py
+-rw-r--r--   0        0        0    27269 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_request.py
+-rw-r--r--   0        0        0     3515 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_session.py
+-rw-r--r--   0        0        0     1473 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_transaction.py
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.8/PKG-INFO
```

### Comparing `payload-api-0.4.7/LICENSE` & `payload-api-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/__init__.py` & `payload-api-0.4.8/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/arm/attr.py` & `payload-api-0.4.8/payload/arm/attr.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/arm/object.py` & `payload-api-0.4.8/payload/arm/object.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/arm/request.py` & `payload-api-0.4.8/payload/arm/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,79 +2,81 @@
 import re
 import sys
 
 import payload
 import requests
 import copy
 
-from ..utils import (convert_fieldmap, map_attrs, map_object,
-                     nested_qstring_keys, object2data)
+from ..utils import convert_fieldmap, map_object, nested_qstring_keys, object2data
 from .attr import Attr
 from .object import ARMObject
 
-if sys.version_info >= (3,0):
+if sys.version_info >= (3, 0):
     from urllib.parse import urljoin
 else:
     from urlparse import urljoin
 
-class ARMRequest(object):
 
+class ARMRequest(object):
     def __init__(self, Object=None, session=None):
         self.Object = Object
         self.session = session
-        self._filters  = []
-        self._attrs    = []
+        self._filters = []
+        self._attrs = []
         self._group_by = []
 
     def _request(self, method, id=None, headers=None, params=None, json=None):
-        session  = self.session or payload
+        session = self.session or payload
         endpoint = self.Object.__spec__['endpoint']
-        headers  = headers or {}
-        params   = nested_qstring_keys(params or {})
-        auth     = (session.api_key, '')
-        files    = {}
+        headers = headers or {}
+        params = nested_qstring_keys(params or {})
+        auth = (session.api_key, '')
+        files = {}
 
         if json:
             flat_data = nested_qstring_keys(copy.copy(json))
             for k in list(flat_data):
-                if hasattr(flat_data[k], 'read'): files[k] = flat_data.pop(k)
+                if hasattr(flat_data[k], 'read'):
+                    files[k] = flat_data.pop(k)
 
-        if id: endpoint = f"{endpoint}/{id}"
+        if id:
+            endpoint = f'{endpoint}/{id}'
 
         if self._filters:
-            for k, v in dict( (f.attr, f.opval) for f in self._filters ).items():
-                if k not in params: params[k] = v
+            for k, v in dict((f.attr, f.opval) for f in self._filters).items():
+                if k not in params:
+                    params[k] = v
 
         if self._attrs:
-            params['fields'] = list(map(str,self._attrs))
+            params['fields'] = list(map(str, self._attrs))
 
         if self._group_by:
-            params['group_by'] = list(map(str,self._group_by))
+            params['group_by'] = list(map(str, self._group_by))
 
         convert_fieldmap(params, self.Object.field_map)
         if json:
             convert_fieldmap(json, self.Object.field_map)
         params = nested_qstring_keys(params)
 
         if files:
             response = getattr(requests, method)(
                 urljoin(session.api_url, endpoint.strip('/')),
                 params=params,
                 auth=auth,
                 data=flat_data,
-                files=files
-                )
+                files=files,
+            )
         else:
             response = getattr(requests, method)(
                 urljoin(session.api_url, endpoint.strip('/')),
                 headers=headers,
                 params=params,
                 auth=auth,
-                json=json
-                )
+                json=json,
+            )
         try:
             data = response.json()
 
             if not isinstance(data, dict):
                 raise payload.UnknownResponse()
         except ValueError:
             if response.status_code == 500:
@@ -87,18 +89,24 @@
                 for row in data['values']:
                     row['_session'] = self.session
                 return list(map(map_object, data['values']))
             else:
                 data['_session'] = self.session
                 return map_object(data)
         else:
-            errors = [ err for _ in payload.PayloadError.__subclasses__() for err in _.__subclasses__()+[_] ]
+            errors = [
+                err
+                for _ in payload.PayloadError.__subclasses__()
+                for err in _.__subclasses__() + [_]
+            ]
             for Error in errors:
-                if Error.__name__ != data.get('error_type') \
-                or Error.http_code != response.status_code:
+                if (
+                    Error.__name__ != data.get('error_type')
+                    or Error.http_code != response.status_code
+                ):
                     continue
                 raise Error(data.get('description'), data)
             if response.status_code == 500:
                 raise payload.InternalServerError(data.get('description'), data)
             raise payload.BadRequest(data.get('description'), data)
 
     def get(self, id, **params):
@@ -112,75 +120,78 @@
 
     def group_by(self, *fields):
         self._group_by.extend(fields)
         return self
 
     def create(self, obj=None, **values):
         obj = obj or values
-        if isinstance( obj, list ):
+        if isinstance(obj, list):
             for o in obj:
-                if not self.Object and not isinstance( o, ARMObject ):
+                if not self.Object and not isinstance(o, ARMObject):
                     raise TypeError('Bulk create requires ARMObject object types')
                 if not self.Object:
                     self.Object = o.__class__
-                elif isinstance( o, dict ):
-                    o.update(self.Object.__spec__.get('polymorphic',{}))
-                elif not isinstance( o, self.Object ):
+                elif isinstance(o, dict):
+                    o.update(self.Object.__spec__.get('polymorphic', {}))
+                elif not isinstance(o, self.Object):
                     raise TypeError('Bulk create requires all objects to be of the same type')
-            obj = { 'object': 'list', 'values': obj }
-        elif isinstance( obj, dict ):
-            obj.update(self.Object.__spec__.get('polymorphic',{}))
+            obj = {'object': 'list', 'values': obj}
+        elif isinstance(obj, dict):
+            obj.update(self.Object.__spec__.get('polymorphic', {}))
 
         obj = object2data(obj)
         return self._request('post', json=obj)
 
     def delete(self, objects=None):
-        if isinstance( objects, list ):
+        if isinstance(objects, list):
             if not objects:
                 raise ValueError('List must not be empty')
             for o in objects:
-                if not isinstance( o, ARMObject ):
+                if not isinstance(o, ARMObject):
                     raise TypeError('Bulk delete requires ARMObject object types')
                 if not self.Object:
                     self.Object = o.__class__
-                elif not isinstance( o, self.Object ):
+                elif not isinstance(o, self.Object):
                     raise TypeError('Bulk delete requires all objects to be of the same type')
-            delete_query = '|'.join([ obj.id for obj in objects ])
+            delete_query = '|'.join([obj.id for obj in objects])
             return self._request('delete', params={'id': delete_query, 'mode': 'query'})
-        elif isinstance( objects, ARMObject ):
+        elif isinstance(objects, ARMObject):
             self.Object = objects.__class__
             return self._request('delete', id=objects.id)
         elif objects is None and self.Object and self._filters:
-            return self._request('delete', params={'mode':'query'})
+            return self._request('delete', params={'mode': 'query'})
         else:
             raise TypeError('Bulk delete requires ARMObject object types')
 
     def update(self, objects=None, **values):
         if objects:
-            if not isinstance( objects, list ):
+            if not isinstance(objects, list):
                 raise ValueError('first parameter must be a list of updates')
-            if not objects or not isinstance( objects[0], (list, tuple) ):
+            if not objects or not isinstance(objects[0], (list, tuple)):
                 raise ValueError('first parameter must be a list of updates')
             for o, upd in objects:
-                if not isinstance( o, ARMObject ):
+                if not isinstance(o, ARMObject):
                     raise TypeError('Bulk update requires ARMObject object types')
                 if not self.Object:
                     self.Object = o.__class__
-                elif not isinstance( o, self.Object ):
+                elif not isinstance(o, self.Object):
                     raise TypeError('Bulk update requires all objects to be of the same type')
-            updates = { 'object': 'list', 'values':
-                list(map( lambda upd: dict( upd[1], id=upd[0].id ), objects )) }
+            updates = {
+                'object': 'list',
+                'values': list(map(lambda upd: dict(upd[1], id=upd[0].id), objects)),
+            }
             return self._request('put', json=updates)
-        return self._request('put', params={'mode':'query'}, json=values)
+        return self._request('put', params={'mode': 'query'}, json=values)
 
     def filter_by(self, *filters, **kw_filters):
         self._filters.extend(filters)
         for key, val in nested_qstring_keys(kw_filters).items():
-            self._filters.append( getattr( Attr, key ) == val )
+            self._filters.append(getattr(Attr, key) == val)
         return self
 
     def all(self):
         return self._request('get')
 
     def first(self):
         resp = self._request('get', params=dict(limit=1))
-        if resp: return resp[0]
+        if resp:
+            return resp[0]
```

### Comparing `payload-api-0.4.7/payload/arm/session.py` & `payload-api-0.4.8/payload/arm/session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/exceptions.py` & `payload-api-0.4.8/payload/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/payload/objects.py` & `payload-api-0.4.8/payload/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 class AccessToken(ARMObject):
     __spec__ = {'object': 'access_token'}
 
 class ClientToken(AccessToken):
     __spec__ = { 'polymorphic': { 'type': 'client' } }
 
+class OAuthToken(ARMObject):
+    __spec__ = { 'endpoint': '/oauth/token', 'object': 'oauth_token' }
+
 class Account(ARMObject):
     __spec__ = { 'object': 'account' }
 
 class Customer(ARMObject):
     __spec__ = { 'object': 'customer' }
 
 class ProcessingAccount(ARMObject):
```

### Comparing `payload-api-0.4.7/payload/utils.py` & `payload-api-0.4.8/payload/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .arm.object import ARMObject, _object_cache
 from .arm.attr import Attr
 
+
 def get_object_cls(item):
     cls = None
     for Object in _object_cache:
         if Object.__spec__['object'] != item.get('object'):
             continue
         if 'polymorphic' in Object.__spec__:
             found = True
@@ -15,93 +16,83 @@
             if found:
                 cls = Object
                 break
         elif not cls:
             cls = Object
     return cls
 
+
 def map_object(item):
     cls = get_object_cls(item)
     if cls:
         return cls(**item)
     return item
 
+
 def nested_qstring_keys(base):
     def recurse(item, fmt='{}'):
-        if isinstance( item, (list,tuple) ):
+        if isinstance(item, (list, tuple)):
             _iter = enumerate(item)
         else:
             _iter = list(item.items())
         for key, val in _iter:
             new_key = fmt.format(key)
             if not isinstance(item[key], (dict, list, tuple)):
                 if isinstance(val, Attr):
                     val = str(Attr)
                 base[new_key] = val
             else:
-                if item is base: del base[key]
-                recurse(val, new_key+'[{}]')
+                if item is base:
+                    del base[key]
+                recurse(val, new_key + '[{}]')
         return base
+
     return recurse(base)
 
+
 def data2object(item, field_map=set(), session=None):
     def recurse(item):
-        if isinstance( item, (list,tuple) ):
+        if isinstance(item, (list, tuple)):
             _iter = enumerate(item)
         else:
             convert_fieldmap(item, field_map)
             _iter = list(item.items())
         for key, val in _iter:
             if isinstance(val, (list, dict)):
                 item[key] = recurse(val)
-            if isinstance(val, dict)\
-            and val.get('object'):
+            if isinstance(val, dict) and val.get('object'):
                 Object = get_object_cls(val)
                 if Object:
                     if session:
                         val['_session'] = session
                     item[key] = Object(**val)
         return item
+
     return recurse(item)
 
+
 def convert_fieldmap(obj, field_map):
     for f in field_map:
-        if 'type' not in obj: continue
+        if 'type' not in obj:
+            continue
         if obj['type'] not in obj:
             obj[obj['type']] = {}
         if f in obj:
             obj[obj['type']][f] = obj.pop(f)
 
+
 def object2data(item):
     def recurse(item):
-        if isinstance( item, (list,tuple) ):
+        if isinstance(item, (list, tuple)):
             _iter = enumerate(item)
         else:
-            if isinstance( item, ARMObject ):
+            if isinstance(item, ARMObject):
                 item = item.data()
             _iter = list(item.items())
         for key, val in _iter:
             if isinstance(val, ARMObject):
                 item[key] = val.data()
             elif isinstance(val, (list, dict)):
                 item[key] = recurse(val)
         return item
-    return recurse(item)
 
-def map_attrs( cls, item ):
-    if isinstance( item, cls ):
-        item = item.data()
-    for key in item:
-        if isinstance(item[key], ARMObject):
-            map_attrs(item[key].__class__, item[key])
-            continue
-        if not cls.__spec__.get('attr_map')\
-        or key not in cls.attr_map:
-            continue
-        key_map = cls.__spec__['attr_map'][key]
-        if isinstance( new_key, str ):
-            obj[key_map] = item.pop(key)
-        else:
-            nested_key = list(key_map.keys())[0]
-            if nested_key not in obj:
-                obj[nested_key] = {}
-            obj[nested_key][key_map[nested_key]] = obj.pop(key)
+    return recurse(item)
```

### Comparing `payload-api-0.4.7/pyproject.toml` & `payload-api-0.4.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "payload-api"
-version = "0.4.7"
+version = "0.4.8"
 description = "Payload Python Library"
 authors = [
     { name = "Ian Halpern", email = "ian@payload.co" },
 ]
 dependencies = [
     "requests",
     "six",
@@ -39,10 +39,10 @@
 
 [tool.pdm.scripts._]
 env_file = ".env"
 
 [tool.black]
 line-length = 96
 target-version = [
-    "py38",
+    "py311",
 ]
 skip-string-normalization = true
```

### Comparing `payload-api-0.4.7/tests/fixtures.py` & `payload-api-0.4.8/tests/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,19 @@
         return processing_account
 
     @pytest.fixture
     def card_payment(self, processing_account):
         card_payment = pl.Payment.create(
             processing_id=processing_account.id,
             amount=random.random() * 100,
-            payment_method=pl.Card(card_number='4242 4242 4242 4242', expiry='12/25'),
+            payment_method=pl.Card(
+                card_number='4242 4242 4242 4242',
+                expiry='12/35',
+                billing_address=dict(postal_code='11111'),
+            ),
         )
         return card_payment
 
     @pytest.fixture
     def bank_payment(self):
         bank_payment = pl.Payment.create(
             type='payment',
```

### Comparing `payload-api-0.4.7/tests/test_account.py` & `payload-api-0.4.8/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/tests/test_billing.py` & `payload-api-0.4.8/tests/test_billing.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/tests/test_invoice.py` & `payload-api-0.4.8/tests/test_invoice.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/tests/test_payment_link.py` & `payload-api-0.4.8/tests/test_payment_link.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/tests/test_payment_method.py` & `payload-api-0.4.8/tests/test_payment_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,18 @@
         rand_description = ''.join(random.choice(letters) for i in range(10))
 
         card_payment = pl.Payment.create(
             amount=100.0,
             description=rand_description,
             processing_id=processing_account.id,
             payment_method=pl.Card(
-                card_number='4242 4242 4242 4242', expiry='05/35', card_code='123'
+                card_number='4242 4242 4242 4242',
+                expiry='05/35',
+                card_code='123',
+                billing_address=dict(postal_code='11111'),
             ),
         )
 
         payments = pl.Payment.filter_by(
             pl.attr.amount > 99,
             pl.attr.amount < (200),
             pl.attr.description.contains(rand_description),
@@ -87,15 +90,15 @@
 
         assert refund.type == 'refund'
         assert refund.amount == bank_payment.amount
         assert refund.status_code == 'approved'
 
     def test_partial_refund_bank_payment(self, api_key, bank_payment):
         refund = pl.Refund.create(
-            amount=10, ledger=[pl.Ledger(assoc_transaction_id=bank_payment.id)]
+            amount=10, ledger=[pl.Ledger(amount=10, assoc_transaction_id=bank_payment.id)]
         )
 
         assert refund.type == 'refund'
         assert refund.amount == 10
         assert refund.status_code == 'approved'
 
     def test_invalid_payment_method_type_invalid_attributes(self, api_key):
```

### Comparing `payload-api-0.4.7/tests/test_request.py` & `payload-api-0.4.8/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from payload.utils import (
     get_object_cls,
     map_object,
     nested_qstring_keys,
     data2object,
     convert_fieldmap,
     object2data,
-    map_attrs,
 )
 
 from payload.utils import get_object_cls
 from mock import Mock, patch, call, create_autospec
 import pytest
 import payload
 from unittest.mock import Mock, patch
@@ -68,15 +67,15 @@
 @pytest.fixture(scope='function')
 def arm_request_from_class(arm_object_class, mock_session):
     return ARMRequest(Object=arm_object_class['Object'], session=mock_session)
 
 
 @pytest.fixture
 def mock_session():
-    return Mock(api_url="test", api_key="test")
+    return Mock(api_url='test', api_key='test')
 
 
 @pytest.fixture
 def mock_response():
     return Mock()
 
 
@@ -86,31 +85,29 @@
 
 
 def test_armrequest_init():
     session = Mock()
     arm_request = ARMRequest(MockArmObject, session)
     assert arm_request.Object == MockArmObject
     assert arm_request.session == session
-    assert arm_request._filters == []
-    assert arm_request._attrs == []
-    assert arm_request._group_by == []
+    assert not arm_request._filters
+    assert not arm_request._attrs
+    assert not arm_request._group_by
 
 
 @pytest.mark.parametrize(
     'test_case',
     [
         {
             'obj': MockArmObject(_session=Mock(), name='Test Object'),
             'expected_json': {'name': 'Test Object'},
         },
         {'obj': {'name': 'Test Object'}, 'expected_json': {'name': 'Test Object'}},
         {
-            'obj': [
-                MockArmObject(_session=Mock(), name='Test Object') for _ in range(2)
-            ],
+            'obj': [MockArmObject(_session=Mock(), name='Test Object') for _ in range(2)],
             'expected_json': {
                 'object': 'list',
                 'values': [{'name': 'Test Object'}, {'name': 'Test Object'}],
             },
         },
         {
             'obj': [{'name': 'John'}, {'name': 'Doe'}],
@@ -124,15 +121,17 @@
             'obj': [Mock()],
             'expected_exception': TypeError,
             'expected_exception_message': 'Bulk create requires ARMObject object types',
         },
         {
             'obj': [Account(), Transaction()],
             'expected_exception': TypeError,
-            'expected_exception_message': 'Bulk create requires all objects to be of the same type',
+            'expected_exception_message': (
+                'Bulk create requires all objects to be of the same type'
+            ),
         },
         {'obj': [], 'expected_json': {}},
     ],
     ids=[
         'single_armobject',
         'single_dictionary',
         'multi_armobjects',
@@ -189,15 +188,17 @@
             'objects': [Mock()],
             'expected_exception': TypeError,
             'expected_exception_message': 'Bulk delete requires ARMObject object types',
         },
         {
             'objects': [Account(id='1'), Transaction(id='1')],
             'expected_exception': TypeError,
-            'expected_exception_message': 'Bulk delete requires all objects to be of the same type',
+            'expected_exception_message': (
+                'Bulk delete requires all objects to be of the same type'
+            ),
         },
     ],
     ids=[
         'single_armobject',
         'multi_armobjects',
         'query_mode',
         'incorrect_object_type',
@@ -235,17 +236,15 @@
             'values': {},
             'expected_json': {
                 'object': 'list',
                 'values': [{'id': '1', 'name': 'Updated Object'}],
             },
         },
         {
-            'objects': [
-                ({'id': '1', 'name': 'Test Object'}, {'name': 'Updated Object'})
-            ],
+            'objects': [({'id': '1', 'name': 'Test Object'}, {'name': 'Updated Object'})],
             'values': {},
             'expected_exception': TypeError,
             'expected_exception_message': 'Bulk update requires ARMObject object types',
         },
         {
             'objects': [
                 (
@@ -302,15 +301,17 @@
         {
             'objects': [
                 (Transaction(), {'name': 'Updated Object 1'}),
                 (Account(), {'name': 'Updated Object 2'}),
             ],
             'values': {},
             'expected_exception': TypeError,
-            'expected_exception_message': 'Bulk update requires all objects to be of the same type',
+            'expected_exception_message': (
+                'Bulk update requires all objects to be of the same type'
+            ),
         },
     ],
     ids=[
         'single_armobject',
         'mutli_values',
         'multi_armobjects',
         'multi_dict',
@@ -334,28 +335,38 @@
                 'put',
                 params=test_case['expected_params'],
                 json=test_case['expected_json'],
             )
         else:
             mock_request.assert_called_once_with('put', json=test_case['expected_json'])
 
-@pytest.mark.parametrize('attrs, expected_filters', [
-    (dict(attr1='value1', attr2='value2'), [['attr1', 'value1', 'value1'], ['attr2', 'value2', 'value2']]),
-    (dict(attr=dict(nested='value')), [['attr[nested]', 'value', 'value']]),
-    ([Attr.attr1=='value1'],[['attr1', 'value1', 'value1']]),
-    ([Attr.attr1!='value1'],[['attr1', '!value1', 'value1']]),
-    ([Attr.attr1>'value1'],[['attr1', '>value1', 'value1']]),
-    ([Attr.attr1>='value1'],[['attr1', '>=value1', 'value1']]),
-    ([Attr.attr1<'value1'],[['attr1', '<value1', 'value1']]),
-    ([Attr.attr1<='value1'],[['attr1', '<=value1', 'value1']]),
-    ([Attr.attr1.contains('value1')],[['attr1', '?*value1', 'value1']]),
-    ([Attr.attr1.func() == 'value1'],[['func(attr1)', 'value1', 'value1']]),
-    ([Attr.attr1.nested.func() == 'value1'],[['func(attr1[nested])', 'value1', 'value1']]),
-    ([Attr.attr1.nested.func() != 'value1'],[['func(attr1[nested])', '!value1', 'value1']]),
-])
+
+@pytest.mark.parametrize(
+    'attrs, expected_filters',
+    [
+        (
+            dict(attr1='value1', attr2='value2'),
+            [['attr1', 'value1', 'value1'], ['attr2', 'value2', 'value2']],
+        ),
+        (dict(attr=dict(nested='value')), [['attr[nested]', 'value', 'value']]),
+        ([Attr.attr1 == 'value1'], [['attr1', 'value1', 'value1']]),
+        ([Attr.attr1 != 'value1'], [['attr1', '!value1', 'value1']]),
+        ([Attr.attr1 > 'value1'], [['attr1', '>value1', 'value1']]),
+        ([Attr.attr1 >= 'value1'], [['attr1', '>=value1', 'value1']]),
+        ([Attr.attr1 < 'value1'], [['attr1', '<value1', 'value1']]),
+        ([Attr.attr1 <= 'value1'], [['attr1', '<=value1', 'value1']]),
+        ([Attr.attr1.contains('value1')], [['attr1', '?*value1', 'value1']]),
+        ([Attr.attr1.func() == 'value1'], [['func(attr1)', 'value1', 'value1']]),
+        ([Attr.attr1.nested.func() == 'value1'], [['func(attr1[nested])', 'value1', 'value1']]),
+        (
+            [Attr.attr1.nested.func() != 'value1'],
+            [['func(attr1[nested])', '!value1', 'value1']],
+        ),
+    ],
+)
 def test_armrequest_filter_by(arm_request, attrs, expected_filters):
     if isinstance(attrs, dict):
         request = arm_request.filter_by(**attrs)
     else:
         request = arm_request.filter_by(*attrs)
 
     assert len(arm_request._filters) == len(expected_filters)
@@ -456,17 +467,15 @@
     )
 
 
 def test_armrequest_request_params(arm_request, mock_response):
     test_params = {'param1': 'value1'}
 
     with patch('requests.get') as mock_get:
-        mock_response.json.return_value = {
-            'object': arm_request.Object.__spec__['object']
-        }
+        mock_response.json.return_value = {'object': arm_request.Object.__spec__['object']}
         mock_response.status_code = 200
         mock_get.return_value = mock_response
 
         arm_request._request('get', params=test_params)
 
         assert_mock_get_called_with_correct_values(
             arm_request, mock_get, expected_params=test_params
@@ -558,17 +567,15 @@
 
     assert_mock_get_called_with_correct_values(arm_request, mock_get)
 
 
 def test_armrequest_request_non_matching_error_and_http_code(arm_request):
     with patch(
         'requests.get',
-        return_value=Mock(
-            status_code=400, json=lambda: {'error_type': 'InternalServerError'}
-        ),
+        return_value=Mock(status_code=400, json=lambda: {'error_type': 'InternalServerError'}),
     ) as mock_get:
         with pytest.raises(payload.BadRequest):
             arm_request._request('get')
 
         assert_mock_get_called_with_correct_values(arm_request, mock_get)
 
 
@@ -622,17 +629,15 @@
 def test_data2object(arm_object_class):
     item_data = {'object': arm_object_class['object']}
     if 'polymorphic' in arm_object_class:
         item_data.update(arm_object_class['polymorphic'])
     field_map = set()
     session = None
     expected = (
-        arm_object_class['Object'](**item_data)
-        if arm_object_class['Object']
-        else item_data
+        arm_object_class['Object'](**item_data) if arm_object_class['Object'] else item_data
     )
     assert data2object(item_data, field_map, session) is expected
 
 
 # Test convert_fieldmap
 @pytest.mark.parametrize('arm_object_class', arm_object_classes)
 def test_convert_fieldmap(arm_object_class):
```

### Comparing `payload-api-0.4.7/tests/test_session.py` & `payload-api-0.4.8/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.7/tests/test_transaction.py` & `payload-api-0.4.8/tests/test_transaction.py`

 * *Files identical despite different names*

