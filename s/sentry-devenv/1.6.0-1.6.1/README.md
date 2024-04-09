# Comparing `tmp/sentry_devenv-1.6.0.tar.gz` & `tmp/sentry_devenv-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_devenv-1.6.0.tar", last modified: Tue Apr  2 18:38:59 2024, max compression
+gzip compressed data, was "sentry_devenv-1.6.1.tar", last modified: Tue Apr  9 01:45:27 2024, max compression
```

## Comparing `sentry_devenv-1.6.0.tar` & `sentry_devenv-1.6.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/repo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/ci/integration/repo/devenv/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/ci/integration/repo/devenv/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/checks/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/doctor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/brew.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/colima.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/direnv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/limactl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/tenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib/volta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.131887 sentry_devenv-1.6.0/devenv/lib_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/brew.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/lib_check/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/pin_gha.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/pythons.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/devenv/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/sentry_devenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 18:38:59.000000 sentry_devenv-1.6.0/sentry_devenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.127887 sentry_devenv-1.6.0/tests/doctor/devenv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.135887 sentry_devenv-1.6.0/tests/doctor/devenv/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/bad_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/bad_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/broken_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/broken_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/failing_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/failing_check_with_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/no_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/devenv/checks/passing_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_attempt_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_filter_failing_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_load_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_prompt_for_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/doctor/test_run_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:38:59.139887 sentry_devenv-1.6.0/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_brew.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_direnv.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/lib/test_volta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 18:38:53.000000 sentry_devenv-1.6.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.118772 sentry_devenv-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-09 01:45:27.118772 sentry_devenv-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.102772 sentry_devenv-1.6.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.102772 sentry_devenv-1.6.1/ci/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.102772 sentry_devenv-1.6.1/ci/integration/repo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.106772 sentry_devenv-1.6.1/ci/integration/repo/devenv/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/ci/integration/repo/devenv/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.106772 sentry_devenv-1.6.1/devenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.106772 sentry_devenv-1.6.1/devenv/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/checks/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/doctor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.110772 sentry_devenv-1.6.1/devenv/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/colima.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/limactl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/tenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib/volta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.110772 sentry_devenv-1.6.1/devenv/lib_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib_check/brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/lib_check/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/pin_gha.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/pythons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/devenv/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.118772 sentry_devenv-1.6.1/sentry_devenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 01:45:27.000000 sentry_devenv-1.6.1/sentry_devenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 01:45:27.118772 sentry_devenv-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.114772 sentry_devenv-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.114772 sentry_devenv-1.6.1/tests/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.106772 sentry_devenv-1.6.1/tests/doctor/devenv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.114772 sentry_devenv-1.6.1/tests/doctor/devenv/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/bad_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/bad_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/broken_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/broken_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/failing_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/failing_check_with_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/no_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/no_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/no_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/devenv/checks/passing_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/test_attempt_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/test_filter_failing_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/test_load_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/test_prompt_for_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/doctor/test_run_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:45:27.118772 sentry_devenv-1.6.1/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_brew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_direnv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/lib/test_volta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/test_pythons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 01:45:06.000000 sentry_devenv-1.6.1/tests/utils.py
```

### Comparing `sentry_devenv-1.6.0/PKG-INFO` & `sentry_devenv-1.6.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,94 @@
 Metadata-Version: 2.1
 Name: sentry_devenv
-Version: 1.6.0
+Version: 1.6.1
 Summary: Utilities for setting up a Sentry development environment
 Author-email: Joshua Li <joshua.li@sentry.io>, Ian Woodard <ian.woodard@sentry.io>, Buck Evan <buck.evan@sentry.io>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions
 Requires-Dist: sentry-sdk
 
 ## devenv
 
-the next generation sentry devenv management tool
+managing dev environments since '24
+
+`devenv` is an extensible execution framework and library for authoring
+a simple set of high level commands - bootstrap, sync, doctor, nuke - that
+manage a repository's dev environment.
+
 
 ## install
 
 Download [this](https://raw.githubusercontent.com/getsentry/devenv/main/install-devenv.sh) and run it:
 
 ```
 bash install-devenv.sh
 ```
 
-**If you are setting up a new laptop, run `devenv bootstrap` after installing.**
+## user guide
+
+`devenv bootstrap [repository name]`
+
+This is intended for initial setup. `sentry` will set up both sentry and getsentry.
+Repositories are cloned to a "coderoot" directory which is specified in the [global configuration](#configuration).
+
+`devenv sync`
+
+When you're inside a repository, this will bring the dev environment up to date,
+or create it if it doesn't exist.
+It runs `[reporoot]/devenv/sync.py`.
+
+`devenv doctor`
+
+When you're inside a repository, this diagnoses and tries to fix common issues.
+Checks and fixes are defined in `[reporoot]/devenv/checks`.
 
+`devenv nuke|uninstall` (wip)
+
+When you're inside a repository, this completely removes the dev environment.
 
 
 ## technical overview
 
-`devenv` is a command-line interface to a set of environment management commands
-that can be custom implemented for a particular repository.
+devenv itself lives in `~/.local/share/sentry-devenv`. Inside:
+- `bin` contains devenv itself and `direnv`
+  - this is the only PATH entry needed for devenv
+- a private python and virtualenv used exclusively by `devenv`
 
-- `sync` brings the dev environment up-to-date
-  - example: in sentry, `sync` updates python+js dependencies, and runs migrations
-- `doctor` diagnoses and fixes common issues
-  - TODO: more on this later, we're working on this at the moment
-  - you can write these doctor "checks" using `devenv` facilities, and they're executed within devenv's environment
-  - example to be available at `sentry/devenv/checks/....py`
-- `exec` (coming soon) execs a command inside of `devenv`'s execution context, useful if things don't work locally
+As much as possible, a repo's dev environment is self-contained within `[reporoot]/.devenv`.
 
-Dependencies like `colima` and `volta` are hermetically installed and used within `devenv`'s execution.
-This lets us dictate how they get installed, and it doesn't affect the rest of the system.
+We're relying on `direnv` (which bootstrap will install, globally) to add `[reporoot]/.devenv/bin` to PATH.
+Therefore a minimum viable `[reporoot]/.envrc` might look like:
 
-`devenv` also:
-- helps new engineers `devenv bootstrap` their new macbooks nearly effortlessly
+```bash
+if [ -f "${PWD}/.env" ]; then
+    dotenv
+fi
 
+PATH_add "${HOME}/.local/share/sentry-devenv/bin"
 
-### per-repository configuration
+if ! command -v devenv >/dev/null; then
+    echo "install devenv: https://github.com/getsentry/devenv#install"
+    return 1
+fi
 
-`REPOROOT/devenv/config.ini`
+PATH_add "${PWD}/.devenv/bin"
+```
 
-an example: if the right `[python]` block is specified (see sentry's),
-we support downloading those prebuilt pythons for a repo's virtualenv
+### configuration
 
+global configuration is at `~/.config/sentry-devenv/config.ini`.
 
-## develop
+repository configuration is at `[reporoot]/devenv/config.ini`.
 
-Purpose: enable `gh act` to work quickly on localhost
 
-To that end:
+## develop
 
-1. build a docker image with python pre-installed at the expected location
-2. the python interpreter machine-architecture should match the host machine
+We use `tox`. The easiest way to run devenv locally is just using the tox venv's executable:
+
+```
+~/code/sentry $  ~/code/devenv/.tox/py311/bin/devenv sync
+```
```

### Comparing `sentry_devenv-1.6.0/ci/integration/repo/devenv/sync.py` & `sentry_devenv-1.6.1/ci/integration/repo/devenv/sync.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/bootstrap.py` & `sentry_devenv-1.6.1/devenv/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/checks/test.py` & `sentry_devenv-1.6.1/devenv/checks/test.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/constants.py` & `sentry_devenv-1.6.1/devenv/constants.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/doctor.py` & `sentry_devenv-1.6.1/devenv/doctor.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/archive.py` & `sentry_devenv-1.6.1/devenv/lib/archive.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/brew.py` & `sentry_devenv-1.6.1/devenv/lib/brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/colima.py` & `sentry_devenv-1.6.1/devenv/lib/colima.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/config.py` & `sentry_devenv-1.6.1/devenv/lib/config.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/direnv.py` & `sentry_devenv-1.6.1/devenv/lib/direnv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/fs.py` & `sentry_devenv-1.6.1/devenv/lib/fs.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/gcloud.py` & `sentry_devenv-1.6.1/devenv/lib/gcloud.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/github.py` & `sentry_devenv-1.6.1/devenv/lib/github.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/limactl.py` & `sentry_devenv-1.6.1/devenv/lib/limactl.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/proc.py` & `sentry_devenv-1.6.1/devenv/lib/proc.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/tenv.py` & `sentry_devenv-1.6.1/devenv/lib/tenv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/venv.py` & `sentry_devenv-1.6.1/devenv/lib/venv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib/volta.py` & `sentry_devenv-1.6.1/devenv/lib/volta.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/lib_check/brew.py` & `sentry_devenv-1.6.1/devenv/lib_check/brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/main.py` & `sentry_devenv-1.6.1/devenv/main.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/pin_gha.py` & `sentry_devenv-1.6.1/devenv/pin_gha.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/devenv/pythons.py` & `sentry_devenv-1.6.1/devenv/pythons.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import os
 
-from devenv.constants import home
+from devenv.constants import root
 from devenv.lib import archive
 
 
 def get(python_version: str, url: str, sha256: str) -> str:
-    unpack_into = f"{home}/pythons/{python_version}"
+    unpack_into = f"{root}/pythons/{python_version}"
 
     if os.path.exists(f"{unpack_into}/python/bin/python3"):
         return f"{unpack_into}/python/bin/python3"
 
     archive_file = archive.download(url, sha256)
     archive.unpack(archive_file, unpack_into)
```

### Comparing `sentry_devenv-1.6.0/devenv/sync.py` & `sentry_devenv-1.6.1/devenv/sync.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/pyproject.toml` & `sentry_devenv-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentry_devenv"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Joshua Li", email="joshua.li@sentry.io" },
   { name="Ian Woodard", email="ian.woodard@sentry.io" },
   { name="Buck Evan", email="buck.evan@sentry.io" },
 ]
 description = "Utilities for setting up a Sentry development environment"
 readme = "README.md"
```

### Comparing `sentry_devenv-1.6.0/sentry_devenv.egg-info/PKG-INFO` & `sentry_devenv-1.6.1/sentry_devenv.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,94 @@
 Metadata-Version: 2.1
 Name: sentry_devenv
-Version: 1.6.0
+Version: 1.6.1
 Summary: Utilities for setting up a Sentry development environment
 Author-email: Joshua Li <joshua.li@sentry.io>, Ian Woodard <ian.woodard@sentry.io>, Buck Evan <buck.evan@sentry.io>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions
 Requires-Dist: sentry-sdk
 
 ## devenv
 
-the next generation sentry devenv management tool
+managing dev environments since '24
+
+`devenv` is an extensible execution framework and library for authoring
+a simple set of high level commands - bootstrap, sync, doctor, nuke - that
+manage a repository's dev environment.
+
 
 ## install
 
 Download [this](https://raw.githubusercontent.com/getsentry/devenv/main/install-devenv.sh) and run it:
 
 ```
 bash install-devenv.sh
 ```
 
-**If you are setting up a new laptop, run `devenv bootstrap` after installing.**
+## user guide
+
+`devenv bootstrap [repository name]`
+
+This is intended for initial setup. `sentry` will set up both sentry and getsentry.
+Repositories are cloned to a "coderoot" directory which is specified in the [global configuration](#configuration).
+
+`devenv sync`
+
+When you're inside a repository, this will bring the dev environment up to date,
+or create it if it doesn't exist.
+It runs `[reporoot]/devenv/sync.py`.
+
+`devenv doctor`
+
+When you're inside a repository, this diagnoses and tries to fix common issues.
+Checks and fixes are defined in `[reporoot]/devenv/checks`.
 
+`devenv nuke|uninstall` (wip)
+
+When you're inside a repository, this completely removes the dev environment.
 
 
 ## technical overview
 
-`devenv` is a command-line interface to a set of environment management commands
-that can be custom implemented for a particular repository.
+devenv itself lives in `~/.local/share/sentry-devenv`. Inside:
+- `bin` contains devenv itself and `direnv`
+  - this is the only PATH entry needed for devenv
+- a private python and virtualenv used exclusively by `devenv`
 
-- `sync` brings the dev environment up-to-date
-  - example: in sentry, `sync` updates python+js dependencies, and runs migrations
-- `doctor` diagnoses and fixes common issues
-  - TODO: more on this later, we're working on this at the moment
-  - you can write these doctor "checks" using `devenv` facilities, and they're executed within devenv's environment
-  - example to be available at `sentry/devenv/checks/....py`
-- `exec` (coming soon) execs a command inside of `devenv`'s execution context, useful if things don't work locally
+As much as possible, a repo's dev environment is self-contained within `[reporoot]/.devenv`.
 
-Dependencies like `colima` and `volta` are hermetically installed and used within `devenv`'s execution.
-This lets us dictate how they get installed, and it doesn't affect the rest of the system.
+We're relying on `direnv` (which bootstrap will install, globally) to add `[reporoot]/.devenv/bin` to PATH.
+Therefore a minimum viable `[reporoot]/.envrc` might look like:
 
-`devenv` also:
-- helps new engineers `devenv bootstrap` their new macbooks nearly effortlessly
+```bash
+if [ -f "${PWD}/.env" ]; then
+    dotenv
+fi
 
+PATH_add "${HOME}/.local/share/sentry-devenv/bin"
 
-### per-repository configuration
+if ! command -v devenv >/dev/null; then
+    echo "install devenv: https://github.com/getsentry/devenv#install"
+    return 1
+fi
 
-`REPOROOT/devenv/config.ini`
+PATH_add "${PWD}/.devenv/bin"
+```
 
-an example: if the right `[python]` block is specified (see sentry's),
-we support downloading those prebuilt pythons for a repo's virtualenv
+### configuration
 
+global configuration is at `~/.config/sentry-devenv/config.ini`.
 
-## develop
+repository configuration is at `[reporoot]/devenv/config.ini`.
 
-Purpose: enable `gh act` to work quickly on localhost
 
-To that end:
+## develop
 
-1. build a docker image with python pre-installed at the expected location
-2. the python interpreter machine-architecture should match the host machine
+We use `tox`. The easiest way to run devenv locally is just using the tox venv's executable:
+
+```
+~/code/sentry $  ~/code/devenv/.tox/py311/bin/devenv sync
+```
```

### Comparing `sentry_devenv-1.6.0/sentry_devenv.egg-info/SOURCES.txt` & `sentry_devenv-1.6.1/sentry_devenv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 sentry_devenv.egg-info/dependency_links.txt
 sentry_devenv.egg-info/entry_points.txt
 sentry_devenv.egg-info/requires.txt
 sentry_devenv.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_main.py
+tests/test_pythons.py
 tests/utils.py
 tests/doctor/__init__.py
 tests/doctor/test_attempt_fix.py
 tests/doctor/test_filter_failing_checks.py
 tests/doctor/test_load_checks.py
 tests/doctor/test_prompt_for_fix.py
 tests/doctor/test_run_checks.py
```

### Comparing `sentry_devenv-1.6.0/tests/doctor/test_attempt_fix.py` & `sentry_devenv-1.6.1/tests/doctor/test_attempt_fix.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/doctor/test_filter_failing_checks.py` & `sentry_devenv-1.6.1/tests/doctor/test_filter_failing_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/doctor/test_load_checks.py` & `sentry_devenv-1.6.1/tests/doctor/test_load_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/doctor/test_prompt_for_fix.py` & `sentry_devenv-1.6.1/tests/doctor/test_prompt_for_fix.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/doctor/test_run_checks.py` & `sentry_devenv-1.6.1/tests/doctor/test_run_checks.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_archive.py` & `sentry_devenv-1.6.1/tests/lib/test_archive.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_brew.py` & `sentry_devenv-1.6.1/tests/lib/test_brew.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_direnv.py` & `sentry_devenv-1.6.1/tests/lib/test_direnv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_fs.py` & `sentry_devenv-1.6.1/tests/lib/test_fs.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_github.py` & `sentry_devenv-1.6.1/tests/lib/test_github.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_proc.py` & `sentry_devenv-1.6.1/tests/lib/test_proc.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_venv.py` & `sentry_devenv-1.6.1/tests/lib/test_venv.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/lib/test_volta.py` & `sentry_devenv-1.6.1/tests/lib/test_volta.py`

 * *Files identical despite different names*

### Comparing `sentry_devenv-1.6.0/tests/test_main.py` & `sentry_devenv-1.6.1/tests/test_main.py`

 * *Files identical despite different names*

