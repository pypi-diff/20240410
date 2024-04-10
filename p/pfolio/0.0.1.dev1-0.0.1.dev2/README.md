# Comparing `tmp/pfolio-0.0.1.dev1.tar.gz` & `tmp/pfolio-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfolio-0.0.1.dev1.tar", max compression
+gzip compressed data, was "pfolio-0.0.1.dev2.tar", max compression
```

## Comparing `pfolio-0.0.1.dev1.tar` & `pfolio-0.0.1.dev2.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0    11355 2024-04-05 14:48:06.450848 pfolio-0.0.1.dev1/LICENSE
--rw-r--r--   0        0        0      407 2024-04-06 14:00:28.815973 pfolio-0.0.1.dev1/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:44:19.444627 pfolio-0.0.1.dev1/pfolio/__init__.py
--rw-r--r--   0        0        0      870 2024-04-06 13:36:17.967016 pfolio-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 pfolio-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-05 14:48:06.450848 pfolio-0.0.1.dev2/LICENSE
+-rw-r--r--   0        0        0      407 2024-04-06 14:00:28.815973 pfolio-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:44:19.444627 pfolio-0.0.1.dev2/pfolio/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:44:39.618232 pfolio-0.0.1.dev2/pfolio/analyses/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:48:22.745728 pfolio-0.0.1.dev2/pfolio/analyses/factor_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:48:20.086983 pfolio-0.0.1.dev2/pfolio/analyses/scenario_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:47:37.550178 pfolio-0.0.1.dev2/pfolio/analytics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:47:26.782131 pfolio-0.0.1.dev2/pfolio/analytics/returns.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:47:16.665083 pfolio-0.0.1.dev2/pfolio/analytics/risks.py
+-rw-r--r--   0        0        0       87 2024-04-07 08:32:09.408511 pfolio-0.0.1.dev2/pfolio/main.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:13:09.421752 pfolio-0.0.1.dev2/pfolio/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:24:19.905612 pfolio-0.0.1.dev2/pfolio/statistics/__init__.py
+-rw-r--r--   0        0        0     2146 2024-04-10 07:24:01.264911 pfolio-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 pfolio-0.0.1.dev2/PKG-INFO
```

### Comparing `pfolio-0.0.1.dev1/LICENSE` & `pfolio-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

