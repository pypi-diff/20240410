# Comparing `tmp/evmchains-0.0.4.tar.gz` & `tmp/evmchains-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evmchains-0.0.4.tar", last modified: Fri Mar  8 22:16:04 2024, max compression
+gzip compressed data, was "evmchains-0.0.5.tar", last modified: Tue Apr  9 22:52:33 2024, max compression
```

## Comparing `evmchains-0.0.4.tar` & `evmchains-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.378147 evmchains-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.370147 evmchains-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.374147 evmchains-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-08 22:15:43.000000 evmchains-0.0.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-08 22:15:43.000000 evmchains-0.0.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-08 22:15:43.000000 evmchains-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-08 22:15:43.000000 evmchains-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15314 2024-03-08 22:16:04.378147 evmchains-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-08 22:15:43.000000 evmchains-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.374147 evmchains-0.0.4/evmchains/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-08 22:15:43.000000 evmchains-0.0.4/evmchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-03-08 22:15:43.000000 evmchains-0.0.4/evmchains/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 22:15:43.000000 evmchains-0.0.4/evmchains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-08 22:15:43.000000 evmchains-0.0.4/evmchains/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.374147 evmchains-0.0.4/evmchains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15314 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-08 22:16:04.000000 evmchains-0.0.4/evmchains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-08 22:15:43.000000 evmchains-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.374147 evmchains-0.0.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-08 22:15:43.000000 evmchains-0.0.4/scripts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-08 22:16:04.378147 evmchains-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 22:15:43.000000 evmchains-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:16:04.374147 evmchains-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-08 22:15:43.000000 evmchains-0.0.4/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 22:52:15.000000 evmchains-0.0.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 22:52:15.000000 evmchains-0.0.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 22:52:15.000000 evmchains-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 22:52:15.000000 evmchains-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 22:52:15.000000 evmchains-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-09 22:52:33.210523 evmchains-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-09 22:52:15.000000 evmchains-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/evmchains/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/evmchains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 22:52:15.000000 evmchains-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-09 22:52:15.000000 evmchains-0.0.5/scripts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 22:52:33.210523 evmchains-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 22:52:15.000000 evmchains-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 22:52:15.000000 evmchains-0.0.5/tests/test_func.py
```

### Comparing `evmchains-0.0.4/.github/workflows/release.yaml` & `evmchains-0.0.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.4/.github/workflows/test.yaml` & `evmchains-0.0.5/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     test:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: ["3.8", "3.9", "3.10", "3.11"]
+                python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
           with:
             fetch-depth: 0
 
         - name: Setup Python
```

### Comparing `evmchains-0.0.4/.gitignore` & `evmchains-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.4/LICENSE` & `evmchains-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.4/PKG-INFO` & `evmchains-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.4
+Version: 0.0.5
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -214,14 +214,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic~=2.5.3
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
@@ -273,7 +274,17 @@
 assert chain.chainId == 1
 ```
 
 ## Development
 
 Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
 Comments, questions, criticisms and pull requests are welcomed.
+
+### Adding Chains
+
+To add a chain to the metadata, please open a pull request with the following changes:
+
+- Update `CHAIN_IDS` in `scripts/update.py` with the chain IDs you want to add
+- Run `python scripts/update.py`
+- Submit a PR with the updated script and updated `evmchain/chains.py` metdata file
+
+**Do not edit `evmchain/chains.py` manually.** Any manual changes are likely to be overwritten later.
```

### Comparing `evmchains-0.0.4/evmchains/__init__.py` & `evmchains-0.0.5/evmchains/__init__.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.4/evmchains/chains.py` & `evmchains-0.0.5/evmchains/chains.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.4/evmchains.egg-info/PKG-INFO` & `evmchains-0.0.5/evmchains.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.4
+Version: 0.0.5
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -214,14 +214,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic~=2.5.3
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
@@ -273,7 +274,17 @@
 assert chain.chainId == 1
 ```
 
 ## Development
 
 Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
 Comments, questions, criticisms and pull requests are welcomed.
+
+### Adding Chains
+
+To add a chain to the metadata, please open a pull request with the following changes:
+
+- Update `CHAIN_IDS` in `scripts/update.py` with the chain IDs you want to add
+- Run `python scripts/update.py`
+- Submit a PR with the updated script and updated `evmchain/chains.py` metdata file
+
+**Do not edit `evmchain/chains.py` manually.** Any manual changes are likely to be overwritten later.
```

### Comparing `evmchains-0.0.4/pyproject.toml` & `evmchains-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Operating System :: MacOS",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pydantic~=2.5.3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
@@ -50,15 +51,15 @@
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 python_files = "test_*.py"
 testpaths = "tests"
```

### Comparing `evmchains-0.0.4/scripts/update.py` & `evmchains-0.0.5/scripts/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             ensure_dict(chains, ecosystem)
             chains[ecosystem][network] = fetch_chain(chain_id)
     return chains
 
 
 def write_chain_const(chains: Dict[str, Dict[str, Chain]]):
     """Write the file with Python constant"""
-    file_str = "# This file is auto-generated by scripts/update_rpc.py\n"
+    file_str = "# This file is auto-generated by scripts/update.py\n"
     file_str += f"# {stamp()}\n"
     file_str += "# Do not edit this file directly.\n"
     file_str += "from typing import Any, Dict\n\n"
     file_str += "PUBLIC_CHAIN_META: Dict[str, Dict[str, Dict[str, Any]]] = {\n"
 
     for ecosystem in chains.keys():
         file_str += f'    "{ecosystem}": {{\n'
```

### Comparing `evmchains-0.0.4/tests/test_func.py` & `evmchains-0.0.5/tests/test_func.py`

 * *Files identical despite different names*

