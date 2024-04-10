# Comparing `tmp/ft-drift-0.0.1.tar.gz` & `tmp/ft-drift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-drift-0.0.1.tar", last modified: Wed Apr 10 06:55:58 2024, max compression
+gzip compressed data, was "ft-drift-0.0.2.tar", last modified: Wed Apr 10 07:17:31 2024, max compression
```

## Comparing `ft-drift-0.0.1.tar` & `ft-drift-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 06:55:58.525018 ft-drift-0.0.1/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.1/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.1/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1000 2024-04-10 06:55:58.524804 ft-drift-0.0.1/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      224 2024-04-10 04:56:45.000000 ft-drift-0.0.1/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 06:55:58.523595 ft-drift-0.0.1/ft_drift/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/cli.py
--rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/compare_funcs.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.1/ft_drift/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/model.py
--rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 06:37:39.000000 ft-drift-0.0.1/ft_drift/parse.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 06:55:58.524626 ft-drift-0.0.1/ft_drift.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1000 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.1/ft_drift.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       49 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 06:55:58.000000 ft-drift-0.0.1/ft_drift.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)     1009 2024-04-10 06:21:51.000000 ft-drift-0.0.1/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 06:55:58.525067 ft-drift-0.0.1/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.1/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.440532 ft-drift-0.0.2/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ft-drift-0.0.2/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ft-drift-0.0.2/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:31.440323 ft-drift-0.0.2/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1002 2024-04-10 07:16:58.000000 ft-drift-0.0.2/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.439080 ft-drift-0.0.2/ft_drift/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2222 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/cli.py
+-rw-r--r--   0 hamel      (501) staff       (20)     3999 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/compare_funcs.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2024-04-09 05:05:40.000000 ft-drift-0.0.2/ft_drift/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2094 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/model.py
+-rw-r--r--   0 hamel      (501) staff       (20)     2166 2024-04-10 07:17:23.000000 ft-drift-0.0.2/ft_drift/parse.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2024-04-10 07:17:31.440140 ft-drift-0.0.2/ft_drift.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1778 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      412 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       90 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2024-04-09 05:22:09.000000 ft-drift-0.0.2/ft_drift.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       54 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2024-04-10 07:17:31.000000 ft-drift-0.0.2/ft_drift.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      904 2024-04-10 07:17:23.000000 ft-drift-0.0.2/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2024-04-10 07:17:31.440580 ft-drift-0.0.2/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ft-drift-0.0.2/setup.py
```

### Comparing `ft-drift-0.0.1/LICENSE` & `ft-drift-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/ft_drift/_modidx.py` & `ft-drift-0.0.2/ft_drift/_modidx.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/ft_drift/cli.py` & `ft-drift-0.0.2/ft_drift/cli.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/ft_drift/compare_funcs.py` & `ft-drift-0.0.2/ft_drift/compare_funcs.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/ft_drift/model.py` & `ft-drift-0.0.2/ft_drift/model.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/ft_drift/parse.py` & `ft-drift-0.0.2/ft_drift/parse.py`

 * *Files identical despite different names*

### Comparing `ft-drift-0.0.1/settings.ini` & `ft-drift-0.0.2/settings.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = ft-drift
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = ft-drift
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
-
-### nbdev ###
 doc_path = _docs
 lib_path = ft_drift
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://hamelsmu.github.io
+doc_baseurl = /ft-drift
+git_url = https://github.com/hamelsmu/ft-drift
+title = ft-drift
 audience = Developers
 author = Hamel Husain
 author_email = hamel.husain@gmail.com
-copyright = 2024 onwards, %(author)s
+copyright = 2024 onwards, Hamel Husain
 description = Check for data drift with OAI data
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = hamelsmu
+requirements = pandas rich openai>=1.12.0 scikit-learn>=1.4.1
+console_scripts = detect_drift=ft_drift.cli:main
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
 
-### Optional ###
-requirements = pandas openai>=1.12.0 scikit-learn>=1.4.1
-# dev_requirements =
-console_scripts = detect_drift=ft_drift.cli:main
```

### Comparing `ft-drift-0.0.1/setup.py` & `ft-drift-0.0.2/setup.py`

 * *Files identical despite different names*

