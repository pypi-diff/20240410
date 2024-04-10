# Comparing `tmp/llnl-thicket-2023.3.1.tar.gz` & `tmp/llnl-thicket-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llnl-thicket-2023.3.1.tar", last modified: Tue Nov 14 21:01:19 2023, max compression
+gzip compressed data, was "llnl-thicket-2024.1.0.tar", last modified: Wed Apr 10 18:47:24 2024, max compression
```

## Comparing `llnl-thicket-2023.3.1.tar` & `llnl-thicket-2024.1.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-11-14 21:01:13.000000 llnl-thicket-2023.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-14 21:01:13.000000 llnl-thicket-2023.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-14 21:01:13.000000 llnl-thicket-2023.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-11-14 21:01:13.000000 llnl-thicket-2023.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.651544 llnl-thicket-2023.3.1/llnl_thicket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-11-14 21:01:19.000000 llnl-thicket-2023.3.1/llnl_thicket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-11-14 21:01:19.000000 llnl-thicket-2023.3.1/llnl_thicket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 21:01:19.000000 llnl-thicket-2023.3.1/llnl_thicket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-14 21:01:19.000000 llnl-thicket-2023.3.1/llnl_thicket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-14 21:01:19.000000 llnl-thicket-2023.3.1/llnl_thicket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.655544 llnl-thicket-2023.3.1/thicket/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15964 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.655544 llnl-thicket-2023.3.1/thicket/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/external/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/model_extrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/ncu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.655544 llnl-thicket-2023.3.1/thicket/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/calc_boxplot_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/check_normality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/correlation_nodewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/display_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/display_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/display_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/median.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/stats/variance.py
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/thicket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.655544 llnl-thicket-2023.3.1/thicket/vis/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.655544 llnl-thicket-2023.3.1/thicket/vis/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/globals.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/datautil.js
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/globals.js
--rw-r--r--   0 runner    (1001) docker     (127)    19679 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/pcp.js
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/scatter.js
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/stackedarea.js
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/store.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/thicket/vis/scripts/topdown/
--rw-r--r--   0 runner    (1001) docker     (127)    14321 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/topdown/stackedbars.js
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/topdown/topdown.js
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/scripts/treetable.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/thicket/vis/static/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/pcp_bundle.html
--rw-r--r--   0 runner    (1001) docker     (127)   338991 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/pcp_bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/topdown_bundle.html
--rw-r--r--   0 runner    (1001) docker     (127)   189342 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/topdown_bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/treetable_bundle.html
--rw-r--r--   0 runner    (1001) docker     (127)   282630 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static/treetable_bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/static_fixer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:01:19.659544 llnl-thicket-2023.3.1/thicket/vis/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/templates/pcp.html
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/templates/topdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/templates/treetable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-11-14 21:01:14.000000 llnl-thicket-2023.3.1/thicket/vis/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/llnl_thicket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 18:47:24.000000 llnl-thicket-2024.1.0/llnl_thicket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-10 18:47:24.000000 llnl-thicket-2024.1.0/llnl_thicket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:47:24.000000 llnl-thicket-2024.1.0/llnl_thicket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 18:47:24.000000 llnl-thicket-2024.1.0/llnl_thicket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:47:24.000000 llnl-thicket-2024.1.0/llnl_thicket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.023985 llnl-thicket-2024.1.0/thicket/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.027985 llnl-thicket-2024.1.0/thicket/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/external/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/model_extrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/ncu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.027985 llnl-thicket-2024.1.0/thicket/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/calc_boxplot_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/check_normality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/correlation_nodewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/display_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/display_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/display_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/display_violinplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/stats/variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49888 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/thicket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.027985 llnl-thicket-2024.1.0/thicket/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.027985 llnl-thicket-2024.1.0/thicket/vis/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/globals.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.027985 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/datautil.js
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/globals.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19679 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/pcp.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/scatter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/stackedarea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/store.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/thicket/vis/scripts/topdown/
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/topdown/stackedbars.js
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/topdown/topdown.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/scripts/treetable.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/thicket/vis/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/pcp_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (127)   338991 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/pcp_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/topdown_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (127)   189342 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/topdown_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/treetable_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (127)   282630 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static/treetable_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/static_fixer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:47:24.031985 llnl-thicket-2024.1.0/thicket/vis/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/templates/pcp.html
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/templates/topdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/templates/treetable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-10 18:47:18.000000 llnl-thicket-2024.1.0/thicket/vis/webpack.config.js
```

### Comparing `llnl-thicket-2023.3.1/LICENSE` & `llnl-thicket-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/NOTICE` & `llnl-thicket-2024.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/llnl_thicket.egg-info/SOURCES.txt` & `llnl-thicket-2024.1.0/llnl_thicket.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 llnl_thicket.egg-info/PKG-INFO
 llnl_thicket.egg-info/SOURCES.txt
 llnl_thicket.egg-info/dependency_links.txt
 llnl_thicket.egg-info/requires.txt
 llnl_thicket.egg-info/top_level.txt
 thicket/__init__.py
 thicket/ensemble.py
+thicket/groupby.py
 thicket/helpers.py
 thicket/model_extrap.py
 thicket/ncu.py
 thicket/thicket.py
 thicket/utils.py
 thicket/version.py
 thicket/external/__init__.py
@@ -22,20 +23,22 @@
 thicket/stats/__init__.py
 thicket/stats/calc_boxplot_statistics.py
 thicket/stats/check_normality.py
 thicket/stats/correlation_nodewise.py
 thicket/stats/display_boxplot.py
 thicket/stats/display_heatmap.py
 thicket/stats/display_histogram.py
+thicket/stats/display_violinplot.py
 thicket/stats/maximum.py
 thicket/stats/mean.py
 thicket/stats/median.py
 thicket/stats/minimum.py
 thicket/stats/percentiles.py
 thicket/stats/preference.py
+thicket/stats/scoring.py
 thicket/stats/std.py
 thicket/stats/ttest.py
 thicket/stats/variance.py
 thicket/vis/__init__.py
 thicket/vis/package.json
 thicket/vis/static_fixer.py
 thicket/vis/visualizations.py
```

### Comparing `llnl-thicket-2023.3.1/setup.py` & `llnl-thicket-2024.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     ],
     include_package_data=True,
     install_requires=[
         "scipy",
         "numpy",
         "pandas >= 1.1",
         "llnl-hatchet",
+        "tqdm",
+        "more-itertools",
     ],
     extras_require={
         "extrap": ["extrap", "matplotlib"],
         "plotting": ["seaborn"],
         "vis": ["beautifulsoup4"],
     },
 )
```

### Comparing `llnl-thicket-2023.3.1/thicket/ensemble.py` & `llnl-thicket-2024.1.0/thicket/ensemble.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,170 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 from collections import OrderedDict
+import warnings
 
 from hatchet import GraphFrame
 import numpy as np
 import pandas as pd
+import tqdm
 
 import thicket.helpers as helpers
-from .utils import validate_dataframe, verify_sorted_profile, verify_thicket_structures
+from .utils import (
+    check_same_frame,
+    validate_dataframe,
+    verify_sorted_profile,
+    verify_thicket_structures,
+)
 
 
 class Ensemble:
     """Operations pertaining to ensembling."""
 
     @staticmethod
-    def _unify(thickets, inplace=False):
+    def _unify(thickets, inplace=False, disable_tqdm=False):
         """Create union graph from list of thickets and sync their DataFrames.
 
         Arguments:
             thickets (list): list of Thicket objects
             inplace (bool): whether to modify the original thicket objects or return new
+            disable_tqdm (bool): whether to disable tqdm progress bar
 
         Returns:
             (tuple): tuple containing:
                 (hatchet.Graph): unified graph
                 (list): list of Thicket objects
         """
+
+        def _merge_dicts(cur_dict, update_dict):
+            """Merge old_to_new dictionary from the result of thicket i and i + 1 with old_to_new from i + 1 and i + 2.
+
+            Arguments:
+                cur_dict (dict): dictionary mapping old node to new node
+                update_dict (dict): dictionary mapping old node to new node
+
+            Returns:
+                (dict): merged dictionary
+            """
+            merged_dict = {}
+
+            if len(cur_dict) == 0:
+                return update_dict
+
+            # Merge values from update_dict into keys from cur_dict
+            seen_keys = []
+            for new_id, new_node in update_dict.items():
+                for cur_id, cur_node in cur_dict.items():
+                    if id(cur_node) == new_id:
+                        merged_dict[cur_id] = new_node
+                        seen_keys.append(new_id)
+
+            # Pairs that are left in update_dict
+            for tid, node in update_dict.items():
+                if tid not in seen_keys:
+                    merged_dict[tid] = node
+
+            return merged_dict
+
+        def _replace_graph_df_nodes(thickets, old_to_new, union_graph):
+            """Replace the node objects in the graph and DataFrame of a Thicket object from the result of graph.union().
+
+            Arguments:
+                thickets (list): list of Thicket objects
+                old_to_new (dict): dictionary mapping old node to new node
+                union_graph (hatchet.Graph): unified graph
+
+            Returns:
+                (Thicket): modified Thicket object
+            """
+            for i in range(len(thickets)):
+                thickets[i].graph = union_graph
+                idx_names = thickets[i].dataframe.index.names
+                thickets[i].dataframe = thickets[i].dataframe.reset_index()
+                replace_dict = {}
+                for node in thickets[i].dataframe["node"]:
+                    node_id = id(node)
+                    if node_id in old_to_new:
+                        check_same_frame(node, old_to_new[node_id])
+                        replace_dict[node] = old_to_new[node_id]
+                thickets[i].dataframe["node"] = (
+                    thickets[i].dataframe["node"].replace(replace_dict)
+                )
+                thickets[i].dataframe = thickets[i].dataframe.set_index(idx_names)
+
+            return thickets
+
         _thickets = thickets
         if not inplace:
             _thickets = [th.deepcopy() for th in thickets]
+        helpers._set_node_ordering(_thickets)
         # Unify graphs if "self" and "other" do not have the same graph
         union_graph = _thickets[0].graph
-        for i in range(len(_thickets) - 1):
-            # Check for same graph id (fast) if not -> check for equality (slow)
-            if (
-                _thickets[i].graph is _thickets[i + 1].graph
-                or _thickets[i].graph == _thickets[i + 1].graph
-            ):
-                continue
-            else:
-                union_graph = union_graph.union(_thickets[i + 1].graph)
-        for i in range(len(_thickets)):
+        old_to_new = {}
+        pbar = tqdm.tqdm(range(len(_thickets) - 1), disable=disable_tqdm)
+        for i in pbar:
+            pbar.set_description("(2/2) Creating Thicket")
+            temp_dict = {}
+            union_graph = union_graph.union(_thickets[i + 1].graph, temp_dict)
             # Set all graphs to the union graph
             _thickets[i].graph = union_graph
+            _thickets[i + 1].graph = union_graph
+            # Merge the current old_to_new dictionary with the new mappings
+            old_to_new = _merge_dicts(old_to_new, temp_dict)
+        # Update the nodes in the dataframe
+        _thickets = _replace_graph_df_nodes(_thickets, old_to_new, union_graph)
+        for i in range(len(_thickets)):
             # For tree diff. dataframes need to be sorted.
             _thickets[i].dataframe.sort_index(inplace=True)
-            # Necessary to change dataframe hatchet id's to match the nodes in the graph
-            helpers._sync_nodes_frame(union_graph, _thickets[i].dataframe)
         return union_graph, _thickets
 
     @staticmethod
     def _columns(
         thickets,
         headers=None,
         metadata_key=None,
+        disable_tqdm=False,
     ):
         """Concatenate Thicket attributes horizontally. For DataFrames, this implies expanding
         in the column direction. New column multi-index will be created with columns
         under separate indexer headers.
 
         Arguments:
             headers (list): List of headers to use for the new columnar multi-index
             metadata_key (str): Name of the column from the metadata tables to replace the 'profile'
                 index. If no argument is provided, it is assumed that there is no profile-wise
                 relationship between the thickets.
+            disable_tqdm (bool): whether to disable tqdm progress bar
 
         Returns:
             (Thicket): New ensembled Thicket object
         """
 
         def _check_structures():
             """Check that the structures of the thicket objects are valid for the incoming operations."""
             # Required/expected format of the data
             for th in thickets:
-                verify_thicket_structures(th.dataframe, index=["node", "profile"])
+                assert th.dataframe.index.nlevels == 2
+                assert th.metadata.index.nlevels == 1
+                assert th.dataframe.index.names[1] == th.metadata.index.name
                 verify_thicket_structures(th.statsframe.dataframe, index=["node"])
-                verify_thicket_structures(th.metadata, index=["profile"])
             # Check for metadata_key in metadata
             if metadata_key:
                 for th in thickets:
-                    verify_thicket_structures(th.metadata, columns=[metadata_key])
+                    if metadata_key != th.metadata.index.name:
+                        verify_thicket_structures(th.metadata, columns=[metadata_key])
             # Check length of profiles match if metadata key is not provided
             if metadata_key is None:
                 for i in range(len(thickets) - 1):
                     if len(thickets[i].profile) != len(thickets[i + 1].profile):
                         raise ValueError(
-                            "Length of all thicket profiles must match if 'metadata_key' is not provided. {} != {}".format(
-                                len(thickets[i].profile), len(thickets[i + 1].profile)
-                            )
+                            f"Length of all thicket profiles must match if 'metadata_key' is not provided. {len(thickets[i].profile)} != {len(thickets[i + 1].profile)}"
                         )
             # Ensure all thickets profiles are sorted. Must be true when metadata_key=None to
             # guarantee performance data table and metadata table match up.
             if metadata_key is None:
                 for th in thickets:
                     verify_sorted_profile(th.dataframe)
                     verify_sorted_profile(th.metadata)
@@ -116,22 +186,24 @@
                 new_tuple = (upper_idx_name, column)
                 new_idx.append(new_tuple)
             return new_idx
 
         def _handle_metadata():
             """Handle operations to create new concatenated columnar axis metadata table."""
             # Update index to reflect performance data table index
-            for i in range(len(thickets_cp)):
-                thickets_cp[i].metadata.reset_index(drop=True, inplace=True)
+            if metadata_key != inner_idx:
+                for i in range(len(thickets_cp)):
+                    thickets_cp[i].metadata.reset_index(drop=True, inplace=True)
             if metadata_key is None:
                 for i in range(len(thickets_cp)):
                     thickets_cp[i].metadata.index.set_names("profile", inplace=True)
             else:
                 for i in range(len(thickets_cp)):
-                    thickets_cp[i].metadata.set_index(metadata_key, inplace=True)
+                    if metadata_key != inner_idx:
+                        thickets_cp[i].metadata.set_index(metadata_key, inplace=True)
                     thickets_cp[i].metadata.sort_index(inplace=True)
 
             # Create multi-index columns
             for i in range(len(thickets_cp)):
                 thickets_cp[i].metadata.columns = pd.MultiIndex.from_tuples(
                     _create_multiindex_columns(thickets_cp[i].metadata, headers[i])
                 )
@@ -175,45 +247,47 @@
             if metadata_key is None:  # Create index from scratch
                 new_profiles = [i for i in range(len(thickets_cp[0].profile))]
                 for i in range(len(thickets_cp)):
                     thickets_cp[i].metadata["new_profiles"] = new_profiles
                     thickets_cp[i].metadata_column_to_perfdata(
                         "new_profiles", drop=True
                     )
-                    thickets_cp[i].dataframe.reset_index(level="profile", inplace=True)
+                    thickets_cp[i].dataframe.reset_index(level=inner_idx, inplace=True)
                     new_mappings.update(
                         pd.Series(
                             thickets_cp[i]
                             .dataframe["new_profiles"]
                             .map(lambda x: (x, headers[i]))
                             .values,
-                            index=thickets_cp[i].dataframe["profile"],
+                            index=thickets_cp[i].dataframe[inner_idx],
                         ).to_dict()
                     )
-                    thickets_cp[i].dataframe.drop("profile", axis=1, inplace=True)
+                    thickets_cp[i].dataframe.drop(inner_idx, axis=1, inplace=True)
                     thickets_cp[i].dataframe.set_index(
                         "new_profiles", append=True, inplace=True
                     )
                     thickets_cp[i].dataframe.index.rename(
                         "profile", level="new_profiles", inplace=True
                     )
             else:  # Change second-level index to be from metadata's "metadata_key" column
                 for i in range(len(thickets_cp)):
-                    thickets_cp[i].metadata_column_to_perfdata(metadata_key)
-                    thickets_cp[i].dataframe.reset_index(level="profile", inplace=True)
+                    if metadata_key not in thickets_cp[i].dataframe.index.names:
+                        thickets_cp[i].metadata_column_to_perfdata(metadata_key)
+                    thickets_cp[i].dataframe.reset_index(level=inner_idx, inplace=True)
                     new_mappings.update(
                         pd.Series(
                             thickets_cp[i]
                             .dataframe[metadata_key]
                             .map(lambda x: (x, headers[i]))
                             .values,
-                            index=thickets_cp[i].dataframe["profile"],
+                            index=thickets_cp[i].dataframe[inner_idx],
                         ).to_dict()
                     )
-                    thickets_cp[i].dataframe.drop("profile", axis=1, inplace=True)
+                    if inner_idx != metadata_key:
+                        thickets_cp[i].dataframe.drop(inner_idx, axis=1, inplace=True)
                     thickets_cp[i].dataframe.set_index(
                         metadata_key, append=True, inplace=True
                     )
                     thickets_cp[i].dataframe.sort_index(inplace=True)
 
             # Create tuple columns
             new_columns = [
@@ -262,22 +336,25 @@
             combined_th.statsframe = GraphFrame(
                 graph=combined_th.graph,
                 dataframe=helpers._new_statsframe_df(
                     combined_th.dataframe, multiindex=True
                 ),
             )
 
-        # Step 0A: Pre-check of data structures
-        _check_structures()
-        # Step 0B: Variable Initialization
+        # Step 0A: Variable Initialization
         combined_th = thickets[0].deepcopy()
         thickets_cp = [th.deepcopy() for th in thickets]
+        inner_idx = thickets_cp[0].dataframe.index.names[1]
+        # Step 0B: Pre-check of data structures
+        _check_structures()
 
-        # Step 1: Unify the thickets
-        union_graph, _thickets = Ensemble._unify(thickets_cp)
+        # Step 1: Unify the thickets. Can be inplace since we are using copies already
+        union_graph, _thickets = Ensemble._unify(
+            thickets_cp, inplace=True, disable_tqdm=disable_tqdm
+        )
         combined_th.graph = union_graph
         thickets_cp = _thickets
 
         # Step 2A: Handle performance data tables
         new_mappings = _handle_perfdata()
         # Step 2B: Handle metadata tables
         _handle_metadata()
@@ -288,56 +365,78 @@
 
         # Validate dataframe
         validate_dataframe(combined_th.dataframe)
 
         return combined_th
 
     @staticmethod
-    def _index(thickets, from_statsframes=False):
+    def _index(thickets, from_statsframes=False, disable_tqdm=False):
         """Unify a list of thickets into a single thicket
 
         Arguments:
+            thickets (list): list of Thicket objects
             from_statsframes (bool): Whether this method was invoked from from_statsframes
+            disable_tqdm (bool): whether to disable tqdm progress bar
 
         Returns:
             unify_graph (hatchet.Graph): unified graph,
             unify_df (DataFrame): unified dataframe,
             unify_exc_metrics (list): exclusive metrics,
             unify_inc_metrics (list): inclusive metrics,
             unify_metadata (DataFrame): unified metadata,
             unify_profile (list): profiles,
             unify_profile_mapping (dict): profile mapping
         """
 
-        def _fill_perfdata(perfdata, fill_value=np.nan):
-            # Fill missing rows in dataframe with NaN's
-            perfdata = perfdata.reindex(
-                pd.MultiIndex.from_product(perfdata.index.levels), fill_value=fill_value
-            )
-            # Replace "NaN" with "None" in columns of string type
-            for col in perfdata.columns:
-                if pd.api.types.is_string_dtype(perfdata[col].dtype):
-                    perfdata[col].replace({fill_value: None}, inplace=True)
+        def _fill_perfdata(df, numerical_fill_value=np.nan):
+            """Create full index for DataFrame and fill created rows with NaN's or None's where applicable.
 
-            return perfdata
+            Arguments:
+                df (DataFrame): DataFrame to fill missing rows in
+                numerical_fill_value (any): value to fill numerical rows with
+
+            Returns:
+                (DataFrame): filled DataFrame
+            """
+            try:
+                # Fill missing rows in dataframe with NaN's
+                df = df.reindex(
+                    pd.MultiIndex.from_product(df.index.levels),
+                    fill_value=numerical_fill_value,
+                )
+                # Replace "NaN" with "None" in columns of string type
+                for col in df.columns:
+                    if pd.api.types.is_string_dtype(df[col].dtype):
+                        df[col].replace({numerical_fill_value: None}, inplace=True)
+            except ValueError as e:
+                estr = str(e)
+                if estr == "cannot handle a non-unique multi-index!":
+                    warnings.warn(
+                        "Non-unique multi-index for DataFrame in _fill_perfdata. Cannot Fill missing rows.",
+                        RuntimeWarning,
+                    )
+                else:
+                    raise
+
+            return df
 
         # Add missing indicies to thickets
         helpers._resolve_missing_indicies(thickets)
 
         # Initialize attributes
         unify_graph = None
         unify_df = pd.DataFrame()
         unify_inc_metrics = []
         unify_exc_metrics = []
         unify_metadata = pd.DataFrame()
         unify_profile = []
         unify_profile_mapping = OrderedDict()
 
         # Unification
-        unify_graph, thickets = Ensemble._unify(thickets)
+        unify_graph, thickets = Ensemble._unify(thickets, disable_tqdm=disable_tqdm)
         for th in thickets:
             # Extend metrics
             unify_inc_metrics.extend(th.inc_metrics)
             unify_exc_metrics.extend(th.exc_metrics)
             # Extend metadata
             if len(th.metadata) > 0:
                 curr_meta = th.metadata.copy()
@@ -349,29 +448,29 @@
             if th.profile_mapping is not None:
                 unify_profile_mapping.update(th.profile_mapping)
             # Extend dataframe
             unify_df = pd.concat([th.dataframe, unify_df])
         # Sort by keys
         unify_profile_mapping = OrderedDict(sorted(unify_profile_mapping.items()))
 
+        # Validate unify_df before next operation
+        validate_dataframe(unify_df)
+
         # Insert missing rows in dataframe
         unify_df = _fill_perfdata(unify_df)
 
         # Sort PerfData
         unify_df.sort_index(inplace=True)
         # Sort Metadata
         unify_metadata.sort_index(inplace=True)
 
         # Remove duplicates in metrics
         unify_inc_metrics = list(set(unify_inc_metrics))
         unify_exc_metrics = list(set(unify_exc_metrics))
 
-        # Validate unify_df
-        validate_dataframe(unify_df)
-
         unify_parts = (
             unify_graph,
             unify_df,
             unify_exc_metrics,
             unify_inc_metrics,
             unify_metadata,
             unify_profile,
```

### Comparing `llnl-thicket-2023.3.1/thicket/external/console.py` & `llnl-thicket-2024.1.0/thicket/external/console.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from hatchet.external.console import ConsoleRenderer
 from hatchet.util.colormaps import ColorMaps
 
 from ..version import __version__
 
 
 class ThicketRenderer(ConsoleRenderer):
+    """Extends the Hatchet ConsoleRenderer to support multi-dimensional Thicket data."""
+
     # pylint: disable=W1401
     def render_preamble(self):
         lines = [
             r"  _____ _     _      _        _   ",
             r" |_   _| |__ (_) ___| | _____| |_ ",
             r"   | | | '_ \| |/ __| |/ / _ \ __|",
             r"   | | | | | | | (__|   <  __/ |_ ",
@@ -46,14 +48,15 @@
         self.depth = kwargs["depth"]
         self.highlight = kwargs["highlight_name"]
         self.colormap = kwargs["colormap"]
         self.invert_colormap = kwargs["invert_colormap"]
         self.colormap_annotations = kwargs["colormap_annotations"]
         self.min_value = kwargs["min_value"]
         self.max_value = kwargs["max_value"]
+        self.indices = kwargs["indices"]
 
         if self.color:
             self.colors = self.colors_enabled
             # set the colormap based on user input
             self.colors.colormap = ColorMaps().get_colors(
                 self.colormap, self.invert_colormap
             )
@@ -136,14 +139,89 @@
             result += self.render_legend()
 
         if self.unicode:
             return result
         else:
             return result.encode("utf-8")
 
+    def render_legend(self):
+        def render_label(index, low, high):
+            metric_range = self.max_metric - self.min_metric
+
+            return (
+                self.colors.colormap[index]
+                + "█ "
+                + self.colors.end
+                + "{:.2f}".format(low * metric_range + self.min_metric)
+                + " - "
+                + "{:.2f}".format(high * metric_range + self.min_metric)
+                + "\n"
+            )
+
+        legend = (
+            "\n"
+            + "\033[4m"
+            + "Legend"
+            + self.colors.end
+            + " (Metric: "
+            + str(self.primary_metric)
+            + " Min: {:.2f}".format(self.min_metric)
+            + " Max: {:.2f}".format(self.max_metric)
+            + " indices: "
+            + str(self.indices)
+            + ")\n"
+        )
+
+        legend += render_label(0, 0.9, 1.0)
+        legend += render_label(1, 0.7, 0.9)
+        legend += render_label(2, 0.5, 0.7)
+        legend += render_label(3, 0.3, 0.5)
+        legend += render_label(4, 0.1, 0.3)
+        legend += render_label(5, 0.0, 0.1)
+
+        legend += "\n" + self._ansi_color_for_name("name") + "name" + self.colors.end
+        legend += " User code    "
+
+        legend += self.colors.left + self.lr_arrows["◀"] + self.colors.end
+        legend += " Only in left graph    "
+        legend += self.colors.right + self.lr_arrows["▶"] + self.colors.end
+        legend += " Only in right graph\n"
+
+        if self.annotation_column is not None:
+            # temporal pattern legend customization
+            if "_pattern" in self.annotation_column:
+                score_ranges = [0.0, 0.2, 0.4, 0.6, 1.0]
+                legend += "\nTemporal Pattern"
+                for k in self.temporal_symbols.keys():
+                    if "none" not in k:
+                        legend += "   " + self.temporal_symbols[k] + " " + k
+                legend += "\nTemporal Score  "
+                if self.colormap_annotations:
+                    legend_color_mapping = sorted(score_ranges)
+                    legend_colormap = ColorMaps().get_colors(
+                        self.colormap_annotations, False
+                    )
+                    for i in range(len(score_ranges) - 1):
+                        color = legend_colormap[
+                            legend_color_mapping.index(score_ranges[i + 1])
+                            % len(legend_colormap)
+                        ]
+                        legend += "{}".format(color)
+                        legend += "   {} - {}".format(
+                            score_ranges[i], score_ranges[i + 1]
+                        )
+                        legend += "{}".format(self.colors_annotations.end)
+                else:  # no color map passed in
+                    for i in range(len(score_ranges) - 1):
+                        legend += "   {} - {}".format(
+                            score_ranges[i], score_ranges[i + 1]
+                        )
+
+        return legend
+
     def render_frame(self, node, dataframe, indent="", child_indent=""):
         node_depth = node._depth
         if node_depth < self.depth:
             df_index = node
             node_metric = dataframe.loc[df_index, self.primary_metric]
 
             metric_precision = "{:." + str(self.precision) + "f}"
```

### Comparing `llnl-thicket-2023.3.1/thicket/helpers.py` & `llnl-thicket-2024.1.0/thicket/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
-import copy
-
+from more_itertools import powerset
 import pandas as pd
 
 
 def _are_synced(gh, df):
     """Check if node objects are equal in graph and dataframe id(graph_node) ==
     id(df_node).
     """
@@ -121,77 +120,27 @@
         for idx in idx_set:
             if idx not in th.dataframe.index.names:
                 print(f"Resolving '{idx}' in thicket: ({id(th)})")
                 th.dataframe[idx] = 0
                 th.dataframe.set_index(idx, append=True, inplace=True)
 
 
-def _sync_nodes(gh, df):
-    """Set the node objects to be equal in both the graph and the dataframe.
-
-    Operations: (n tree nodes) X (m df nodes) X (m)
+def _set_node_ordering(thickets):
+    """Set node ordering for each thicket in a list. All thickets must have node ordering on, otherwise it will be set to False.
 
-    id(graph_node) == id(df_node) after this function for nodes with equivalent hatchet
-    nid's.
+    Arguments:
+        thickets (list): list of Thicket objects
     """
-    index_names = df.index.names
-    df.reset_index(inplace=True)
-    for graph_node in gh.traverse():
-        df["node"] = df["node"].apply(
-            lambda df_node: graph_node
-            if (hash(graph_node) == hash(df_node))
-            else df_node
-        )
-    df.set_index(index_names, inplace=True)
-
-
-def _sync_nodes_frame(gh, df):
-    """Update dataframe node objects hnid's based off their positioning relative to a
-    given graph.
-
-    id(graph_node) == id(df_node) after this function for nodes with equivalent hatchet
-    nid's.
-
-    TODO: This function may be superior to _sync_nodes and may be able to replace it.
-    Need to investigate.
-    """
-
-    # TODO: Graph function to list conversion: move to Hatchet?
-    gh_node_list = []
-    for gh_node in gh.traverse():
-        gh_node_list.append(gh_node)
-    # Sort the graph node list
-    gh_node_list.sort(key=lambda node: hash(node))
-
-    index_names = df.index.names
-    df_node_list = list(set(df.index.get_level_values("node")))
-    df_node_list_cp = copy.deepcopy(df_node_list)
-    # Check list sorted
-    assert sorted(df_node_list, key=lambda node: hash(node))
+    node_order = all([tk.graph.node_ordering for tk in thickets])
 
-    # Sequentially walk through graph and dataframe and modify dataframe hnid's based off graph equivalent
-    i = 0
-    j = 0
-    while i < len(gh_node_list) and j < len(df_node_list):
-        if gh_node_list[i].frame == df_node_list[j].frame:
-            df_node_list[j] = gh_node_list[i]
-            j += 1
-        else:
-            i += 1
-
-    # Extend list to match multi-index dataframe structure
-    df_list_full = []
-    for i, node in enumerate(df_node_list):
-        num_profiles = len(df.loc[df_node_list_cp[i]])
-        df_list_full.extend([node] * num_profiles)
-    # Update nodes in the dataframe
-    df.reset_index(inplace=True)
-    df["node"] = df_list_full
-
-    df.set_index(index_names, inplace=True)
+    for tk in thickets:
+        if tk.graph.node_ordering:
+            tk.graph.node_ordering = node_order
+            # Have to re-enumerate the traverse
+            tk.graph.enumerate_traverse()
 
 
 def _get_perf_columns(df):
     """Get list of performance dataframe columns that are numeric.
 
     Numeric columns can be used with thicket's statistical functions.
 
@@ -210,7 +159,12 @@
         if "nid" in numeric_columns:
             numeric_columns.remove("nid")
 
         return numeric_columns
     # columnar joined thicket object
     else:
         return [x for x in numeric_columns if "nid" not in x]
+
+
+def _powerset_from_tuple(tup):
+    pset = [y for y in powerset(tup)]
+    return {x[0] if len(x) == 1 else x for x in pset}
```

### Comparing `llnl-thicket-2023.3.1/thicket/model_extrap.py` & `llnl-thicket-2024.1.0/thicket/model_extrap.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/ncu.py` & `llnl-thicket-2024.1.0/thicket/ncu.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/calc_boxplot_statistics.py` & `llnl-thicket-2024.1.0/thicket/stats/calc_boxplot_statistics.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/check_normality.py` & `llnl-thicket-2024.1.0/thicket/stats/check_normality.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/correlation_nodewise.py` & `llnl-thicket-2024.1.0/thicket/stats/correlation_nodewise.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/display_boxplot.py` & `llnl-thicket-2024.1.0/thicket/stats/display_boxplot.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 #
 # SPDX-License-Identifier: MIT
 
 import pandas as pd
 import seaborn as sns
 import hatchet as ht
 
+import thicket as th
 from ..utils import verify_thicket_structures
 
 
-def display_boxplot(thicket, nodes=[], columns=[], **kwargs):
+def display_boxplot(thicket, nodes=None, columns=None, **kwargs):
     """Display a boxplot for each user passed node(s) and column(s). The passed nodes
     and columns must be from the performance data table.
 
     Designed to take in a thicket, and display a plot with one or more boxplots
     depending on the number of nodes and columns passed.
 
     Arguments:
@@ -23,14 +24,26 @@
         column (list): List of hardware/timing metrics to view on the y-axis. Note, if
             using a columnar joined thicket a list of tuples must be passed in with the
             format (column index, column name).
 
     Returns:
         (matplotlib Axes): Object for managing boxplot.
     """
+    if columns is None or nodes is None:
+        raise ValueError(
+            "Both 'nodes' and 'columns' must be provided. To see a list of valid columns, run 'Thicket.performance_cols'."
+        )
+    if not isinstance(thicket, th.Thicket):
+        raise ValueError(
+            "Value passed to 'thicket' argument must be of type thicket.Thicket."
+        )
+    if not isinstance(nodes, list):
+        raise ValueError("Value passed to 'nodes' argument must be of type list.")
+    if not isinstance(columns, list):
+        raise ValueError("Value passed to 'columns' argument must be of type list.")
     for node in nodes:
         if not isinstance(node, ht.node.Node):
             raise ValueError(
                 "Value(s) passed to node argument must be of type hatchet.node.Node."
             )
 
     verify_thicket_structures(thicket.dataframe, index=["node"], columns=columns)
```

### Comparing `llnl-thicket-2023.3.1/thicket/stats/display_heatmap.py` & `llnl-thicket-2024.1.0/thicket/stats/display_heatmap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import seaborn as sns
 
+import thicket as th
 from ..utils import verify_thicket_structures
 
 
 def display_heatmap(thicket, columns=None, **kwargs):
     """Display a heatmap which contains a full list of nodes and user passed columns.
     Columns must be from the aggregated statistics table.
 
     Arguments:
         thicket (thicket): Thicket object
         columns (list): List of hardware/timing metrics from aggregated statistics table
-            to display. Note, if using a columnar joined thicket a list of tuples must
-            be passed in with the format (column index, column name).
+            to display. Note: if using a column thicket, the argument must be a tuple.
 
     Returns:
         (matplotlib Axes): Object for managing heatmap plot.
     """
     if columns is None:
         raise ValueError(
-            "To see a list of valid columns, run 'Thicket.performance_cols'."
+            "Chosen columns must be from the thicket.statsframe.dataframe."
         )
+    if not isinstance(thicket, th.Thicket):
+        raise ValueError(
+            "Value passed to 'thicket' argument must be of type thicket.Thicket."
+        )
+    if not isinstance(columns, list):
+        raise ValueError("Value passed to 'columns' argument must be of type list.")
 
     verify_thicket_structures(
         thicket.statsframe.dataframe, index=["node"], columns=columns
     )
 
     # thicket object without columnar index
     if thicket.dataframe.columns.nlevels == 1:
```

### Comparing `llnl-thicket-2023.3.1/thicket/stats/display_histogram.py` & `llnl-thicket-2024.1.0/thicket/stats/display_histogram.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,54 @@
 # Copyright 2022 Lawrence Livermore National Security, LLC and other
 # Thicket Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
-import pandas as pd
-import seaborn as sns
 import hatchet as ht
 
+import thicket as th
 from ..utils import verify_thicket_structures
 
 
 def display_histogram(thicket, node=None, column=None, **kwargs):
     """Display a histogram for a user passed node and column. Node and column must come
     from the performance data table.
 
     Arguments:
         thicket (thicket): Thicket object
         node (node): Node object
-        column (str): Column from performance data table. Note, if using a
-            columnar joined thicket a tuple must be passed in with the format
-            (column index, column name).
+        column (str): Column from performance data table. Note: if using a
+            column thicket, the argument must be a tuple.
 
     Returns:
-        (matplotlib Axes): Object for managing histogram plot.
+        (matplotlib.AxesSubplot or numpy.ndarray of them)
     """
+
     if column is None or node is None:
         raise ValueError(
-            "To see a list of valid columns, run 'Thicket.performance_cols'."
+            "Both 'node' and 'column' must be provided. To see a list of valid columns, run 'Thicket.performance_cols'."
+        )
+    if not isinstance(thicket, th.Thicket):
+        raise ValueError(
+            "Value passed to 'thicket' argument must be of type thicket.Thicket."
         )
-
     if not isinstance(node, ht.node.Node):
         raise ValueError(
-            "Value passed to node argument must be of type hatchet.node.Node."
+            "Value passed to 'node' argument must be of type hatchet.node.Node."
+        )
+    if not isinstance(column, (str, tuple)):
+        raise ValueError(
+            "Value passed to column argument must be of type str (or tuple(str) for column thickets)."
         )
 
     verify_thicket_structures(thicket.dataframe, index=["node"], columns=[column])
 
     # thicket object without columnar index
     if thicket.dataframe.columns.nlevels == 1:
-        df = pd.melt(
-            thicket.dataframe.reset_index(),
-            id_vars="node",
-            value_vars=column,
-            value_name=" ",
-        )
-
-        filtered_df = df[df["node"] == node]
-
-        ax = sns.displot(filtered_df, x=" ", kind="hist", **kwargs)
+        ax = thicket.dataframe.loc[node].hist(column=column, **kwargs)
 
         return ax
     # columnar joined thicket object
     else:
-        col_idx, column_value = column[0], column[1]
-        df_subset = thicket.dataframe[col_idx]
-
-        df = pd.melt(
-            df_subset.reset_index(),
-            id_vars="node",
-            value_vars=column_value,
-            value_name=" ",
-        )
-
-        filtered_df = df[df["node"] == node]
-
-        ax = sns.displot(filtered_df, x=" ", kind="hist", **kwargs)
+        ax = thicket.dataframe.loc[node].hist(column=column, **kwargs)
 
         return ax
```

### Comparing `llnl-thicket-2023.3.1/thicket/stats/maximum.py` & `llnl-thicket-2024.1.0/thicket/stats/maximum.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/mean.py` & `llnl-thicket-2024.1.0/thicket/stats/mean.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/median.py` & `llnl-thicket-2024.1.0/thicket/stats/median.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/minimum.py` & `llnl-thicket-2024.1.0/thicket/stats/minimum.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/preference.py` & `llnl-thicket-2024.1.0/thicket/stats/preference.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,22 @@
 
 def preference(thicket, columns, comparison_func, test="ttest", *args, **kwargs):
     """Determine a preference between compilers, architecture, platform, etc.
 
     Designed to take in a thicket and will append eight total columns to the
     aggregated statistics table. As a note, preferred will stand for the preferred
     choice between two options.
-        1. columns[0] mean
-        2. columns[0] std
-        3. columns[1] mean
-        4. columns[1] std
-        5. columns[0] + columns[1] tvalue
-        6. columns[0] + columns[1] tstatistic
-        7. columns[0] + columns[1] std preferred
-        8. columns[0] + columns[1] mean preferred
-
-    Column names will have the following two formats:
-        1. <column_name>_{std,mean}
-        2. <column_name> vs <column_name>_{tvalue,tstatistic,preferred}
+        - <columns[0]>_mean
+        - <columns[0]>_std
+        - <columns[1]>_mean
+        - <columns[1]>_std
+        - <columns[0]> vs <columns[1]>_tvalue
+        - <columns[0]> vs <columns[1]>_tstatistic
+        - <columns[0]> vs <columns[1]>_std_preferred
+        - <columns[0]> vs <columns[1]>_mean_preferred
 
     Arguments:
         thicket (thicket): Thicket object
         columns (list): List of hardware/timing metrics to determine a preference for.
             Note, if using a columnar joined thicket a list of tuples must be passed in
             with the format (column index, column name). List should be length 2.
         comparison_func (function): User-defined python or lambda function to decide a
```

### Comparing `llnl-thicket-2023.3.1/thicket/stats/std.py` & `llnl-thicket-2024.1.0/thicket/stats/std.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/stats/ttest.py` & `llnl-thicket-2024.1.0/thicket/stats/ttest.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     # nobs for parameter two for ttest
     nobs_column2 = len(thicket.dataframe.loc[n][columns[0]])
 
     # subtract by len(columns) due to estimating a t-test with two parameters
     # alpha/2 is done for a two tail t-test
     tvalue = t.ppf(q=1 - alpha / 2, df=nobs_column1 + nobs_column2 - len(columns))
 
-    th.mean(thicket, columns)
-    th.std(thicket, columns)
+    th.stats.mean(thicket, columns)
+    th.stats.std(thicket, columns)
 
     # thicket object with columnar index
     if thicket.dataframe.columns.nlevels > 1:
         mean_columns = [(idx, col + "_mean") for idx, col in columns]
         std_columns = [(idx, col + "_std") for idx, col in columns]
         t_statistics = []
         for i in range(0, len(thicket.statsframe.dataframe)):
```

### Comparing `llnl-thicket-2023.3.1/thicket/stats/variance.py` & `llnl-thicket-2024.1.0/thicket/stats/variance.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/thicket.py` & `llnl-thicket-2024.1.0/thicket/thicket.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 # SPDX-License-Identifier: MIT
 
 import copy
 import os
 import sys
 import json
 import warnings
-from collections import OrderedDict
+from collections import defaultdict, OrderedDict
 from hashlib import md5
 
 import pandas as pd
 import numpy as np
 from hatchet import GraphFrame
+from hatchet.graph import Graph
 from hatchet.query import AbstractQuery, QueryMatcher
+import tqdm
 
 from thicket.ensemble import Ensemble
 import thicket.helpers as helpers
-from .utils import verify_thicket_structures
+from .groupby import GroupBy
+from .utils import (
+    verify_thicket_structures,
+    check_duplicate_metadata_key,
+    validate_profile,
+    validate_nodes,
+)
 from .external.console import ThicketRenderer
 
 
 class Thicket(GraphFrame):
     """Ensemble of profiles, includes a graph and three dataframes, performance data,
     metadata, and aggregated statistics.
     """
@@ -121,14 +129,28 @@
             + "\n"
             + self.statsframe.dataframe
         )
 
         return s
 
     @staticmethod
+    def profile_hasher(obj, hex_len=8):
+        """Convert an object to a profile hash for Thicket.
+
+        Arguments:
+            obj (object): hashable object
+            hex_len (int): length of the hex string before being converted to an integer.
+
+        Returns:
+            (int): hash of the object
+        """
+
+        return int(md5(obj.encode("utf-8")).hexdigest()[:hex_len], 16)
+
+    @staticmethod
     def thicketize_graphframe(gf, prf):
         """Necessary function to handle output from using GraphFrame readers.
 
         Arguments:
             gf (GraphFrame): hatchet GraphFrame object
             prf (str): profile source of the GraphFrame
 
@@ -144,18 +166,15 @@
         )
 
         if th.profile is None and isinstance(prf, str):
             # Store used profiles and profile mappings using a truncated md5 hash of their string.
             # Resulting int hash will be at least hex_length digits and theoretically up to
             # ceil(log_10(16^n - 1)) digits after conversion.
 
-            # length of the hex string before being converted to an integer.
-            hex_length = 8
-
-            hash_arg = int(md5(prf.encode("utf-8")).hexdigest()[:hex_length], 16)
+            hash_arg = Thicket.profile_hasher(prf)
             th.profile = [hash_arg]
             th.profile_mapping = OrderedDict({hash_arg: prf})
 
             # format metadata as a dict of dicts
             temp_meta = {}
             temp_meta[hash_arg] = th.metadata
             th.metadata = pd.DataFrame.from_dict(temp_meta, orient="index")
@@ -167,83 +186,139 @@
             index_names.insert(1, "profile")
             th.dataframe.reset_index(inplace=True)
             th.dataframe.set_index(index_names, inplace=True)
 
         return th
 
     @staticmethod
-    def from_caliper(filename_or_stream, query=None, intersection=False):
+    def from_caliper(
+        filename_or_stream, query=None, intersection=False, disable_tqdm=False
+    ):
         """Read in a Caliper .cali or .json file.
 
         Arguments:
             filename_or_stream (str or file-like): name of a Caliper output file in
                 `.cali` or JSON-split format, or an open file object to read one
             query (str): cali-query in CalQL format
             intersection (bool): whether to perform intersection or union (default)
+            disable_tqdm (bool): whether to display tqdm progress bar
         """
         return Thicket.reader_dispatch(
-            GraphFrame.from_caliper, intersection, filename_or_stream, query
+            GraphFrame.from_caliper,
+            intersection,
+            disable_tqdm,
+            filename_or_stream,
+            query,
         )
 
     @staticmethod
-    def from_hpctoolkit(dirname, intersection=False):
+    def from_hpctoolkit(dirname, intersection=False, disable_tqdm=False):
         """Create a GraphFrame using hatchet's HPCToolkit reader and use its attributes
         to make a new thicket.
 
         Arguments:
             dirname (str): parent directory of an HPCToolkit experiment.xml file
             intersection (bool): whether to perform intersection or union (default)
+            disable_tqdm (bool): whether to display tqdm progress bar
 
         Returns:
             (thicket): new thicket containing HPCToolkit profile data
         """
         return Thicket.reader_dispatch(
-            GraphFrame.from_hpctoolkit, intersection, dirname
+            GraphFrame.from_hpctoolkit, intersection, disable_tqdm, dirname
         )
 
     @staticmethod
-    def from_caliperreader(filename_or_caliperreader, intersection=False):
+    def from_caliperreader(
+        filename_or_caliperreader, intersection=False, disable_tqdm=False
+    ):
         """Helper function to read one caliper file.
 
         Arguments:
             filename_or_caliperreader (str or CaliperReader): name of a Caliper output
                 file in `.cali` format, or a CaliperReader object
             intersection (bool): whether to perform intersection or union (default)
+            disable_tqdm (bool): whether to display tqdm progress bar
         """
         return Thicket.reader_dispatch(
-            GraphFrame.from_caliperreader, intersection, filename_or_caliperreader
+            GraphFrame.from_caliperreader,
+            intersection,
+            disable_tqdm,
+            filename_or_caliperreader,
         )
 
     @staticmethod
-    def reader_dispatch(func, intersection=False, *args, **kwargs):
+    def from_literal(graph_dict):
+        """Create a Thicket from a list of dictionarires.
+
+        Arguments:
+            graph_dict (list): list of dictionaries representing a graph
+
+        Returns:
+            (Thicket): new Thicket
+
+        Example:
+            graph_dict = [
+                {
+                    "frame": {"name": "Foo", "type": "function"},
+                    "metrics": {"memory": 30.0, "time": 0.1},
+                    "children": [
+                        {
+                            "frame": {"name": "Bar", "type": "function"},
+                            "metrics": {"memory": 11.0, "time": 5.0},
+                            "children": [],
+                        },
+                    ],
+                },
+                {
+                    "frame": {"name": "Baz", "type": "function"},
+                    "metrics": {"memory": 6.0, "time": 5.0},
+                    "children": [],
+                },
+            ]
+        """
+        profile = str(graph_dict)
+
+        tk = Thicket.thicketize_graphframe(GraphFrame.from_literal(graph_dict), profile)
+
+        return tk
+
+    @staticmethod
+    def reader_dispatch(func, intersection, disable_tqdm, *args, **kwargs):
         """Create a thicket from a list, directory of files, or a single file.
 
         Arguments:
             func (function): reader function to be used
             intersection (bool): whether to perform intersection or union (default).
+            tdmq_output (bool): whether to display tqdm progress bar
             args (list): list of args; args[0] should be an object that can be read from
         """
         ens_list = []
         obj = args[0]  # First arg should be readable object
         extra_args = []
         if len(args) > 1:
             extra_args = args[1:]
+        pbar_desc = "(1/2) Reading Files"
 
         # Parse the input object
         # if a list of files
         if isinstance(obj, (list, tuple)):
-            for file in obj:
+            pbar = tqdm.tqdm(obj, disable=disable_tqdm)
+            for file in pbar:
+                pbar.set_description(pbar_desc)
                 ens_list.append(
                     Thicket.thicketize_graphframe(
                         func(file, *extra_args, **kwargs), file
                     )
                 )
         # if directory of files
         elif os.path.isdir(obj):
-            for file in os.listdir(obj):
+            pbar = tqdm.tqdm(os.listdir(obj), disable=disable_tqdm)
+            for file in pbar:
+                pbar.set_description(pbar_desc)
                 f = os.path.join(obj, file)
                 ens_list.append(
                     Thicket.thicketize_graphframe(func(f, *extra_args, **kwargs), f)
                 )
         # if single file
         elif os.path.isfile(obj):
             return Thicket.thicketize_graphframe(func(*args, **kwargs), args[0])
@@ -262,59 +337,67 @@
         calltree = "union"
         if intersection:
             calltree = "intersection"
         thicket_object = Thicket.concat_thickets(
             thickets=ens_list,
             axis="index",
             calltree=calltree,
+            disable_tqdm=disable_tqdm,
         )
 
         return thicket_object
 
     @staticmethod
-    def concat_thickets(thickets, axis="index", calltree="union", **kwargs):
-        """Concatenate thickets together on index or columns. The calltree can either be unioned or
-        intersected which will affect the other structures.
+    def concat_thickets(
+        thickets, axis="index", calltree="union", disable_tqdm=False, **kwargs
+    ):
+        """Concatenate thickets together on index or columns.
+
+        The calltree can either be unioned or intersected which will affect the other structures.
 
         Arguments:
             thickets (list): list of thicket objects
             axis (str): axis to concatenate on -> "index" or "column"
             calltree (str): calltree to use -> "union" or "intersection"
 
-            valid kwargs:
-                if axis="index":
-                    from_statsframes (bool): Whether this method was invoked from from_statsframes
-                if axis="columns":
-                    headers (list): List of headers to use for the new columnar multi-index.
-                    metadata_key (str): Name of the column from the metadata tables to replace the 'profile'
+        Keyword Arguments:
+            headers (list): (if axis="columns") List of headers to use for the new columnar multi-index
+            metadata_key (str): (if axis="columns") Name of the column from the metadata tables to replace the 'profile'
                 index. If no argument is provided, it is assumed that there is no profile-wise
                 relationship between the thickets.
 
         Returns:
             (thicket): concatenated thicket
         """
 
-        def _index(thickets, from_statsframes=False):
+        def _index(thickets, from_statsframes=False, disable_tqdm=disable_tqdm):
             thicket_parts = Ensemble._index(
-                thickets=thickets, from_statsframes=from_statsframes
+                thickets=thickets,
+                from_statsframes=from_statsframes,
+                disable_tqdm=disable_tqdm,
             )
 
             return Thicket(
                 graph=thicket_parts[0],
                 dataframe=thicket_parts[1],
                 exc_metrics=thicket_parts[2],
                 inc_metrics=thicket_parts[3],
                 metadata=thicket_parts[4],
                 profile=thicket_parts[5],
                 profile_mapping=thicket_parts[6],
             )
 
-        def _columns(thickets, headers=None, metadata_key=None):
+        def _columns(
+            thickets, headers=None, metadata_key=None, disable_tqdm=disable_tqdm
+        ):
             combined_thicket = Ensemble._columns(
-                thickets=thickets, headers=headers, metadata_key=metadata_key
+                thickets=thickets,
+                headers=headers,
+                metadata_key=metadata_key,
+                disable_tqdm=disable_tqdm,
             )
 
             return combined_thicket
 
         if calltree not in ["union", "intersection"]:
             raise ValueError("calltree must be 'union' or 'intersection'")
 
@@ -413,66 +496,170 @@
             self.metadata[metadata_key], on=self.dataframe.index.names[1]
         )
 
         # Drop column
         if drop:
             self.metadata.drop(metadata_key, axis=1, inplace=True)
 
-    def squash(self, update_inc_cols=True):
+    def squash(self, update_inc_cols=True, new_statsframe=True):
         """Rewrite the Graph to include only nodes present in the performance
         data table's rows.
 
         This can be used to simplify the Graph, or to normalize Graph indexes between
         two Thickets.
 
         Arguments:
             update_inc_cols (boolean, optional): if True, update inclusive columns.
+            new_statsframe (boolean, optional): if True, create a new statsframe from the new dataframe. Only set to False if the statsframe nodes equal the dataframe nodes.
 
         Returns:
-            (Thicket): a newly squashed Thicket object
+            (thicket): a newly squashed Thicket object
         """
-        squashed_gf = GraphFrame.squash(self, update_inc_cols=update_inc_cols)
-        new_graph = squashed_gf.graph
-        # The following code updates the performance data and the aggregated statistics
-        # table with the remaining (re-indexed) nodes. The dataframe is internally
-        # updated in squash(), so we can easily just save it to our thicket performance
-        # data. For the aggregated statistics table, we'll have to come up with a better
-        # way eventually, but for now, we'll just create a new aggregated statistics
-        # table the same way we do when we create a new thicket.
-        new_dataframe = squashed_gf.dataframe
+
+        #####
+        # Hatchet's squash code
+        #####
+        index_names = self.dataframe.index.names
+        self.dataframe.reset_index(inplace=True)
+
+        # create new nodes for each unique node in the old dataframe
+        old_to_new = {n: n.copy() for n in set(self.dataframe["node"])}
+        for i in old_to_new:
+            old_to_new[i]._hatchet_nid = i._hatchet_nid
+
+        # Maintain sets of connections to make for each old node.
+        # Start with old -> new mapping and update as we traverse subgraphs.
+        connections = defaultdict(lambda: set())
+        connections.update({k: {v} for k, v in old_to_new.items()})
+
+        new_roots = []  # list of new roots
+
+        # connect new nodes to children according to transitive
+        # relationships in the old graph.
+        def rewire(node, new_parent, visited):
+            # make all transitive connections for the node we're visiting
+            for n in connections[node]:
+                if new_parent:
+                    # there is a parent in the new graph; connect it
+                    if n not in new_parent.children:
+                        new_parent.add_child(n)
+                        n.add_parent(new_parent)
+
+                elif n not in new_roots:
+                    # this is a new root
+                    new_roots.append(n)
+
+            new_node = old_to_new.get(node)
+            transitive = set()
+            if node not in visited:
+                visited.add(node)
+                for child in node.children:
+                    transitive |= rewire(child, new_node or new_parent, visited)
+
+            if new_node:
+                # since new_node exists in the squashed graph, we only
+                # need to connect new_node
+                return {new_node}
+            else:
+                # connect parents to the first transitively reachable
+                # new_nodes of nodes we're removing with this squash
+                connections[node] |= transitive
+                return connections[node]
+
+        # run rewire for each root and make a new graph
+        visited = set()
+        for root in self.graph.roots:
+            rewire(root, None, visited)
+        graph = Graph(new_roots)
+        if self.graph.node_ordering:
+            graph.node_ordering = True
+        graph.enumerate_traverse()
+
+        # reindex new dataframe with new nodes
+        df = self.dataframe.copy()
+        df["node"] = df["node"].apply(lambda x: old_to_new[x])
+
+        # at this point, the graph is potentially invalid, as some nodes
+        # may have children with identical frames.
+        merges = graph.normalize()
+        df["node"] = df["node"].apply(lambda n: merges.get(n, n))
+
+        self.dataframe.set_index(index_names, inplace=True)
+        df.set_index(index_names, inplace=True)
+        # create dict that stores aggregation function for each column
+        agg_dict = {}
+        for col in df.columns.tolist():
+            if col in self.exc_metrics + self.inc_metrics:
+                # use min_count=1 (default is 0) here, so sum of an all-NA
+                # series is NaN, not 0
+                # when min_count=1, sum([NaN, NaN)] = NaN
+                # when min_count=0, sum([NaN, NaN)] = 0
+                agg_dict[col] = lambda x: x.sum(min_count=1)
+            else:
+                agg_dict[col] = lambda x: x.iloc[0]
+
+        # perform a groupby to merge nodes with the same callpath
+        agg_df = df.groupby(index_names).agg(agg_dict)
+        agg_df.sort_index(inplace=True)
+
+        #####
+        # Thicket's squash code
+        #####
         multiindex = False
         if isinstance(self.statsframe.dataframe.columns, pd.MultiIndex):
             multiindex = True
-        stats_df = helpers._new_statsframe_df(new_dataframe, multiindex=multiindex)
-        sframe = GraphFrame(
-            graph=new_graph,
-            dataframe=stats_df,
-        )
-        return Thicket(
-            new_graph,
-            new_dataframe,
+
+        if new_statsframe:
+            stats_df = helpers._new_statsframe_df(agg_df, multiindex=multiindex)
+            sframe = GraphFrame(
+                graph=graph,
+                dataframe=stats_df,
+            )
+        else:
+            # Update the node objects in the old statsframe.
+            sframe = self.statsframe
+            sframe.dataframe = sframe.dataframe.reset_index()
+            replace_dict = {}
+            for node in sframe.dataframe["node"]:
+                if node in old_to_new:
+                    replace_dict[node] = old_to_new[node]
+            sframe.dataframe["node"] = sframe.dataframe["node"].replace(replace_dict)
+            sframe.dataframe = sframe.dataframe.set_index("node")
+
+        new_tk = Thicket(
+            graph,
+            agg_df,
             exc_metrics=self.exc_metrics,
             inc_metrics=self.inc_metrics,
             default_metric=self.default_metric,
             metadata=self.metadata,
             profile=self.profile,
             profile_mapping=self.profile_mapping,
             statsframe=sframe,
         )
 
+        if update_inc_cols:
+            new_tk.update_inclusive_columns()
+
+        new_tk._sync_profile_components(new_tk.dataframe)
+        validate_profile(new_tk)
+        validate_nodes(new_tk)
+
+        return new_tk
+
     def copy(self):
         """Return a partially shallow copy of the Thicket.
 
         See GraphFrame.copy() for more details
 
         Arguments:
             self (Thicket): object to make a copy of
 
         Returns:
-            other (Thicket): copy of self
+            other (thicket): copy of self
                 (graph ... default_metric): Same behavior as GraphFrame
                 metadata (DataFrame): pandas "non-deep" copy of dataframe
                 profile (list): copy of self's profile
                 profile_mapping (dict): copy of self's profile_mapping
                 statsframe (GraphFrame): calls GraphFrame.copy()
         """
         gf = GraphFrame.copy(self)
@@ -494,15 +681,15 @@
 
         See GraphFrame.deepcopy() for more details
 
         Arguments:
             self (Thicket): object to make a copy of
 
         Returns:
-            other (Thicket): copy of self
+            other (thicket): copy of self
                 (graph ... default_metric): same behavior as GraphFrame
                 metadata (DataFrame): pandas "deep" copy of dataframe
                 profile (list): copy of self's profile
                 profile_mapping (dict): copy of self's profile_mapping
                 statsframe (GraphFrame): Calls GraphFrame.deepcopy()
         """
         gf = GraphFrame.deepcopy(self)
@@ -533,14 +720,15 @@
         highlight_name=False,
         colormap="RdYlGn",
         invert_colormap=False,
         colormap_annotations=None,
         render_header=True,
         min_value=None,
         max_value=None,
+        indices=None,
     ):
         """Visualize the Thicket as a tree
 
         Arguments:
             metric_column (str, tuple, list, optional): Columns to use the metrics from. Defaults to None.
             annotation_column (str, optional): Column to use as an annotation. Defaults to None.
             precision (int, optional): Precision of shown numbers. Defaults to 3.
@@ -553,17 +741,18 @@
             highlight_name (bool, optional): Highlights the names of the nodes. Defaults to False.
             colormap (str, optional): Specifies a colormap to use. Defaults to "RdYlGn".
             invert_colormap (bool, optional): Reverts the chosen colormap. Defaults to False.
             colormap_annotations (str, list, dict, optional): Either provide the name of a colormap, a list of colors to use or a dictionary which maps the used annotations to a color. Defaults to None.
             render_header (bool, optional): Shows the Preamble. Defaults to True.
             min_value (int, optional): Overwrites the min value for the coloring legend. Defaults to None.
             max_value (int, optional): Overwrites the max value for the coloring legend. Defaults to None.
+            indices(tuple, list, optional): Index/indices to display on the DataFrame. Defaults to None.
 
         Returns:
-            str: String representation of the tree, ready to print
+            (str): String representation of the tree, ready to print
         """
         color = sys.stdout.isatty()
         shell = None
         if metric_column is None:
             metric_column = self.default_metric
 
         if color is False:
@@ -578,17 +767,62 @@
                 color = True
 
         if sys.version_info.major == 2:
             unicode = False
         elif sys.version_info.major == 3:
             unicode = True
 
+        if indices is None:
+            # Create slice out of first values found starting after the first index.
+            indices = self.dataframe.index[0][1:]
+        elif isinstance(indices, tuple):
+            pass
+        elif isinstance(indices, list):  # Convert list to tuple
+            indices = tuple(indices)
+        else:  # Support for non-iterable types (int, str, ...)
+            try:
+                indices = tuple([indices])
+            except TypeError:
+                raise TypeError(
+                    f"Value provided to 'indices' = {indices} is an unsupported type {type(indices)}"
+                )
+        # For tree legend
+        idx_dict = {
+            self.dataframe.index.names[k + 1]: indices[k] for k in range(len(indices))
+        }
+        # Slices the DataFrame to simulate a single-level index
+        try:
+            slice_df = (
+                self.dataframe.loc[(slice(None),) + indices, :]
+                .reset_index()
+                .set_index("node")
+            )
+        except KeyError:
+            missing_indices = {
+                list(idx_dict.keys())[i]: idx
+                for i, idx in enumerate(indices)
+                if all(idx not in df_idx[1:] for df_idx in self.dataframe.index)
+            }
+            raise KeyError(
+                f"The indices, {missing_indices}, do not exist in the index 'self.dataframe.index'"
+            )
+        # Check for compatibility
+        if len(slice_df) != len(self.graph):
+            raise KeyError(
+                f"Either dataframe cannot be represented as a single index or provided slice, '{indices}' results in a multi-index. See self.dataframe.loc[(slice(None),)+{indices},{metric_column}]"
+            )
+
+        # Prep DataFrame by filling None rows in the "name" column with the node's name.
+        slice_df["name"] = [
+            n.frame["name"] for n in slice_df.index.get_level_values("node")
+        ]
+
         return ThicketRenderer(unicode=unicode, color=color).render(
             self.graph.roots,
-            self.statsframe.dataframe,
+            slice_df,
             metric_column=metric_column,
             annotation_column=annotation_column,
             precision=precision,
             name_column=name_column,
             expand_name=expand_name,
             context_column=context_column,
             rank=rank,
@@ -597,87 +831,85 @@
             highlight_name=highlight_name,
             colormap=colormap,
             invert_colormap=invert_colormap,
             colormap_annotations=colormap_annotations,
             render_header=render_header,
             min_value=min_value,
             max_value=max_value,
+            indices=idx_dict,
         )
 
     @staticmethod
-    def from_statsframes(th_list, metadata_key=None):
+    def from_statsframes(tk_list, metadata_key=None, disable_tqdm=False):
         """Compose a list of Thickets with data in their statsframes.
 
         The Thicket's individual aggregated statistics tables are ensembled and become the
-        new Thickets performance data table.
+        new Thickets performance data table. This also results in aggregation of the metadata.
 
         Arguments:
-            th_list (list): list of thickets
+            tk_list (list): list of thickets
             metadata_key (str, optional): name of the metadata column to use as
                 the new second-level index. Uses the first value so this only makes
                 sense if provided column is all equal values and each thicket's columns
                 differ in value.
 
         Returns:
             (thicket): New Thicket object.
         """
         # Pre-check of data structures
-        for th in th_list:
+        for tk in tk_list:
             verify_thicket_structures(
-                th.dataframe, index=["node", "profile"]
+                tk.dataframe, index=["node", "profile"]
             )  # Required for deepcopy operation
             verify_thicket_structures(
-                th.statsframe.dataframe, index=["node"]
+                tk.statsframe.dataframe, index=["node"]
             )  # Required for deepcopy operation
 
         # Setup names list
-        th_names = []
+        tk_names = []
         if metadata_key is None:
-            for i in range(len(th_list)):
-                th_names.append(i)
+            idx_name = "profile"  # Set index name to general "profile"
+            for i in range(len(tk_list)):
+                tk_names.append(i)
         else:  # metadata_key was provided.
-            for th in th_list:
+            check_duplicate_metadata_key(tk_list, metadata_key)
+            idx_name = metadata_key  # Set index name to metadata_key
+            for tk in tk_list:
                 # Get name from metadata table
-                name_list = th.metadata[metadata_key].tolist()
+                name_list = tk.metadata[metadata_key].tolist()
 
-                if len(name_list) > 1:
+                if len(set(name_list)) > 1:
                     warnings.warn(
-                        f"Multiple values for name {name_list} at thicket.metadata[{metadata_key}]. Only the first will be used."
+                        f"Multiple values for name {name_list} at thicket.metadata['{metadata_key}']. Only the first value will be used for the new DataFrame index."
                     )
-                th_names.append(name_list[0])
+                tk_names.append(name_list[0])
 
-        th_copy_list = []
-        for i in range(len(th_list)):
-            th_copy = th_list[i].deepcopy()
+        tk_copy_list = []
+        for i in range(len(tk_list)):
+            tk_copy = tk_list[i].deepcopy()
 
-            th_id = th_names[i]
+            tk_id = tk_names[i]
 
-            if metadata_key is None:
-                idx_name = "profile"
-            else:
-                idx_name = metadata_key
-
-            # Modify graph
-            # Necessary so node ids match up
-            th_copy.graph = th_copy.statsframe.graph
+            # Modify graph. Necessary so node ids match up
+            tk_copy.graph = tk_copy.statsframe.graph
 
             # Modify the performance data table
-            df = th_copy.statsframe.dataframe
-            df[idx_name] = th_id
+            df = tk_copy.statsframe.dataframe
+            df[idx_name] = tk_id
             df.set_index(idx_name, inplace=True, append=True)
-            th_copy.dataframe = df
+            tk_copy.dataframe = df
 
             # Adjust profile and profile_mapping
-            th_copy.profile = [th_id]
-            profile_paths = list(th_copy.profile_mapping.values())
-            th_copy.profile_mapping = OrderedDict({th_id: profile_paths})
+            tk_copy.profile = [tk_id]
+            profile_paths = list(tk_copy.profile_mapping.values())
+            tk_copy.profile_mapping = OrderedDict({tk_id: profile_paths})
 
             # Modify metadata dataframe
-            th_copy.metadata[idx_name] = th_id
-            th_copy.metadata.set_index(idx_name, inplace=True)
+            tk_copy.metadata[idx_name] = tk_id
+            tk_copy.metadata.set_index(idx_name, inplace=True)
 
             def _agg_to_set(obj):
                 """Aggregate values in 'obj' into a set to remove duplicates."""
                 if len(obj) <= 1:
                     return obj
                 else:
                     if isinstance(obj.iloc[0], list) or isinstance(obj.iloc[0], set):
@@ -686,20 +918,22 @@
                         _set = set(obj)
                     if len(_set) == 1:
                         return _set.pop()
                     else:
                         return _set
 
             # Execute aggregation
-            th_copy.metadata = th_copy.metadata.groupby(idx_name).agg(_agg_to_set)
+            tk_copy.metadata = tk_copy.metadata.groupby(idx_name).agg(_agg_to_set)
 
             # Append copy to list
-            th_copy_list.append(th_copy)
+            tk_copy_list.append(tk_copy)
 
-        return Thicket.concat_thickets(th_copy_list, from_statsframes=True)
+        return Thicket.concat_thickets(
+            tk_copy_list, from_statsframes=True, disable_tqdm=disable_tqdm
+        )
 
     def to_json(self, ensemble=True, metadata=True, stats=True):
         jsonified_thicket = {}
 
         # jsonify graph
         """
         Nodes: {hatchet_nid: {node data, children:[by-id]}}
@@ -746,18 +980,16 @@
         Nodes not contained in all profiles are removed.
 
         Returns:
             (thicket): intersected thicket
         """
 
         # Row that didn't exist will contain "None" in the name column.
-        query = (
-            QueryMatcher()
-            .match(".", lambda row: row["name"].apply(lambda n: n is not None).all())
-            .rel("*")
+        query = QueryMatcher().match(
+            ".", lambda row: row["name"].apply(lambda n: n is not None).all()
         )
         intersected_th = self.query(query)
 
         return intersected_th
 
     def filter_metadata(self, select_function):
         """Filter thicket object based on a metadata key.
@@ -800,14 +1032,17 @@
                     )
                 ]
 
                 # create an empty aggregated statistics table with the name column
                 new_thicket.statsframe.dataframe = helpers._new_statsframe_df(
                     new_thicket.dataframe
                 )
+
+                new_thicket._sync_profile_components(new_thicket.metadata)
+                validate_profile(new_thicket)
             else:
                 raise EmptyMetadataTable(
                     "The provided Thicket object has an empty MetadataTable."
                 )
 
         else:
             raise InvalidFilter("The argument passed to filter must be a callable.")
@@ -831,15 +1066,15 @@
                 Hatchet's AbstractQuery
             squash (bool): if true, run Thicket.squash before returning the result of
                 the query
             update_inc_cols (boolean, optional): if True, update inclusive columns when
                 performing squash.
 
         Returns:
-            (Thicket): a new Thicket object containing the data that matches the query
+            (thicket): a new Thicket object containing the data that matches the query
         """
         if isinstance(query_obj, (list, str)):
             raise UnsupportedQuery(
                 "Object and String queries from Hatchet are not yet supported in Thicket"
             )
         elif not issubclass(type(query_obj), AbstractQuery):
             raise TypeError(
@@ -892,40 +1127,33 @@
                 profile_id = df.index.values.tolist()
                 sub_thicket.dataframe = sub_thicket.dataframe[
                     sub_thicket.dataframe.index.get_level_values("profile").isin(
                         profile_id
                     )
                 ]
 
-                # Updates the profiles to only contain the remaining ones
-                profile_mapping_tmp = sub_thicket.profile_mapping.copy()
-                for profile_mapping_key in profile_mapping_tmp:
-                    if profile_mapping_key not in profile_id:
-                        sub_thicket.profile_mapping.pop(profile_mapping_key)
-
-                sub_thicket.profile = [
-                    profile for profile in sub_thicket.profile if profile in profile_id
-                ]
-
                 # clear the aggregated statistics table for current unique group
                 sub_thicket.statsframe.dataframe = helpers._new_statsframe_df(
                     sub_thicket.dataframe
                 )
 
                 # add thicket to dictionary
                 sub_thickets[key] = sub_thicket
+
+                sub_thicket._sync_profile_components(sub_thicket.metadata)
+                validate_profile(sub_thicket)
         else:
             raise EmptyMetadataTable(
                 "The provided Thicket object has an empty metadata table."
             )
 
         print(len(sub_thickets), " thickets created...")
         print(sub_thickets)
 
-        return sub_thickets
+        return GroupBy(by, sub_thickets)
 
     def filter_stats(self, filter_function):
         """Filter thicket object based on a stats column.
 
         Propagate changes to the entire thicket object.
 
         Arguments:
@@ -934,31 +1162,28 @@
 
         Returns:
             (thicket): new thicket object with applied filter function
         """
         # copy thicket
         new_thicket = self.copy()
 
-        # filter aggregated statistics table based on greater than restriction
+        # filter aggregated statistics table
         filtered_rows = new_thicket.statsframe.dataframe.apply(filter_function, axis=1)
         new_thicket.statsframe.dataframe = new_thicket.statsframe.dataframe[
             filtered_rows
         ]
 
         # filter performance data table based on filtered nodes
         filtered_nodes = new_thicket.statsframe.dataframe.index.values.tolist()
         new_thicket.dataframe = new_thicket.dataframe[
             new_thicket.dataframe.index.get_level_values("node").isin(filtered_nodes)
         ]
 
         # filter nodes in the graphframe based on the dataframe nodes
-        # TODO see if the new Thicket.squash function will work here
-        filtered_graphframe = GraphFrame.squash(new_thicket)
-        new_thicket.graph = filtered_graphframe.graph
-        new_thicket.statsframe.graph = filtered_graphframe.graph
+        new_thicket = new_thicket.squash(new_statsframe=False)
 
         return new_thicket
 
     def get_unique_metadata(self):
         """Get unique values per column in metadata.
 
         Returns:
@@ -991,14 +1216,89 @@
 
                 sorted_meta.append(
                     (idx, dict(sorted(unique_meta.items(), key=lambda x: x[0].lower())))
                 )
 
         return sorted_meta
 
+    def _sync_profile_components(self, component):
+        """Synchronize the Performance DataFrame, Metadata Dataframe, profile and
+        profile mapping objects based on the component's index. This is useful when a
+        non-Thicket function modifies the profiles in an object and those changes need
+        to be reflected in the other objects.
+
+        Arguments:
+            component (DataFrame) -> (Thicket.dataframe or Thicket.metadata): The index
+            of this component is used to synchronize the other objects.
+
+        Returns:
+            (thicket): self
+        """
+
+        def _profile_truth_from_component(component):
+            """Derive the profiles from the component index."""
+            # Option A: Columnar-indexed Thicket
+            if isinstance(component.columns, pd.MultiIndex):
+                # Performance DataFrame
+                if isinstance(component.index, pd.MultiIndex):
+                    row_idx = component.index.droplevel(level="node")
+                # Metadata DataFrame
+                else:
+                    row_idx = component.index
+                profile_truth = [
+                    prof
+                    for prof in self.profile
+                    if any([row_prof in prof for row_prof in row_idx])
+                ]
+            # Option B: Non-columnar-indexed Thicket
+            else:
+                # Performance DataFrame
+                if isinstance(component.index, pd.MultiIndex):
+                    profile_truth = component.index.droplevel(level="node")
+                # Metadata DataFrame
+                else:
+                    profile_truth = component.index
+            return list(set(profile_truth))
+
+        def _sync_indices(component, profile_truth):
+            """Sync the Thicket attributes"""
+            self.profile = profile_truth
+            self.profile_mapping = OrderedDict(
+                {
+                    prof: file
+                    for prof, file in self.profile_mapping.items()
+                    if prof in profile_truth
+                }
+            )
+
+            # For Columnar-indexed Thicket
+            if isinstance(component.columns, pd.MultiIndex):
+                # Create powerset from all profiles
+                pset = set()
+                for p in profile_truth:
+                    pset.update(helpers._powerset_from_tuple(p))
+                profile_truth = pset
+
+            self.dataframe = self.dataframe[
+                self.dataframe.index.droplevel(level="node").isin(profile_truth)
+            ]
+            self.metadata = self.metadata[self.metadata.index.isin(profile_truth)]
+
+            return self
+
+        if not isinstance(component, pd.DataFrame):
+            raise ValueError(
+                "Component must be either Thicket.dataframe or Thicket.metadata"
+            )
+
+        profile_truth = _profile_truth_from_component(component)
+        self = _sync_indices(component, profile_truth)
+
+        return self
+
 
 class InvalidFilter(Exception):
     """Raised when an invalid argument is passed to the filter function."""
 
 
 class EmptyMetadataTable(Exception):
     """Raised when a Thicket object argument is passed with an empty MetadataTable to
```

### Comparing `llnl-thicket-2023.3.1/thicket/vis/__init__.py` & `llnl-thicket-2024.1.0/thicket/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/package.json` & `llnl-thicket-2024.1.0/thicket/vis/package.json`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/datautil.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/datautil.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/pcp.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/pcp.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/scatter.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/scatter.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/stackedarea.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/stackedarea.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/pcp/store.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/pcp/store.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/topdown/stackedbars.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/topdown/stackedbars.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/scripts/treetable.js` & `llnl-thicket-2024.1.0/thicket/vis/scripts/treetable.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/static/pcp_bundle.html` & `llnl-thicket-2024.1.0/thicket/vis/static/pcp_bundle.html`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/static/pcp_bundle.js` & `llnl-thicket-2024.1.0/thicket/vis/static/pcp_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/static/topdown_bundle.js` & `llnl-thicket-2024.1.0/thicket/vis/static/topdown_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/static/treetable_bundle.js` & `llnl-thicket-2024.1.0/thicket/vis/static/treetable_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/static_fixer.py` & `llnl-thicket-2024.1.0/thicket/vis/static_fixer.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/templates/pcp.html` & `llnl-thicket-2024.1.0/thicket/vis/templates/pcp.html`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/visualizations.py` & `llnl-thicket-2024.1.0/thicket/vis/visualizations.py`

 * *Files identical despite different names*

### Comparing `llnl-thicket-2023.3.1/thicket/vis/webpack.config.js` & `llnl-thicket-2024.1.0/thicket/vis/webpack.config.js`

 * *Files identical despite different names*

