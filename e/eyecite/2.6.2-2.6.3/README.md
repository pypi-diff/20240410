# Comparing `tmp/eyecite-2.6.2.tar.gz` & `tmp/eyecite-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyecite-2.6.2.tar", max compression
+gzip compressed data, was "eyecite-2.6.3.tar", max compression
```

## Comparing `eyecite-2.6.2.tar` & `eyecite-2.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1326 2024-03-20 00:34:30.440385 eyecite-2.6.2/LICENSE
--rw-r--r--   0        0        0    18110 2024-03-20 00:34:30.440385 eyecite-2.6.2/README.rst
--rw-r--r--   0        0        0      465 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/__init__.py
--rw-r--r--   0        0        0     8563 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/annotate.py
--rw-r--r--   0        0        0     2693 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/clean.py
--rw-r--r--   0        0        0     8212 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/find.py
--rw-r--r--   0        0        0    10229 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/helpers.py
--rw-r--r--   0        0        0    24804 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/models.py
--rw-r--r--   0        0        0        0 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/py.typed
--rw-r--r--   0        0        0     9062 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/regexes.py
--rw-r--r--   0        0        0    11021 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/resolve.py
--rw-r--r--   0        0        0     3340 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/test_factories.py
--rw-r--r--   0        0        0    19456 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/tokenizers.py
--rw-r--r--   0        0        0     4269 2024-03-20 00:34:30.440385 eyecite-2.6.2/eyecite/utils.py
--rw-r--r--   0        0        0     2303 2024-03-20 00:34:30.444385 eyecite-2.6.2/pyproject.toml
--rw-r--r--   0        0        0    19572 1970-01-01 00:00:00.000000 eyecite-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1326 2024-04-10 01:30:15.938811 eyecite-2.6.3/LICENSE
+-rw-r--r--   0        0        0    18110 2024-04-10 01:30:15.938811 eyecite-2.6.3/README.rst
+-rw-r--r--   0        0        0      465 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/__init__.py
+-rw-r--r--   0        0        0     8563 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/annotate.py
+-rw-r--r--   0        0        0     2693 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/clean.py
+-rw-r--r--   0        0        0     8212 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/find.py
+-rw-r--r--   0        0        0    10229 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/helpers.py
+-rw-r--r--   0        0        0    24804 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/models.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/py.typed
+-rw-r--r--   0        0        0     9062 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/regexes.py
+-rw-r--r--   0        0        0    11021 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/resolve.py
+-rw-r--r--   0        0        0     3340 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/test_factories.py
+-rw-r--r--   0        0        0    20145 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/tokenizers.py
+-rw-r--r--   0        0        0     4269 2024-04-10 01:30:15.942812 eyecite-2.6.3/eyecite/utils.py
+-rw-r--r--   0        0        0     2303 2024-04-10 01:30:15.942812 eyecite-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0    19572 1970-01-01 00:00:00.000000 eyecite-2.6.3/PKG-INFO
```

### Comparing `eyecite-2.6.2/LICENSE` & `eyecite-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/README.rst` & `eyecite-2.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/annotate.py` & `eyecite-2.6.3/eyecite/annotate.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/clean.py` & `eyecite-2.6.3/eyecite/clean.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/find.py` & `eyecite-2.6.3/eyecite/find.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/helpers.py` & `eyecite-2.6.3/eyecite/helpers.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/models.py` & `eyecite-2.6.3/eyecite/models.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/regexes.py` & `eyecite-2.6.3/eyecite/regexes.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/resolve.py` & `eyecite-2.6.3/eyecite/resolve.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/test_factories.py` & `eyecite-2.6.3/eyecite/test_factories.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/eyecite/tokenizers.py` & `eyecite-2.6.3/eyecite/tokenizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,15 +516,28 @@
                 fingerprint = hashlib.md5(
                     str(expressions).encode("utf8") + str(flags).encode("utf8")
                 ).hexdigest()
                 cache_dir = Path(self.cache_dir)
                 cache_dir.mkdir(exist_ok=True)
                 cache = cache_dir / fingerprint
                 if cache.exists():
-                    hyperscan_db = hyperscan.loadb(cache.read_bytes())
+                    cache_bytes = cache.read_bytes()
+                    try:
+                        # hyperscan >= 0.5.0 added a mandatory mode argument
+                        hyperscan_db = hyperscan.loadb(
+                            cache_bytes, mode=hyperscan.HS_MODE_BLOCK
+                        )
+                    except TypeError:
+                        hyperscan_db = hyperscan.loadb(cache_bytes)
+                    try:
+                        # at some point Scratch became necessary --
+                        # https://github.com/darvid/python-hyperscan/issues/50#issuecomment-1386243477
+                        hyperscan_db.scratch = hyperscan.Scratch(hyperscan_db)
+                    except AttributeError:
+                        pass
 
             if not hyperscan_db:
                 # No cache, so compile database.
                 hyperscan_db = hyperscan.Database()
                 hyperscan_db.compile(expressions=expressions, flags=flags)
                 if cache:
                     cache.write_bytes(hyperscan.dumpb(hyperscan_db))
```

### Comparing `eyecite-2.6.2/eyecite/utils.py` & `eyecite-2.6.3/eyecite/utils.py`

 * *Files identical despite different names*

### Comparing `eyecite-2.6.2/pyproject.toml` & `eyecite-2.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "2.6.2"
+version = "2.6.3"
 authors = ["Free Law Project <info@free.law>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
```

### Comparing `eyecite-2.6.2/PKG-INFO` & `eyecite-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyecite
-Version: 2.6.2
+Version: 2.6.3
 Summary: Tool for extracting legal citations from text strings.
 Home-page: https://github.com/freelawproject/eyecite
 License: BSD-2-Clause
 Keywords: legal,courts,citations,extraction,cites
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
```

