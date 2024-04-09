# Comparing `tmp/libbs-1.2.4.tar.gz` & `tmp/libbs-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.4.tar", last modified: Mon Apr  8 18:23:21 2024, max compression
+gzip compressed data, was "libbs-1.2.5.tar", last modified: Tue Apr  9 22:17:49 2024, max compression
```

## Comparing `libbs-1.2.4.tar` & `libbs-1.2.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.911141 libbs-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-08 18:23:18.000000 libbs-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-08 18:23:21.911141 libbs-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-08 18:23:18.000000 libbs-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.899140 libbs-1.2.4/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.899140 libbs-1.2.4/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.903141 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.907141 libbs-1.2.4/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32750 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.911141 libbs-1.2.4/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.911141 libbs-1.2.4/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 18:23:18.000000 libbs-1.2.4/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.911141 libbs-1.2.4/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 18:23:21.000000 libbs-1.2.4/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 18:23:21.911141 libbs-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 18:23:18.000000 libbs-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:23:21.911141 libbs-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-08 18:23:18.000000 libbs-1.2.4/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 18:23:18.000000 libbs-1.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-08 18:23:18.000000 libbs-1.2.4/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.672402 libbs-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 22:17:46.000000 libbs-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-09 22:17:49.672402 libbs-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-09 22:17:46.000000 libbs-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.660402 libbs-1.2.5/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.660402 libbs-1.2.5/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.664402 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.668402 libbs-1.2.5/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32838 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.672402 libbs-1.2.5/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.672402 libbs-1.2.5/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 22:17:46.000000 libbs-1.2.5/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.672402 libbs-1.2.5/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 22:17:49.000000 libbs-1.2.5/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 22:17:49.672402 libbs-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 22:17:46.000000 libbs-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:17:49.672402 libbs-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-09 22:17:46.000000 libbs-1.2.5/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-09 22:17:46.000000 libbs-1.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-09 22:17:46.000000 libbs-1.2.5/tests/test_decompilers.py
```

### Comparing `libbs-1.2.4/LICENSE` & `libbs-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/PKG-INFO` & `libbs-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.4
+Version: 1.2.5
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
```

### Comparing `libbs-1.2.4/README.md` & `libbs-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/__main__.py` & `libbs-1.2.5/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/api/artifact_dict.py` & `libbs-1.2.5/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/api/artifact_lifter.py` & `libbs-1.2.5/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/api/decompiler_interface.py` & `libbs-1.2.5/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/api/type_parser.py` & `libbs-1.2.5/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/api/utils.py` & `libbs-1.2.5/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/artifact.py` & `libbs-1.2.5/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/comment.py` & `libbs-1.2.5/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/decompilation.py` & `libbs-1.2.5/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/enum.py` & `libbs-1.2.5/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/func.py` & `libbs-1.2.5/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/global_variable.py` & `libbs-1.2.5/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/patch.py` & `libbs-1.2.5/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/stack_variable.py` & `libbs-1.2.5/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/artifacts/struct.py` & `libbs-1.2.5/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.5/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.5/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/angr/compat.py` & `libbs-1.2.5/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/angr/interface.py` & `libbs-1.2.5/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.5/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/binja/hooks.py` & `libbs-1.2.5/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/binja/interface.py` & `libbs-1.2.5/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.5/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.5/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ghidra/hooks.py` & `libbs-1.2.5/libbs/decompilers/ghidra/hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,20 +38,20 @@
                 self.changeManager.DOCR_DATA_TYPE_SETTING_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_MOVED,
                 self.changeManager.DOCR_DATA_TYPE_ADDED
             ]
 
             for record in ev:
                 # NOTE: This excludes type changes anything as they are DomainObjectChangeRecord
-                if not "ProgramChangeRecord" in str(type(record)):
+
+                if not self._interface.ghidra.isinstance(record, self.programChangeRecord):
                     continue
 
                 changeType = record.getEventType()
                 newValue = record.getNewValue()
-                oldValue = record.getOldValue()
                 obj = record.getObject()
 
                 if changeType in funcEvents:
                     pass
                 elif changeType in typeEvents:
                     try:
                         struct = self._interface.structs[newValue.name]
@@ -70,15 +70,15 @@
 
                 elif changeType in symDelEvents:
                     # Currently unused and unsupported
                     pass
                 elif changeType in symChgEvents:
                     if obj is None and newValue is not None:
                         obj = newValue
-                    if "VariableSymbolDB" in str(type(obj)):
+                    if self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
                         parent_namespace = obj.getParentNamespace()
                         storage = obj.getVariableStorage()
                         if (
                             (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
                             and (parent_namespace is not None)
                         ):
                             self._interface.stack_variable_changed(
@@ -99,25 +99,25 @@
                             # print(f"Old value: {oldValue}")
                             # print(f"New value: {newValue}")
                             # typ = obj.getDataType()
                             # stackVar = StackVariable(None, None, typ, None, None)
                             # self._interface.stack_variable_changed(stackVar)
                             pass
                         continue
-                    elif "CodeSymbol" in str(type(obj)):
+                    elif self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
                         # TODO: Find trigger for global var changes
                         # gVar = GlobalVariable(None, newValue)
                         # self._interface.global_variable_changed(gVar)
                         continue
-                    elif "FunctionSymbol" in str(type(obj)):
+                    elif self._interface.ghidra.isinstance(obj, self.db.symbol.FunctionSymbol):
                         header = FunctionHeader(newValue, int(obj.getAddress().offset))
                         self._interface.function_header_changed(
                             self._interface.art_lifter.lift(header)
                         )
-                    elif "FunctionDB" in str(type(obj)):
+                    elif self._interface.ghidra.isinstance(obj, self.db.function.FunctionDB):
                         # TODO: Fix argument name support
                         #changed_arg = FunctionArgument(None, newValue, None, None)
                         #header = FunctionHeader(None, None, args={None: changed_arg})
                         #self._interface.function_header_changed(header)
                         pass
                     else:
                         continue
```

### Comparing `libbs-1.2.4/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.5/libbs/decompilers/ghidra/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,15 +506,17 @@
         members = self._get_enum_members(name)
         return Enum(name, members) if members else None
 
     def _enums(self) -> Dict[str, Enum]:
         names: Optional[List[str]] = self.ghidra.bridge.remote_eval(
             "[dType.getPathName() "
             "for dType in currentProgram.getDataTypeManager().getAllDataTypes()"
-            "if str(type(dType)) == \"<type 'ghidra.program.database.data.EnumDB'>\"]"
+            "if ghidra.isinstance(dType, EnumDBType)]",
+        ghidra=self.ghidra,
+        EnumDBType=self.ghidra.import_module_object("ghidra.program.model.data", "EnumDB")
         )
         enums = {}
         for name in names:
             # XXX: we dont really know why this is here, but we assume its because you cant have
             # an enum nested in a folder in ghidra
             if name.count("/") != 1:
                 continue
```

### Comparing `libbs-1.2.4/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.5/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ida/compat.py` & `libbs-1.2.5/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ida/hooks.py` & `libbs-1.2.5/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/decompilers/ida/interface.py` & `libbs-1.2.5/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/logger.py` & `libbs-1.2.5/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/plugin_installer.py` & `libbs-1.2.5/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/ui/__init__.py` & `libbs-1.2.5/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/ui/qt_objects.py` & `libbs-1.2.5/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs/ui/utils.py` & `libbs-1.2.5/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/libbs.egg-info/PKG-INFO` & `libbs-1.2.5/libbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.4
+Version: 1.2.5
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
```

### Comparing `libbs-1.2.4/libbs.egg-info/SOURCES.txt` & `libbs-1.2.5/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/setup.cfg` & `libbs-1.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/tests/test_artifacts.py` & `libbs-1.2.5/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/tests/test_cli.py` & `libbs-1.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.4/tests/test_decompilers.py` & `libbs-1.2.5/tests/test_decompilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 class TestHeadlessInterfaces(unittest.TestCase):
     def setUp(self):
         self._generic_renamed_name = "binsync_main"
         self._fauxware_path = TEST_BINARY_DIR / "fauxware"
 
     def test_ghidra(self):
-        # TODO: Add test cases for structs and enums
         # useful command for testing, kills all Headless-Ghidra:
         # kill $(ps aux | grep 'Ghidra-Headless' | awk '{print $2}')
         deci = DecompilerInterface.discover(
             force_decompiler=GHIDRA_DECOMPILER,
             headless=True,
             headless_dec_path=DEC_TO_HEADLESS[GHIDRA_DECOMPILER],
             binary_path=self._fauxware_path,
```

