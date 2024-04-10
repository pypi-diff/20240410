# Comparing `tmp/auto_walrus-0.3.0.tar.gz` & `tmp/auto_walrus-0.3.1.tar.gz`

## Comparing `auto_walrus-0.3.0.tar` & `auto_walrus-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/auto_walrus.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/requirements-dev.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/tox.ini
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/.github/workflows/tox.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/tests/main_test.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/utils/bump_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/LICENSE
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 auto_walrus-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/auto_walrus.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/requirements-dev.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/tox.ini
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/.github/workflows/tox.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/tests/main_test.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/utils/bump_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 auto_walrus-0.3.1/PKG-INFO
```

### Comparing `auto_walrus-0.3.0/auto_walrus.py` & `auto_walrus-0.3.1/auto_walrus.py`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/.github/workflows/publish_to_pypi.yml` & `auto_walrus-0.3.1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/.github/workflows/tox.yml` & `auto_walrus-0.3.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/tests/main_test.py` & `auto_walrus-0.3.1/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/utils/bump_version.py` & `auto_walrus-0.3.1/utils/bump_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 content = content.replace(f'version = "{old_version}"', f'version = "{version}"')
 with open("pyproject.toml", "w", encoding="utf-8") as f:
     f.write(content)
 
 subprocess.run(["git", "commit", "-a", "-m", f"Bump version to {version}"])
 subprocess.run(["git", "tag", "-a", version, "-m", version])
 subprocess.run(["git", "push", "--follow-tags"])
-
```

### Comparing `auto_walrus-0.3.0/LICENSE` & `auto_walrus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/README.md` & `auto_walrus-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.0/pyproject.toml` & `auto_walrus-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto-walrus"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Automatically apply the awesome walrus operator"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `auto_walrus-0.3.0/PKG-INFO` & `auto_walrus-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: auto-walrus
-Version: 0.3.0
+Version: 0.3.1
 Summary: Automatically apply the awesome walrus operator
 Project-URL: Homepage, https://github.com/MarcoGorelli/auto-walrus
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/auto-walrus
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

