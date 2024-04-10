# Comparing `tmp/virt-lightning-2.3.1.tar.gz` & `tmp/virt-lightning-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-lightning-2.3.1.tar", last modified: Thu Sep 28 13:05:14 2023, max compression
+gzip compressed data, was "virt-lightning-2.3.2.tar", last modified: Wed Apr 10 15:56:20 2024, max compression
```

## Comparing `virt-lightning-2.3.1.tar` & `virt-lightning-2.3.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.759925 virt-lightning-2.3.1/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.751925 virt-lightning-2.3.1/.github/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.753925 virt-lightning-2.3.1/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      836 2023-02-09 19:11:48.000000 virt-lightning-2.3.1/.github/workflows/codeql.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)      162 2023-04-19 20:57:19.000000 virt-lightning-2.3.1/.github/workflows/ruff.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1178 2023-09-28 00:01:39.000000 virt-lightning-2.3.1/.github/workflows/tests.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)      643 2023-04-22 22:23:27.000000 virt-lightning-2.3.1/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)      933 2023-09-22 15:10:12.000000 virt-lightning-2.3.1/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11358 2022-03-13 22:53:30.000000 virt-lightning-2.3.1/LICENSE-2.0.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       97 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9678 2023-09-28 13:05:14.759925 virt-lightning-2.3.1/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     8926 2023-09-28 00:01:39.000000 virt-lightning-2.3.1/README.md
--rw-r--r--   0 goneri    (1002) goneri    (1002)     3505 2023-09-28 00:08:57.000000 virt-lightning-2.3.1/changelog.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.753925 virt-lightning-2.3.1/conf/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2022-03-13 22:53:30.000000 virt-lightning-2.3.1/conf/example.ini
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.754925 virt-lightning-2.3.1/logo/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    19245 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/logo/logo.png
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13991 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/logo/logo.svg
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11483 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/logo/logo_no_text.png
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1583 2023-04-22 22:19:39.000000 virt-lightning-2.3.1/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       28 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/requirements.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-09-28 13:05:14.759925 virt-lightning-2.3.1/setup.cfg
--rw-r--r--   0 goneri    (1002) goneri    (1002)      419 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/test-requirements.txt
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.754925 virt-lightning-2.3.1/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1860 2023-04-19 21:06:34.000000 virt-lightning-2.3.1/tests/conftest.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      924 2023-04-19 21:06:34.000000 virt-lightning-2.3.1/tests/test_configure.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      734 2023-04-19 20:24:56.000000 virt-lightning-2.3.1/tests/test_domain.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2445 2023-04-19 20:58:26.000000 virt-lightning-2.3.1/tests/test_hv.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.754925 virt-lightning-2.3.1/tools/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      202 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/tools/release
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1044 2023-04-22 23:01:48.000000 virt-lightning-2.3.1/tox.ini
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.755925 virt-lightning-2.3.1/virt-lightning.org/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1428 2023-09-01 17:31:02.000000 virt-lightning-2.3.1/virt-lightning.org/bench_images_startup.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.751925 virt-lightning-2.3.1/virt-lightning.org/etc/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.751925 virt-lightning-2.3.1/virt-lightning.org/etc/caddy/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.755925 virt-lightning-2.3.1/virt-lightning.org/etc/caddy/conf.d/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    18981 2023-09-01 17:31:02.000000 virt-lightning-2.3.1/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf
--rwxr-xr-x   0 goneri    (1002) goneri    (1002)      252 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/virt-lightning.org/update.sh
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.751925 virt-lightning-2.3.1/virt-lightning.org/www/
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.755925 virt-lightning-2.3.1/virt-lightning.org/www/images/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1009 2023-09-01 17:31:02.000000 virt-lightning-2.3.1/virt-lightning.org/www/images/index.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.757925 virt-lightning-2.3.1/virt_lightning/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      101 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/virt_lightning/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    17120 2023-04-22 22:19:34.000000 virt-lightning-2.3.1/virt_lightning/api.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2354 2023-09-01 17:31:02.000000 virt-lightning-2.3.1/virt_lightning/configuration.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13385 2023-09-22 15:10:12.000000 virt-lightning-2.3.1/virt_lightning/shell.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      642 2022-07-14 16:24:35.000000 virt-lightning-2.3.1/virt_lightning/symbols.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2953 2023-04-19 20:38:48.000000 virt-lightning-2.3.1/virt_lightning/templates.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1313 2023-02-09 19:11:20.000000 virt-lightning-2.3.1/virt_lightning/ui.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      274 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning/version.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    34700 2023-09-22 15:10:12.000000 virt-lightning-2.3.1/virt_lightning/virt_lightning.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-09-28 13:05:14.758925 virt-lightning-2.3.1/virt_lightning.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9678 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1034 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       92 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       40 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       15 2023-09-28 13:05:14.000000 virt-lightning-2.3.1/virt_lightning.egg-info/top_level.txt
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.757869 virt-lightning-2.3.2/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.749869 virt-lightning-2.3.2/.github/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.751869 virt-lightning-2.3.2/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      836 2023-02-09 19:11:48.000000 virt-lightning-2.3.2/.github/workflows/codeql.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      162 2023-04-19 20:57:19.000000 virt-lightning-2.3.2/.github/workflows/ruff.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1178 2023-09-28 00:01:39.000000 virt-lightning-2.3.2/.github/workflows/tests.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      643 2024-04-10 15:40:08.000000 virt-lightning-2.3.2/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      933 2023-09-22 15:10:12.000000 virt-lightning-2.3.2/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11358 2022-03-13 22:53:30.000000 virt-lightning-2.3.2/LICENSE-2.0.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       97 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9620 2024-04-10 15:56:20.757869 virt-lightning-2.3.2/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     8876 2023-12-07 15:51:15.000000 virt-lightning-2.3.2/README.md
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     3771 2024-04-10 15:05:07.000000 virt-lightning-2.3.2/changelog.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.751869 virt-lightning-2.3.2/conf/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2022-03-13 22:53:30.000000 virt-lightning-2.3.2/conf/example.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.752869 virt-lightning-2.3.2/logo/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    19245 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/logo/logo.png
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13991 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/logo/logo.svg
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11483 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/logo/logo_no_text.png
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1575 2023-12-07 15:51:15.000000 virt-lightning-2.3.2/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       28 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/requirements.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2024-04-10 15:56:20.757869 virt-lightning-2.3.2/setup.cfg
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      419 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/test-requirements.txt
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.752869 virt-lightning-2.3.2/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1860 2023-04-19 21:06:34.000000 virt-lightning-2.3.2/tests/conftest.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      924 2023-04-19 21:06:34.000000 virt-lightning-2.3.2/tests/test_configure.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      734 2023-04-19 20:24:56.000000 virt-lightning-2.3.2/tests/test_domain.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2445 2023-04-19 20:58:26.000000 virt-lightning-2.3.2/tests/test_hv.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1514 2024-04-10 14:26:28.000000 virt-lightning-2.3.2/tests/test_util.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.752869 virt-lightning-2.3.2/tools/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      202 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/tools/release
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1070 2024-04-10 15:40:08.000000 virt-lightning-2.3.2/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.753869 virt-lightning-2.3.2/virt-lightning.org/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1414 2024-04-10 14:26:28.000000 virt-lightning-2.3.2/virt-lightning.org/bench_images_startup.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.749869 virt-lightning-2.3.2/virt-lightning.org/etc/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.749869 virt-lightning-2.3.2/virt-lightning.org/etc/caddy/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.753869 virt-lightning-2.3.2/virt-lightning.org/etc/caddy/conf.d/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    19145 2023-12-07 15:51:15.000000 virt-lightning-2.3.2/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf
+-rwxr-xr-x   0 goneri    (1002) goneri    (1002)      252 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/virt-lightning.org/update.sh
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.749869 virt-lightning-2.3.2/virt-lightning.org/www/
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.753869 virt-lightning-2.3.2/virt-lightning.org/www/images/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1021 2023-12-07 15:51:15.000000 virt-lightning-2.3.2/virt-lightning.org/www/images/index.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.755869 virt-lightning-2.3.2/virt_lightning/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      101 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/virt_lightning/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    17119 2024-04-10 14:17:18.000000 virt-lightning-2.3.2/virt_lightning/api.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2354 2023-09-01 17:31:02.000000 virt-lightning-2.3.2/virt_lightning/configuration.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13341 2024-04-10 14:26:28.000000 virt-lightning-2.3.2/virt_lightning/shell.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      642 2022-07-14 16:24:35.000000 virt-lightning-2.3.2/virt_lightning/symbols.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2953 2023-12-07 15:51:07.000000 virt-lightning-2.3.2/virt_lightning/templates.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1313 2023-02-09 19:11:20.000000 virt-lightning-2.3.2/virt_lightning/ui.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      734 2024-04-10 14:17:18.000000 virt-lightning-2.3.2/virt_lightning/util.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      411 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning/version.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    34854 2024-04-10 14:17:18.000000 virt-lightning-2.3.2/virt_lightning/virt_lightning.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2024-04-10 15:56:20.756869 virt-lightning-2.3.2/virt_lightning.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9620 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1076 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       92 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       40 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       15 2024-04-10 15:56:20.000000 virt-lightning-2.3.2/virt_lightning.egg-info/top_level.txt
```

### Comparing `virt-lightning-2.3.1/.github/workflows/codeql.yml` & `virt-lightning-2.3.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/.github/workflows/tests.yml` & `virt-lightning-2.3.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/.github/workflows/tox.yml` & `virt-lightning-2.3.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/.gitignore` & `virt-lightning-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/LICENSE-2.0.txt` & `virt-lightning-2.3.2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/PKG-INFO` & `virt-lightning-2.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: virt-lightning
-Version: 2.3.1
+Version: 2.3.2
 Summary: Deploy your testing VM in a couple of seconds
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
-Project-URL: Homepage, https://https://virt-lightning.org/
+Project-URL: Homepage, https://virt-lightning.org/
 Project-URL: Source, https://github.com/virt-lightning/virt-lightning
 Keywords: libvirt,cloud,qemu,cloudinit
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
@@ -55,32 +55,40 @@
 1. use the list of distribution to generate a virt-lightning.yaml file.
 2. we then create a environment based on this file
 3. once the environment is ready, we generate an Ansible inventory file
 4. and we use it to call Ansible's ping module on all the host.
 
 [![demo](https://asciinema.org/a/230671.svg)](https://asciinema.org/a/230671?autoplay=1)
 
-## Pre-requirements
 
-- Python 3.8 or greater.
-- The Python3 binding for libvirt, the package is probably called `python3-libvirt`.
-- You can also just build the binding during the install, in this case, you will need to install some packages first:
-    - `dnf install libvirt-devel python3-devel` (Fedora/RHEL)
-    - `apt install libvirt-dev python3-dev` (Debian/Ubuntu)
-- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+## Requirements
+- Python 3.8 or greater
+- The Python3 binding for libvirt, the package is probably called `python3-libvirt` or 'libvirt-python' according to pip.
 - Libvirt must be running, most of the time you just need to run: `sudo systemctl start --now libvirtd`
 - Finally, be sure your user can access the system libvirt daemon, e.g with: `virsh -c qemu:///system`
 
-## Installation
+## Optional
+- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+
 
+## Installation (Fedora/RHEL)
 ```shell
-pip3 install --user virt-lightning
+sudo dnf install libvirt-devel gcc python3-devel pipx
+pipx ensurepath
+pipx install virt-lightning
 ```
 
-If you use Ubuntu, you will need the `--no-deps` argument (See: https://github.com/pypa/pip/issues/4222).
+## Installation (Debian/Ubuntu)
+```shell
+sudo apt install python3-venv pkg-config gcc libvirt-dev python3-dev pipx
+pipx ensurepath
+pipx install virt-lightning
+```
+
+## Post Installation
 
 `virt-lightning` will be installed in ~/.local/bin/. Add it in your `$PATH` if
 it's not already the case. For instance if you use:
 
 ```shell
 echo "export PATH=$PATH:~/.local/bin/" >> ~/.bashrc
 source ~/.bashrc
@@ -268,21 +276,21 @@
 # create second snapshot
 virsh snapshot-create-as --domain vm_name --name snapshot_2
 # validate that both of them were saved
 virsh snapshot-list vm_name
 # and revert to the first one
 virsh snapshot-revert vm_name --snapshotname snapshot_1
 ```
-=======
+
 ### Development
 install libvirt-dev package:
 
 Debian/Ubuntu:
 ```shell
-apt-get install python3-venv python3-dev pkg-config gcc libvirt-dev
+apt install python3-venv pkg-config gcc libvirt-dev python3-dev
 ```
 
 Fedora/RHEL:
 ```shell
 dnf install python3-devel gcc libvirt-devel
 ```
```

### Comparing `virt-lightning-2.3.1/README.md` & `virt-lightning-2.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,32 +34,40 @@
 1. use the list of distribution to generate a virt-lightning.yaml file.
 2. we then create a environment based on this file
 3. once the environment is ready, we generate an Ansible inventory file
 4. and we use it to call Ansible's ping module on all the host.
 
 [![demo](https://asciinema.org/a/230671.svg)](https://asciinema.org/a/230671?autoplay=1)
 
-## Pre-requirements
 
-- Python 3.8 or greater.
-- The Python3 binding for libvirt, the package is probably called `python3-libvirt`.
-- You can also just build the binding during the install, in this case, you will need to install some packages first:
-    - `dnf install libvirt-devel python3-devel` (Fedora/RHEL)
-    - `apt install libvirt-dev python3-dev` (Debian/Ubuntu)
-- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+## Requirements
+- Python 3.8 or greater
+- The Python3 binding for libvirt, the package is probably called `python3-libvirt` or 'libvirt-python' according to pip.
 - Libvirt must be running, most of the time you just need to run: `sudo systemctl start --now libvirtd`
 - Finally, be sure your user can access the system libvirt daemon, e.g with: `virsh -c qemu:///system`
 
-## Installation
+## Optional
+- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+
 
+## Installation (Fedora/RHEL)
 ```shell
-pip3 install --user virt-lightning
+sudo dnf install libvirt-devel gcc python3-devel pipx
+pipx ensurepath
+pipx install virt-lightning
 ```
 
-If you use Ubuntu, you will need the `--no-deps` argument (See: https://github.com/pypa/pip/issues/4222).
+## Installation (Debian/Ubuntu)
+```shell
+sudo apt install python3-venv pkg-config gcc libvirt-dev python3-dev pipx
+pipx ensurepath
+pipx install virt-lightning
+```
+
+## Post Installation
 
 `virt-lightning` will be installed in ~/.local/bin/. Add it in your `$PATH` if
 it's not already the case. For instance if you use:
 
 ```shell
 echo "export PATH=$PATH:~/.local/bin/" >> ~/.bashrc
 source ~/.bashrc
@@ -247,21 +255,21 @@
 # create second snapshot
 virsh snapshot-create-as --domain vm_name --name snapshot_2
 # validate that both of them were saved
 virsh snapshot-list vm_name
 # and revert to the first one
 virsh snapshot-revert vm_name --snapshotname snapshot_1
 ```
-=======
+
 ### Development
 install libvirt-dev package:
 
 Debian/Ubuntu:
 ```shell
-apt-get install python3-venv python3-dev pkg-config gcc libvirt-dev
+apt install python3-venv pkg-config gcc libvirt-dev python3-dev
 ```
 
 Fedora/RHEL:
 ```shell
 dnf install python3-devel gcc libvirt-devel
 ```
```

### Comparing `virt-lightning-2.3.1/changelog.md` & `virt-lightning-2.3.2/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# 2.3.2
+
+- Fixed error message for missing genisoimage
+- Remove and replace distutils.util.strtobool
+- Enabled Python 3.12 for tests
+- Add fedora-39 image
+- Remove duplicate protocol from Homepage URL
+- Update Readme installation instructions for Debian to use pip
+
 # 2.3.1
 
 - Renamed Tox env name in GH Actions job
 - README: explain how to install the dep to build the Python binding
 - clean up ruff errors, convert string.format calls to f-strings (#279)
 - remove debian-testing image, link nolonger exists, and was based on debian-10 add debian-12 image add debian-sid
 - Update README with snapshots example
```

### Comparing `virt-lightning-2.3.1/logo/logo.png` & `virt-lightning-2.3.2/logo/logo.png`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/logo/logo.svg` & `virt-lightning-2.3.2/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/logo/logo_no_text.png` & `virt-lightning-2.3.2/logo/logo_no_text.png`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/pyproject.toml` & `virt-lightning-2.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
         "Operating System :: POSIX :: Linux",
 ]
 dynamic = ["dependencies", "version"]
 keywords = ["libvirt", "cloud", "qemu", "cloudinit"]
 
 [project.urls]
-Homepage = "https://https://virt-lightning.org/"
+Homepage = "https://virt-lightning.org/"
 Source = "https://github.com/virt-lightning/virt-lightning"
 
 [project.optional-dependencies]
 test = [
     "tox",
 ]
```

### Comparing `virt-lightning-2.3.1/tests/conftest.py` & `virt-lightning-2.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/tests/test_configure.py` & `virt-lightning-2.3.2/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/tests/test_domain.py` & `virt-lightning-2.3.2/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/tests/test_hv.py` & `virt-lightning-2.3.2/tests/test_hv.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/tox.ini` & `virt-lightning-2.3.2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [tox]
-envlist = flake8,py39,py310,py311,black
+envlist = flake8,py39,py310,py311,py312,black
+isolated_build=True
 
 [gh-actions]
 python =
     3.9: py39
     3.10: py310
     3.11: py311, flake8, black
```

### Comparing `virt-lightning-2.3.1/virt-lightning.org/bench_images_startup.py` & `virt-lightning-2.3.2/virt-lightning.org/bench_images_startup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,10 +44,8 @@
             distro=distro,
             enable_console=True,
             console_fd=my_fd,
         )
         elapsed_time = time.time() - start_time
         sum += elapsed_time
         print(f"- elapsed_time={elapsed_time:06.2f}")
-    print(
-        f"FINAL distro={distro}: {sum / number_of_runs}"
-    )
+    print(f"FINAL distro={distro}: {sum / number_of_runs}")
```

### Comparing `virt-lightning-2.3.1/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf` & `virt-lightning-2.3.2/virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,23 @@
     redir /images/fedora-32/fedora-32.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/32/Cloud/x86_64/images/Fedora-Cloud-Base-32-1.6.x86_64.qcow2
     redir /images/fedora-33/fedora-33.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/33/Cloud/x86_64/images/Fedora-Cloud-Base-33-1.2.x86_64.qcow2
     redir /images/fedora-34/fedora-34.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/34/Cloud/x86_64/images/Fedora-Cloud-Base-34-1.2.x86_64.qcow2
     redir /images/fedora-35/fedora-35.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/35/Cloud/x86_64/images/Fedora-Cloud-Base-35-1.2.x86_64.qcow2
     redir /images/fedora-36/fedora-36.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/36/Cloud/x86_64/images/Fedora-Cloud-Base-36-1.5.x86_64.qcow2
     redir /images/fedora-37/fedora-37.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/37/Cloud/x86_64/images/Fedora-Cloud-Base-37-1.7.x86_64.qcow2
     redir /images/fedora-38/fedora-38.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/38/Cloud/x86_64/images/Fedora-Cloud-Base-38-1.6.x86_64.qcow2
+    redir /images/fedora-39/fedora-39.qcow2 https://download.fedoraproject.org/pub/fedora/linux/releases/39/Cloud/x86_64/images/Fedora-Cloud-Base-39-1.5.x86_64.qcow2
 
     # Debian
     redir /images/debian-9/debian-9.qcow2 https://cdimage.debian.org/cdimage/openstack/current-9/debian-9-openstack-amd64.qcow2
     redir /images/debian-10/debian-10.qcow2 https://cdimage.debian.org/cdimage/openstack/current-10/debian-10-openstack-amd64.qcow2
     redir /images/debian-11/debian-11.qcow2 https://cdimage.debian.org/cdimage/cloud/bullseye/latest/debian-11-generic-amd64.qcow2
     redir /images/debian-12/debian-12.qcow2 https://cdimage.debian.org/cdimage/cloud/bookworm/latest/debian-12-generic-amd64.qcow2
     redir /images/debian-sid/debian-sid.qcow2 https://cdimage.debian.org/cdimage/cloud/sid/daily/latest/debian-sid-generic-amd64-daily.qcow2
 
-
-
     # CentOS
     redir /images/centos-7/centos-7.qcow2 http://cloud.centos.org/centos/7/images/CentOS-7-x86_64-GenericCloud.qcow2
     redir /images/centos-6/centos-6.qcow2 https://cloud.centos.org/centos/6/images/CentOS-6-x86_64-GenericCloud.qcow2
     redir /images/centos-8/centos-8.qcow2 https://cloud.centos.org/centos/8/x86_64/images/CentOS-8-GenericCloud-8.1.1911-20200113.3.x86_64.qcow2
     redir /images/centos-8-stream/centos-8-stream.qcow2 https://cloud.centos.org/centos/8-stream/x86_64/images/CentOS-Stream-GenericCloud-8-20220125.1.x86_64.qcow2
     redir /images/centos-9-stream/centos-9-stream.qcow2 https://cloud.centos.org/centos/9-stream/x86_64/images/CentOS-Stream-GenericCloud-9-20220330.1.x86_64.qcow2
```

### Comparing `virt-lightning-2.3.1/virt-lightning.org/www/images/index.md` & `virt-lightning-2.3.2/virt-lightning.org/www/images/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 - fedora-32
 - fedora-33
 - fedora-34
 - fedora-35
 - fedora-36
 - fedora-37
 - fedora-38
+- fedora-39
 - freebsd-11.4
 - freebsd-12.1
 - freebsd-12.2
 - freebsd-13.0-ufs
 - freebsd-13.0-zfs
 - freebsd-13.2-ufs
 - freebsd-13.2-zfs
```

### Comparing `virt-lightning-2.3.1/virt_lightning/api.py` & `virt-lightning-2.3.2/virt_lightning/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 
 import asyncio
 import collections
-import distutils.util
 import ipaddress
 import logging
 import pathlib
 import re
 import sys
 import urllib.request
 from concurrent.futures import ThreadPoolExecutor
 
 import libvirt
 
 import virt_lightning.virt_lightning as vl
 from virt_lightning.configuration import Configuration
 from virt_lightning.symbols import get_symbols
+from virt_lightning.util import strtobool
 
 BASE_URL = "https://virt-lightning.org"
 
 logger = logging.getLogger("virt_lightning")
 
 
 def libvirt_callback(userdata, err):
@@ -416,15 +416,15 @@
     hv.init_storage_pool(configuration.storage_pool)
     for domain in hv.list_domains():
         if domain.context != context:
             continue
         logger.info("%s purging %s", symbols.TRASHBIN.value, domain.name)
         hv.clean_up(domain)
 
-    if bool(distutils.util.strtobool(configuration.network_auto_clean_up)):
+    if strtobool(configuration.network_auto_clean_up):
         hv.network_obj.destroy()
 
 
 def distro_list(configuration, **kwargs):
     """Return a list of VM images that are available on the system."""
     conn = _connect_libvirt(configuration.libvirt_uri)
     hv = vl.LibvirtHypervisor(conn)
```

### Comparing `virt-lightning-2.3.1/virt_lightning/configuration.py` & `virt-lightning-2.3.2/virt_lightning/configuration.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/virt_lightning/shell.py` & `virt-lightning-2.3.2/virt_lightning/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,17 @@
         go_viewer(hv.get_domain_by_name(name))
 
     ui.Selector(sorted(hv.list_domains()), go_viewer)
 
 
 def progress_callback(cur, length):
     percent = (cur * 100) / length
-    line = "🌍 ➡️  💻 [{percent:06.2f}%]  {done:6}MB/{full}MB\r".format(
-        percent=percent,
-        done=int(cur / virt_lightning.api.MB),
-        full=int(length / virt_lightning.api.MB),
-    )
+    done = int(cur / virt_lightning.api.MB)
+    full = int(length / virt_lightning.api.MB)
+    line = f"🌍 ➡️  💻 [{percent:06.2f}%]  {done:6}MB/{full}MB\r"
     print(line, end="")  # noqa: T001
 
 
 def list_from_yaml_file(value):
     file_path = pathlib.PosixPath(value)
     if not file_path.exists():
         raise argparse.ArgumentTypeError(f"{value} does not exist.")
```

### Comparing `virt-lightning-2.3.1/virt_lightning/symbols.py` & `virt-lightning-2.3.2/virt_lightning/symbols.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/virt_lightning/templates.py` & `virt-lightning-2.3.2/virt_lightning/templates.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/virt_lightning/ui.py` & `virt-lightning-2.3.2/virt_lightning/ui.py`

 * *Files identical despite different names*

### Comparing `virt-lightning-2.3.1/virt_lightning/virt_lightning.py` & `virt-lightning-2.3.2/virt_lightning/virt_lightning.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,20 @@
     def iso_binary(self):
         paths = [pathlib.PosixPath(i) for i in os.environ["PATH"].split(os.pathsep)]
         for i in paths:
             for binary in ISO_BINARIES:
                 exe = i / binary
                 if exe.exists():
                     return exe
-        raise Exception("Failed to find %s in %s", ":".join(ISO_BINARIES), paths)
+        error_msg = (
+            f"Failed to find {' or '.join(ISO_BINARIES)} in "
+            f"{', '.join([x.as_posix() for x in paths])} "
+            "\nPlease install genisoimage tool"
+        )
+        raise Exception(error_msg)
 
     def init_network(self, network_name, network_cidr):
         try:
             self.network_obj = self.conn.networkLookupByName(network_name)
         except libvirt.libvirtError as e:
             if e.get_error_code() != libvirt.VIR_ERR_NO_NETWORK:
                 raise (e)
```

### Comparing `virt-lightning-2.3.1/virt_lightning.egg-info/PKG-INFO` & `virt-lightning-2.3.2/virt_lightning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: virt-lightning
-Version: 2.3.1
+Version: 2.3.2
 Summary: Deploy your testing VM in a couple of seconds
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
-Project-URL: Homepage, https://https://virt-lightning.org/
+Project-URL: Homepage, https://virt-lightning.org/
 Project-URL: Source, https://github.com/virt-lightning/virt-lightning
 Keywords: libvirt,cloud,qemu,cloudinit
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
@@ -55,32 +55,40 @@
 1. use the list of distribution to generate a virt-lightning.yaml file.
 2. we then create a environment based on this file
 3. once the environment is ready, we generate an Ansible inventory file
 4. and we use it to call Ansible's ping module on all the host.
 
 [![demo](https://asciinema.org/a/230671.svg)](https://asciinema.org/a/230671?autoplay=1)
 
-## Pre-requirements
 
-- Python 3.8 or greater.
-- The Python3 binding for libvirt, the package is probably called `python3-libvirt`.
-- You can also just build the binding during the install, in this case, you will need to install some packages first:
-    - `dnf install libvirt-devel python3-devel` (Fedora/RHEL)
-    - `apt install libvirt-dev python3-dev` (Debian/Ubuntu)
-- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+## Requirements
+- Python 3.8 or greater
+- The Python3 binding for libvirt, the package is probably called `python3-libvirt` or 'libvirt-python' according to pip.
 - Libvirt must be running, most of the time you just need to run: `sudo systemctl start --now libvirtd`
 - Finally, be sure your user can access the system libvirt daemon, e.g with: `virsh -c qemu:///system`
 
-## Installation
+## Optional
+- You make also want to install `python3-urwid` if you want to get the fancy list of VM. This dependency is optional.
+
 
+## Installation (Fedora/RHEL)
 ```shell
-pip3 install --user virt-lightning
+sudo dnf install libvirt-devel gcc python3-devel pipx
+pipx ensurepath
+pipx install virt-lightning
 ```
 
-If you use Ubuntu, you will need the `--no-deps` argument (See: https://github.com/pypa/pip/issues/4222).
+## Installation (Debian/Ubuntu)
+```shell
+sudo apt install python3-venv pkg-config gcc libvirt-dev python3-dev pipx
+pipx ensurepath
+pipx install virt-lightning
+```
+
+## Post Installation
 
 `virt-lightning` will be installed in ~/.local/bin/. Add it in your `$PATH` if
 it's not already the case. For instance if you use:
 
 ```shell
 echo "export PATH=$PATH:~/.local/bin/" >> ~/.bashrc
 source ~/.bashrc
@@ -268,21 +276,21 @@
 # create second snapshot
 virsh snapshot-create-as --domain vm_name --name snapshot_2
 # validate that both of them were saved
 virsh snapshot-list vm_name
 # and revert to the first one
 virsh snapshot-revert vm_name --snapshotname snapshot_1
 ```
-=======
+
 ### Development
 install libvirt-dev package:
 
 Debian/Ubuntu:
 ```shell
-apt-get install python3-venv python3-dev pkg-config gcc libvirt-dev
+apt install python3-venv pkg-config gcc libvirt-dev python3-dev
 ```
 
 Fedora/RHEL:
 ```shell
 dnf install python3-devel gcc libvirt-devel
 ```
```

### Comparing `virt-lightning-2.3.1/virt_lightning.egg-info/SOURCES.txt` & `virt-lightning-2.3.2/virt_lightning.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 logo/logo.png
 logo/logo.svg
 logo/logo_no_text.png
 tests/conftest.py
 tests/test_configure.py
 tests/test_domain.py
 tests/test_hv.py
+tests/test_util.py
 tools/release
 virt-lightning.org/bench_images_startup.py
 virt-lightning.org/update.sh
 virt-lightning.org/etc/caddy/conf.d/virt-lightning.org.conf
 virt-lightning.org/www/images/index.md
 virt_lightning/__init__.py
 virt_lightning/api.py
 virt_lightning/configuration.py
 virt_lightning/shell.py
 virt_lightning/symbols.py
 virt_lightning/templates.py
 virt_lightning/ui.py
+virt_lightning/util.py
 virt_lightning/version.py
 virt_lightning/virt_lightning.py
 virt_lightning.egg-info/PKG-INFO
 virt_lightning.egg-info/SOURCES.txt
 virt_lightning.egg-info/dependency_links.txt
 virt_lightning.egg-info/entry_points.txt
 virt_lightning.egg-info/requires.txt
```

