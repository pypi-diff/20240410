# Comparing `tmp/saucelabs_visual-0.0.2.tar.gz` & `tmp/saucelabs_visual-0.0.3.tar.gz`

## Comparing `saucelabs_visual-0.0.2.tar` & `saucelabs_visual-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/build.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/dev.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/requirements/user.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/__init__.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/client.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/regions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/__init__.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/robot.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/.gitignore
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/README.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/requirements/build.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/requirements/dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/requirements/user.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/__init__.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/client.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/regions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/frameworks/__init__.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/src/saucelabs_visual/frameworks/robot.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/.gitignore
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/README.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.3/PKG-INFO
```

### Comparing `saucelabs_visual-0.0.2/src/saucelabs_visual/client.py` & `saucelabs_visual-0.0.3/src/saucelabs_visual/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
     def get_client(self) -> Client:
         return self.client
 
     def create_build(
             self,
             name: str = environ.get('SAUCE_VISUAL_BUILD_NAME') or None,
-            project: str = environ.get('SAUCE_VISUAL_PROJECT_NAME') or None,
-            branch: str = environ.get('SAUCE_VISUAL_BRANCH_NAME') or None,
-            default_branch: str = environ.get('SAUCE_VISUAL_DEFAULT_BRANCH_NAME') or None,
+            project: str = environ.get('SAUCE_VISUAL_PROJECT') or None,
+            branch: str = environ.get('SAUCE_VISUAL_BRANCH') or None,
+            default_branch: str = environ.get('SAUCE_VISUAL_DEFAULT_BRANCH') or None,
             custom_id: str = environ.get('SAUCE_VISUAL_CUSTOM_ID') or None,
             keep_alive_timeout: int = None
     ):
         query = gql(
             # language=GraphQL
             """
             mutation createBuild(
```

### Comparing `saucelabs_visual-0.0.2/src/saucelabs_visual/regions.py` & `saucelabs_visual-0.0.3/src/saucelabs_visual/regions.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.2/src/saucelabs_visual/frameworks/robot.py` & `saucelabs_visual-0.0.3/src/saucelabs_visual/frameworks/robot.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.2/.gitignore` & `saucelabs_visual-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.2/pyproject.toml` & `saucelabs_visual-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saucelabs_visual"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python bindings for Sauce Labs Visual"
 dependencies=[
     "aiohttp",
     "gql",
 ]
 readme = "README.md"
```

