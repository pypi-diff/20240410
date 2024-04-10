# Comparing `tmp/nbsite-0.8.6a1.tar.gz` & `tmp/nbsite-0.8.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsite-0.8.6a1.tar", last modified: Tue Apr  9 10:07:43 2024, max compression
+gzip compressed data, was "nbsite-0.8.6a2.tar", last modified: Wed Apr 10 10:37:17 2024, max compression
```

## Comparing `nbsite-0.8.6a1.tar` & `nbsite-0.8.6a2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.456228 nbsite-0.8.6a1/nbsite/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/holoviz-icon-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/_shared_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/js/goatcounter.js
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_templates/github-stars-button.html
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/_shared_templates/sidebar-nav-bs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31439 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23511 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (127)    17465 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.452228 nbsite-0.8.6a1/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.460228 nbsite-0.8.6a1/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18588 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/tests/test_nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 10:07:43.000000 nbsite-0.8.6a1/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 10:07:43.464228 nbsite-0.8.6a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-09 10:06:50.000000 nbsite-0.8.6a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.638002 nbsite-0.8.6a2/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.638002 nbsite-0.8.6a2/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/holoviz-icon-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.638002 nbsite-0.8.6a2/nbsite/_shared_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/js/goatcounter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_templates/github-stars-button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/_shared_templates/sidebar-nav-bs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31439 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23511 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.634003 nbsite-0.8.6a2/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.642002 nbsite-0.8.6a2/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18588 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/tests/test_nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 10:37:17.000000 nbsite-0.8.6a2/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5869 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11144 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 10:37:17.646002 nbsite-0.8.6a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-10 10:36:29.000000 nbsite-0.8.6a2/setup.py
```

### Comparing `nbsite-0.8.6a1/LICENSE.txt` & `nbsite-0.8.6a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/PKG-INFO` & `nbsite-0.8.6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a1
+Version: 0.8.6a2
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.6a1/README.md` & `nbsite-0.8.6a2/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/__main__.py` & `nbsite-0.8.6a2/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/alert.css` & `nbsite-0.8.6a2/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.6a2/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.6a2/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/js/goatcounter.js` & `nbsite-0.8.6a2/nbsite/_shared_static/js/goatcounter.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.6a2/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.6a2/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/notebook.css` & `nbsite-0.8.6a2/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_static/scroller.css` & `nbsite-0.8.6a2/nbsite/_shared_static/scroller.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.6a2/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/_shared_templates/layout.html` & `nbsite-0.8.6a2/nbsite/_shared_templates/layout.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/analytics/__init__.py` & `nbsite-0.8.6a2/nbsite/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/cmd.py` & `nbsite-0.8.6a2/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/gallery/gen.py` & `nbsite-0.8.6a2/nbsite/gallery/gen.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.6a2/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/nbbuild.py` & `nbsite-0.8.6a2/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/paramdoc.py` & `nbsite-0.8.6a2/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.6a2/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.6a2/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.6a2/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/__init__.py` & `nbsite-0.8.6a2/nbsite/pyodide/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     js, js_exports, js_modules, css = [], {}, {}, []
     with set_resource_mode('cdn'):
         for name, model in Model.model_class_reverse_map.items():
             if hasattr(model, '__javascript__'):
                 js += model.__javascript__
             if hasattr(model, '__css__'):
                 css += model.__css__
-            if hasattr(model, '__javascript_module__'):
+            if hasattr(model, '__javascript_modules__'):
                 js_modules.update({
                     jsm.split("/")[-1][:-3]: jsm for jsm in model.__javascript_modules__
                     if jsm.endswith('.js')
                 })
             if hasattr(model, '__javascript_module_exports__'):
                 js_exports.update(
                     dict(zip(model.__javascript_module_exports__,
```

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.6a2/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.6a2/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.6a2/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/shared_conf.py` & `nbsite-0.8.6a2/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/templates/basic/conf.py` & `nbsite-0.8.6a2/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.6a2/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/tests/test_cmd.py` & `nbsite-0.8.6a2/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/tests/test_nbbuild.py` & `nbsite-0.8.6a2/nbsite/tests/test_nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/tests/test_util.py` & `nbsite-0.8.6a2/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite/util.py` & `nbsite-0.8.6a2/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.6a2/nbsite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.6a1
+Version: 0.8.6a2
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.6a1/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.6a2/nbsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/pyproject.toml` & `nbsite-0.8.6a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.6a2/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/scripts/nbsite_fix_links.py` & `nbsite-0.8.6a2/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/scripts/nbsite_generate_modules.py` & `nbsite-0.8.6a2/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.6a2/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/setup.cfg` & `nbsite-0.8.6a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.6a1/setup.py` & `nbsite-0.8.6a2/setup.py`

 * *Files identical despite different names*

