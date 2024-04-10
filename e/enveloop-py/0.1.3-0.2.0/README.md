# Comparing `tmp/enveloop_py-0.1.3.tar.gz` & `tmp/enveloop_py-0.2.0.tar.gz`

## Comparing `enveloop_py-0.1.3.tar` & `enveloop_py-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/api.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/client.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/message.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/message_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/template.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/src/enveloop_py/template_response.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/LICENSE
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 enveloop_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/api.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/client.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/message.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/message_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/template.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/src/enveloop_py/template_response.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 enveloop_py-0.2.0/PKG-INFO
```

### Comparing `enveloop_py-0.1.3/src/enveloop_py/client.py` & `enveloop_py-0.2.0/src/enveloop_py/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     """Client class."""
 
     def __init__(self, api_key=None, api_host=None, ssl=None):
         """Initialize the client."""
         self._api_key = api_key
         self._endpoint = 'https://{}'.format(api_host) if ssl else 'http://{}'.format(api_host)
 
-    def send_message(self, template=None, to=None, from_address=None, subject=None, template_variables={}):
+    def send_message(self, template=None, html=None, to=None, from_address=None, subject=None, template_variables={}):
         data = {
             'to': to,
             'from': from_address,
             'subject': subject,
             'template': template,
+            'html': html,
             'templateVariables': template_variables
         }
 
         res = requests.post(
             '{}/messages'.format(self._endpoint),
             json=data,
             headers={'Authorization': 'token {}'.format(self._api_key)}
```

### Comparing `enveloop_py-0.1.3/src/enveloop_py/message.py` & `enveloop_py-0.2.0/src/enveloop_py/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 class Message:
     """Message class."""
 
     def __init__(self, api_response={}):
         """Initialize the template."""
+        self._message_id = api_response['messageId']
         self._to = api_response['to']
         self._from_address = api_response['from']
         self._body = api_response['body']
 
     @property
+    def message_id(self):
+        """Return the subject."""
+        return self._message_id
+
+    @property
     def to(self):
         """Return the subject."""
         return self._to
 
     @property
     def from_address(self):
         """Return the subject."""
```

### Comparing `enveloop_py-0.1.3/src/enveloop_py/message_response.py` & `enveloop_py-0.2.0/src/enveloop_py/message_response.py`

 * *Files identical despite different names*

### Comparing `enveloop_py-0.1.3/src/enveloop_py/template_response.py` & `enveloop_py-0.2.0/src/enveloop_py/template_response.py`

 * *Files identical despite different names*

### Comparing `enveloop_py-0.1.3/.gitignore` & `enveloop_py-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enveloop_py-0.1.3/LICENSE` & `enveloop_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enveloop_py-0.1.3/README.md` & `enveloop_py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `enveloop_py-0.1.3/pyproject.toml` & `enveloop_py-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "enveloop-py"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Ben Wyrosdick", email="ben.wyrosdick@gmail.com" },
 ]
 description = "Enveloop API SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `enveloop_py-0.1.3/PKG-INFO` & `enveloop_py-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: enveloop-py
-Version: 0.1.3
+Version: 0.2.0
 Summary: Enveloop API SDK
 Project-URL: Homepage, https://github.com/enveloophq/enveloop-py
 Project-URL: Bug Tracker, https://github.com/enveloophq/enveloop-py/issues
 Author-email: Ben Wyrosdick <ben.wyrosdick@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

