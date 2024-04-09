# Comparing `tmp/python2verilog-0.4.3rc1.tar.gz` & `tmp/python2verilog-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.4.3rc1.tar", last modified: Tue Feb 27 20:28:15 2024, max compression
+gzip compressed data, was "python2verilog-0.5.0rc1.tar", last modified: Tue Apr  9 23:31:20 2024, max compression
```

## Comparing `python2verilog-0.4.3rc1.tar` & `python2verilog-0.5.0rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.093862 python2verilog-0.4.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-02-27 20:28:15.089862 python2verilog-0.4.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.081862 python2verilog-0.4.3rc1/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.081862 python2verilog-0.4.3rc1/python2verilog/api/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/exit_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/file_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/api/verilogify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/backend/verilog/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/fsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/backend/verilog/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/frontend/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/ir/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/ir/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.085862 python2verilog-0.4.3rc1/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/optimizer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/optimizer/increase_work.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.089862 python2verilog-0.4.3rc1/python2verilog/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/simulation/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/simulation/iverilog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.089862 python2verilog-0.4.3rc1/python2verilog/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/cytoscape.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/mit_license.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/peek_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-02-27 20:27:59.000000 python2verilog-0.4.3rc1/python2verilog/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:28:15.089862 python2verilog-0.4.3rc1/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-02-27 20:28:15.000000 python2verilog-0.4.3rc1/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-27 20:28:15.000000 python2verilog-0.4.3rc1/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 20:28:15.000000 python2verilog-0.4.3rc1/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-27 20:28:15.000000 python2verilog-0.4.3rc1/python2verilog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-27 20:28:15.000000 python2verilog-0.4.3rc1/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 20:28:15.093862 python2verilog-0.4.3rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.758576 python2verilog-0.5.0rc1/python2verilog/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/exit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/file_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/verilogify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/backend/verilog/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/fsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32090 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/frontend/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/increase_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/iverilog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/cytoscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/mit_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/peek_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/setup.cfg
```

### Comparing `python2verilog-0.4.3rc1/LICENSE` & `python2verilog-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/PKG-INFO` & `python2verilog-0.5.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.4.3rc1
+Version: 0.5.0rc1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
-Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
-Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
+Project-URL: Homepage, https://github.com/WorldofKerry/ToHDL/
+Project-URL: Bug Tracker, https://github.com/WorldofKerry/ToHDL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions
 Requires-Dist: pytohdl
@@ -25,14 +25,16 @@
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: tabulate; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: networkx[default]; extra == "dev"
 Requires-Dist: dash_cytoscape; extra == "dev"
 Requires-Dist: dash; extra == "dev"
 Requires-Dist: parameterized; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/WorldofKerry/Python2Verilog/blob/main/examples/notebook.ipynb)
 [![pypi](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)](https://pypi.org/project/python2verilog/)
 ![py versions](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2FWorldofKerry%2FPython2Verilog%2Fmain%2F.github%2Fworkflows%2Fpytest.yml&query=%24.jobs.full.strategy.matrix%5B%22python-version%22%5D&label=python%20versions)
 [![pypi downloads](https://img.shields.io/pypi/dm/python2verilog)](https://pypi.org/project/python2verilog/)
 [![pytest](https://github.com/worldofkerry/python2verilog/actions/workflows/pytest.yml/badge.svg)](https://github.com/WorldofKerry/Python2Verilog/actions/workflows/pytest.yml)
 
@@ -85,40 +87,54 @@
 
 [Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) are used for tracking.
 
 Sphinx is used for the docs. Follow the [sphinx workflow](.github/workflows/sphinx.yml) to generate a local copy.
 
 ## Development
 
-### Requirements
+### Setup
 
 For most up-to-date information, refer to the [pytest workflow](.github/workflows/pytest.yml) or the [packaging workflow](.github/workflows/packaging.yml).
 
 A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used to avoid writing to disk)
 
-Install required python libraries use
-
+Steps
 ```bash
 source ./build.sh venv
-./build.sh ci
+./build.sh all
+pre-commit install
 ```
 
 For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
-`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
+```bash
+sudo apt install expect
+# This adds `iverilog` to PATH
+git submodule update --init
+./extern/iverilog_setup.sh
+```
 
 The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
 ### Running Tests
 
-To run tests, use `pytest`.
+Run Python tests with `pytest`.
+Run rust tests with `cargo test`.
 
 CLI arguments for test configuration can be found in [tests/conftest.py](tests/conftest.py).
 
 Use `./clean.sh` to remove gitignored and generated files.
 
+### Troubleshooting
+
+#### `cargo test` Errors
+- error: linker \`cc\` not found
+    - On Ubuntu run `sudo apt install build-essential`
+- /usr/bin/ld: cannot find -lpython3.10: No such file or directory
+    - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
+
 ## Flamegraph
 
 ```bash
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
```

### Comparing `python2verilog-0.4.3rc1/README.md` & `python2verilog-0.5.0rc1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -53,40 +53,54 @@
 
 [Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) are used for tracking.
 
 Sphinx is used for the docs. Follow the [sphinx workflow](.github/workflows/sphinx.yml) to generate a local copy.
 
 ## Development
 
-### Requirements
+### Setup
 
 For most up-to-date information, refer to the [pytest workflow](.github/workflows/pytest.yml) or the [packaging workflow](.github/workflows/packaging.yml).
 
 A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used to avoid writing to disk)
 
-Install required python libraries use
-
+Steps
 ```bash
 source ./build.sh venv
-./build.sh ci
+./build.sh all
+pre-commit install
 ```
 
 For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
-`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
+```bash
+sudo apt install expect
+# This adds `iverilog` to PATH
+git submodule update --init
+./extern/iverilog_setup.sh
+```
 
 The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
 ### Running Tests
 
-To run tests, use `pytest`.
+Run Python tests with `pytest`.
+Run rust tests with `cargo test`.
 
 CLI arguments for test configuration can be found in [tests/conftest.py](tests/conftest.py).
 
 Use `./clean.sh` to remove gitignored and generated files.
 
+### Troubleshooting
+
+#### `cargo test` Errors
+- error: linker \`cc\` not found
+    - On Ubuntu run `sudo apt install build-essential`
+- /usr/bin/ld: cannot find -lpython3.10: No such file or directory
+    - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
+
 ## Flamegraph
 
 ```bash
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
```

### Comparing `python2verilog-0.4.3rc1/pyproject.toml` & `python2verilog-0.5.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python2verilog"
-version = "0.4.3-rc1"
+version = "0.5.0rc1"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -27,19 +27,21 @@
     "pandas",
     "tabulate",
     "matplotlib",
     "networkx[default]",
     "dash_cytoscape",
     "dash",
     "parameterized",
+    "pylint",
+    "mypy",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/WorldofKerry/Python2Verilog/"
-"Bug Tracker" = "https://github.com/WorldofKerry/Python2Verilog/issues"
+"Homepage" = "https://github.com/WorldofKerry/ToHDL/"
+"Bug Tracker" = "https://github.com/WorldofKerry/ToHDL/issues"
 
 [build-system]
 requires = ["setuptools", "typing-extensions"]
 
 [tool.setuptools.packages.find]
 "include" = ["python2verilog*"]
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/__main__.py` & `python2verilog-0.5.0rc1/python2verilog/__main__.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/context.py` & `python2verilog-0.5.0rc1/python2verilog/api/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Functions that take text as input
 """
 
-
 import logging
+import textwrap
 
 import pytohdl  # pylint: disable=import-error
 
 from python2verilog import ir
 from python2verilog.backend import verilog
 from python2verilog.backend.verilog.config import CodegenConfig, TestbenchConfig
 from python2verilog.frontend.function import Function
@@ -43,28 +43,38 @@
     Converts a context to a verilog module and testbench
 
     :return: (module, testbench)
     """
     typed(context, ir.Context)
     ver_code_gen, _ = context_to_codegen(context)
 
-    # Filter for generators and contexts that do not reference other contexts
     if context.is_generator and context.optimization_level == 0:
         try:
-            # assert False, f"{context.name} {context.is_generator}"
-            to_hdl = pytohdl.translate(context.py_string) # pylint: disable=no-member
-            module_str = to_hdl
-            # assert False
-        except AssertionError:
-            module_str = ver_code_gen.get_module_str()
-        except:  # pylint: disable=bare-except
-            # assert False, sys.exc_info().__str__()
+            assert all(
+                v.name == context.name or not v.is_generator
+                for v in context.namespace.values()
+            ), "Only function or generator calling other functions supported"
+
+            functions = {
+                k: textwrap.dedent(v.py_string or "")
+                for k, v in context.namespace.items()
+            }
+            module_str = pytohdl.translate(  # pylint: disable=no-member
+                pytohdl.PyContext(context.name, functions)  # pylint: disable=no-member
+            )
+            # logging.error("Path 1")
+        except BaseException as e:  # pylint: disable=broad-exception-caught
             module_str = ver_code_gen.get_module_str()
+            logging.info(
+                "Failed to use Rust backend, falling back to Python backend with error: %s",
+                e,
+            )
     else:
         module_str = ver_code_gen.get_module_str()
+        # logging.warning("Path 3")
 
     tb_str = ver_code_gen.get_testbench_str(config)
     return module_str, tb_str
 
 
 def context_to_verilog_and_dump(context: ir.Context) -> tuple[str, str, str]:
     """
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/exit_handler.py` & `python2verilog-0.5.0rc1/python2verilog/api/exit_handler.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/modes.py` & `python2verilog-0.5.0rc1/python2verilog/api/modes.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/namespace.py` & `python2verilog-0.5.0rc1/python2verilog/api/namespace.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/python.py` & `python2verilog-0.5.0rc1/python2verilog/api/python.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/api/verilogify.py` & `python2verilog-0.5.0rc1/python2verilog/api/verilogify.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/ast.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/ast.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/codegen.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/codegen.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/config.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/config.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/fsm.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/fsm.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/module.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/module.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/backend/verilog/testbench.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/testbench.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/exceptions/__init__.py` & `python2verilog-0.5.0rc1/python2verilog/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/frontend/function.py` & `python2verilog-0.5.0rc1/python2verilog/frontend/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The freshest in-order generator parser
 """
+
 from __future__ import annotations
 
 import ast as pyast
 import copy
 import itertools
 import logging
 from typing import Collection, Iterable, Optional, TypeVar, cast
@@ -202,19 +203,22 @@
                 stmts = [self._parse_expression(ret.value)]
             else:
                 raise UnsupportedSyntaxError.from_pyast(ret, self.__context.name)
         except Exception as e:
             raise UnsupportedSyntaxError.from_pyast(ret, self.__context.name) from e
 
         self.__context.validate()
-        head, tail = self._weave_nonclocked_edges(
-            self._create_assign_nodes(self.__context.output_vars, stmts, prefix),
-            f"{prefix}_e",
-        )
-        tail.edge = ir.ClockedEdge(unique_id=f"{prefix}_last_e")
+        try:
+            head, tail = self._weave_nonclocked_edges(
+                self._create_assign_nodes(self.__context.output_vars, stmts, prefix),
+                f"{prefix}_e",
+            )
+            tail.edge = ir.ClockedEdge(unique_id=f"{prefix}_last_e")
+        except Exception as e:
+            raise RuntimeError(f"{e} in {self.__context.name}") from e
         return head, [tail.edge]
 
     def _parse_stmts(
         self,
         stmts: list[pyast.stmt],
         prefix: str,
         breaks: list[ir.Edge],
@@ -906,30 +910,32 @@
 
     def _parse_binop(self, expr: pyast.BinOp) -> ir.Expression:
         """
         <left> <op> <right>
 
         With special case for floor division
         """
+        left = self._parse_expression(expr.left)
+        right = self._parse_expression(expr.right)
+
         if isinstance(expr.op, pyast.Add):
-            return ir.Add(
-                self._parse_expression(expr.left), self._parse_expression(expr.right)
-            )
+            return ir.Add(left, right)
         if isinstance(expr.op, pyast.Sub):
-            return ir.Sub(
-                self._parse_expression(expr.left), self._parse_expression(expr.right)
-            )
-
+            return ir.Sub(left, right)
         if isinstance(expr.op, pyast.Mult):
-            return ir.Mul(
-                self._parse_expression(expr.left), self._parse_expression(expr.right)
-            )
-
+            return ir.Mul(left, right)
         if isinstance(expr.op, pyast.FloorDiv):
-            left = self._parse_expression(expr.left)
-            right = self._parse_expression(expr.right)
             return ir.FloorDiv(left, right)
         if isinstance(expr.op, pyast.Mod):
-            left = self._parse_expression(expr.left)
-            right = self._parse_expression(expr.right)
             return ir.Mod(left, right)
+        if isinstance(expr.op, pyast.BitOr):
+            return ir.BitOr(left, right)
+        if isinstance(expr.op, pyast.BitAnd):
+            return ir.BitAnd(left, right)
+        if isinstance(expr.op, pyast.BitXor):
+            return ir.BitXor(left, right)
+        if isinstance(expr.op, pyast.LShift):
+            return ir.LShift(left, right)
+        if isinstance(expr.op, pyast.RShift):
+            return ir.RShift(left, right)
+
         raise UnsupportedSyntaxError(f"Unsupported binop `{pyast.dump(expr.op)}")
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/__init__.py` & `python2verilog-0.5.0rc1/python2verilog/ir/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     Expression,
     FloorDiv,
     Int,
     LessThan,
     Mod,
     Mul,
     Pow,
+    BitAnd,
+    BitOr,
+    BitXor,
+    LShift,
+    RShift,
     State,
     Sub,
     Ternary,
     UBinOp,
     UInt,
     UnaryOp,
     Unknown,
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/context.py` & `python2verilog-0.5.0rc1/python2verilog/ir/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         assert guard(self._output_vars, list), f"Unknown output variables {self}"
         return copy.deepcopy(self._output_vars)
 
     def default_output_vars(self):
         """
         Sets own output vars to default based on number of output variables
         """
-        assert self.output_types is not None
+        assert self.output_types is not None, f"{self.name}"
         self._output_vars = [
             ExclusiveVar(f"{self.prefix}_output_{i}")
             for i in range(len(self.output_types))
         ]
 
     def refresh_input_output_vars(self):
         """
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/expressions.py` & `python2verilog-0.5.0rc1/python2verilog/ir/expressions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Intermediate Representation Expressions
 
 Represents the subset of Python expressions
 that are synthesizable
 
 """
+
 from __future__ import annotations
 
 from typing import Optional
 
 from python2verilog.utils.generics import GenericRepr
 from python2verilog.utils.typed import guard, typed, typed_list, typed_strict
 
@@ -282,14 +283,59 @@
     <left> % <right>
     """
 
     def __init__(self, left: Expression, right: Expression):
         super().__init__(left, "%", right)
 
 
+class BitOr(UBinOp):
+    """
+    <left> | <right>
+    """
+
+    def __init__(self, left: Expression, right: Expression):
+        super().__init__(left, "|", right)
+
+
+class BitAnd(UBinOp):
+    """
+    <left> & <right>
+    """
+
+    def __init__(self, left: Expression, right: Expression):
+        super().__init__(left, "&", right)
+
+
+class BitXor(UBinOp):
+    """
+    <left> ^ <right>
+    """
+
+    def __init__(self, left: Expression, right: Expression):
+        super().__init__(left, "^", right)
+
+
+class LShift(UBinOp):
+    """
+    <left> << <right>
+    """
+
+    def __init__(self, left: Expression, right: Expression):
+        super().__init__(left, "<<", right)
+
+
+class RShift(UBinOp):
+    """
+    <left> >> <right>
+    """
+
+    def __init__(self, left: Expression, right: Expression):
+        super().__init__(left, ">>", right)
+
+
 class UnaryOp(Expression):
     """
     <op>(<expr>)
     """
 
     def __init__(self, oper: str, expr: Expression):
         self.oper = typed_strict(oper, str)
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/graph.py` & `python2verilog-0.5.0rc1/python2verilog/ir/graph.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/instance.py` & `python2verilog-0.5.0rc1/python2verilog/ir/instance.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/ir/signals.py` & `python2verilog-0.5.0rc1/python2verilog/ir/signals.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/optimizer/helpers.py` & `python2verilog-0.5.0rc1/python2verilog/optimizer/helpers.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/optimizer/increase_work.py` & `python2verilog-0.5.0rc1/python2verilog/optimizer/increase_work.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/simulation/display.py` & `python2verilog-0.5.0rc1/python2verilog/simulation/display.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/simulation/iverilog.py` & `python2verilog-0.5.0rc1/python2verilog/simulation/iverilog.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/cytoscape.py` & `python2verilog-0.5.0rc1/python2verilog/utils/cytoscape.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/decorator.py` & `python2verilog-0.5.0rc1/python2verilog/utils/decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,8 +21,10 @@
     def new_dec(*args, **kwargs):
         if len(args) == 1 and len(kwargs) == 0 and isinstance(args[0], FunctionType):
             # actual decorated function
             return func(args[0])
         # decorator arguments
         return lambda real_func: func(real_func, *args, **kwargs)
 
+    new_dec.__doc__ = func.__doc__
+
     return new_dec
```

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/env.py` & `python2verilog-0.5.0rc1/python2verilog/utils/env.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/generics.py` & `python2verilog-0.5.0rc1/python2verilog/utils/generics.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/lines.py` & `python2verilog-0.5.0rc1/python2verilog/utils/lines.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/mit_license.py` & `python2verilog-0.5.0rc1/python2verilog/utils/mit_license.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/peek_counter.py` & `python2verilog-0.5.0rc1/python2verilog/utils/peek_counter.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/typed.py` & `python2verilog-0.5.0rc1/python2verilog/utils/typed.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog/utils/visualization.py` & `python2verilog-0.5.0rc1/python2verilog/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.4.3rc1/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.5.0rc1/python2verilog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.4.3rc1
+Version: 0.5.0rc1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
-Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
-Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
+Project-URL: Homepage, https://github.com/WorldofKerry/ToHDL/
+Project-URL: Bug Tracker, https://github.com/WorldofKerry/ToHDL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions
 Requires-Dist: pytohdl
@@ -25,14 +25,16 @@
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: tabulate; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: networkx[default]; extra == "dev"
 Requires-Dist: dash_cytoscape; extra == "dev"
 Requires-Dist: dash; extra == "dev"
 Requires-Dist: parameterized; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/WorldofKerry/Python2Verilog/blob/main/examples/notebook.ipynb)
 [![pypi](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)](https://pypi.org/project/python2verilog/)
 ![py versions](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2FWorldofKerry%2FPython2Verilog%2Fmain%2F.github%2Fworkflows%2Fpytest.yml&query=%24.jobs.full.strategy.matrix%5B%22python-version%22%5D&label=python%20versions)
 [![pypi downloads](https://img.shields.io/pypi/dm/python2verilog)](https://pypi.org/project/python2verilog/)
 [![pytest](https://github.com/worldofkerry/python2verilog/actions/workflows/pytest.yml/badge.svg)](https://github.com/WorldofKerry/Python2Verilog/actions/workflows/pytest.yml)
 
@@ -85,40 +87,54 @@
 
 [Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) are used for tracking.
 
 Sphinx is used for the docs. Follow the [sphinx workflow](.github/workflows/sphinx.yml) to generate a local copy.
 
 ## Development
 
-### Requirements
+### Setup
 
 For most up-to-date information, refer to the [pytest workflow](.github/workflows/pytest.yml) or the [packaging workflow](.github/workflows/packaging.yml).
 
 A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used to avoid writing to disk)
 
-Install required python libraries use
-
+Steps
 ```bash
 source ./build.sh venv
-./build.sh ci
+./build.sh all
+pre-commit install
 ```
 
 For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
-`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
+```bash
+sudo apt install expect
+# This adds `iverilog` to PATH
+git submodule update --init
+./extern/iverilog_setup.sh
+```
 
 The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
 ### Running Tests
 
-To run tests, use `pytest`.
+Run Python tests with `pytest`.
+Run rust tests with `cargo test`.
 
 CLI arguments for test configuration can be found in [tests/conftest.py](tests/conftest.py).
 
 Use `./clean.sh` to remove gitignored and generated files.
 
+### Troubleshooting
+
+#### `cargo test` Errors
+- error: linker \`cc\` not found
+    - On Ubuntu run `sudo apt install build-essential`
+- /usr/bin/ld: cannot find -lpython3.10: No such file or directory
+    - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
+
 ## Flamegraph
 
 ```bash
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
```

### Comparing `python2verilog-0.4.3rc1/python2verilog.egg-info/SOURCES.txt` & `python2verilog-0.5.0rc1/python2verilog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

