# Comparing `tmp/pymasscode-1.0.0b2.tar.gz` & `tmp/pymasscode-1.0.0b3.tar.gz`

## Comparing `pymasscode-1.0.0b2.tar` & `pymasscode-1.0.0b3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/requirements-dev.lock
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/requirements.lock
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/.vscode/launch.json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/.vscode/settings.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/README.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/__init__.py
--rw-r--r--   0        0        0     8622 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/dcls.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/loader.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/model.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/pyproject.toml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/etc/clsprop.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/etc/fileProp.py
--rw-r--r--   0        0        0    22187 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/etc/tinydb_query.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/src/pymasscode/etc/utils.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/README.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pymasscode-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/requirements-dev.lock
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/requirements.lock
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/.vscode/launch.json
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/.vscode/settings.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/README.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/__init__.py
+-rw-r--r--   0        0        0     8622 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/dcls.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/loader.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/model.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/pyproject.toml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/etc/clsprop.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/etc/fileProp.py
+-rw-r--r--   0        0        0    22202 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/etc/tinydb_query.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/src/pymasscode/etc/utils.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/README.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pymasscode-1.0.0b3/PKG-INFO
```

### Comparing `pymasscode-1.0.0b2/.vscode/launch.json` & `pymasscode-1.0.0b3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pymasscode-1.0.0b2/src/pymasscode/dcls.py` & `pymasscode-1.0.0b3/src/pymasscode/dcls.py`

 * *Files identical despite different names*

### Comparing `pymasscode-1.0.0b2/src/pymasscode/loader.py` & `pymasscode-1.0.0b3/src/pymasscode/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,55 +50,61 @@
         self.__dbLockGate = 0
 
         if config is not None:
             self.config = config
         else:
             self.config = LoaderConfig.defaultConfig()
 
-        self.dbPath = dbPath
-        self.appdataPath = appdataPath
+        self.__dbPath = dbPath
+        self.__appdataPath = appdataPath
 
-        if self.dbPath and os.path.join(self.dbPath):
-            self.dbPath = os.path.abspath(self.dbPath)
-            assert os.path.exists(self.dbPath)
-            assert self.dbPath.endswith("db.json")
+        if self.__dbPath and os.path.join(self.__dbPath):
+            self.__dbPath = os.path.abspath(self.__dbPath)
+            assert os.path.exists(self.__dbPath)
+            assert self.__dbPath.endswith("db.json")
         else:
-            if not self.appdataPath:
-                self.appdataPath = Loader.getPossiblePathByPlatform()
+            if not self.__appdataPath:
+                self.__appdataPath = Loader.getPossiblePathByPlatform()
 
-            if not os.path.exists(self.appdataPath):
+            if not os.path.exists(self.__appdataPath):
                 raise RuntimeError(
                     "MassCode is not installed or initialized correctly."
                 )
 
-            self.dbPath = os.path.join(self.preferences["storagePath"], "db.json")
+            self.__dbPath = os.path.join(self.preferences["storagePath"], "db.json")
 
         # check if db path is empty (0kb), if yes, assume an error occured and restore bkup file if it exists
-        if not os.path.exists(self.dbPath) or os.path.getsize(self.dbPath) == 0:
-            if os.path.exists(os.path.dirname(self.dbPath) + "/db.bkup.json"):
-                shutil.copy(os.path.dirname(self.dbPath) + "/db.bkup.json", self.dbPath)
+        if not os.path.exists(self.__dbPath) or os.path.getsize(self.__dbPath) == 0:
+            if os.path.exists(os.path.dirname(self.__dbPath) + "/db.bkup.json"):
+                shutil.copy(os.path.dirname(self.__dbPath) + "/db.bkup.json", self.__dbPath)
 
         if self.config["create_bkup"]:
-            shutil.copy(self.dbPath, os.path.dirname(self.dbPath) + "/db.bkup.json")
+            shutil.copy(self.__dbPath, os.path.dirname(self.__dbPath) + "/db.bkup.json")
+
+    @property
+    def dbPath(self):
+        return self.__dbPath
+    
+    @property
+    def appdataPath(self):
+        return self.__appdataPath
 
     @property
     def preferencePath(self):
-        return os.path.join(self.appdataPath, "v2", "preferences.json")
+        return os.path.join(self.__appdataPath, "v2", "preferences.json")
 
-    preferences: dict = FileProperty(
-        os.path.join("{self.appdataPath}", "v2", "preferences.json")
-    )
+    preferences: dict = FileProperty(preferencePath)
 
     @property
     def appconfigPath(self):
-        return os.path.join(self.appdataPath, "v2", "app.json")
+        return os.path.join(self.__appdataPath, "v2", "app.json")
 
-    appconfig: dict = FileProperty(os.path.join("{self.appdataPath}", "v2", "app.json"))
+    appconfig: dict = FileProperty(appconfigPath)
 
-    dbIo: io.TextIOWrapper = FileProperty("{self.dbPath}", passOverIoOnly=True)
+    dbIo: io.TextIOWrapper = FileProperty(dbPath, loadmethod=FileProperty.returnIOWrapper)
 
     def dbFolders(self):
         for folder in self.dbContent["folders"]:
             yield folder
 
     def dbSnippets(self):
         for snippet in self.dbContent["snippets"]:
@@ -112,21 +118,21 @@
     def __dbContent(self):
         self.dbIo.seek(0)
         return json.load(self.dbIo)
 
     @property
     def dbContent(self) -> StorageData:
         if not hasattr(self, "__dbContentLastModified"):
-            self.__dbContentLastModified = os.path.getmtime(self.dbPath)
+            self.__dbContentLastModified = os.path.getmtime(self.__dbPath)
 
-        if self.__dbContentLastModified == os.path.getmtime(self.dbPath):
+        if self.__dbContentLastModified == os.path.getmtime(self.__dbPath):
             return self.__dbContent
 
         self.__dict__.pop("__dbContent", None)
-        self.__dbContentLastModified = os.path.getmtime(self.dbPath)
+        self.__dbContentLastModified = os.path.getmtime(self.__dbPath)
 
         return self.__dbContent
 
     @contextmanager
     def dbLock(self):
         try:
             self.__dbLockGate += 1
```

### Comparing `pymasscode-1.0.0b2/src/pymasscode/model.py` & `pymasscode-1.0.0b3/src/pymasscode/model.py`

 * *Files identical despite different names*

### Comparing `pymasscode-1.0.0b2/src/pymasscode/pyproject.toml` & `pymasscode-1.0.0b3/src/pymasscode/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymasscode-1.0.0b2/src/pymasscode/etc/tinydb_query.py` & `pymasscode-1.0.0b3/src/pymasscode/etc/tinydb_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     """
     A shorthand for ``Query()[key]``
     """
     return Query()[key]
 
 
 # ANCHOR modifications
-from thefuzz import fuzz  # noqa
+from thefuzz import fuzz  # type: ignore # noqa
 
 
 class MQuery(Query):
     @staticmethod
     def __childrunner(paths, test, value):
         try:
             # Resolve the path
```

### Comparing `pymasscode-1.0.0b2/pyproject.toml` & `pymasscode-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymasscode"
-version = "1.0.0b2"
+version = "1.0.0b3"
 description = "Masscode query and api wrapper"
 authors = [
     { name = "ZackaryW", email = "36378555+ZackaryW@users.noreply.github.com" }
 ]
 dependencies = [
     "thefuzz>=0.22.1",
 ]
```

