# Comparing `tmp/hauntedhouse-0.1.8.tar.gz` & `tmp/hauntedhouse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hauntedhouse-0.1.8.tar", last modified: Mon Mar 25 19:08:12 2024, max compression
+gzip compressed data, was "hauntedhouse-0.1.9.tar", last modified: Wed Apr 10 15:25:06 2024, max compression
```

## Comparing `hauntedhouse-0.1.8.tar` & `hauntedhouse-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-03-25 19:08:12.664969 hauntedhouse-0.1.8/
--rw-r--r--   0 asdougl   (1000) asdougl   (1000)      353 2024-03-25 19:08:12.664969 hauntedhouse-0.1.8/PKG-INFO
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-03-25 19:08:12.664969 hauntedhouse-0.1.8/hauntedhouse/
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       49 2024-02-06 15:47:31.000000 hauntedhouse-0.1.8/hauntedhouse/__init__.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     4185 2024-03-25 19:01:21.000000 hauntedhouse-0.1.8/hauntedhouse/client.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        0 2023-11-16 19:07:26.000000 hauntedhouse-0.1.8/hauntedhouse/py.typed
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-03-25 19:08:12.664969 hauntedhouse-0.1.8/hauntedhouse.egg-info/
--rw-r--r--   0 asdougl   (1000) asdougl   (1000)      353 2024-03-25 19:08:12.000000 hauntedhouse-0.1.8/hauntedhouse.egg-info/PKG-INFO
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      273 2024-03-25 19:08:12.000000 hauntedhouse-0.1.8/hauntedhouse.egg-info/SOURCES.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        1 2024-03-25 19:08:12.000000 hauntedhouse-0.1.8/hauntedhouse.egg-info/dependency_links.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       20 2024-03-25 19:08:12.000000 hauntedhouse-0.1.8/hauntedhouse.egg-info/requires.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       13 2024-03-25 19:08:12.000000 hauntedhouse-0.1.8/hauntedhouse.egg-info/top_level.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      461 2024-03-25 19:06:19.000000 hauntedhouse-0.1.8/pyproject.toml
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      108 2023-11-06 17:43:31.000000 hauntedhouse-0.1.8/readme.md
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       38 2024-03-25 19:08:12.664969 hauntedhouse-0.1.8/setup.cfg
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-04-10 15:25:06.151364 hauntedhouse-0.1.9/
+-rw-r--r--   0 asdougl   (1000) asdougl   (1000)      353 2024-04-10 15:25:06.151364 hauntedhouse-0.1.9/PKG-INFO
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-04-10 15:25:06.151364 hauntedhouse-0.1.9/hauntedhouse/
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       49 2024-02-06 15:47:31.000000 hauntedhouse-0.1.9/hauntedhouse/__init__.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     4416 2024-04-10 15:16:59.000000 hauntedhouse-0.1.9/hauntedhouse/client.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        0 2023-11-16 19:07:26.000000 hauntedhouse-0.1.9/hauntedhouse/py.typed
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2024-04-10 15:25:06.151364 hauntedhouse-0.1.9/hauntedhouse.egg-info/
+-rw-r--r--   0 asdougl   (1000) asdougl   (1000)      353 2024-04-10 15:25:06.000000 hauntedhouse-0.1.9/hauntedhouse.egg-info/PKG-INFO
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      273 2024-04-10 15:25:06.000000 hauntedhouse-0.1.9/hauntedhouse.egg-info/SOURCES.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        1 2024-04-10 15:25:06.000000 hauntedhouse-0.1.9/hauntedhouse.egg-info/dependency_links.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       20 2024-04-10 15:25:06.000000 hauntedhouse-0.1.9/hauntedhouse.egg-info/requires.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       13 2024-04-10 15:25:06.000000 hauntedhouse-0.1.9/hauntedhouse.egg-info/top_level.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      461 2024-04-10 15:23:07.000000 hauntedhouse-0.1.9/pyproject.toml
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      108 2023-11-06 17:43:31.000000 hauntedhouse-0.1.9/readme.md
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       38 2024-04-10 15:25:06.151364 hauntedhouse-0.1.9/setup.cfg
```

### Comparing `hauntedhouse-0.1.8/hauntedhouse/client.py` & `hauntedhouse-0.1.9/hauntedhouse/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,20 @@
             self.session.verify = False
         self.session.headers['Authorization'] = 'Bearer ' + api_key
 
     def close(self):
         """Close requests session."""
         self.session.close()
 
+    def status(self) -> dict:
+        """Load the status blob from the haunted house instance."""
+        result = self.session.get(self.address + '/status/detailed')
+        result.raise_for_status()
+        return result.json()
+
     def start_search(self, yara_rule: str, rule_classification: str, search_classification: str,
                      creator: str, description: str, expiry, indices='hot_and_archive') -> str:
         """Start a new search."""
         logger.info("Start retrohunt search for %s", creator)
         indices = indices.lower()
         if indices not in INDEX_GROUPS:
             raise ValueError(f"Index parameter set to {indices}, expected one of {INDEX_GROUPS}")
```

