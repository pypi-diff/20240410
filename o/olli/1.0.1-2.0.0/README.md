# Comparing `tmp/olli-1.0.1.tar.gz` & `tmp/olli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olli-1.0.1.tar", max compression
+gzip compressed data, was "olli-2.0.0.tar", max compression
```

## Comparing `olli-1.0.1.tar` & `olli-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1054 2023-09-12 23:51:35.736124 olli-1.0.1/LICENSE
--rw-r--r--   0        0        0      757 2023-09-12 23:51:35.736124 olli-1.0.1/README.md
--rw-r--r--   0        0        0       73 2023-09-12 23:51:35.736124 olli-1.0.1/olli/__init__.py
--rw-r--r--   0        0        0      460 2023-09-12 23:51:35.736124 olli-1.0.1/olli/__main__.py
--rw-r--r--   0        0        0     2049 2023-09-12 23:51:35.736124 olli-1.0.1/olli/alert.py
--rw-r--r--   0        0        0     1332 2023-09-12 23:51:35.736124 olli-1.0.1/olli/api.py
--rw-r--r--   0        0        0     3237 2023-09-12 23:51:35.736124 olli-1.0.1/olli/config.py
--rw-r--r--   0        0        0      506 2023-09-12 23:51:35.736124 olli-1.0.1/olli/structures.py
--rw-r--r--   0        0        0     2453 2023-09-12 23:51:35.736124 olli-1.0.1/olli/webhook.py
--rw-r--r--   0        0        0     1577 2023-09-12 23:51:35.736124 olli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 olli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-04-10 16:17:34.409455 olli-2.0.0/LICENSE
+-rw-r--r--   0        0        0      757 2024-04-10 16:17:34.409455 olli-2.0.0/README.md
+-rw-r--r--   0        0        0       73 2024-04-10 16:17:34.409455 olli-2.0.0/olli/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-10 16:17:34.409455 olli-2.0.0/olli/__main__.py
+-rw-r--r--   0        0        0     2049 2024-04-10 16:17:34.409455 olli-2.0.0/olli/alert.py
+-rw-r--r--   0        0        0     1344 2024-04-10 16:17:34.409455 olli-2.0.0/olli/api.py
+-rw-r--r--   0        0        0     3237 2024-04-10 16:17:34.409455 olli-2.0.0/olli/config.py
+-rw-r--r--   0        0        0      506 2024-04-10 16:17:34.409455 olli-2.0.0/olli/structures.py
+-rw-r--r--   0        0        0     2453 2024-04-10 16:17:34.409455 olli-2.0.0/olli/webhook.py
+-rw-r--r--   0        0        0     1624 2024-04-10 16:17:34.409455 olli-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 olli-2.0.0/PKG-INFO
```

### Comparing `olli-1.0.1/LICENSE` & `olli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `olli-1.0.1/README.md` & `olli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `olli-1.0.1/olli/alert.py` & `olli-2.0.0/olli/alert.py`

 * *Files identical despite different names*

### Comparing `olli-1.0.1/olli/api.py` & `olli-2.0.0/olli/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         start_ts = start_time.timestamp() * 1_000_000_000
 
         job_regex = "|".join(LOKI_CONFIG.jobs)
 
         case_filter = "(?i)" if not token.case_sensitive else ""
 
         resp = httpx.get(self.route("query_range"), params={
-            "query": f'{{job=~"({job_regex})"}} |~ "{case_filter}{token.token}"',
+            "query": f'{{service_name=~"({job_regex})-.+"}} |~ "{case_filter}{token.token}"',
             "start": f"{start_ts:0.0f}",
             "limit": LOKI_CONFIG.max_logs,
         })
 
         resp.raise_for_status()
 
         return resp.json()
```

### Comparing `olli-1.0.1/olli/config.py` & `olli-2.0.0/olli/config.py`

 * *Files identical despite different names*

### Comparing `olli-1.0.1/olli/webhook.py` & `olli-2.0.0/olli/webhook.py`

 * *Files identical despite different names*

### Comparing `olli-1.0.1/pyproject.toml` & `olli-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olli"
-version = "1.0.1"
+version = "2.0.0"
 description = "Olli searches your Loki logs and relays matching terms to Discord."
 authors = ["Joe Banks <joseph@josephbanks.me>", "Chris Lovering <chris.lovering.95@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 # Links
 homepage = "https://python-discord.github.io/olli/"
@@ -19,47 +19,50 @@
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators"
 ]
 
 [tool.poetry.dependencies]
 python = "3.11.*"
 
-httpx = "0.25.0"
+httpx = "0.25.2"
 loguru = "0.7.2"
-pydantic = "2.0.3"
-pydantic-settings = "2.0.3"
-schedule = "1.2.0"
+pydantic = "2.5.2"
+pydantic-settings = "2.1.0"
+schedule = "1.2.1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "3.4.0"
-ruff = "0.0.288"
-taskipy = "1.12.0"
+pre-commit = "3.5.0"
+ruff = "0.1.7"
+taskipy = "1.12.2"
 
 [tool.poetry.scripts]
 olli = "olli.__main__:start"
 
 [tool.taskipy.tasks]
 lint = "pre-commit run --all-files"
 precommit = "pre-commit install"
 olli = "python -m olli"
 
 [tool.ruff]
 target-version = "py311"
 extend-exclude = [".cache"]
+select = ["ALL"]
 ignore = [
     "ANN002", "ANN003", "ANN101", "ANN102", "ANN401",
     "ARG003",
     "C901",
+    "CPY001",
     "D100", "D104", "D105", "D107", "D203", "D212", "D214", "D215", "D416",
     "EM101",
     "PLR",
     "TRY003",
 ]
 line-length = 120
-select = ["ALL"]
+unsafe-fixes = true
+preview = true
 
 [tool.ruff.isort]
 order-by-type = false
 case-sensitive = true
 combine-as-imports = true
 
 [build-system]
```

### Comparing `olli-1.0.1/PKG-INFO` & `olli-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: olli
-Version: 1.0.1
+Version: 2.0.0
 Summary: Olli searches your Loki logs and relays matching terms to Discord.
 Home-page: https://python-discord.github.io/olli/
 License: MIT
 Keywords: loki,discord,logs,observability
 Author: Joe Banks
 Author-email: joseph@josephbanks.me
 Requires-Python: ==3.11.*
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (==0.25.0)
+Requires-Dist: httpx (==0.25.2)
 Requires-Dist: loguru (==0.7.2)
-Requires-Dist: pydantic (==2.0.3)
-Requires-Dist: pydantic-settings (==2.0.3)
-Requires-Dist: schedule (==1.2.0)
+Requires-Dist: pydantic (==2.5.2)
+Requires-Dist: pydantic-settings (==2.1.0)
+Requires-Dist: schedule (==1.2.1)
 Project-URL: Documentation, https://python-discord.github.io/olli/
 Project-URL: Repository, https://github.com/python-discord/olli
 Description-Content-Type: text/markdown
 
 # Olli
 
 [![PyPI version fury.io](https://badge.fury.io/py/olli.svg)](https://pypi.python.org/pypi/olli/)
```

