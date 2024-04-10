# Comparing `tmp/PyLoadAPI-1.0.0.tar.gz` & `tmp/PyLoadAPI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLoadAPI-1.0.0.tar", last modified: Mon Apr  8 17:01:59 2024, max compression
+gzip compressed data, was "PyLoadAPI-1.0.1.tar", last modified: Tue Apr  9 21:20:16 2024, max compression
```

## Comparing `PyLoadAPI-1.0.0.tar` & `PyLoadAPI-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:01:59.644626 PyLoadAPI-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 17:01:59.644626 PyLoadAPI-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 17:01:59.644626 PyLoadAPI-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:01:59.640626 PyLoadAPI-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:01:59.644626 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 17:01:59.000000 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 17:01:59.000000 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:01:59.000000 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 17:01:59.000000 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 17:01:59.000000 PyLoadAPI-1.0.0/src/PyLoadAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:01:59.644626 PyLoadAPI-1.0.0/src/pyloadapi/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/src/pyloadapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/src/pyloadapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/src/pyloadapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:01:49.000000 PyLoadAPI-1.0.0/src/pyloadapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:20:16.658829 PyLoadAPI-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 21:20:16.658829 PyLoadAPI-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 21:20:16.658829 PyLoadAPI-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:20:16.654829 PyLoadAPI-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:20:16.654829 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 21:20:16.000000 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 21:20:16.000000 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:20:16.000000 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 21:20:16.000000 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 21:20:16.000000 PyLoadAPI-1.0.1/src/PyLoadAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:20:16.654829 PyLoadAPI-1.0.1/src/pyloadapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/src/pyloadapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/src/pyloadapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/src/pyloadapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 21:20:05.000000 PyLoadAPI-1.0.1/src/pyloadapi/types.py
```

### Comparing `PyLoadAPI-1.0.0/LICENSE` & `PyLoadAPI-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLoadAPI-1.0.0/pyproject.toml` & `PyLoadAPI-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyLoadAPI-1.0.0/setup.cfg` & `PyLoadAPI-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyLoadAPI
-version = 1.0.0
+version = 1.0.1
 author = Manfred Dennerlein Rodelo
 author_email = manfred@dennerlein.name
 description = "Simple wrapper for pyLoad's API."
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/tr4nt0r/PyLoadAPI
```

### Comparing `PyLoadAPI-1.0.0/src/pyloadapi/api.py` & `PyLoadAPI-1.0.1/src/pyloadapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             async with self._session.post(url, data=user_data) as r:
                 _LOGGER.debug(
                     "Response from %s [%s]: %s", url, r.status, (await r.text())
                 )
                 r.raise_for_status()
                 try:
                     data = await r.json()
-                    if not r:
+                    if not data:
                         raise InvalidAuth
                     return LoginResponse.from_dict(data)
                 except JSONDecodeError as e:
                     _LOGGER.error(
                         "Exception: Cannot parse login response:\n %s",
                         traceback.format_exc(),
                     )
@@ -63,17 +63,18 @@
         """Get general status information of pyLoad."""
         url = f"{self.api_url}api/statusServer"
         try:
             async with self._session.get(url) as r:
                 _LOGGER.debug(
                     "Response from %s [%s]: %s", url, r.status, (await r.text())
                 )
-                r.raise_for_status()
+
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     raise InvalidAuth
+                r.raise_for_status()
                 try:
                     data = await r.json()
                     return StatusServerResponse.from_dict(data)
                 except JSONDecodeError as e:
                     _LOGGER.error(
                         "Exception: Cannot parse status response:\n %s",
                         traceback.format_exc(),
```

### Comparing `PyLoadAPI-1.0.0/src/pyloadapi/types.py` & `PyLoadAPI-1.0.1/src/pyloadapi/types.py`

 * *Files identical despite different names*

