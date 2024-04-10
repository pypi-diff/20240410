# Comparing `tmp/netcheck-0.5.2.tar.gz` & `tmp/netcheck-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.5.2.tar", max compression
+gzip compressed data, was "netcheck-0.5.3.tar", max compression
```

## Comparing `netcheck-0.5.2.tar` & `netcheck-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-25 08:04:29.133452 netcheck-0.5.2/LICENSE
--rw-r--r--   0        0        0     9727 2024-03-25 08:04:29.133452 netcheck-0.5.2/README.md
--rw-r--r--   0        0        0        0 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/checks/__init__.py
--rw-r--r--   0        0        0     2347 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/checks/dns.py
--rw-r--r--   0        0        0     2164 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/checks/http.py
--rw-r--r--   0        0        0      412 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/checks/internal.py
--rw-r--r--   0        0        0     5892 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/cli.py
--rw-r--r--   0        0        0     3776 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/context.py
--rw-r--r--   0        0        0     6178 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/runner.py
--rw-r--r--   0        0        0     2197 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/validation.py
--rw-r--r--   0        0        0      214 2024-03-25 08:04:29.149452 netcheck-0.5.2/netcheck/version.py
--rw-r--r--   0        0        0      867 2024-03-25 08:04:29.157452 netcheck-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    10570 1970-01-01 00:00:00.000000 netcheck-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 11:47:00.581887 netcheck-0.5.3/LICENSE
+-rw-r--r--   0        0        0     9727 2024-04-10 11:47:00.581887 netcheck-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/checks/__init__.py
+-rw-r--r--   0        0        0     2347 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/checks/dns.py
+-rw-r--r--   0        0        0     2164 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/checks/http.py
+-rw-r--r--   0        0        0      412 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/checks/internal.py
+-rw-r--r--   0        0        0     5892 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/cli.py
+-rw-r--r--   0        0        0     3776 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/context.py
+-rw-r--r--   0        0        0     6178 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/runner.py
+-rw-r--r--   0        0        0     2197 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/validation.py
+-rw-r--r--   0        0        0      214 2024-04-10 11:47:00.593887 netcheck-0.5.3/netcheck/version.py
+-rw-r--r--   0        0        0      867 2024-04-10 11:47:00.601887 netcheck-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    10570 1970-01-01 00:00:00.000000 netcheck-0.5.3/PKG-INFO
```

### Comparing `netcheck-0.5.2/LICENSE` & `netcheck-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/README.md` & `netcheck-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/checks/dns.py` & `netcheck-0.5.3/netcheck/checks/dns.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/checks/http.py` & `netcheck-0.5.3/netcheck/checks/http.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/cli.py` & `netcheck-0.5.3/netcheck/cli.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/context.py` & `netcheck-0.5.3/netcheck/context.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/runner.py` & `netcheck-0.5.3/netcheck/runner.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/netcheck/validation.py` & `netcheck-0.5.3/netcheck/validation.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.5.2/pyproject.toml` & `netcheck-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netcheck"
-version = "0.5.2"
+version = "0.5.3"
 description = "Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "netcheck"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `netcheck-0.5.2/PKG-INFO` & `netcheck-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.5.2
+Version: 0.5.3
 Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

