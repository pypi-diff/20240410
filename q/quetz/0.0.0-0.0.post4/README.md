# Comparing `tmp/quetz-0.0.0.tar.gz` & `tmp/quetz-0.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\quetz-0.0.0.tar", last modified: Tue Jun  9 11:35:31 2020, max compression
+gzip compressed data, was "quetz-0.0.post4.tar", last modified: Wed Apr 10 11:25:58 2024, max compression
```

## Comparing `quetz-0.0.0.tar` & `quetz-0.0.post4.tar`

### file list

```diff
@@ -1,12 +1,49 @@
-drwxrwxrwx   0        0        0        0 2020-06-09 11:35:31.000000 quetz-0.0.0/
--rw-rw-rw-   0        0        0      499 2020-06-09 11:35:31.000000 quetz-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       87 2020-06-09 10:10:58.000000 quetz-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz/
--rw-rw-rw-   0        0        0      120 2020-06-09 11:34:57.000000 quetz-0.0.0/quetz/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz.egg-info/
--rw-rw-rw-   0        0        0      499 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2020-06-09 11:35:31.000000 quetz-0.0.0/quetz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-09 11:35:31.000000 quetz-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      849 2020-06-09 11:35:04.000000 quetz-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:58.018711 quetz-0.0.post4/
+-rw-rw-rw-   0        0        0       85 2024-04-10 11:23:04.000000 quetz-0.0.post4/.gitattributes
+-rw-rw-rw-   0        0        0     2017 2023-12-20 14:44:42.000000 quetz-0.0.post4/.gitignore
+-rw-rw-rw-   0        0        0     1121 2023-12-20 14:47:16.000000 quetz-0.0.post4/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    27030 2022-10-03 09:02:20.000000 quetz-0.0.post4/LICENSE
+-rw-rw-rw-   0        0        0    36663 2024-04-10 11:25:58.014713 quetz-0.0.post4/PKG-INFO
+-rw-rw-rw-   0        0        0     4543 2024-04-10 11:21:51.000000 quetz-0.0.post4/README.rst
+-rw-rw-rw-   0        0        0    22821 2024-02-23 00:48:41.000000 quetz-0.0.post4/autodoc_typehints.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:57.816854 quetz-0.0.post4/docs/
+-rw-rw-rw-   0        0        0      660 2021-12-28 15:57:54.000000 quetz-0.0.post4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:57.831845 quetz-0.0.post4/docs/api/
+-rw-rw-rw-   0        0        0      225 2021-12-29 16:43:15.000000 quetz-0.0.post4/docs/api/PACKAGE_NAME.SCRIPT_MODULE_NAME.rst
+-rw-rw-rw-   0        0        0       60 2021-12-29 16:43:15.000000 quetz-0.0.post4/docs/api/PACKAGE_NAME.rst
+-rw-rw-rw-   0        0        0       82 2024-04-10 08:56:22.000000 quetz-0.0.post4/docs/api-toc.rst
+-rw-rw-rw-   0        0        0        4 2023-12-20 15:27:17.000000 quetz-0.0.post4/docs/autodoc-type-aliases.json
+-rw-rw-rw-   0        0        0     4711 2024-04-10 08:56:22.000000 quetz-0.0.post4/docs/conf.py
+-rw-rw-rw-   0        0        0      350 2024-04-10 08:56:22.000000 quetz-0.0.post4/docs/getting-started.rst
+-rw-rw-rw-   0        0        0      327 2024-04-10 08:56:22.000000 quetz-0.0.post4/docs/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:57.944829 quetz-0.0.post4/docs/intersphinx/
+-rw-rw-rw-   0        0        0   105583 2023-12-12 14:45:21.000000 quetz-0.0.post4/docs/intersphinx/matplotlib-objects.inv
+-rw-rw-rw-   0        0        0    51830 2023-12-12 14:44:58.000000 quetz-0.0.post4/docs/intersphinx/networkx-objects.inv
+-rw-rw-rw-   0        0        0    78006 2023-12-12 14:42:56.000000 quetz-0.0.post4/docs/intersphinx/numpy-objects.inv
+-rw-rw-rw-   0        0        0      558 2024-02-23 00:48:38.000000 quetz-0.0.post4/docs/intersphinx/optmanage-objects.inv
+-rw-rw-rw-   0        0        0   205141 2023-12-12 14:44:40.000000 quetz-0.0.post4/docs/intersphinx/pandas-objects.inv
+-rw-rw-rw-   0        0        0   134856 2023-12-12 14:43:33.000000 quetz-0.0.post4/docs/intersphinx/python-objects.inv
+-rw-rw-rw-   0        0        0   112828 2023-12-12 14:44:22.000000 quetz-0.0.post4/docs/intersphinx/scipy-objects.inv
+-rw-rw-rw-   0        0        0    55596 2023-12-12 14:45:56.000000 quetz-0.0.post4/docs/intersphinx/sympy-objects.inv
+-rw-rw-rw-   0        0        0      667 2024-01-16 17:03:02.000000 quetz-0.0.post4/docs/intersphinx/typed-descriptors-objects.inv
+-rw-rw-rw-   0        0        0      597 2023-12-12 14:44:00.000000 quetz-0.0.post4/docs/intersphinx/typing-validation-objects.inv
+-rwxrwxrwx   0        0        0       56 2021-12-29 15:40:05.000000 quetz-0.0.post4/docs/make-api-clean-html.bat
+-rw-rw-rw-   0        0        0      474 2024-04-10 08:56:22.000000 quetz-0.0.post4/docs/make-api.json
+-rw-rw-rw-   0        0        0    12113 2023-12-20 14:39:39.000000 quetz-0.0.post4/docs/make-api.py
+-rwxrwxrwx   0        0        0      855 2021-12-28 15:57:43.000000 quetz-0.0.post4/docs/make.bat
+-rw-rw-rw-   0        0        0      104 2023-12-20 14:47:30.000000 quetz-0.0.post4/docs/requirements.txt
+-rw-rw-rw-   0        0        0       64 2024-04-10 09:59:34.000000 quetz-0.0.post4/mypy.ini
+-rwxrwxrwx   0        0        0      101 2024-02-23 00:48:38.000000 quetz-0.0.post4/pypi-upload.bat
+-rw-rw-rw-   0        0        0     1994 2024-04-10 11:22:37.000000 quetz-0.0.post4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:57.959828 quetz-0.0.post4/quetz/
+-rw-rw-rw-   0        0        0      950 2024-04-10 10:35:26.000000 quetz-0.0.post4/quetz/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-07-01 14:25:12.000000 quetz-0.0.post4/quetz/py.typed
+-rw-rw-rw-   0        0        0     1394 2024-04-10 09:59:44.000000 quetz-0.0.post4/quetz/scripts.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:25:58.009705 quetz-0.0.post4/quetz.egg-info/
+-rw-rw-rw-   0        0        0    36663 2024-04-10 11:25:57.000000 quetz-0.0.post4/quetz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2024-04-10 11:25:57.000000 quetz-0.0.post4/quetz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:25:57.000000 quetz-0.0.post4/quetz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-10 11:25:57.000000 quetz-0.0.post4/quetz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:25:57.000000 quetz-0.0.post4/quetz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        3 2021-09-20 19:05:47.000000 quetz-0.0.post4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:25:58.018711 quetz-0.0.post4/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

