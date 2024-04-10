# Comparing `tmp/audiness-0.3.1.tar.gz` & `tmp/audiness-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiness-0.3.1.tar", max compression
+gzip compressed data, was "audiness-0.3.2.tar", max compression
```

## Comparing `audiness-0.3.1.tar` & `audiness-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1112 2024-02-17 20:42:20.911611 audiness-0.3.1/LICENSE
--rw-r--r--   0        0        0     4859 2024-03-06 08:49:52.251747 audiness-0.3.1/README.md
--rw-r--r--   0        0        0       39 2024-02-18 00:47:45.686574 audiness-0.3.1/audiness/__init__.py
--rw-r--r--   0        0        0       51 2024-02-18 00:47:45.686574 audiness-0.3.1/audiness/commands/__init__.py
--rw-r--r--   0        0        0     1353 2024-02-29 12:00:55.323746 audiness-0.3.1/audiness/commands/folders.py
--rw-r--r--   0        0        0      973 2024-03-05 22:22:18.529099 audiness-0.3.1/audiness/commands/policies.py
--rw-r--r--   0        0        0     2967 2024-03-05 21:10:50.073605 audiness-0.3.1/audiness/commands/scans.py
--rw-r--r--   0        0        0     1793 2024-03-05 22:23:39.485777 audiness-0.3.1/audiness/commands/server.py
--rw-r--r--   0        0        0      231 2024-02-29 12:00:55.323746 audiness-0.3.1/audiness/commands/software.py
--rw-r--r--   0        0        0      646 2024-03-05 20:35:05.159941 audiness-0.3.1/audiness/helpers.py
--rw-r--r--   0        0        0     1577 2024-03-05 22:22:18.530099 audiness-0.3.1/audiness/main.py
--rw-r--r--   0        0        0      701 2024-03-06 08:49:52.255747 audiness-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 audiness-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-02-17 20:42:20.911611 audiness-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4983 2024-04-01 20:55:34.004187 audiness-0.3.2/README.md
+-rw-r--r--   0        0        0       39 2024-02-18 00:47:45.686574 audiness-0.3.2/audiness/__init__.py
+-rw-r--r--   0        0        0       51 2024-02-18 00:47:45.686574 audiness-0.3.2/audiness/commands/__init__.py
+-rw-r--r--   0        0        0     1353 2024-02-29 12:00:55.323746 audiness-0.3.2/audiness/commands/folders.py
+-rw-r--r--   0        0        0      973 2024-03-05 22:22:18.529099 audiness-0.3.2/audiness/commands/policies.py
+-rw-r--r--   0        0        0     2967 2024-04-10 21:42:07.914924 audiness-0.3.2/audiness/commands/scans.py
+-rw-r--r--   0        0        0     1793 2024-03-05 22:23:39.485777 audiness-0.3.2/audiness/commands/server.py
+-rw-r--r--   0        0        0      231 2024-02-29 12:00:55.323746 audiness-0.3.2/audiness/commands/software.py
+-rw-r--r--   0        0        0      646 2024-03-05 20:35:05.159941 audiness-0.3.2/audiness/helpers.py
+-rw-r--r--   0        0        0     1577 2024-03-05 22:22:18.530099 audiness-0.3.2/audiness/main.py
+-rw-r--r--   0        0        0      703 2024-04-10 21:43:25.378827 audiness-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 audiness-0.3.2/PKG-INFO
```

### Comparing `audiness-0.3.1/LICENSE` & `audiness-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/README.md` & `audiness-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 To get the lastest state:
 
 ```bash
 $ pip install git+https://github.com/audiusGmbH/audiness.git
 ```
 
-For Nix or NixOS users is a package available. Keep in mind that the lastest releases might only
+For Nix or NixOS users is a [package](https://search.nixos.org/packages?channel=unstable&from=0&size=50&sort=relevance&type=packages&query=audiness)
+available in Nixpkgs. Keep in mind that the lastest releases might only
 be present in the ``unstable`` channel.
 
 ```bash
 $ nix-env -iA nixos.audiness
 ```
 
 ## Setup
```

### Comparing `audiness-0.3.1/audiness/commands/folders.py` & `audiness-0.3.2/audiness/commands/folders.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/audiness/commands/policies.py` & `audiness-0.3.2/audiness/commands/policies.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/audiness/commands/scans.py` & `audiness-0.3.2/audiness/commands/scans.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             single_scan = scan_history[-abs(history)]
 
             short_date = datetime.fromtimestamp(
                 single_scan["last_modification_date"]
             ).strftime("%Y%m")
             historic_scan_id = single_scan["history_id"]
 
-            filename = Path(path) / Path(f'{scan["name"]}-{short_date}.nessus')
+            filename = Path(path) / Path(f'{scan["name"]}_{short_date}.nessus')
             scan_data = connection.scans.export_scan(
                 scan_id=scan["id"], history_id=historic_scan_id, format="nessus"
             )
             Path(filename).write_bytes(scan_data.getbuffer())
         print(f"{len(relevant_scans)} files exported.")
     except IndexError:
         print("Scan not available")
```

### Comparing `audiness-0.3.1/audiness/commands/server.py` & `audiness-0.3.2/audiness/commands/server.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/audiness/helpers.py` & `audiness-0.3.2/audiness/helpers.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/audiness/main.py` & `audiness-0.3.2/audiness/main.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.1/pyproject.toml` & `audiness-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "audiness"
-version = "0.3.1"
+version = "0.3.2"
 description = "CLI tool to interact with Tenable's Nessus"
 authors = ["Fabian Affolter <fabian-affolter@audius.de>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["vulnerabilites", "nessus"]
 homepage = "https://github.com/audiusGmbH/audiness"
 repository = "https://github.com/audiusGmbH/audiness"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9"}
 pytenable = "^1.4"
-validators = "^0.22"
+validators = "^0.24"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8"
-black = "^24"
+black = "^24.3"
 isort = "^5.13"
 
 [tool.poetry.scripts]
 audiness = "audiness.main:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `audiness-0.3.1/PKG-INFO` & `audiness-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiness
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI tool to interact with Tenable's Nessus
 Home-page: https://github.com/audiusGmbH/audiness
 License: MIT
 Keywords: vulnerabilites,nessus
 Author: Fabian Affolter
 Author-email: fabian-affolter@audius.de
 Requires-Python: >=3.9,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytenable (>=1.4,<2.0)
 Requires-Dist: typer[all] (>=0.9,<0.10)
-Requires-Dist: validators (>=0.22,<0.23)
+Requires-Dist: validators (>=0.24,<0.25)
 Project-URL: Repository, https://github.com/audiusGmbH/audiness
 Description-Content-Type: text/markdown
 
 # audiness
 
 Helper scripts to interact with Nessus instances. The CLI allows one to perform tasks on a 
 Nessus installation without using the web interface.
@@ -35,15 +35,16 @@
 
 To get the lastest state:
 
 ```bash
 $ pip install git+https://github.com/audiusGmbH/audiness.git
 ```
 
-For Nix or NixOS users is a package available. Keep in mind that the lastest releases might only
+For Nix or NixOS users is a [package](https://search.nixos.org/packages?channel=unstable&from=0&size=50&sort=relevance&type=packages&query=audiness)
+available in Nixpkgs. Keep in mind that the lastest releases might only
 be present in the ``unstable`` channel.
 
 ```bash
 $ nix-env -iA nixos.audiness
 ```
 
 ## Setup
```

