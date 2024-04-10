# Comparing `tmp/sphinx-design-elements-0.3.0.tar.gz` & `tmp/sphinx-design-elements-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-design-elements-0.3.0.tar", last modified: Sat Apr  6 16:27:47 2024, max compression
+gzip compressed data, was "sphinx-design-elements-0.3.1.tar", last modified: Wed Apr 10 13:47:53 2024, max compression
```

## Comparing `sphinx-design-elements-0.3.0.tar` & `sphinx-design-elements-0.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.184218 sphinx-design-elements-0.3.0/
--rw-r--r--   0 amo        (501) staff       (20)      702 2024-04-06 16:25:38.000000 sphinx-design-elements-0.3.0/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.3.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     8082 2024-04-06 16:27:47.183787 sphinx-design-elements-0.3.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3069 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.164605 sphinx-design-elements-0.3.0/docs/
--rw-r--r--   0 amo        (501) staff       (20)      772 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.0/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)      702 2024-04-06 16:25:38.000000 sphinx-design-elements-0.3.0/docs/changes.md
--rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.0/docs/css_classes.md
--rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.3.0/docs/get_started.md
--rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.0/docs/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)    33174 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/hyper.md
--rw-r--r--   0 amo        (501) staff       (20)     3835 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/index.md
--rw-r--r--   0 amo        (501) staff       (20)     2145 2024-04-06 16:09:47.000000 sphinx-design-elements-0.3.0/docs/info.md
--rw-r--r--   0 amo        (501) staff       (20)     2996 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/docs/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.3.0/docs/project.md
--rw-r--r--   0 amo        (501) staff       (20)     3069 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/docs/readme.md
--rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.3.0/docs/sandbox.md
--rw-r--r--   0 amo        (501) staff       (20)    12371 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.0/docs/shield.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.165063 sphinx-design-elements-0.3.0/docs/snippets/
--rw-r--r--   0 amo        (501) staff       (20)       73 2024-03-24 17:03:31.000000 sphinx-design-elements-0.3.0/docs/snippets/index.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.168316 sphinx-design-elements-0.3.0/docs/snippets/myst/
--rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)      643 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/hyper.md
--rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/shield.md
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/tag.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.171068 sphinx-design-elements-0.3.0/docs/snippets/rst/
--rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/dropdown-group.rst
--rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/gridtable.rst
--rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/infocard.rst
--rw-r--r--   0 amo        (501) staff       (20)      201 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/shield.rst
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/tag.rst
--rw-r--r--   0 amo        (501) staff       (20)     2822 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/tag.md
--rw-r--r--   0 amo        (501) staff       (20)     5928 2024-04-06 16:24:49.000000 sphinx-design-elements-0.3.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-06 16:27:47.184304 sphinx-design-elements-0.3.0/setup.cfg
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.176599 sphinx-design-elements-0.3.0/sphinx_design_elements/
--rw-r--r--   0 amo        (501) staff       (20)      434 2024-03-07 23:44:18.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.179273 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/addon.js
--rw-r--r--   0 amo        (501) staff       (20)     1431 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/style.css
--rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/dropdown_group.py
--rw-r--r--   0 amo        (501) staff       (20)     2849 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/extension.py
--rw-r--r--   0 amo        (501) staff       (20)     5218 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/gridtable.py
--rw-r--r--   0 amo        (501) staff       (20)    13371 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/hyper.py
--rw-r--r--   0 amo        (501) staff       (20)     3751 2024-03-20 22:48:06.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/infocard.py
--rw-r--r--   0 amo        (501) staff       (20)     4004 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/shield.py
--rw-r--r--   0 amo        (501) staff       (20)     2006 2024-03-07 23:25:56.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/tag.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.180364 sphinx-design-elements-0.3.0/sphinx_design_elements/util/
--rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     4565 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/directive.py
--rw-r--r--   0 amo        (501) staff       (20)     4469 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/role.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.180961 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     8082 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     1412 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      331 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       29 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.555605 sphinx-design-elements-0.3.1/
+-rw-r--r--   0 amo        (501) staff       (20)      768 2024-04-10 13:47:11.000000 sphinx-design-elements-0.3.1/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.3.1/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     8142 2024-04-10 13:47:53.555203 sphinx-design-elements-0.3.1/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.532962 sphinx-design-elements-0.3.1/docs/
+-rw-r--r--   0 amo        (501) staff       (20)      772 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.1/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)      768 2024-04-10 13:47:11.000000 sphinx-design-elements-0.3.1/docs/changes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.1/docs/css_classes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.3.1/docs/get_started.md
+-rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.1/docs/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)    33174 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)     3835 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/index.md
+-rw-r--r--   0 amo        (501) staff       (20)     2163 2024-04-10 04:43:18.000000 sphinx-design-elements-0.3.1/docs/info.md
+-rw-r--r--   0 amo        (501) staff       (20)     2996 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.1/docs/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.3.1/docs/project.md
+-rw-r--r--   0 amo        (501) staff       (20)     3129 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/docs/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.3.1/docs/sandbox.md
+-rw-r--r--   0 amo        (501) staff       (20)    12371 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.1/docs/shield.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.533360 sphinx-design-elements-0.3.1/docs/snippets/
+-rw-r--r--   0 amo        (501) staff       (20)       73 2024-03-24 17:03:31.000000 sphinx-design-elements-0.3.1/docs/snippets/index.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.537208 sphinx-design-elements-0.3.1/docs/snippets/myst/
+-rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)      643 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/shield.md
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.1/docs/snippets/myst/tag.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.540413 sphinx-design-elements-0.3.1/docs/snippets/rst/
+-rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/dropdown-group.rst
+-rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/gridtable.rst
+-rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/infocard.rst
+-rw-r--r--   0 amo        (501) staff       (20)      201 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/shield.rst
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.1/docs/snippets/rst/tag.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2822 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/docs/tag.md
+-rw-r--r--   0 amo        (501) staff       (20)     6056 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-10 13:47:53.555696 sphinx-design-elements-0.3.1/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.546989 sphinx-design-elements-0.3.1/sphinx_design_elements/
+-rw-r--r--   0 amo        (501) staff       (20)      434 2024-03-07 23:44:18.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.550291 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/addon.js
+-rw-r--r--   0 amo        (501) staff       (20)     1431 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/style.css
+-rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/dropdown_group.py
+-rw-r--r--   0 amo        (501) staff       (20)     2849 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/extension.py
+-rw-r--r--   0 amo        (501) staff       (20)     5218 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/gridtable.py
+-rw-r--r--   0 amo        (501) staff       (20)    13371 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/hyper.py
+-rw-r--r--   0 amo        (501) staff       (20)     3751 2024-03-20 22:48:06.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/infocard.py
+-rw-r--r--   0 amo        (501) staff       (20)     4004 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/shield.py
+-rw-r--r--   0 amo        (501) staff       (20)     2006 2024-03-07 23:25:56.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/tag.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.551835 sphinx-design-elements-0.3.1/sphinx_design_elements/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4565 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/directive.py
+-rw-r--r--   0 amo        (501) staff       (20)     4482 2024-04-10 13:46:31.000000 sphinx-design-elements-0.3.1/sphinx_design_elements/util/role.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 13:47:53.552546 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     8142 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     1412 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      331 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       29 2024-04-10 13:47:53.000000 sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/top_level.txt
```

### Comparing `sphinx-design-elements-0.3.0/CHANGES.md` & `sphinx-design-elements-0.3.1/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Change Log
 
 ## Unreleased
 
+## v0.3.1 - 2024-04-10
+- Fix compatibility issue with Python 3.8
+
 ## v0.3.0 - 2024-04-06
 - Accept more options on grid table's `sd-item` directive
 - Add `shield` directive, to render badges through Shields.io
 - Add `hyper` role, to render different kinds of hyperlinks
 
 ## v0.2.1 - 2023-08-08
```

### Comparing `sphinx-design-elements-0.3.0/LICENSE` & `sphinx-design-elements-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/PKG-INFO` & `sphinx-design-elements-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -149,32 +149,32 @@
 ## Acknowledgements
 
 Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
 and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/tech-writing/sphinx-design-elements/blob/main/CHANGES.md
 [Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
-[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/tech-writing/sphinx-design-elements/issues
+[License]: https://github.com/tech-writing/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/pyveci/sphinx-design-elements
+[Source code]: https://github.com/tech-writing/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
 [sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-coverage]: https://codecov.io/gh/tech-writing/sphinx-design-elements/branch/main/graph/badge.svg
 [badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
-[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-license]: https://img.shields.io/github/license/tech-writing/sphinx-design-elements.svg
 [badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
 [badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
 [badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
-[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[badge-tests]: https://github.com/tech-writing/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/tech-writing/sphinx-design-elements
 [project-downloads]: https://pepy.tech/project/sphinx-design-elements/
-[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-license]: https://github.com/tech-writing/sphinx-design-elements/blob/main/LICENSE
 [project-pypi]: https://pypi.org/project/sphinx-design-elements
-[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
+[project-tests]: https://github.com/tech-writing/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.3.0/docs/backlog.md` & `sphinx-design-elements-0.3.1/docs/backlog.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/changes.md` & `sphinx-design-elements-0.3.1/docs/changes.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Change Log
 
 ## Unreleased
 
+## v0.3.1 - 2024-04-10
+- Fix compatibility issue with Python 3.8
+
 ## v0.3.0 - 2024-04-06
 - Accept more options on grid table's `sd-item` directive
 - Add `shield` directive, to render badges through Shields.io
 - Add `hyper` role, to render different kinds of hyperlinks
 
 ## v0.2.1 - 2023-08-08
```

### Comparing `sphinx-design-elements-0.3.0/docs/css_classes.md` & `sphinx-design-elements-0.3.1/docs/css_classes.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/dropdown-group.md` & `sphinx-design-elements-0.3.1/docs/dropdown-group.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/get_started.md` & `sphinx-design-elements-0.3.1/docs/get_started.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/gridtable.md` & `sphinx-design-elements-0.3.1/docs/gridtable.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/hyper.md` & `sphinx-design-elements-0.3.1/docs/hyper.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/index.md` & `sphinx-design-elements-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/info.md` & `sphinx-design-elements-0.3.1/docs/info.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # Info
 
 ## Discourse Something
 {hyper}`https://community.panodata.org/t/technical-advancements-in-sphinx/278 {type=badge,outline=true,short-title=true}`
 
 ## Codecov Coverage Status
 :::{code} markdown
-{info}`vcsName=github,user=pyveci,repo=sphinx-design-elements {type=shield}`
+{info}`vcsName=github,user=tech-writing,repo=sphinx-design-elements {type=shield}`
 :::
 https://shields.io/badges/codecov
 :::{code} markdown
-{info}`vcsName=github,user=pyveci,repo=sphinx-design-elements,token=a1b2c3d4e5,flag=flag_name {type=shield}`
+{info}`vcsName=github,user=tech-writing,repo=sphinx-design-elements,token=a1b2c3d4e5,flag=flag_name {type=shield}`
 :::
 
 ## GitHub Actions Workflow Status
 :::{code} markdown
-{info}`user=pyveci,repo=sphinx-design-elements,workflow=main.yml {type=shield}`
+{info}`user=tech-writing,repo=sphinx-design-elements,workflow=main.yml {type=shield}`
 :::
 https://shields.io/badges/git-hub-actions-workflow-status
 
 
 
 ::::{dropdown} Build Status Shortcuts
 :animate: fade-in-slide-down
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 --- orphan: true --- # Info ## Discourse Something {hyper}`https://
 community.panodata.org/t/technical-advancements-in-sphinx/278
 {type=badge,outline=true,short-title=true}` ## Codecov Coverage Status :::
-{code} markdown {info}`vcsName=github,user=pyveci,repo=sphinx-design-elements
-{type=shield}` ::: https://shields.io/badges/codecov :::{code} markdown
-{info}`vcsName=github,user=pyveci,repo=sphinx-design-
+{code} markdown {info}`vcsName=github,user=tech-writing,repo=sphinx-design-
+elements {type=shield}` ::: https://shields.io/badges/codecov :::{code}
+markdown {info}`vcsName=github,user=tech-writing,repo=sphinx-design-
 elements,token=a1b2c3d4e5,flag=flag_name {type=shield}` ::: ## GitHub Actions
-Workflow Status :::{code} markdown {info}`user=pyveci,repo=sphinx-design-
+Workflow Status :::{code} markdown {info}`user=tech-writing,repo=sphinx-design-
 elements,workflow=main.yml {type=shield}` ::: https://shields.io/badges/git-
 hub-actions-workflow-status ::::{dropdown} Build Status Shortcuts :animate:
 fade-in-slide-down :open: Shield shortcut roles help saving a few keystrokes.
 Examples: `hyper-navigate`, `hyper-open`, `hyper-tutorial`, `hyper-read-more`,
 `hyper-readme-github`, `hyper-nb-colab`, `hyper-nb-binder`, `hyper-nb-github`.
 --- :::{code} markdown {hyper-github-workflow}`Apache Kafka, Apache Flink
 ratedb-examples/actions/workflows/application-apache-kafka-flink.yml>` :::
```

### Comparing `sphinx-design-elements-0.3.0/docs/infocard.md` & `sphinx-design-elements-0.3.1/docs/infocard.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/sandbox.md` & `sphinx-design-elements-0.3.1/docs/sandbox.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/shield.md` & `sphinx-design-elements-0.3.1/docs/shield.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/snippets/myst/hyper.md` & `sphinx-design-elements-0.3.1/docs/snippets/myst/hyper.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/snippets/rst/infocard.rst` & `sphinx-design-elements-0.3.1/docs/snippets/rst/infocard.rst`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/docs/tag.md` & `sphinx-design-elements-0.3.1/docs/tag.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/pyproject.toml` & `sphinx-design-elements-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -167,39 +167,45 @@
 markers = [
 ]
 
 [tool.ruff]
 line-length = 120
 
 lint.select = [
+  # Pycodestyle
+  "E",
+  "W",
+  # Pyflakes
+  "F",
+  # isort
+  "I",
   # Bandit
   "S",
-  # Bugbear
-  "B",
-  # Builtins
-  "A",
-  # comprehensions
-  "C4",
+  # flake8-quotes
+  "Q",
   # eradicate
   "ERA",
   # flake8-2020
   "YTT",
-  # isort
-  "I",
-  # pandas-vet
-  "PD",
   # print
   "T20",
-  # Pycodestyle
-  "E",
-  "W",
-  # Pyflakes
-  "F",
   # return
   "RET",
+  # pyupgrade
+  # "UP",
+  # flake8-commas
+  # "COM",
+  # future-annotations
+  # "FA",
+  # flake8-type-checking
+  "TCH",
+  # flake8-unused-arguments
+  # "ARG",
+  # flake8-use-pathlib
+  # "PTH"
 ]
 
 lint.extend-ignore = [
   # zip() without an explicit strict= parameter
   "B905",
   # df is a bad variable name. Be kinder to your future self.
   "PD901",
```

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/addon.js` & `sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/addon.js`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/style.css` & `sphinx-design-elements-0.3.1/sphinx_design_elements/compiled/style.css`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/extension.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/gridtable.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/gridtable.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/hyper.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/hyper.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/infocard.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/infocard.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/shield.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/shield.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/tag.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/tag.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/util/directive.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/util/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements/util/role.py` & `sphinx-design-elements-0.3.1/sphinx_design_elements/util/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import lru_cache
-from typing import Any, Optional, Union
+from typing import Any, List, Optional, Tuple, Union
 
 from docutils import nodes
 from myst_parser.mocking import MockInliner
 from sphinx import addnodes
 from sphinx.environment import BuildEnvironment
 from sphinx.ext.intersphinx import resolve_reference_detect_inventory
 
@@ -83,15 +83,15 @@
 
     soup = BeautifulSoup(urlopen(url), "html.parser")  # noqa: S310
     return soup.title and soup.title.get_text() or url
 
 
 def parse_block_myst(
     self: MockInliner, text: str, lineno: int, memo: Any, parent: nodes.Element, with_container: bool = False
-) -> tuple[list[nodes.Node], list[nodes.system_message]]:
+) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
     """
     Parse the text and return a list of nodes.
 
     Similar to `myst_parser.mocking.MockInliner.parse`, but uses
     `inline=False` for rendering, and returns only the inner node.
     """
     with self._renderer.current_node_context(parent):
@@ -105,15 +105,15 @@
     else:
         ref = container.next_node().next_node()
     return [ref], []
 
 
 def parse_block_rst(  # pragma: nocover
     self: MockInliner, text: str, lineno: int, memo: Any, parent: nodes.Element
-) -> tuple[list[nodes.Node], list[nodes.system_message]]:
+) -> Tuple[List[nodes.Node], List[nodes.system_message]]:
     """
     mw = MarkdownWrapper()
     res = mw.render(text)
     return res, []
 
     memo.reporter = self.reporter
     memo.document = self.document
```

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/PKG-INFO` & `sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -149,32 +149,32 @@
 ## Acknowledgements
 
 Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
 and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/tech-writing/sphinx-design-elements/blob/main/CHANGES.md
 [Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
-[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/tech-writing/sphinx-design-elements/issues
+[License]: https://github.com/tech-writing/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/pyveci/sphinx-design-elements
+[Source code]: https://github.com/tech-writing/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
 [sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-coverage]: https://codecov.io/gh/tech-writing/sphinx-design-elements/branch/main/graph/badge.svg
 [badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
-[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-license]: https://img.shields.io/github/license/tech-writing/sphinx-design-elements.svg
 [badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
 [badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
 [badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
-[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[badge-tests]: https://github.com/tech-writing/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/tech-writing/sphinx-design-elements
 [project-downloads]: https://pepy.tech/project/sphinx-design-elements/
-[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-license]: https://github.com/tech-writing/sphinx-design-elements/blob/main/LICENSE
 [project-pypi]: https://pypi.org/project/sphinx-design-elements
-[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
+[project-tests]: https://github.com/tech-writing/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/SOURCES.txt` & `sphinx-design-elements-0.3.1/sphinx_design_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

