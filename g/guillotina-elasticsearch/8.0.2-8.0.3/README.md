# Comparing `tmp/guillotina_elasticsearch-8.0.2.tar.gz` & `tmp/guillotina_elasticsearch-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guillotina_elasticsearch-8.0.2.tar", last modified: Mon Mar 25 17:29:08 2024, max compression
+gzip compressed data, was "guillotina_elasticsearch-8.0.3.tar", last modified: Wed Apr 10 15:04:34 2024, max compression
```

## Comparing `guillotina_elasticsearch-8.0.2.tar` & `guillotina_elasticsearch-8.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/
--rw-rw-r--   0 nil       (1000) nil       (1000)    20494 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/CHANGELOG.rst
--rw-rw-r--   0 nil       (1000) nil       (1000)     1315 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/LICENSE
--rw-rw-r--   0 nil       (1000) nil       (1000)      141 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/MANIFEST.in
--rw-r--r--   0 nil       (1000) nil       (1000)    26224 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/PKG-INFO
--rw-rw-r--   0 nil       (1000) nil       (1000)     4601 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/README.rst
--rw-rw-r--   0 nil       (1000) nil       (1000)        6 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/VERSION
--rw-rw-r--   0 nil       (1000) nil       (1000)      727 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/config.json
--rw-rw-r--   0 nil       (1000) nil       (1000)      536 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/docker-compose.yml
-drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/
--rw-rw-r--   0 nil       (1000) nil       (1000)     2405 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/__init__.py
-drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/
--rw-rw-r--   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/__init__.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     2674 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/fields.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     3085 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/migrate.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     2541 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/reindex.py
--rw-rw-r--   0 nil       (1000) nil       (1000)    13106 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/vacuum.py
--rw-rw-r--   0 nil       (1000) nil       (1000)      210 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/directives.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1274 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/events.py
--rw-rw-r--   0 nil       (1000) nil       (1000)      320 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/exceptions.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1940 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/interfaces.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     4878 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/manager.py
--rw-rw-r--   0 nil       (1000) nil       (1000)    22845 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/migration.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     7346 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/parser.py
--rw-rw-r--   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/py.typed
--rw-rw-r--   0 nil       (1000) nil       (1000)      959 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/queries.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1141 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/reindex.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     4338 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/schema.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1744 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/testing.py
-drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/
--rw-rw-r--   0 nil       (1000) nil       (1000)     2946 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/_test_flaky.py
--rw-rw-r--   0 nil       (1000) nil       (1000)      470 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/conftest.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     3762 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/fixtures.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     2500 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_catalog.py
--rw-rw-r--   0 nil       (1000) nil       (1000)      904 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_indexer.py
--rw-rw-r--   0 nil       (1000) nil       (1000)    17963 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_migration.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1045 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_package.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     4080 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_parser.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     1673 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_schema.py
--rw-rw-r--   0 nil       (1000) nil       (1000)    14202 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_search.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     8479 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_vacuum.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     3581 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/utils.py
--rw-rw-r--   0 nil       (1000) nil       (1000)    22346 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/utility.py
--rw-rw-r--   0 nil       (1000) nil       (1000)     3212 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/utils.py
-drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/
--rw-r--r--   0 nil       (1000) nil       (1000)    26224 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/PKG-INFO
--rw-rw-r--   0 nil       (1000) nil       (1000)     1699 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/SOURCES.txt
--rw-rw-r--   0 nil       (1000) nil       (1000)        1 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/dependency_links.txt
--rw-rw-r--   0 nil       (1000) nil       (1000)      257 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/requires.txt
--rw-rw-r--   0 nil       (1000) nil       (1000)       25 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/top_level.txt
--rw-rw-r--   0 nil       (1000) nil       (1000)        1 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/zip-safe
--rw-rw-r--   0 nil       (1000) nil       (1000)      440 2024-03-25 17:29:08.005166 guillotina_elasticsearch-8.0.2/setup.cfg
--rw-rw-r--   0 nil       (1000) nil       (1000)     1488 2024-03-25 17:29:07.000000 guillotina_elasticsearch-8.0.2/setup.py
+drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/
+-rw-rw-r--   0 nil       (1000) nil       (1000)    20593 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/CHANGELOG.rst
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1315 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/LICENSE
+-rw-rw-r--   0 nil       (1000) nil       (1000)      141 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/MANIFEST.in
+-rw-r--r--   0 nil       (1000) nil       (1000)    26323 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/PKG-INFO
+-rw-rw-r--   0 nil       (1000) nil       (1000)     4601 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/README.rst
+-rw-rw-r--   0 nil       (1000) nil       (1000)        6 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/VERSION
+-rw-rw-r--   0 nil       (1000) nil       (1000)      727 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/config.json
+-rw-rw-r--   0 nil       (1000) nil       (1000)      536 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/docker-compose.yml
+drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.575334 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/
+-rw-rw-r--   0 nil       (1000) nil       (1000)     2405 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/__init__.py
+drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/
+-rw-rw-r--   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/__init__.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     2674 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/fields.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     3085 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/migrate.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     2541 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/reindex.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)    13106 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/vacuum.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)      210 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/directives.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1274 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/events.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)      320 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/exceptions.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1940 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/interfaces.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     4878 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/manager.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)    22845 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/migration.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     7346 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/parser.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/py.typed
+-rw-rw-r--   0 nil       (1000) nil       (1000)      959 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/queries.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1141 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/reindex.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     4471 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/schema.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1744 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/testing.py
+drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/
+-rw-rw-r--   0 nil       (1000) nil       (1000)     2946 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/_test_flaky.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)      470 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/conftest.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     3762 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/fixtures.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     2500 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_catalog.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)      904 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_indexer.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)    17963 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_migration.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1081 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_package.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     4080 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_parser.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1712 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_schema.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)    14202 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_search.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     8479 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_vacuum.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     3581 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/utils.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)    22346 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/utility.py
+-rw-rw-r--   0 nil       (1000) nil       (1000)     3212 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/utils.py
+drwxrwxr-x   0 nil       (1000) nil       (1000)        0 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/
+-rw-r--r--   0 nil       (1000) nil       (1000)    26323 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/PKG-INFO
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1699 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 nil       (1000) nil       (1000)        1 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 nil       (1000) nil       (1000)      257 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/requires.txt
+-rw-rw-r--   0 nil       (1000) nil       (1000)       25 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/top_level.txt
+-rw-rw-r--   0 nil       (1000) nil       (1000)        1 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/zip-safe
+-rw-rw-r--   0 nil       (1000) nil       (1000)      440 2024-04-10 15:04:34.579334 guillotina_elasticsearch-8.0.3/setup.cfg
+-rw-rw-r--   0 nil       (1000) nil       (1000)     1488 2024-04-10 15:04:34.000000 guillotina_elasticsearch-8.0.3/setup.py
```

### Comparing `guillotina_elasticsearch-8.0.2/CHANGELOG.rst` & `guillotina_elasticsearch-8.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+8.0.3 (2024-04-10)
+------------------
+
+- Adding search analyzers functionality
+  [nilbacardit26]
+
+
 8.0.2 (2024-03-25)
 ------------------
 
 - Being able to search using multifields
   [nilbacardit26]
```

### Comparing `guillotina_elasticsearch-8.0.2/LICENSE` & `guillotina_elasticsearch-8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/PKG-INFO` & `guillotina_elasticsearch-8.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guillotina_elasticsearch
-Version: 8.0.2
+Version: 8.0.3
 Summary: elasticsearch catalog support for guillotina
 Home-page: https://github.com/plone/guillotina_elasticsearch
 Author: Ramon Navarro Bosch & Nathan Van Gheem
 Author-email: ramon@plone.org
 License: GPL version 3
 Keywords: search async guillotina elasticsearch
 Classifier: Programming Language :: Python :: 3.7
@@ -203,14 +203,21 @@
         hosts:
           - "127.0.0.1:9200"
         sniffer_timeout: 0.5
         sniff_on_start: true
         use_ssl: true
         http_auth: admin:admin
 
+8.0.3 (2024-04-10)
+------------------
+
+- Adding search analyzers functionality
+  [nilbacardit26]
+
+
 8.0.2 (2024-03-25)
 ------------------
 
 - Being able to search using multifields
   [nilbacardit26]
```

### Comparing `guillotina_elasticsearch-8.0.2/README.rst` & `guillotina_elasticsearch-8.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/config.json` & `guillotina_elasticsearch-8.0.3/config.json`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/docker-compose.yml` & `guillotina_elasticsearch-8.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/__init__.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/fields.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/fields.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/migrate.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/reindex.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/reindex.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/commands/vacuum.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/commands/vacuum.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/events.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/events.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/interfaces.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/interfaces.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/manager.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/manager.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/migration.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/migration.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/parser.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/parser.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/queries.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/queries.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/reindex.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/reindex.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/schema.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
                 field_mapping["store"] = catalog_info["store"]
             if "analyzer" in catalog_info:
                 field_mapping["analyzer"] = catalog_info["analyzer"]
             if "normalizer" in catalog_info:
                 field_mapping["normalizer"] = catalog_info["normalizer"]
             if "multifields" in catalog_info:
                 field_mapping["fields"] = catalog_info["multifields"]
+            if "search_analyzer" in catalog_info:
+                field_mapping["search_analyzer"] = catalog_info["search_analyzer"]
             if schema_info:
                 if "_schemas" not in field_mapping:
                     field_mapping["_schemas"] = []
                 if schema.__identifier__ not in field_mapping["_schemas"]:
                     field_mapping["_schemas"].append(schema.__identifier__)
 
             if index_name in mappings and mappings[index_name] != field_mapping:
```

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/testing.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/testing.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/_test_flaky.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/_test_flaky.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/fixtures.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_catalog.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_indexer.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_migration.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_package.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_package.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     index_field(
         "item_text",
         type="text",
         analyzer="common_analyzer",
         field="item_text",
         store=True,
         multifields={"raw": {"type": "keyword"}},
+        search_analyzer="standard",
     )
     item_text = TextLine()
 
 
 @implementer(IFooContent)
 class FooContent(Resource):
     pass
```

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_parser.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_schema.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,8 +52,9 @@
     }
     assert mappings["properties"]["item_text"] == {
         "index": True,
         "analyzer": "common_analyzer",
         "type": "text",
         "store": True,
         "fields": {"raw": {"type": "keyword"}},
+        "search_analyzer": "standard",
     }
```

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_search.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/test_vacuum.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/tests/utils.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/tests/utils.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/utility.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/utility.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch/utils.py` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch/utils.py`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/PKG-INFO` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guillotina-elasticsearch
-Version: 8.0.2
+Version: 8.0.3
 Summary: elasticsearch catalog support for guillotina
 Home-page: https://github.com/plone/guillotina_elasticsearch
 Author: Ramon Navarro Bosch & Nathan Van Gheem
 Author-email: ramon@plone.org
 License: GPL version 3
 Keywords: search async guillotina elasticsearch
 Classifier: Programming Language :: Python :: 3.7
@@ -203,14 +203,21 @@
         hosts:
           - "127.0.0.1:9200"
         sniffer_timeout: 0.5
         sniff_on_start: true
         use_ssl: true
         http_auth: admin:admin
 
+8.0.3 (2024-04-10)
+------------------
+
+- Adding search analyzers functionality
+  [nilbacardit26]
+
+
 8.0.2 (2024-03-25)
 ------------------
 
 - Being able to search using multifields
   [nilbacardit26]
```

### Comparing `guillotina_elasticsearch-8.0.2/guillotina_elasticsearch.egg-info/SOURCES.txt` & `guillotina_elasticsearch-8.0.3/guillotina_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guillotina_elasticsearch-8.0.2/setup.py` & `guillotina_elasticsearch-8.0.3/setup.py`

 * *Files identical despite different names*

