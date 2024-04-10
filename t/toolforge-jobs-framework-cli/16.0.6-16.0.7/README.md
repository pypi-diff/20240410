# Comparing `tmp/toolforge-jobs-framework-cli-16.0.6.tar.gz` & `tmp/toolforge-jobs-framework-cli-16.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-jobs-framework-cli-16.0.6.tar", last modified: Tue Apr  9 12:05:37 2024, max compression
+gzip compressed data, was "toolforge-jobs-framework-cli-16.0.7.tar", last modified: Wed Apr 10 14:58:03 2024, max compression
```

## Comparing `toolforge-jobs-framework-cli-16.0.6.tar` & `toolforge-jobs-framework-cli-16.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11108 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    32483 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11090 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    32304 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-10 14:57:58.000000 toolforge-jobs-framework-cli-16.0.7/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:03.784200 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-10 14:58:03.000000 toolforge-jobs-framework-cli-16.0.7/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge-jobs-framework-cli-16.0.6/LICENSE` & `toolforge-jobs-framework-cli-16.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/README.md` & `toolforge-jobs-framework-cli-16.0.7/README.md`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/tests/test_api.py` & `toolforge-jobs-framework-cli-16.0.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/tests/test_dump.py` & `toolforge-jobs-framework-cli-16.0.7/tests/test_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 DumpTestCase_3_mount = {
     "api_job": {
         "name": "mount-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "False",
+        "filelog": False,
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
@@ -109,15 +109,15 @@
 
 DumpTestCase_4_mount = {
     "api_job": {
         "name": "mount-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "False",
+        "filelog": False,
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
@@ -132,15 +132,15 @@
 
 DumpTestCase_5_filelog_stdout = {
     "api_job": {
         "name": "filelog-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "True",
+        "filelog": True,
         "filelog_stdout": "/something",
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
@@ -157,15 +157,15 @@
 
 DumpTestCase_5_filelog_stderr = {
     "api_job": {
         "name": "filelog-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "True",
+        "filelog": True,
         "filelog_stdout": None,
         "filelog_stderr": "/something",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
@@ -182,15 +182,15 @@
 
 DumpTestCase_6_filelog_buildservice = {
     "api_job": {
         "name": "filelog-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "False",
+        "filelog": False,
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
@@ -205,15 +205,15 @@
 
 DumpTestCase_7_filelog_buildservice = {
     "api_job": {
         "name": "filelog-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "image_state": "stable",
-        "filelog": "True",
+        "filelog": True,
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
@@ -229,15 +229,15 @@
 
 DumpTestCase_8_filelog_non_buildservice = {
     "api_job": {
         "name": "filelog-test",
         "cmd": "./mycommand.sh --argument1",
         "image": "bookworm",
         "image_state": "stable",
-        "filelog": "False",
+        "filelog": False,
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
@@ -253,15 +253,15 @@
 
 DumpTestCase_9_memory = {
     "api_job": {
         "name": "mem",
         "cmd": "./mycommand.sh --argument1",
         "image": "bookworm",
         "image_state": "stable",
-        "filelog": "True",
+        "filelog": True,
         "filelog_stdout": "/data/project/tf-test/mem.out",
         "filelog_stderr": "/data/project/tf-test/mem.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
@@ -278,15 +278,15 @@
 
 DumpTestCase_10_filelog_path_shorten = {
     "api_job": {
         "name": "short",
         "cmd": "./mycommand.sh --argument1",
         "image": "bookworm",
         "image_state": "stable",
-        "filelog": "True",
+        "filelog": True,
         "filelog_stdout": "/data/project/tf-test/dir/something.out",
         "filelog_stderr": "$TOOL_DATA_DIR/dir/something.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
```

### Comparing `toolforge-jobs-framework-cli-16.0.6/tests/test_loader.py` & `toolforge-jobs-framework-cli-16.0.7/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/tjf_cli/api.py` & `toolforge-jobs-framework-cli-16.0.7/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/tjf_cli/cli.py` & `toolforge-jobs-framework-cli-16.0.7/tjf_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,18 +377,15 @@
     elif cont is not None:
         job["type"] = "continuous"
         job.pop("continuous", None)
     else:
         job["type"] = "one-off"
 
     filelog = job.get("filelog", False)
-    # We are currently sending a stringified boolean, remove str support once
-    # https://gitlab.wikimedia.org/repos/cloud/toolforge/jobs-api/-/merge_requests/70
-    # is in
-    if str(filelog) == "True":
+    if filelog:
         job["filelog"] = "yes"
     else:
         job["filelog"] = "no"
 
     if retry == 0:
         job["retry"] = "no"
     else:
@@ -854,30 +851,30 @@
 
     # let's fail if these key are not present. It would be very unexpected, we want the explicit failure
     job["command"] = job["cmd"]
     image = job["image"]
     jobname = job["name"]
 
     filelog = job.pop("filelog", False)
-    if filelog == "True":
+    if filelog:
         if _image_is_buildservice(image):
             # this was explicitly set for a buildservice image, show it
             job["filelog"] = "yes"
     else:
         if not _image_is_buildservice(image):
             # this was explicitly set for a non-buildservice image, show it
             job["no-filelog"] = "true"
 
     # drop default and None filelog paths
     stdout = job.get("filelog_stdout")
-    if not is_default_filelog_file(filelog=stdout, jobname=jobname, filesuffix="out"):
+    if stdout and not is_default_filelog_file(filelog=stdout, jobname=jobname, filesuffix="out"):
         job["filelog-stdout"] = shorten_filelog_path(stdout)
 
     stderr = job.get("filelog_stderr")
-    if not is_default_filelog_file(filelog=stderr, jobname=jobname, filesuffix="err"):
+    if stderr and not is_default_filelog_file(filelog=stderr, jobname=jobname, filesuffix="err"):
         job["filelog-stderr"] = shorten_filelog_path(stderr)
 
     if job.get("mount") == "none":
         if _image_is_buildservice(image):
             # this is the default for a buildservice image, hide it
             job.pop("mount")
     elif job.get("mount") == "all":
```

### Comparing `toolforge-jobs-framework-cli-16.0.6/tjf_cli/errors.py` & `toolforge-jobs-framework-cli-16.0.7/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.6/tjf_cli/loader.py` & `toolforge-jobs-framework-cli-16.0.7/tjf_cli/loader.py`

 * *Files identical despite different names*

