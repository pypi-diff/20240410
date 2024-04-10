# Comparing `tmp/imy-0.2.1.tar.gz` & `tmp/imy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.1.tar", max compression
+gzip compressed data, was "imy-0.2.2.tar", max compression
```

## Comparing `imy-0.2.1.tar` & `imy-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.1/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.1/imy/__init__.py
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.1/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.1/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.1/imy/config.py
--rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.1/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.1/imy/docstrings/models.py
--rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.1/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8342 2024-04-07 17:07:13.593234 imy-0.2.1/imy/inject.py
--rw-r--r--   0        0        0    12893 2024-03-31 11:34:08.656709 imy-0.2.1/imy/logs.py
--rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.1/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-08 18:36:41.516140 imy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.2/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.2/imy/__init__.py
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.2/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.2/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.2/imy/config.py
+-rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.2/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.2/imy/docstrings/models.py
+-rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.2/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.2/imy/inject.py
+-rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.2/imy/logs.py
+-rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.2/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-10 14:11:15.450664 imy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.2/PKG-INFO
```

### Comparing `imy-0.2.1/LICENSE` & `imy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/assets.py` & `imy-0.2.2/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/async_utils.py` & `imy-0.2.2/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/config.py` & `imy-0.2.2/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/docstrings/models.py` & `imy-0.2.2/imy/docstrings/models.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/docstrings/parsers.py` & `imy-0.2.2/imy/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/imy/inject.py` & `imy-0.2.2/imy/inject.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,14 +264,22 @@
 
             # Register the factory
             self._factories[key_type] = (param_keys, func)
             return func
 
         return decorator
 
+    def clear(self) -> None:
+        """
+        Removes any previously added components and factories from the injector.
+        """
+        self._components.clear()
+        self._factories.clear()
+
 
 # Expose a global injector
 GLOBAL_INJECTOR = Injector()
 
 get = GLOBAL_INJECTOR.__getitem__
 set = GLOBAL_INJECTOR.__setitem__
 bind = GLOBAL_INJECTOR.bind
+clear = GLOBAL_INJECTOR.clear
```

### Comparing `imy-0.2.1/imy/logs.py` & `imy-0.2.2/imy/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,14 +329,31 @@
         def sync_iterator() -> Iterator[LogEntry]:
             for change in self._sync_collection.watch(pipeline=pipeline):
                 yield LogEntry.from_bson(change["fullDocument"])
 
         return async_utils.iterator_to_thread(sync_iterator(), batch_size=1)
 
 
+def reset_logging() -> None:
+    """
+    Resets the logging system to its initial state. This removes all handlers
+    from the root logger and resets its level to `WARNING`.
+    """
+
+    # Get the root logger
+    root_logger = logging.getLogger()
+
+    # Remove all existing handlers
+    for handler in root_logger.handlers[:]:
+        root_logger.removeHandler(handler)
+
+    # Reset the root logger level
+    root_logger.setLevel(logging.WARNING)
+
+
 @overload
 def setup_logging(
     *,
     info_log_path: Path | None = None,
     debug_log_path: Path | None = None,
 ) -> MongoDbLogger:
     ...
@@ -363,15 +380,17 @@
     database_collection: pymongo.collection.Collection | None = None,
     database_environment: Environment | None = None,
     database_host: str | None = None,
     database_app: str | None = None,
     database_log_level: LogLevel = "debug",
 ) -> MongoDbLogger | None:
     """
-    Creates a nice logging setup.
+    Creates a nice logging setup. Any previously registered handlers are
+    removed, which means it is safe to call this function multiple times without
+    creating duplicate log entries.
 
     - INFO logs to `info_log_path`, keeping logs indefinitely
     - DEBUG logs to `stdout`
     - DEBUG logs to `debug_log_path`, keeping a limited number of days
     - DEBUG logs into the database
 
     Persistence loggers can lose some log entries if they are not flushed before
@@ -385,14 +404,18 @@
     """
 
     root_logger = logging.getLogger("")
     root_logger.setLevel(logging.DEBUG)
 
     formatter = logging.Formatter("%(asctime)s  %(levelname)-8s  %(message)s")
 
+    # Make sure not to add multiple handlers if the function is called multiple
+    # times.
+    reset_logging()
+
     # Info -> file
     if info_log_path is not None:
         info_log_path.parent.mkdir(parents=True, exist_ok=True)
 
         handler = logging.handlers.TimedRotatingFileHandler(
             info_log_path,
             encoding="utf-8",
```

### Comparing `imy-0.2.1/imy/package_metadata.py` & `imy-0.2.2/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.1/pyproject.toml` & `imy-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.1"
+version = "0.2.2"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.1/PKG-INFO` & `imy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

