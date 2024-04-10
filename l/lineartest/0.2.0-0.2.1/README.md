# Comparing `tmp/lineartest-0.2.0.tar.gz` & `tmp/lineartest-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.2.0.tar", max compression
+gzip compressed data, was "lineartest-0.2.1.tar", max compression
```

## Comparing `lineartest-0.2.0.tar` & `lineartest-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.2.0/LICENSE
--rw-r--r--   0        0        0     2237 2024-04-10 01:04:34.122025 lineartest-0.2.0/README.md
--rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.2.0/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-10 00:55:49.307063 lineartest-0.2.0/lineartest/_log.py
--rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.2.0/lineartest/_type.py
--rw-r--r--   0        0        0     7255 2024-04-10 00:57:52.049261 lineartest-0.2.0/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:00:18.116728 lineartest-0.2.0/lineartest/schedule.py
--rw-r--r--   0        0        0     1196 2024-04-10 01:03:55.785942 lineartest-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 lineartest-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2237 2024-04-10 07:28:02.170648 lineartest-0.2.1/README.md
+-rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.2.1/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.2.1/lineartest/_log.py
+-rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.2.1/lineartest/_type.py
+-rw-r--r--   0        0        0     7263 2024-04-10 07:28:02.171163 lineartest-0.2.1/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.2.1/lineartest/schedule.py
+-rw-r--r--   0        0        0     1196 2024-04-10 07:28:07.746983 lineartest-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 lineartest-0.2.1/PKG-INFO
```

### Comparing `lineartest-0.2.0/LICENSE` & `lineartest-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.0/README.md` & `lineartest-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.0/lineartest/_log.py` & `lineartest-0.2.1/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.0/lineartest/client.py` & `lineartest-0.2.1/lineartest/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         Initialize the `LinearClient` instance.
         :param test_client: the Starlette TestClient instance
         """
         super().__init__()
         self.test_client = test_client
 
     def _log(self, prefix: str, dct: dict[str, Any]):
-        for line in yaml.dump(dct).split('\n'):
+        for line in yaml.dump(dct).strip().split('\n'):
             print(prefix, line, sep='')
 
     def request(
         self,
         method: str,
         url: str,
         *,
```

### Comparing `lineartest-0.2.0/lineartest/schedule.py` & `lineartest-0.2.1/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.0/pyproject.toml` & `lineartest-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.2.0"
+version = "0.2.1"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `lineartest-0.2.0/PKG-INFO` & `lineartest-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.2.0
+Version: 0.2.1
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

