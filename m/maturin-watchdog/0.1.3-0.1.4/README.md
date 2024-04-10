# Comparing `tmp/maturin_watchdog-0.1.3.tar.gz` & `tmp/maturin_watchdog-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.3.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.4.tar", max compression
```

## Comparing `maturin_watchdog-0.1.3.tar` & `maturin_watchdog-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.3/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:28:54.546372 maturin_watchdog-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1152 2024-04-10 16:28:35.354602 maturin_watchdog-0.1.3/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.4/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:33:22.078838 maturin_watchdog-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2447 2024-04-10 16:33:14.285661 maturin_watchdog-0.1.4/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.4/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.3/pyproject.toml` & `maturin_watchdog-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.3"
+version = "0.1.4"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

