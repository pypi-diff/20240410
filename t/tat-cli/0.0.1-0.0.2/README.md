# Comparing `tmp/tat_cli-0.0.1.tar.gz` & `tmp/tat_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tat_cli-0.0.1.tar", last modified: Thu Mar 28 19:33:53 2024, max compression
+gzip compressed data, was "tat_cli-0.0.2.tar", last modified: Wed Apr 10 15:31:35 2024, max compression
```

## Comparing `tat_cli-0.0.1.tar` & `tat_cli-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:33:53.007684 tat_cli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-28 19:33:44.000000 tat_cli-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-28 19:33:53.007684 tat_cli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-28 19:33:44.000000 tat_cli-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-28 19:33:44.000000 tat_cli-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:33:53.007684 tat_cli-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:33:53.003684 tat_cli-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:33:53.003684 tat_cli-0.0.1/src/tat_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 19:33:44.000000 tat_cli-0.0.1/src/tat_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 19:33:44.000000 tat_cli-0.0.1/src/tat_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-28 19:33:44.000000 tat_cli-0.0.1/src/tat_cli/tat.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-28 19:33:44.000000 tat_cli-0.0.1/src/tat_cli/tat_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:33:53.007684 tat_cli-0.0.1/src/tat_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-28 19:33:52.000000 tat_cli-0.0.1/src/tat_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 19:33:52.000000 tat_cli-0.0.1/src/tat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:33:52.000000 tat_cli-0.0.1/src/tat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-28 19:33:52.000000 tat_cli-0.0.1/src/tat_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 19:33:52.000000 tat_cli-0.0.1/src/tat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:31:35.291283 tat_cli-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 15:31:30.000000 tat_cli-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 15:31:35.291283 tat_cli-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-10 15:31:30.000000 tat_cli-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-10 15:31:30.000000 tat_cli-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:31:35.291283 tat_cli-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:31:35.287283 tat_cli-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:31:35.287283 tat_cli-0.0.2/src/tat_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 15:31:30.000000 tat_cli-0.0.2/src/tat_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 15:31:30.000000 tat_cli-0.0.2/src/tat_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-10 15:31:30.000000 tat_cli-0.0.2/src/tat_cli/tat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 15:31:30.000000 tat_cli-0.0.2/src/tat_cli/tat_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:31:35.291283 tat_cli-0.0.2/src/tat_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 15:31:35.000000 tat_cli-0.0.2/src/tat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 15:31:35.000000 tat_cli-0.0.2/src/tat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:31:35.000000 tat_cli-0.0.2/src/tat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 15:31:35.000000 tat_cli-0.0.2/src/tat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 15:31:35.000000 tat_cli-0.0.2/src/tat_cli.egg-info/top_level.txt
```

### Comparing `tat_cli-0.0.1/LICENSE` & `tat_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tat_cli-0.0.1/PKG-INFO` & `tat_cli-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: tat_cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Colorize terminal output with regex.
 Author-email: salt-die <salt-die@protonmail.com>
 License: MIT
 Project-URL: repository, https://github.com/salt-die/tat_cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tat_cli
-A command-line tool to colorize terminal output with regex. 
+A command-line tool to colorize terminal output with regex. `pip install tat-cli` to install.
 
 Each group in the regex will be colored independently. `tat-cli` supports nested groups and 24-bit colors.
 
 Example usage:
 
 ```sh
 $ echo "start [121 45567 345] - [454 45563 676] end" | tat "(\[(\d(\d\d)) (\d(\d(\d)\d)\d) ((\d\d)\d)\])"
```

### Comparing `tat_cli-0.0.1/README.md` & `tat_cli-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tat_cli
-A command-line tool to colorize terminal output with regex. 
+A command-line tool to colorize terminal output with regex. `pip install tat-cli` to install.
 
 Each group in the regex will be colored independently. `tat-cli` supports nested groups and 24-bit colors.
 
 Example usage:
 
 ```sh
 $ echo "start [121 45567 345] - [454 45563 676] end" | tat "(\[(\d(\d\d)) (\d(\d(\d)\d)\d) ((\d\d)\d)\])"
```

### Comparing `tat_cli-0.0.1/pyproject.toml` & `tat_cli-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tat_cli-0.0.1/src/tat_cli/tat.py` & `tat_cli-0.0.2/src/tat_cli/tat.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,20 +43,23 @@
 def tat(pattern: str, colors: list[str] | None = None) -> None:
     """
     Colorize stdin with a regex pattern.
 
     Parameters
     ----------
     pattern : str
-        Regex pattern used on stdin.
+        Regex pattern used on stdin. Only groups in the regex are colored. If a regex
+        pattern has no groups, the whole match will be treated as a group.
     colors : list[str] | None, default: None
         Color or color-pair for each group in the regex pattern. If none or too few are
         provided, rainbow colors are used.
     """
     regex = re.compile(pattern)
+    if regex.groups == 0:
+        regex = re.compile(f"({pattern})")
 
     if colors is None or len(colors) < regex.groups:
         colors = _rainbow_gradient(regex.groups)
     colors = [_ansi_from_hexcode(color) for color in colors]
 
     piped = sys.stdin.read()
     out = []
```

### Comparing `tat_cli-0.0.1/src/tat_cli/tat_cli.py` & `tat_cli-0.0.2/src/tat_cli/tat_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from .tat import tat
 
 
 def tat_cli() -> None:
     """Parse command-line arguments for `tat`."""
     parser = argparse.ArgumentParser(description="Colorize terminal output with regex.")
     parser.add_argument(
-        "pattern", metavar="REGEX", help="A regex pattern to be used on output."
+        "pattern",
+        metavar="REGEX",
+        help=(
+            "A regex pattern to be used on output. Only groups in the regex are "
+            "colored. If a regex pattern has no groups, the whole match will be "
+            "treated as a group."
+        ),
     )
     parser.add_argument(
         "colors",
         metavar="COLORS",
         nargs="*",
         help=(
             "List of colors or color-pairs for each group in the regex. "
```

### Comparing `tat_cli-0.0.1/src/tat_cli.egg-info/PKG-INFO` & `tat_cli-0.0.2/src/tat_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: tat_cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Colorize terminal output with regex.
 Author-email: salt-die <salt-die@protonmail.com>
 License: MIT
 Project-URL: repository, https://github.com/salt-die/tat_cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tat_cli
-A command-line tool to colorize terminal output with regex. 
+A command-line tool to colorize terminal output with regex. `pip install tat-cli` to install.
 
 Each group in the regex will be colored independently. `tat-cli` supports nested groups and 24-bit colors.
 
 Example usage:
 
 ```sh
 $ echo "start [121 45567 345] - [454 45563 676] end" | tat "(\[(\d(\d\d)) (\d(\d(\d)\d)\d) ((\d\d)\d)\])"
```

