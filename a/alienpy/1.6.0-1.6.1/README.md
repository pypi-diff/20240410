# Comparing `tmp/alienpy-1.6.0.tar.gz` & `tmp/alienpy-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alienpy-1.6.0.tar", last modified: Fri Mar 15 15:06:07 2024, max compression
+gzip compressed data, was "alienpy-1.6.1.tar", last modified: Wed Apr 10 12:34:56 2024, max compression
```

## Comparing `alienpy-1.6.0.tar` & `alienpy-1.6.1.tar`

### file list

```diff
@@ -1,92 +1,33 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.036416 alienpy-1.6.0/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      345 2023-11-22 12:00:12.000000 alienpy-1.6.0/.deepsource.toml
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2882 2023-11-24 11:00:29.000000 alienpy-1.6.0/.flake8
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2021-03-11 10:24:30.000000 alienpy-1.6.0/.gitattributes
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       30 2020-03-10 22:07:14.000000 alienpy-1.6.0/.gitconfig
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.029416 alienpy-1.6.0/.github/
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.032416 alienpy-1.6.0/.github/workflows/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3997 2023-05-09 12:41:38.000000 alienpy-1.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 adrian    (1000) adrian    (1000)      223 2023-05-09 12:41:38.000000 alienpy-1.6.0/.gitignore
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16199 2023-06-07 09:27:41.000000 alienpy-1.6.0/.pylintrc
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2019-08-11 12:01:54.000000 alienpy-1.6.0/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10577 2024-03-15 15:06:07.036416 alienpy-1.6.0/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2021-08-24 15:12:24.000000 alienpy-1.6.0/README.md
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.033416 alienpy-1.6.0/alienpy/
--rw-r--r--   0 adrian    (1000) adrian    (1000)       51 2023-11-24 11:00:29.000000 alienpy-1.6.0/alienpy/__init__.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)    94887 2024-03-14 18:15:24.000000 alienpy-1.6.0/alienpy/alien.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3100 2023-11-24 11:00:29.000000 alienpy-1.6.0/alienpy/async_tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    15688 2023-11-27 10:56:06.000000 alienpy-1.6.0/alienpy/connect_ssl.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5970 2023-11-24 11:00:29.000000 alienpy-1.6.0/alienpy/data_structs.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3909 2024-02-02 14:18:58.000000 alienpy-1.6.0/alienpy/global_vars.py
--rwxrwxr-x   0 adrian    (1000) adrian    (1000)     2034 2020-06-09 11:54:43.000000 alienpy-1.6.0/alienpy/jboxpy
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1727 2023-11-22 12:41:49.000000 alienpy-1.6.0/alienpy/setup_cwd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2486 2023-11-22 13:59:54.000000 alienpy-1.6.0/alienpy/setup_logging.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1846 2024-03-14 18:15:24.000000 alienpy-1.6.0/alienpy/tools_history.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    48988 2024-03-14 18:15:24.000000 alienpy-1.6.0/alienpy/tools_nowb.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1866 2023-11-22 12:00:12.000000 alienpy-1.6.0/alienpy/tools_shell.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      897 2023-11-22 12:00:12.000000 alienpy-1.6.0/alienpy/tools_stackcmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2024-03-15 15:05:20.000000 alienpy-1.6.0/alienpy/version.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    23930 2024-02-02 14:32:44.000000 alienpy-1.6.0/alienpy/wb_api.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10963 2023-12-13 09:23:11.000000 alienpy-1.6.0/alienpy/wb_async.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    59144 2024-03-14 18:15:24.000000 alienpy-1.6.0/alienpy/xrd_core.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    26177 2024-03-15 15:04:15.000000 alienpy-1.6.0/alienpy/xrd_tools.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.036416 alienpy-1.6.0/alienpy.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10577 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1707 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/SOURCES.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/dependency_links.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)      828 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/entry_points.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/requires.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2024-03-15 15:06:07.000000 alienpy-1.6.0/alienpy.egg-info/top_level.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)       35 2023-05-09 12:41:38.000000 alienpy-1.6.0/compile
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2020-03-13 14:44:31.000000 alienpy-1.6.0/devs_add_gitconfig
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/examples/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      887 2023-07-03 12:53:56.000000 alienpy-1.6.0/examples/alien_cp.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1809 2022-09-25 23:31:15.000000 alienpy-1.6.0/examples/alien_cp_grid2grid.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1995 2023-05-09 12:41:38.000000 alienpy-1.6.0/examples/alien_download_root.C
--rwxrwxr-x   0 adrian    (1000) adrian    (1000)      890 2020-10-27 20:27:20.000000 alienpy-1.6.0/examples/alien_envelope
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1684 2022-09-25 23:31:15.000000 alienpy-1.6.0/examples/alien_macro_lowlevel.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-09-25 23:31:15.000000 alienpy-1.6.0/examples/alien_wbtime
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1555 2023-06-07 09:27:41.000000 alienpy-1.6.0/examples/alienpy_help_mkdoc.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     4600 2023-06-07 09:27:41.000000 alienpy-1.6.0/examples/app_template.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1364 2023-11-22 12:00:12.000000 alienpy-1.6.0/examples/ccdb_cpv_noise.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1410 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_cpv_pedestal.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1600 2023-11-22 12:00:12.000000 alienpy-1.6.0/examples/ccdb_cpv_pedestal_dcs_fee.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1271 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_its_thr.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1278 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_mch_calib.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1276 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_mft_noise.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1279 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_mid_calib.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1986 2024-01-31 13:47:49.000000 alienpy-1.6.0/examples/ccdb_run2time.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1295 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_tpc_laser.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1281 2023-06-30 17:47:21.000000 alienpy-1.6.0/examples/ccdb_tpc_pedestal.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1348 2023-11-22 12:00:12.000000 alienpy-1.6.0/examples/ccdb_tpc_pulser.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      845 2024-01-31 13:47:49.000000 alienpy-1.6.0/examples/extract_ccdb_paths.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      357 2022-09-25 23:31:15.000000 alienpy-1.6.0/examples/tokeninfo.C
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      216 2019-08-11 13:20:32.000000 alienpy-1.6.0/exec_package.txt
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/git-hooks/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      315 2023-05-09 12:41:38.000000 alienpy-1.6.0/git-hooks/post-commit
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      179 2023-05-09 12:41:38.000000 alienpy-1.6.0/git-hooks/pre-commit
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      143 2022-06-08 20:03:53.000000 alienpy-1.6.0/install_user
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      144 2022-06-08 20:03:53.000000 alienpy-1.6.0/install_user_dev
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      209 2019-08-11 12:01:54.000000 alienpy-1.6.0/minify_python.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      545 2023-05-09 12:41:38.000000 alienpy-1.6.0/pypi_build
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      123 2020-06-09 11:54:43.000000 alienpy-1.6.0/pypi_install_test
--rwxrwxr-x   0 adrian    (1000) adrian    (1000)       30 2020-06-11 10:12:10.000000 alienpy-1.6.0/pypi_upload
--rwxrwxr-x   0 adrian    (1000) adrian    (1000)       52 2020-06-11 10:12:18.000000 alienpy-1.6.0/pypi_upload_test
--rw-r--r--   0 adrian    (1000) adrian    (1000)      358 2023-06-07 09:27:41.000000 alienpy-1.6.0/pyrightconfig.json
--rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2023-05-09 12:41:38.000000 alienpy-1.6.0/requirements.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2024-03-15 15:06:07.036416 alienpy-1.6.0/setup.cfg
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3991 2024-03-15 11:42:24.000000 alienpy-1.6.0/setup.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      679 2023-05-09 12:41:38.000000 alienpy-1.6.0/tag
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/tests/
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/tests/001_exit_codes.test/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1172 2023-12-13 09:58:07.000000 alienpy-1.6.0/tests/001_exit_codes.test/test.sh
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/tests/002_env_tokens.test/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     1534 2023-12-13 10:26:48.000000 alienpy-1.6.0/tests/002_env_tokens.test/test.sh
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/tests/003_find.test/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      685 2024-03-14 18:15:24.000000 alienpy-1.6.0/tests/003_find.test/test.sh
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.035416 alienpy-1.6.0/tests/004_cp.test/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      643 2024-03-14 18:15:24.000000 alienpy-1.6.0/tests/004_cp.test/test.sh
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-03-15 15:06:07.036416 alienpy-1.6.0/tests/005_cp_dir.test/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2304 2024-03-14 18:15:24.000000 alienpy-1.6.0/tests/005_cp_dir.test/test.sh
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      788 2024-03-14 18:15:24.000000 alienpy-1.6.0/tests/run_tests
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)      372 2023-05-09 12:41:38.000000 alienpy-1.6.0/update_version
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-10 12:34:56.402435 alienpy-1.6.1/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.6.1/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10577 2024-04-10 12:34:56.402435 alienpy-1.6.1/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.6.1/README.md
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-10 12:34:56.401435 alienpy-1.6.1/alienpy/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       51 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/__init__.py
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)    94978 2024-04-10 12:31:53.000000 alienpy-1.6.1/alienpy/alien.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3100 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/async_tools.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    15688 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/connect_ssl.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5970 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/data_structs.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3909 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/global_vars.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1727 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/setup_cwd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2486 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/setup_logging.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1846 2024-04-05 08:25:10.000000 alienpy-1.6.1/alienpy/tools_history.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    48988 2024-04-05 08:25:10.000000 alienpy-1.6.1/alienpy/tools_nowb.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1866 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/tools_shell.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      897 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/tools_stackcmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2024-04-10 12:34:04.000000 alienpy-1.6.1/alienpy/version.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    23930 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/wb_api.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10963 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/wb_async.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    59144 2024-03-05 09:21:03.000000 alienpy-1.6.1/alienpy/xrd_core.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    26177 2024-03-05 09:18:27.000000 alienpy-1.6.1/alienpy/xrd_tools.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-10 12:34:56.402435 alienpy-1.6.1/alienpy.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10577 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      606 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      828 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/entry_points.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/requires.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2024-04-10 12:34:56.000000 alienpy-1.6.1/alienpy.egg-info/top_level.txt
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-10 12:34:56.402435 alienpy-1.6.1/examples/
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.6.1/examples/alien_wbtime
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2024-04-10 12:34:56.402435 alienpy-1.6.1/setup.cfg
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3991 2024-04-05 08:25:10.000000 alienpy-1.6.1/setup.py
```

### Comparing `alienpy-1.6.0/LICENSE` & `alienpy-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/PKG-INFO` & `alienpy-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.6.0
+Version: 1.6.1
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.6.0/README.md` & `alienpy-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/alien.py` & `alienpy-1.6.1/alienpy/alien.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #!/usr/bin/env python3
 """Executable/module for interaction with GRID services of ALICE experiment"""
 
+import ctypes
+try:
+    libgcc_s = ctypes.CDLL('libgcc_s.so.1')
+except Exception:
+    pass
+
 import os
 import sys
 if sys.version_info[0] < 3 or (sys.version_info[0] == 3 and sys.version_info[1] < 6):
     print("This packages requires a minimum of Python version 3.6", file = sys.stderr, flush = True)
     sys.exit(1)
 import collections
 import datetime
```

### Comparing `alienpy-1.6.0/alienpy/async_tools.py` & `alienpy-1.6.1/alienpy/async_tools.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/connect_ssl.py` & `alienpy-1.6.1/alienpy/connect_ssl.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/data_structs.py` & `alienpy-1.6.1/alienpy/data_structs.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/global_vars.py` & `alienpy-1.6.1/alienpy/global_vars.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/setup_cwd.py` & `alienpy-1.6.1/alienpy/setup_cwd.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/setup_logging.py` & `alienpy-1.6.1/alienpy/setup_logging.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/tools_history.py` & `alienpy-1.6.1/alienpy/tools_history.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/tools_nowb.py` & `alienpy-1.6.1/alienpy/tools_nowb.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/tools_shell.py` & `alienpy-1.6.1/alienpy/tools_shell.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/tools_stackcmd.py` & `alienpy-1.6.1/alienpy/tools_stackcmd.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/wb_api.py` & `alienpy-1.6.1/alienpy/wb_api.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/wb_async.py` & `alienpy-1.6.1/alienpy/wb_async.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/xrd_core.py` & `alienpy-1.6.1/alienpy/xrd_core.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy/xrd_tools.py` & `alienpy-1.6.1/alienpy/xrd_tools.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/alienpy.egg-info/PKG-INFO` & `alienpy-1.6.1/alienpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.6.0
+Version: 1.6.1
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.6.0/alienpy.egg-info/entry_points.txt` & `alienpy-1.6.1/alienpy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/examples/alien_wbtime` & `alienpy-1.6.1/examples/alien_wbtime`

 * *Files identical despite different names*

### Comparing `alienpy-1.6.0/setup.py` & `alienpy-1.6.1/setup.py`

 * *Files identical despite different names*

