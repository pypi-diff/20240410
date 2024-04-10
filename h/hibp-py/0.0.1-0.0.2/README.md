# Comparing `tmp/hibp-py-0.0.1.tar.gz` & `tmp/hibp_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibp-py-0.0.1.tar", last modified: Mon Jun  5 19:38:40 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hibp-py-0.0.1.tar` & `hibp_py-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 19:38:40.743657 hibp-py-0.0.1/
--rw-rw-rw-   0        0        0     1022 2023-06-05 19:38:40.744654 hibp-py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-06-05 19:35:01.000000 hibp-py-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1097 2023-06-05 19:38:40.748640 hibp-py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-06-05 19:38:18.000000 hibp-py-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:38:40.684853 hibp-py-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 19:38:40.714753 hibp-py-0.0.1/src/hibp_py/
--rw-rw-rw-   0        0        0      910 2023-05-23 19:12:40.000000 hibp-py-0.0.1/src/hibp_py/ad.py
--rw-rw-rw-   0        0        0     1366 2023-05-23 19:11:44.000000 hibp-py-0.0.1/src/hibp_py/api.py
--rw-rw-rw-   0        0        0      640 2023-04-27 15:29:46.000000 hibp-py-0.0.1/src/hibp_py/args.py
--rw-rw-rw-   0        0        0        0 2023-05-23 19:12:24.000000 hibp-py-0.0.1/src/hibp_py/main.py
--rw-rw-rw-   0        0        0        0 2023-04-27 15:55:05.000000 hibp-py-0.0.1/src/hibp_py/report.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:38:40.740666 hibp-py-0.0.1/src/hibp_py.egg-info/
--rw-rw-rw-   0        0        0     1022 2023-06-05 19:38:40.000000 hibp-py-0.0.1/src/hibp_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-05 19:38:40.000000 hibp-py-0.0.1/src/hibp_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:38:40.000000 hibp-py-0.0.1/src/hibp_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 19:38:39.000000 hibp-py-0.0.1/src/hibp_py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-05 19:38:40.000000 hibp-py-0.0.1/src/hibp_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 19:38:40.000000 hibp-py-0.0.1/src/hibp_py.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 hibp_py-0.0.2/SECURITY.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 hibp_py-0.0.2/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 hibp_py-0.0.2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 hibp_py-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 hibp_py-0.0.2/input/t_domain.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/__main__.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/ad.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/api.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/args.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hibp_py-0.0.2/src/hibp_py/report.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 hibp_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hibp_py-0.0.2/LICENSE
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hibp_py-0.0.2/README.md
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 hibp_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 hibp_py-0.0.2/PKG-INFO
```

### Comparing `hibp-py-0.0.1/src/hibp_py/ad.py` & `hibp_py-0.0.2/src/hibp_py/ad.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import win32api
-import win32security
-
-
-class ActiveDirectoryConnection():
-    def __init__(self) -> None:
-        import win32api
-        import win32security
-
-        # Get the process handle for the current process
-        process_handle = win32api.GetCurrentProcess()
-
-        # Get the token handle for the process
-        token_handle = win32security.OpenProcessToken(
-            process_handle, win32security.TOKEN_READ)
-
-        # Get the SID for the current user
-        user_sid = win32security.GetTokenInformation(
-            token_handle, win32security.TokenUser)[0]
-
-        # Get the user object from Active Directory using the user's SID
-        user_obj = win32security.LookupAccountSid(None, user_sid)
-
-        # Print the user's domain, username, and full name
-        print(
-            f"Domain: {user_obj[0]}\nUsername: {user_obj[1]}\nFull Name: {user_obj[2]}")
+import win32api
+import win32security
+
+
+class ActiveDirectoryConnection():
+    def __init__(self) -> None:
+        import win32api
+        import win32security
+
+        # Get the process handle for the current process
+        process_handle = win32api.GetCurrentProcess()
+
+        # Get the token handle for the process
+        token_handle = win32security.OpenProcessToken(
+            process_handle, win32security.TOKEN_READ)
+
+        # Get the SID for the current user
+        user_sid = win32security.GetTokenInformation(
+            token_handle, win32security.TokenUser)[0]
+
+        # Get the user object from Active Directory using the user's SID
+        user_obj = win32security.LookupAccountSid(None, user_sid)
+
+        # Print the user's domain, username, and full name
+        print(
+            f"Domain: {user_obj[0]}\nUsername: {user_obj[1]}\nFull Name: {user_obj[2]}")
```

