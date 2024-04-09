# Comparing `tmp/dump_psql_roles_grants-0.2.2.dev4.tar.gz` & `tmp/dump_psql_roles_grants-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dump_psql_roles_grants-0.2.2.dev4.tar", max compression
+gzip compressed data, was "dump_psql_roles_grants-0.3.0.tar", max compression
```

## Comparing `dump_psql_roles_grants-0.2.2.dev4.tar` & `dump_psql_roles_grants-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1265 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/README.md
--rw-r--r--   0        0        0      290 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/__main__.py
--rw-r--r--   0        0        0      429 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/classes.py
--rw-r--r--   0        0        0     3248 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/cli.py
--rw-r--r--   0        0        0     3674 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/commands.py
--rw-r--r--   0        0        0      920 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/config.py
--rwxr-xr-x   0        0        0     7698 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/get_data.py
--rw-r--r--   0        0        0     5560 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/table.py
--rw-r--r--   0        0        0      959 2024-04-09 21:36:04.151664 dump_psql_roles_grants-0.2.2.dev4/pyproject.toml
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 dump_psql_roles_grants-0.2.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/README.md
+-rw-r--r--   0        0        0      290 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/__main__.py
+-rw-r--r--   0        0        0      429 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/classes.py
+-rw-r--r--   0        0        0     3248 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/cli.py
+-rw-r--r--   0        0        0     3674 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/commands.py
+-rw-r--r--   0        0        0      920 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/config.py
+-rwxr-xr-x   0        0        0     7698 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/get_data.py
+-rw-r--r--   0        0        0     5560 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/table.py
+-rw-r--r--   0        0        0      856 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 dump_psql_roles_grants-0.3.0/PKG-INFO
```

### Comparing `dump_psql_roles_grants-0.2.2.dev4/README.md` & `dump_psql_roles_grants-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # Dump Postgres Roles and Grants
 
 ## Install
 
-You can choose
-
-- plain python package `dump-psql-roles-grants` that requires `libpq` system library
-- or package `dump-psql-roles-grants[binary]` that have binaries included
-
 ### pipx
 
 ```shell
-pipx install 'dump-psql-roles-grants[binary]'
+pipx install dump-psql-roles-grants
 dump-psql-roles-grants --help
 ```
 
 ### pip
 
 ```shell
-pip install 'dump-psql-roles-grants[binary]'
+pip install dump-psql-roles-grants
 python -m dump_psql_roles_grants --help
 ```
 
 ### docker
 
 ```shell
 docker pull rgeraskin/dump_psql_roles_grants
```

### Comparing `dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/cli.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/cli.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/commands.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/commands.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/config.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/config.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/get_data.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/get_data.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.2.dev4/dump_psql_roles_grants/table.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/table.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.2.dev4/pyproject.toml` & `dump_psql_roles_grants-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 [tool.poetry]
 name = "dump-psql-roles-grants"
-version = "0.2.2.dev4"
+version = "0.3.0"
 description = "Dump Postgres Roles and Grants"
 authors = ["Roman Geraskin <roman.n.geraskin@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/rgeraskin/dump_psql_roles_grants"
 keywords = ["postgres", "psql", "roles", "grants", "dump"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 icecream = "^2.1.3"
 pytablewriter = "^1.2.0"
 click = "^8.1.7"
 rich = "^13.7.1"
-psycopg = "^3.1.18"
-psycopg-binary = {version = "^3.1.18", optional = true}
+psycopg-binary = "^3.1.18"
 psycopg-infdate = "^1.0.3"
 PyYAML = "^6.0.1"
 
-[tool.poetry.extras]
-binary = ["psycopg-binary"]
-
 [tool.poetry.scripts]
 dump_psql_roles_grants = "dump_psql_roles_grants.cli:cli"
 
+
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 [build-system]
```

### Comparing `dump_psql_roles_grants-0.2.2.dev4/PKG-INFO` & `dump_psql_roles_grants-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 Metadata-Version: 2.1
 Name: dump-psql-roles-grants
-Version: 0.2.2.dev4
+Version: 0.3.0
 Summary: Dump Postgres Roles and Grants
 Home-page: https://github.com/rgeraskin/dump_psql_roles_grants
 License: MIT
 Keywords: postgres,psql,roles,grants,dump
 Author: Roman Geraskin
 Author-email: roman.n.geraskin@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: binary
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
-Requires-Dist: psycopg (>=3.1.18,<4.0.0)
-Requires-Dist: psycopg-binary (>=3.1.18,<4.0.0) ; extra == "binary"
+Requires-Dist: psycopg-binary (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg-infdate (>=1.0.3,<2.0.0)
 Requires-Dist: pytablewriter (>=1.2.0,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Repository, https://github.com/rgeraskin/dump_psql_roles_grants
 Description-Content-Type: text/markdown
 
 # Dump Postgres Roles and Grants
 
 ## Install
 
-You can choose
-
-- plain python package `dump-psql-roles-grants` that requires `libpq` system library
-- or package `dump-psql-roles-grants[binary]` that have binaries included
-
 ### pipx
 
 ```shell
-pipx install 'dump-psql-roles-grants[binary]'
+pipx install dump-psql-roles-grants
 dump-psql-roles-grants --help
 ```
 
 ### pip
 
 ```shell
-pip install 'dump-psql-roles-grants[binary]'
+pip install dump-psql-roles-grants
 python -m dump_psql_roles_grants --help
 ```
 
 ### docker
 
 ```shell
 docker pull rgeraskin/dump_psql_roles_grants
```

