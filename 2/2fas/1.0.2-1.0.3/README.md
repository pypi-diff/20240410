# Comparing `tmp/2fas-1.0.2.tar.gz` & `tmp/2fas-1.0.3.tar.gz`

## Comparing `2fas-1.0.2.tar` & `2fas-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 2fas-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/.gitignore
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d___about___py.html
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d___init___py.html
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d__security_py.html
--rw-r--r--   0        0        0    24236 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d__types_py.html
--rw-r--r--   0        0        0   124441 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_py.html
--rw-r--r--   0        0        0    36226 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_settings_py.html
--rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_support_py.html
--rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_core_py.html
--rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_main_py.html
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_utils_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/status.json
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 2fas-1.0.2/htmlcov/style.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/__init__.py
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/cli.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/cli_settings.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/cli_support.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 2fas-1.0.2/src/twofas/py.typed
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/2fas-demo-nopass.2fas
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/2fas-demo-pass.2fas
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/_shared.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/test_cli.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/test_cli_support.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/test_clisettings.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 2fas-1.0.2/tests/test_mypy_clear.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 2fas-1.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 2fas-1.0.2/LICENSE
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 2fas-1.0.2/README.md
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 2fas-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 2fas-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 2fas-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/.gitignore
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d___about___py.html
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d___init___py.html
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d__security_py.html
+-rw-r--r--   0        0        0    24236 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d__types_py.html
+-rw-r--r--   0        0        0   124441 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_py.html
+-rw-r--r--   0        0        0    36226 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_settings_py.html
+-rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_support_py.html
+-rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_core_py.html
+-rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_main_py.html
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/status.json
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 2fas-1.0.3/htmlcov/style.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/__init__.py
+-rw-r--r--   0        0        0    13736 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/cli.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/cli_settings.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/cli_support.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 2fas-1.0.3/src/twofas/py.typed
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/2fas-demo-nopass.2fas
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/2fas-demo-pass.2fas
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/_shared.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/test_cli_support.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/test_clisettings.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 2fas-1.0.3/tests/test_mypy_clear.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 2fas-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 2fas-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 2fas-1.0.3/README.md
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 2fas-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 2fas-1.0.3/PKG-INFO
```

### Comparing `2fas-1.0.2/CHANGELOG.md` & `2fas-1.0.3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.3 (2024-04-10)
+
+### Fix
+
+* Bump lib2fas version to fix some issues with keyring ([`b093bdc`](https://github.com/robinvandernoord/2fas-python/commit/b093bdc434841ace1dbd526149a2cac5238f0924))
+* Don't crash without args (= None instead of []) ([`efa1e69`](https://github.com/robinvandernoord/2fas-python/commit/efa1e69183c9ce1a204a5ac75b1a7d458c92c647))
+
 ## v1.0.2 (2024-02-29)
 
 ### Fix
 
 * Explicitly add typing-extensions as dependency ([`2f5c7ab`](https://github.com/robinvandernoord/2fas-python/commit/2f5c7ab92a12e0568dad40f29446187895db2e91))
 
 ## v1.0.1 (2024-01-29)
```

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d___about___py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d___about___py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d___init___py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d___init___py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d__security_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d__security_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d__types_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d__types_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_settings_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_settings_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_cli_support_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_cli_support_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_core_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_core_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_main_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_main_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/d_ece9e2c2b8514e4d_utils_py.html` & `2fas-1.0.3/htmlcov/d_ece9e2c2b8514e4d_utils_py.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/favicon_32.png` & `2fas-1.0.3/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/index.html` & `2fas-1.0.3/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/keybd_closed.png` & `2fas-1.0.3/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/keybd_open.png` & `2fas-1.0.3/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/status.json` & `2fas-1.0.3/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/htmlcov/style.css` & `2fas-1.0.3/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/src/twofas/cli.py` & `2fas-1.0.3/src/twofas/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,16 @@
     """
     # stateless actions:
     if version:
         return print_version()
     elif self_update:
         return command_update()
 
+    args = args or []
+
     # stateful:
 
     settings = load_cli_settings()
     state.update(verbose=settings.auto_verbose or verbose, settings=settings)
 
     file_args = [_ for _ in args if _.endswith(".2fas")]
     if len(file_args) > 1:
```

### Comparing `2fas-1.0.2/src/twofas/cli_settings.py` & `2fas-1.0.3/src/twofas/cli_settings.py`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/src/twofas/cli_support.py` & `2fas-1.0.3/src/twofas/cli_support.py`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/tests/2fas-demo-nopass.2fas` & `2fas-1.0.3/tests/2fas-demo-nopass.2fas`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/tests/2fas-demo-pass.2fas` & `2fas-1.0.3/tests/2fas-demo-pass.2fas`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/tests/test_cli_support.py` & `2fas-1.0.3/tests/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/tests/test_clisettings.py` & `2fas-1.0.3/tests/test_clisettings.py`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/tests/test_mypy_clear.py` & `2fas-1.0.3/tests/test_mypy_clear.py`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/LICENSE` & `2fas-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/README.md` & `2fas-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `2fas-1.0.2/pyproject.toml` & `2fas-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "lib2fas",
+    "lib2fas>=0.1.7",
     "configuraptor>=1.25",
     "typer[all]",
     "questionary",
     "typing-extensions",
 ]
 
 [template.plugins.default]
```

### Comparing `2fas-1.0.2/PKG-INFO` & `2fas-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2fas
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial implementation of 2fas for Python (as a CLI tool)
 Project-URL: Documentation, https://github.com/robinvandernoord/2fas-python#readme
 Project-URL: Issues, https://github.com/robinvandernoord/2fas-python/issues
 Project-URL: Source, https://github.com/robinvandernoord/2fas-python
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: configuraptor>=1.25
-Requires-Dist: lib2fas
+Requires-Dist: lib2fas>=0.1.7
 Requires-Dist: questionary
 Requires-Dist: typer[all]
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: edwh; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest-mypy-testing; extra == 'dev'
```

