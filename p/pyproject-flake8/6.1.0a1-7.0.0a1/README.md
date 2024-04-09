# Comparing `tmp/pyproject_flake8-6.1.0a1.tar.gz` & `tmp/pyproject_flake8-7.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_flake8-6.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyproject_flake8-7.0.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyproject_flake8-6.1.0a1.tar` & `pyproject_flake8-7.0.0a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/LICENSE
--rw-r--r--   0        0        0     3189 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/README.md
--rw-r--r--   0        0        0     3937 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pflake8/__init__.py
--rw-r--r--   0        0        0       76 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pflake8/__main__.py
--rw-r--r--   0        0        0      766 2023-09-23 10:46:05.475748 pyproject_flake8-6.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 pyproject_flake8-6.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-09 22:05:49.621688 pyproject_flake8-7.0.0a1/LICENSE
+-rw-r--r--   0        0        0     3189 2024-04-09 22:05:49.621688 pyproject_flake8-7.0.0a1/README.md
+-rw-r--r--   0        0        0     4250 2024-04-09 22:05:49.621688 pyproject_flake8-7.0.0a1/pflake8/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-09 22:05:49.621688 pyproject_flake8-7.0.0a1/pflake8/__main__.py
+-rw-r--r--   0        0        0      829 2024-04-09 22:05:49.621688 pyproject_flake8-7.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 pyproject_flake8-7.0.0a1/PKG-INFO
```

### Comparing `pyproject_flake8-6.1.0a1/LICENSE` & `pyproject_flake8-7.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_flake8-6.1.0a1/README.md` & `pyproject_flake8-7.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_flake8-6.1.0a1/pflake8/__init__.py` & `pyproject_flake8-7.0.0a1/pflake8/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ pyproject-flake8 (`pflake8`), a monkey patching wrapper to connect flake8 with pyproject.toml configuration """  # noqa
 
-__version__ = '6.1.0a1'
+__version__ = '7.0.0a1'
 
 import ast
 import configparser
 import multiprocessing.pool
 import sys
 from pathlib import Path
 from types import ModuleType
@@ -28,16 +28,19 @@
             toml_config = toml_load(fp.buffer)
 
             section_to_copy = (
                 toml_config if not is_pyproject else toml_config.get('tool', {})
             )
 
             for section, config in section_to_copy.items():
-                self.add_section(section)
-                self._sections[section] = self._dict(config)
+                try:
+                    self.add_section(section)
+                except (configparser.DuplicateSectionError):
+                    pass
+                self._sections.setdefault(section, self._dict()).update(self._dict(config))
         else:
             super(ConfigParserTomlMixin, self)._read(fp, filename)
 
     def _convert_to_boolean(self, value):
         if isinstance(value, bool):
             return value
         else:
@@ -48,21 +51,28 @@
     pass
 
 
 class DivertingConfigParser(ConfigParserTomlMixin, configparser.ConfigParser):
     pass
 
 
-class DivertingSafeConfigParser(ConfigParserTomlMixin, configparser.SafeConfigParser):
-    pass
+try:
+
+    class DivertingSafeConfigParser(
+        ConfigParserTomlMixin, configparser.SafeConfigParser
+    ):
+        pass
+
+    configparser.SafeConfigParser = DivertingSafeConfigParser
+except AttributeError:
+    pass  # does not exist on Python 3.12 (https://github.com/python/cpython/issues/89336#issuecomment-1094366625)
 
 
 configparser.RawConfigParser = DivertingRawConfigParser
 configparser.ConfigParser = DivertingConfigParser
-configparser.SafeConfigParser = DivertingSafeConfigParser
 
 
 class FixFilenames(ast.NodeTransformer):
     tuple_of_interest = ("setup.cfg", "tox.ini", ".flake8")
 
     modern = sys.version_info[0] >= 3 and sys.version_info[1] > 7
```

### Comparing `pyproject_flake8-6.1.0a1/pyproject.toml` & `pyproject_flake8-7.0.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 authors = [{name = "Christian Sachs", email = "sachs.christian@gmail.com"}]
 readme = "README.md"
 license = { file = "LICENSE" } 
 classifiers = []
 requires-python = ">=3.8.1"
 dependencies = [
     "tomli; python_version < '3.11'",
-    "flake8 >= 6.1.0"
+    "flake8 >= 7.0.0"
 ]
 
 [project.urls]
 Home = "https://github.com/csachs/pyproject-flake8"
 
 [project.scripts]
 pflake8 = "pflake8.__main__:main"
 
 [tool.flit.module]
 name = "pflake8"
 
 [tool.black]
 skip-string-normalization = 1
+force-exclude = [
+    "test/data/dummy.py",
+]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.flake8]
 max-line-length = 88
 extend-ignore = ["E203"]
 max-complexity = 10
-exclude = "venv"
+exclude = ["venv", "test/data/"]
```

### Comparing `pyproject_flake8-6.1.0a1/PKG-INFO` & `pyproject_flake8-7.0.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyproject-flake8
-Version: 6.1.0a1
+Version: 7.0.0a1
 Summary: pyproject-flake8 (`pflake8`), a monkey patching wrapper to connect flake8 with pyproject.toml configuration 
 Author-email: Christian Sachs <sachs.christian@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Requires-Dist: tomli; python_version < '3.11'
-Requires-Dist: flake8 >= 6.1.0
+Requires-Dist: flake8 >= 7.0.0
 Project-URL: Home, https://github.com/csachs/pyproject-flake8
 
 # pyproject-flake8 (`pflake8`)
 
 A monkey patching wrapper to connect flake8 with `pyproject.toml` configuration.
 
 ## Update concerning versioning:
```

