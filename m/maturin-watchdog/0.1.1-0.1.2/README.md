# Comparing `tmp/maturin_watchdog-0.1.1.tar.gz` & `tmp/maturin_watchdog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.1.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.1.2.tar", max compression
```

## Comparing `maturin_watchdog-0.1.1.tar` & `maturin_watchdog-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.1/README.md
--rw-r--r--   0        0        0      421 2024-04-10 16:23:14.083128 maturin_watchdog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1105 2024-04-10 16:20:11.085950 maturin_watchdog-0.1.1/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.2/README.md
+-rw-r--r--   0        0        0      529 2024-04-10 16:26:42.020243 maturin_watchdog-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1105 2024-04-10 16:20:11.085950 maturin_watchdog-0.1.2/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.2/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.1/src/maturin_watchdog/plugin.py` & `maturin_watchdog-0.1.2/src/maturin_watchdog/plugin.py`

 * *Files identical despite different names*

