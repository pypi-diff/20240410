# Comparing `tmp/kbve-1.0.2.tar.gz` & `tmp/kbve-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbve-1.0.2.tar", max compression
+gzip compressed data, was "kbve-1.0.3.tar", max compression
```

## Comparing `kbve-1.0.2.tar` & `kbve-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0       35 2023-10-14 14:30:55.360253 kbve-1.0.2/README.md
--rw-r--r--   0        0        0      161 2023-10-14 14:30:55.360253 kbve-1.0.2/kbve_atlas/OAI_CONFIG_LIST.json
--rw-r--r--   0        0        0       12 2023-10-14 14:30:55.360253 kbve-1.0.2/kbve_atlas/__init__.py
--rw-r--r--   0        0        0      940 2023-10-14 14:30:55.364253 kbve-1.0.2/kbve_atlas/atlas_autogen.py
--rw-r--r--   0        0        0      473 2023-10-14 14:30:55.364253 kbve-1.0.2/kbve_atlas/hello.py
--rw-r--r--   0        0        0    10246 2023-10-14 14:30:56.232277 kbve-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5980 1970-01-01 00:00:00.000000 kbve-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-04-09 21:15:33.551920 kbve-1.0.3/README.md
+-rw-r--r--   0        0        0      161 2024-04-09 21:15:33.551920 kbve-1.0.3/kbve_atlas/OAI_CONFIG_LIST.json
+-rw-r--r--   0        0        0       12 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/__init__.py
+-rw-r--r--   0        0        0      940 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/atlas_autogen.py
+-rw-r--r--   0        0        0      619 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/bigman.py
+-rw-r--r--   0        0        0      221 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/bitcoin.py
+-rw-r--r--   0        0        0     1480 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/doom.py
+-rw-r--r--   0        0        0     1167 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/enter_the_matrix.py
+-rw-r--r--   0        0        0      473 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/hello.py
+-rw-r--r--   0        0        0     4640 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/memetris.py
+-rw-r--r--   0        0        0     2012 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/pacman.py
+-rw-r--r--   0        0        0     1379 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/snake.py
+-rw-r--r--   0        0        0     2215 2024-04-09 21:15:33.555920 kbve-1.0.3/kbve_atlas/tetris.py
+-rw-r--r--   0        0        0    11634 2024-04-09 21:15:34.247919 kbve-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6783 1970-01-01 00:00:00.000000 kbve-1.0.3/PKG-INFO
```

### Comparing `kbve-1.0.2/kbve_atlas/atlas_autogen.py` & `kbve-1.0.3/kbve_atlas/atlas_autogen.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.2/pyproject.toml` & `kbve-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,83 +7,88 @@
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html:'../../coverage/apps/atlas/html' --cov-report xml:'../../coverage/apps/atlas/coverage.xml' --html='../../reports/apps/atlas/unittests/html/index.html' --junitxml='../../reports/apps/atlas/unittests/junit.xml'"
 
 [tool.poetry]
 name = "kbve"
-version = "1.0.2"
+version = "1.0.3"
 description = "ATLAS"
 authors = [ ]
 license = "Proprietary"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "kbve_atlas"
 
   [tool.poetry.dependencies]
   python = ">=3.9,<3.11"
 
     [tool.poetry.dependencies.aiohttp]
-    version = "3.8.5 "
+    version = "3.9.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.aiosignal]
     version = "1.3.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.alembic]
-    version = "1.12.0 "
+    version = "1.13.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
-    [tool.poetry.dependencies.appdirs]
-    version = "1.4.4 "
+    [tool.poetry.dependencies.annotated-types]
+    version = "0.6.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
+    [tool.poetry.dependencies.anyio]
+    version = "4.3.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.async-timeout]
     version = "4.0.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.attrs]
-    version = "23.1.0 "
+    version = "23.2.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.autopage]
-    version = "0.5.1 "
+    version = "0.5.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.beautifulsoup4]
-    version = "4.12.2 "
+    version = "4.12.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.certifi]
-    version = "2023.7.22 "
+    version = "2024.2.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.charset-normalizer]
-    version = "3.3.0 "
+    version = "3.3.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.click]
     version = "8.1.7 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.cliff]
-    version = "4.3.0 "
+    version = "4.6.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.cmaes]
     version = "0.10.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
@@ -95,232 +100,272 @@
 
     [tool.poetry.dependencies.colorama]
     version = "0.4.6 "
     markers = 'python_version >= "3.9" and python_version < "3.11" and (platform_system == "Windows" or sys_platform == "win32")'
     optional = false
 
     [tool.poetry.dependencies.colorlog]
-    version = "6.7.0 "
+    version = "6.8.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.diskcache]
     version = "5.6.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
+    [tool.poetry.dependencies.distro]
+    version = "1.9.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
     [tool.poetry.dependencies.docker]
     version = "6.1.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
+    [tool.poetry.dependencies.exceptiongroup]
+    version = "1.2.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
     [tool.poetry.dependencies.filelock]
-    version = "3.12.4 "
+    version = "3.13.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.flaml]
-    version = "2.1.1 "
+    version = "2.1.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
     extras = [ "blendsearch" ]
 
     [tool.poetry.dependencies.frozenlist]
-    version = "1.4.0 "
+    version = "1.4.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.fsspec]
-    version = "2023.9.2 "
+    version = "2024.3.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.greenlet]
-    version = "3.0.0 "
+    version = "3.0.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")'
     optional = false
 
+    [tool.poetry.dependencies.h11]
+    version = "0.14.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
+    [tool.poetry.dependencies.httpcore]
+    version = "1.0.5 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
+    [tool.poetry.dependencies.httpx]
+    version = "0.27.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
     [tool.poetry.dependencies.huggingface-hub]
-    version = "0.16.4 "
+    version = "0.22.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.idna]
-    version = "3.4 "
+    version = "3.6 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.importlib-metadata]
-    version = "6.8.0 "
+    version = "7.1.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.jinja2]
-    version = "3.1.2 "
+    version = "3.1.3 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.litellm]
-    version = "0.1.824 "
+    version = "1.34.34 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.mako]
-    version = "1.2.4 "
+    version = "1.3.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.markupsafe]
-    version = "2.1.3 "
+    version = "2.1.5 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.multidict]
-    version = "6.0.4 "
+    version = "6.0.5 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.numpy]
-    version = "1.26.0 "
+    version = "1.26.4 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.openai]
-    version = "0.28.1 "
+    version = "1.16.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.optuna]
     version = "2.8.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.packaging]
-    version = "23.2 "
+    version = "24.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.pbr]
-    version = "5.11.1 "
+    version = "6.0.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.prettytable]
-    version = "3.9.0 "
+    version = "3.10.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.pyautogen]
-    version = "0.1.6 "
+    version = "0.1.12 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
     extras = [ "blendsearch" ]
 
+    [tool.poetry.dependencies.pydantic-core]
+    version = "2.16.3 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
+    [tool.poetry.dependencies.pydantic]
+    version = "2.6.4 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
     [tool.poetry.dependencies.pyperclip]
     version = "1.8.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.pyreadline3]
     version = "3.4.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11" and sys_platform == "win32"'
     optional = false
 
     [tool.poetry.dependencies.python-dotenv]
-    version = "1.0.0 "
+    version = "1.0.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.pywin32]
     version = "306 "
     markers = 'python_version >= "3.9" and python_version < "3.11" and sys_platform == "win32"'
     optional = false
 
     [tool.poetry.dependencies.pyyaml]
     version = "6.0.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.regex]
-    version = "2023.10.3 "
+    version = "2023.12.25 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.requests]
     version = "2.31.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.scipy]
-    version = "1.11.3 "
+    version = "1.13.0 "
+    markers = 'python_version >= "3.9" and python_version < "3.11"'
+    optional = false
+
+    [tool.poetry.dependencies.sniffio]
+    version = "1.3.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.soupsieve]
     version = "2.5 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.sqlalchemy]
-    version = "2.0.21 "
+    version = "2.0.29 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.stevedore]
-    version = "5.1.0 "
+    version = "5.2.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.termcolor]
-    version = "2.3.0 "
+    version = "2.4.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.tiktoken]
-    version = "0.5.1 "
+    version = "0.6.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.tokenizers]
-    version = "0.14.0 "
+    version = "0.15.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.tqdm]
-    version = "4.66.1 "
+    version = "4.66.2 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.typing-extensions]
-    version = "4.8.0 "
+    version = "4.11.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.urllib3]
-    version = "2.0.6 "
+    version = "2.2.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.wcwidth]
-    version = "0.2.8 "
+    version = "0.2.13 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.websocket-client]
-    version = "1.6.3 "
+    version = "1.7.0 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.yarl]
-    version = "1.9.2 "
+    version = "1.9.4 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
     [tool.poetry.dependencies.zipp]
-    version = "3.17.0 "
+    version = "3.18.1 "
     markers = 'python_version >= "3.9" and python_version < "3.11"'
     optional = false
 
 [tool.poetry.group.dev]
 dependencies = { }
 
 [build-system]
```

### Comparing `kbve-1.0.2/PKG-INFO` & `kbve-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,84 @@
 Metadata-Version: 2.1
 Name: kbve
-Version: 1.0.2
+Version: 1.0.3
 Summary: ATLAS
 License: Proprietary
 Requires-Python: >=3.9,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: aiohttp (==3.8.5) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: aiohttp (==3.9.3) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: aiosignal (==1.3.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: alembic (==1.12.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: appdirs (==1.4.4) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: alembic (==1.13.1) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: annotated-types (==0.6.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: anyio (==4.3.0) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: async-timeout (==4.0.3) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: attrs (==23.1.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: autopage (==0.5.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: beautifulsoup4 (==4.12.2) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: certifi (==2023.7.22) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: charset-normalizer (==3.3.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: attrs (==23.2.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: autopage (==0.5.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: beautifulsoup4 (==4.12.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: certifi (==2024.2.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: charset-normalizer (==3.3.2) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: click (==8.1.7) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: cliff (==4.3.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: cliff (==4.6.0) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: cmaes (==0.10.0) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: cmd2 (==2.4.3) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: colorama (==0.4.6) ; python_version >= "3.9" and python_version < "3.11" and (platform_system == "Windows" or sys_platform == "win32")
-Requires-Dist: colorlog (==6.7.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: colorlog (==6.8.2) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: diskcache (==5.6.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: distro (==1.9.0) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: docker (==6.1.3) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: filelock (==3.12.4) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: flaml[blendsearch] (==2.1.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: frozenlist (==1.4.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: fsspec (==2023.9.2) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: greenlet (==3.0.0) ; python_version >= "3.9" and python_version < "3.11" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
-Requires-Dist: huggingface-hub (==0.16.4) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: idna (==3.4) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: importlib-metadata (==6.8.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: jinja2 (==3.1.2) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: litellm (==0.1.824) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: mako (==1.2.4) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: markupsafe (==2.1.3) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: multidict (==6.0.4) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: numpy (==1.26.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: openai (==0.28.1) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: exceptiongroup (==1.2.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: filelock (==3.13.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: flaml[blendsearch] (==2.1.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: frozenlist (==1.4.1) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: fsspec (==2024.3.1) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: greenlet (==3.0.3) ; python_version >= "3.9" and python_version < "3.11" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
+Requires-Dist: h11 (==0.14.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: httpcore (==1.0.5) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: httpx (==0.27.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: huggingface-hub (==0.22.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: idna (==3.6) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: importlib-metadata (==7.1.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: jinja2 (==3.1.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: litellm (==1.34.34) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: mako (==1.3.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: markupsafe (==2.1.5) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: multidict (==6.0.5) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: numpy (==1.26.4) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: openai (==1.16.2) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: optuna (==2.8.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: packaging (==23.2) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: pbr (==5.11.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: prettytable (==3.9.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: pyautogen[blendsearch] (==0.1.6) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: packaging (==24.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: pbr (==6.0.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: prettytable (==3.10.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: pyautogen[blendsearch] (==0.1.12) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: pydantic (==2.6.4) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: pydantic-core (==2.16.3) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: pyperclip (==1.8.2) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: pyreadline3 (==3.4.1) ; python_version >= "3.9" and python_version < "3.11" and sys_platform == "win32"
-Requires-Dist: python-dotenv (==1.0.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: python-dotenv (==1.0.1) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: pywin32 (==306) ; python_version >= "3.9" and python_version < "3.11" and sys_platform == "win32"
 Requires-Dist: pyyaml (==6.0.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: regex (==2023.10.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: regex (==2023.12.25) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: requests (==2.31.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: scipy (==1.11.3) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: scipy (==1.13.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: sniffio (==1.3.1) ; python_version >= "3.9" and python_version < "3.11"
 Requires-Dist: soupsieve (==2.5) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: sqlalchemy (==2.0.21) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: stevedore (==5.1.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: termcolor (==2.3.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: tiktoken (==0.5.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: tokenizers (==0.14.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: tqdm (==4.66.1) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: typing-extensions (==4.8.0) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: urllib3 (==2.0.6) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: wcwidth (==0.2.8) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: websocket-client (==1.6.3) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: yarl (==1.9.2) ; python_version >= "3.9" and python_version < "3.11"
-Requires-Dist: zipp (==3.17.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: sqlalchemy (==2.0.29) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: stevedore (==5.2.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: termcolor (==2.4.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: tiktoken (==0.6.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: tokenizers (==0.15.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: tqdm (==4.66.2) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: typing-extensions (==4.11.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: urllib3 (==2.2.1) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: wcwidth (==0.2.13) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: websocket-client (==1.7.0) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: yarl (==1.9.4) ; python_version >= "3.9" and python_version < "3.11"
+Requires-Dist: zipp (==3.18.1) ; python_version >= "3.9" and python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # atlas
 
 Project description here.
```

