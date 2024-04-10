# Comparing `tmp/python_cmr-0.8.0.tar.gz` & `tmp/python_cmr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_cmr-0.8.0.tar", max compression
+gzip compressed data, was "python_cmr-0.9.0.tar", max compression
```

## Comparing `python_cmr-0.8.0.tar` & `python_cmr-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-07-06 22:12:32.770764 python_cmr-0.8.0/LICENSE
--rw-r--r--   0        0        0     8379 2023-07-06 22:12:32.770764 python_cmr-0.8.0/README.md
--rw-r--r--   0        0        0      244 2023-07-06 22:12:32.770764 python_cmr-0.8.0/cmr/__init__.py
--rw-r--r--   0        0        0    27169 2023-07-06 22:12:32.770764 python_cmr-0.8.0/cmr/queries.py
--rw-r--r--   0        0        0      617 2023-07-06 22:12:32.770764 python_cmr-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9172 1970-01-01 00:00:00.000000 python_cmr-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-26 18:46:43.693112 python_cmr-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8615 2023-07-26 18:46:43.693112 python_cmr-0.9.0/README.md
+-rw-r--r--   0        0        0      244 2023-07-26 18:46:43.693112 python_cmr-0.9.0/cmr/__init__.py
+-rw-r--r--   0        0        0    28477 2023-07-26 18:46:43.693112 python_cmr-0.9.0/cmr/queries.py
+-rw-r--r--   0        0        0      617 2023-07-26 18:46:43.693112 python_cmr-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9408 1970-01-01 00:00:00.000000 python_cmr-0.9.0/PKG-INFO
```

### Comparing `python_cmr-0.8.0/LICENSE` & `python_cmr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_cmr-0.8.0/README.md` & `python_cmr-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 Examples
 ========
 
 This library is broken into two classes, CollectionQuery and GranuleQuery. Each of these classes provide a large set of
 methods used to build a query for CMR. Not all parameters provided by the CMR API are covered by this version of
 python-cmr.
 
-The following methods are available to both collecton and granule queries:
+The following methods are available to both collection and granule queries:
 
     # search for granules matching a specific product/short_name
     >>> api.short_name("AST_L1T")
 
     # search for granules matching a specific version
     >>> api.version("006")
 
@@ -117,14 +117,18 @@
     # filter by cloud cover percentage range
     >>> api.cloud_cover(25, 75)
 
     # filter by specific instrument or platform
     >>> api.instrument("MODIS")
     >>> api.platform("Terra")
 
+    # filter by a sort_key note: sort_keys are require some other fields to find some existing granules before they can be sorted
+
+    >>> api.parameters(short_name="OMNO2", version="003", provider='GES_DISC', sort_key='-start_date')
+
 Collection searches support these methods (in addition to the shared methods above):
 
     # search for collections from a specific archive center
     >>> api.archive_center("LP DAAC")
 
     # case insensitive, wildcard enabled text search through most collection fields
     >>> api.keyword("M*D09")
@@ -192,15 +196,15 @@
         version="003",
         point=(-100, 42)
     )
 
 Note: the kwarg key should match the name of a method from the above examples, and the value should be a tuple if it's a
 parameter that requires multiple values.
 
-To inspect and retreive results from the API, the following methods are available:
+To inspect and retrieve results from the API, the following methods are available:
 
     # inspect the number of results the query will return without downloading the results
     >>> print(api.hits())
 
     # retrieve 100 granules
     >>> granules = api.get(100)
```

### Comparing `python_cmr-0.8.0/cmr/queries.py` & `python_cmr-0.9.0/cmr/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -669,14 +669,60 @@
 
         if not platform:
             raise ValueError("Please provide a value for platform")
 
         self.params['platform'] = platform
         return self
 
+
+    def sort_key(self, sort_key=""):
+        """
+        See
+        https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html#sorting-granule-results
+        for valid granule sort_keys
+
+        Filter some defined sort_key; 
+        use negative (-) for start_date and end_date to sort by ascending
+
+        :param sort_key: name of the sort key
+        :returns: Query instance
+        """
+
+        valid_sort_keys = [
+        'campaign',
+        'entry_title',
+        'dataset_id',
+        'data_size',
+        'end_date',
+        '-end_date'
+        'granule_ur',
+        'producer_granule_id'
+        'project',
+        'provider',
+        'readable_granule_name',
+        'short_name',
+        '-start_date',
+        'start_date',
+        'version',
+        'platform',
+        'instrument',
+        'sensor',
+        'day_night_flag',
+        'online_only',
+        'browsable',
+        'browse_only',
+        'cloud_cover',
+        'revision_date']
+        # also covers if empty string
+        if sort_key not in valid_sort_keys:
+            raise ValueError("Please provide a valid sort_key for granules query see https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html#sorting-granule-results for valid sort_keys")
+
+        self.params['sort_key'] = sort_key
+        return self
+
     def granule_ur(self, granule_ur=""):
         """
         Filter by the granules unique ID. Note this will result in at most one granule
         being returned.
 
         :param granule_ur: UUID of a granule
         :returns: Query instance
```

### Comparing `python_cmr-0.8.0/pyproject.toml` & `python_cmr-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-cmr"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python wrapper to the NASA Common Metadata Repository (CMR) API."
 authors = ["python_cmr <nasa/python_cmr@github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nasa/python_cmr"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `python_cmr-0.8.0/PKG-INFO` & `python_cmr-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmr
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper to the NASA Common Metadata Repository (CMR) API.
 Home-page: https://github.com/nasa/python_cmr
 License: MIT
 Author: python_cmr
 Author-email: nasa/python_cmr@github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,15 +73,15 @@
 Examples
 ========
 
 This library is broken into two classes, CollectionQuery and GranuleQuery. Each of these classes provide a large set of
 methods used to build a query for CMR. Not all parameters provided by the CMR API are covered by this version of
 python-cmr.
 
-The following methods are available to both collecton and granule queries:
+The following methods are available to both collection and granule queries:
 
     # search for granules matching a specific product/short_name
     >>> api.short_name("AST_L1T")
 
     # search for granules matching a specific version
     >>> api.version("006")
 
@@ -137,14 +137,18 @@
     # filter by cloud cover percentage range
     >>> api.cloud_cover(25, 75)
 
     # filter by specific instrument or platform
     >>> api.instrument("MODIS")
     >>> api.platform("Terra")
 
+    # filter by a sort_key note: sort_keys are require some other fields to find some existing granules before they can be sorted
+
+    >>> api.parameters(short_name="OMNO2", version="003", provider='GES_DISC', sort_key='-start_date')
+
 Collection searches support these methods (in addition to the shared methods above):
 
     # search for collections from a specific archive center
     >>> api.archive_center("LP DAAC")
 
     # case insensitive, wildcard enabled text search through most collection fields
     >>> api.keyword("M*D09")
@@ -212,15 +216,15 @@
         version="003",
         point=(-100, 42)
     )
 
 Note: the kwarg key should match the name of a method from the above examples, and the value should be a tuple if it's a
 parameter that requires multiple values.
 
-To inspect and retreive results from the API, the following methods are available:
+To inspect and retrieve results from the API, the following methods are available:
 
     # inspect the number of results the query will return without downloading the results
     >>> print(api.hits())
 
     # retrieve 100 granules
     >>> granules = api.get(100)
```

