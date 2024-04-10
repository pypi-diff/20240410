# Comparing `tmp/brownie_safe-0.8.5.tar.gz` & `tmp/brownie_safe-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brownie_safe-0.8.5.tar", max compression
+gzip compressed data, was "brownie_safe-0.8.6.tar", max compression
```

## Comparing `brownie_safe-0.8.5.tar` & `brownie_safe-0.8.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18594 2023-09-23 09:24:27.456103 brownie_safe-0.8.5/brownie_safe.py
--rw-r--r--   0        0        0      539 2023-09-23 09:24:34.018233 brownie_safe-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.5/readme.md
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 brownie_safe-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    18663 2024-04-10 17:41:39.063300 brownie_safe-0.8.6/brownie_safe.py
+-rw-r--r--   0        0        0      539 2024-04-10 17:43:26.928908 brownie_safe-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.6/readme.md
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 brownie_safe-0.8.6/PKG-INFO
```

### Comparing `brownie_safe-0.8.5/brownie_safe.py` & `brownie_safe-0.8.6/brownie_safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,17 @@
         return EthAddress(self.address)
 
     def __repr__(self):
         return f'BrownieSafe("{self.address}")'
 
     @cached_property
     def client(self):
-        match = re.search('(anvil|hardhat|ganache)', web3.clientVersion.lower())
-        return match.group(1)
+        client_version = web3.clientVersion
+        match = re.search('(anvil|hardhat|ganache)', client_version.lower())
+        return match.group(1) if match else client_version
 
     @property
     def account(self) -> LocalAccount:
         """
         Unlocked Brownie account for Gnosis Safe.
         """
         return accounts.at(self.address, force=True)
```

### Comparing `brownie_safe-0.8.5/pyproject.toml` & `brownie_safe-0.8.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brownie-safe"
-version = "0.8.5"
+version = "0.8.6"
 description = "Build complex Gnosis Safe transactions and safely preview them in a forked environment."
 authors = ["banteg"]
 license = "MIT"
 repository = "https://github.com/banteg/brownie-safe"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
```

### Comparing `brownie_safe-0.8.5/readme.md` & `brownie_safe-0.8.6/readme.md`

 * *Files identical despite different names*

### Comparing `brownie_safe-0.8.5/PKG-INFO` & `brownie_safe-0.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brownie-safe
-Version: 0.8.5
+Version: 0.8.6
 Summary: Build complex Gnosis Safe transactions and safely preview them in a forked environment.
 Home-page: https://github.com/banteg/brownie-safe
 License: MIT
 Author: banteg
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

