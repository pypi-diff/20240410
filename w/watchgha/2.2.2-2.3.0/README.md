# Comparing `tmp/watchgha-2.2.2.tar.gz` & `tmp/watchgha-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ned/watchgha/dist/.tmp-vgw79uv8/watchgha-2.2.2.tar", last modified: Sat Feb  3 17:52:04 2024, max compression
+gzip compressed data, was "/Users/ned/watchgha/dist/.tmp-ci_dahsk/watchgha-2.3.0.tar", last modified: Wed Apr 10 17:25:22 2024, max compression
```

## Comparing `watchgha-2.2.2.tar` & `watchgha-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-02-03 17:52:04.000000 watchgha-2.2.2/
--rw-r--r--   0 ned        (501) wheel        (0)      515 2022-12-02 14:22:28.000000 watchgha-2.2.2/.editorconfig
--rw-r--r--   0 ned        (501) wheel        (0)    10177 2022-12-02 14:18:16.000000 watchgha-2.2.2/LICENSE.txt
--rw-r--r--   0 ned        (501) wheel        (0)       86 2023-07-02 23:07:34.000000 watchgha-2.2.2/MANIFEST.in
--rw-r--r--   0 ned        (501) wheel        (0)     3189 2024-01-27 11:33:56.000000 watchgha-2.2.2/Makefile
--rw-r--r--   0 ned        (501) wheel        (0)    12400 2024-02-03 17:52:04.000000 watchgha-2.2.2/PKG-INFO
--rw-r--r--   0 ned        (501) wheel        (0)    11452 2024-02-03 17:46:37.000000 watchgha-2.2.2/README.rst
--rw-r--r--   0 ned        (501) wheel        (0)       91 2023-06-30 21:19:24.000000 watchgha-2.2.2/dev-requirements.txt
--rw-r--r--   0 ned        (501) wheel        (0)     1443 2023-07-05 11:21:51.000000 watchgha-2.2.2/pyproject.toml
--rw-r--r--   0 ned        (501) wheel        (0)       38 2024-02-03 17:52:04.000000 watchgha-2.2.2/setup.cfg
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha/
--rw-r--r--   0 ned        (501) wheel        (0)       22 2024-02-03 17:47:00.000000 watchgha-2.2.2/src/watchgha/__init__.py
--rw-r--r--   0 ned        (501) wheel        (0)      729 2023-09-07 19:35:47.000000 watchgha-2.2.2/src/watchgha/bucketer.py
--rw-r--r--   0 ned        (501) wheel        (0)     7312 2024-02-02 20:14:35.000000 watchgha-2.2.2/src/watchgha/data_core.py
--rw-r--r--   0 ned        (501) wheel        (0)     3438 2023-09-07 19:42:56.000000 watchgha-2.2.2/src/watchgha/demo.py
--rw-r--r--   0 ned        (501) wheel        (0)      620 2024-02-03 17:51:00.000000 watchgha-2.2.2/src/watchgha/git_help.py
--rw-r--r--   0 ned        (501) wheel        (0)     3338 2024-01-12 00:10:20.000000 watchgha-2.2.2/src/watchgha/http_help.py
--rw-r--r--   0 ned        (501) wheel        (0)     1109 2023-09-07 19:42:56.000000 watchgha-2.2.2/src/watchgha/utils.py
--rw-r--r--   0 ned        (501) wheel        (0)     6042 2024-01-11 11:38:15.000000 watchgha-2.2.2/src/watchgha/watch_runs.py
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/
--rw-r--r--   0 ned        (501) wheel        (0)    12400 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/PKG-INFO
--rw-r--r--   0 ned        (501) wheel        (0)      518 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/SOURCES.txt
--rw-r--r--   0 ned        (501) wheel        (0)        1 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/dependency_links.txt
--rw-r--r--   0 ned        (501) wheel        (0)       60 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/entry_points.txt
--rw-r--r--   0 ned        (501) wheel        (0)       53 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/requires.txt
--rw-r--r--   0 ned        (501) wheel        (0)        9 2024-02-03 17:52:04.000000 watchgha-2.2.2/src/watchgha.egg-info/top_level.txt
--rw-r--r--   0 ned        (501) wheel        (0)   401606 2024-01-13 04:02:39.000000 watchgha-2.2.2/watch.gif
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/
+-rw-r--r--   0 ned        (501) wheel        (0)      515 2022-12-02 14:22:28.000000 watchgha-2.3.0/.editorconfig
+-rw-r--r--   0 ned        (501) wheel        (0)    10177 2022-12-02 14:18:16.000000 watchgha-2.3.0/LICENSE.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       86 2023-07-02 23:07:34.000000 watchgha-2.3.0/MANIFEST.in
+-rw-r--r--   0 ned        (501) wheel        (0)     3292 2024-02-03 17:53:04.000000 watchgha-2.3.0/Makefile
+-rw-r--r--   0 ned        (501) wheel        (0)    12978 2024-04-10 17:25:22.000000 watchgha-2.3.0/PKG-INFO
+-rw-r--r--   0 ned        (501) wheel        (0)    12030 2024-04-10 17:23:28.000000 watchgha-2.3.0/README.rst
+-rw-r--r--   0 ned        (501) wheel        (0)       91 2023-06-30 21:19:24.000000 watchgha-2.3.0/dev-requirements.txt
+-rw-r--r--   0 ned        (501) wheel        (0)     1443 2023-07-05 11:21:51.000000 watchgha-2.3.0/pyproject.toml
+-rw-r--r--   0 ned        (501) wheel        (0)       38 2024-04-10 17:25:22.000000 watchgha-2.3.0/setup.cfg
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha/
+-rw-r--r--   0 ned        (501) wheel        (0)       22 2024-04-10 17:23:45.000000 watchgha-2.3.0/src/watchgha/__init__.py
+-rw-r--r--   0 ned        (501) wheel        (0)      729 2023-09-07 19:35:47.000000 watchgha-2.3.0/src/watchgha/bucketer.py
+-rw-r--r--   0 ned        (501) wheel        (0)     7311 2024-04-02 13:27:28.000000 watchgha-2.3.0/src/watchgha/data_core.py
+-rw-r--r--   0 ned        (501) wheel        (0)     3438 2023-09-07 19:42:56.000000 watchgha-2.3.0/src/watchgha/demo.py
+-rw-r--r--   0 ned        (501) wheel        (0)      620 2024-02-03 17:51:00.000000 watchgha-2.3.0/src/watchgha/git_help.py
+-rw-r--r--   0 ned        (501) wheel        (0)     3338 2024-01-12 00:10:20.000000 watchgha-2.3.0/src/watchgha/http_help.py
+-rw-r--r--   0 ned        (501) wheel        (0)     1109 2023-09-07 19:42:56.000000 watchgha-2.3.0/src/watchgha/utils.py
+-rw-r--r--   0 ned        (501) wheel        (0)     6296 2024-04-10 17:13:14.000000 watchgha-2.3.0/src/watchgha/watch_runs.py
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/
+-rw-r--r--   0 ned        (501) wheel        (0)    12978 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/PKG-INFO
+-rw-r--r--   0 ned        (501) wheel        (0)      518 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/SOURCES.txt
+-rw-r--r--   0 ned        (501) wheel        (0)        1 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/dependency_links.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       60 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/entry_points.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       53 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/requires.txt
+-rw-r--r--   0 ned        (501) wheel        (0)        9 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/top_level.txt
+-rw-r--r--   0 ned        (501) wheel        (0)   401606 2024-01-13 04:02:39.000000 watchgha-2.3.0/watch.gif
```

### Comparing `watchgha-2.2.2/.editorconfig` & `watchgha-2.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/LICENSE.txt` & `watchgha-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/Makefile` & `watchgha-2.3.0/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 release: _check_credentials clean check_release dist pypi tag gh_release comment	## Do all the steps for a release
 
 _check_credentials:
 	@if [[ -z "$$TWINE_PASSWORD" ]]; then \
 		echo 'Missing TWINE_PASSWORD: opvars'; \
 		exit 1; \
 	fi
+	@if [[ -z "$$GITHUB_TOKEN" ]]; then \
+		echo 'Missing GITHUB_TOKEN: opvars github'; \
+		exit 1; \
+	fi
 
 check_release: _check_manifest _check_tree _check_readme _check_version	## Check that we are ready for a release
 	@echo "Release checks passed"
 
 _pip_install_e:
 	python -m pip install -q -e .
```

### Comparing `watchgha-2.2.2/PKG-INFO` & `watchgha-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.2.2
+Version: 2.3.0
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -58,14 +58,18 @@
         }; f"
 
 Now ``git runs`` will show a live display of the current runs on your branch.
 
 You can authenticate against GitHub if needed using either an entry in your
 .netrc file, or by setting the ``GITHUB_TOKEN`` environment variable.
 
+If you use GitHub Enterprise, you can set the environment variables
+``GITHUB_SERVER_URL`` (default: ``https://github.com``) and
+``GITHUB_API_URL`` (default: ``https://api.github.com``)
+to match your instance.
 
 Usage
 =====
 
 .. [[[cog
     import os
     import subprocess
@@ -201,14 +205,27 @@
     - This changelog is updated manually, not with scriv.
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.0 – 2024-04-10
+------------------
+
+- GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
+  ``GITHUB_API_URL`` environment variables.
+  Thanks, `Colin Marquardt <pull 21_>`_.
+
+- Fix: in unusual cases, GitHub can return strange statuses for job steps.
+  Those are now displayed as question marks.
+
+.. _pull 21: https://github.com/nedbat/watchgha/pull/21
+
+
 2.2.2 – 2024-02-03
 ------------------
 
 - Fix: steps can be in a "pending" state, and are now displayed with a dot
   instead of "pending".
```

### Comparing `watchgha-2.2.2/README.rst` & `watchgha-2.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         }; f"
 
 Now ``git runs`` will show a live display of the current runs on your branch.
 
 You can authenticate against GitHub if needed using either an entry in your
 .netrc file, or by setting the ``GITHUB_TOKEN`` environment variable.
 
+If you use GitHub Enterprise, you can set the environment variables
+``GITHUB_SERVER_URL`` (default: ``https://github.com``) and
+``GITHUB_API_URL`` (default: ``https://api.github.com``)
+to match your instance.
 
 Usage
 =====
 
 .. [[[cog
     import os
     import subprocess
@@ -178,14 +182,27 @@
     - This changelog is updated manually, not with scriv.
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.0 – 2024-04-10
+------------------
+
+- GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
+  ``GITHUB_API_URL`` environment variables.
+  Thanks, `Colin Marquardt <pull 21_>`_.
+
+- Fix: in unusual cases, GitHub can return strange statuses for job steps.
+  Those are now displayed as question marks.
+
+.. _pull 21: https://github.com/nedbat/watchgha/pull/21
+
+
 2.2.2 – 2024-02-03
 ------------------
 
 - Fix: steps can be in a "pending" state, and are now displayed with a dot
   instead of "pending".
```

### Comparing `watchgha-2.2.2/pyproject.toml` & `watchgha-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/bucketer.py` & `watchgha-2.3.0/src/watchgha/bucketer.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/data_core.py` & `watchgha-2.3.0/src/watchgha/data_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                                 current_step = f"failure {step['name']}"
                                 break
                             if step["status"] == "in_progress":
                                 done = False
                                 stepdots = ""
                                 for s in steps:
                                     ssum = summary_style_icon(s)[0]
-                                    stepdots += STEPDOTS.get(ssum, ssum)
+                                    stepdots += STEPDOTS.get(ssum, "?")
                                 current_step = f" {step['name']}"
                                 break
                         else:
                             if steps:
                                 current_step = steps[-1]["name"]
                             elif (
                                 job["status"] == "completed"
```

### Comparing `watchgha-2.2.2/src/watchgha/demo.py` & `watchgha-2.3.0/src/watchgha/demo.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/git_help.py` & `watchgha-2.3.0/src/watchgha/git_help.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/http_help.py` & `watchgha-2.3.0/src/watchgha/http_help.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/utils.py` & `watchgha-2.3.0/src/watchgha/utils.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/src/watchgha/watch_runs.py` & `watchgha-2.3.0/src/watchgha/watch_runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,22 +126,25 @@
         params["branch"] = branch
     url_args = urllib.parse.urlencode(params)
 
     github_urls = []
     for repo_url in repo_urls:
         # repo_url = "https://github.com/owner/repo.git"
         # repo_url = "git@github.com:someorg/somerepo.git"
+        # see also https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
+        server_url = os.getenv("GITHUB_SERVER_URL", "https://github.com")
         repo_match = re.fullmatch(
-            r"(?:https://github.com/|git@github.com:)([^/]+/[^/]+?)(?:\.git|/)?",
+            rf"(?:{re.escape(server_url)}/|git@github.com:)([^/]+/[^/]+?)(?:\.git|/)?",
             repo_url,
         )
         if repo_match is None:
             continue
 
-        url = f"https://api.github.com/repos/{repo_match[1]}/actions/runs?{url_args}"
+        api_url = os.getenv("GITHUB_API_URL", "https://api.github.com")
+        url = f"{api_url}/repos/{repo_match[1]}/actions/runs?{url_args}"
         github_urls.append(url)
 
     if not github_urls:
         fatal(f"Couldn't find GitHub repo from remote urls: {repo_urls!r}")
 
     return github_urls
```

### Comparing `watchgha-2.2.2/src/watchgha.egg-info/PKG-INFO` & `watchgha-2.3.0/src/watchgha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.2.2
+Version: 2.3.0
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -58,14 +58,18 @@
         }; f"
 
 Now ``git runs`` will show a live display of the current runs on your branch.
 
 You can authenticate against GitHub if needed using either an entry in your
 .netrc file, or by setting the ``GITHUB_TOKEN`` environment variable.
 
+If you use GitHub Enterprise, you can set the environment variables
+``GITHUB_SERVER_URL`` (default: ``https://github.com``) and
+``GITHUB_API_URL`` (default: ``https://api.github.com``)
+to match your instance.
 
 Usage
 =====
 
 .. [[[cog
     import os
     import subprocess
@@ -201,14 +205,27 @@
     - This changelog is updated manually, not with scriv.
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.0 – 2024-04-10
+------------------
+
+- GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
+  ``GITHUB_API_URL`` environment variables.
+  Thanks, `Colin Marquardt <pull 21_>`_.
+
+- Fix: in unusual cases, GitHub can return strange statuses for job steps.
+  Those are now displayed as question marks.
+
+.. _pull 21: https://github.com/nedbat/watchgha/pull/21
+
+
 2.2.2 – 2024-02-03
 ------------------
 
 - Fix: steps can be in a "pending" state, and are now displayed with a dot
   instead of "pending".
```

### Comparing `watchgha-2.2.2/src/watchgha.egg-info/SOURCES.txt` & `watchgha-2.3.0/src/watchgha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.2.2/watch.gif` & `watchgha-2.3.0/watch.gif`

 * *Files identical despite different names*

