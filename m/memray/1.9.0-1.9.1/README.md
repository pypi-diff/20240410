# Comparing `tmp/memray-1.9.0.tar.gz` & `tmp/memray-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memray-1.9.0.tar", last modified: Fri Jul 28 17:02:09 2023, max compression
+gzip compressed data, was "memray-1.9.1.tar", last modified: Tue Aug  1 22:54:47 2023, max compression
```

## Comparing `memray-1.9.0.tar` & `memray-1.9.1.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.941002 memray-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 17:01:54.000000 memray-1.9.0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-28 17:01:54.000000 memray-1.9.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-28 17:01:54.000000 memray-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-28 17:01:54.000000 memray-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-28 17:01:54.000000 memray-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 17:01:54.000000 memray-1.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-28 17:01:54.000000 memray-1.9.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-07-28 17:02:09.941002 memray-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-28 17:01:54.000000 memray-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   529986 2023-07-28 17:01:54.000000 memray-1.9.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 17:01:54.000000 memray-1.9.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-28 17:01:54.000000 memray-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:02:09.941002 memray-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-28 17:01:54.000000 memray-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.900999 memray-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray/_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_ipython/flamegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.921000 memray-1.9.0/src/memray/_memray/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/algorithm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/alloc.h
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/alloc.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/compat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/elf_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/elf_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/frame_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.h
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/inject.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/linker_shenanigans.h
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/lz4_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/macho_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/macho_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/pthread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/python_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/python_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.h
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.h
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    34716 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17955 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.h
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.h
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.h
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    36947 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.h
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54621 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray_test_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_test_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.921000 memray-1.9.0/src/memray/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/_attach.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/_attach.lldb
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/attach.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/common.js
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/common.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/temporal_flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/frame_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/templates/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.css
--rw-r--r--   0 runner    (1001) docker     (123)    78020 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)    73346 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/table.css
--rw-r--r--   0 runner    (1001) docker     (123)    72863 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)    81214 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/temporal_flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/classic_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/flamegraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/temporal_flamegraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.937001 memray-1.9.0/src/vendor/libbacktrace/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/aclocal.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/allocfail.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/allocfail.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/atomic.c
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace-supported.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace.c
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace.h
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/btest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.941002 memray-1.9.0/src/vendor/libbacktrace/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/enable.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/lead-dot.m4
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/multi.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/override.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/warnings.m4
--rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.guess
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.sub
--rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/configure
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/configure.ac
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/debuginfod_support.h
--rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/dwarf.c
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/edtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/edtest2.c
--rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/elf.c
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/fileline.c
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/filenames.h
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/filetype.awk
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/install-sh
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/instrumented_alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/internal.h
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltmain.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/macho.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/missing
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mmapio.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/move-if-change
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/nounwind.c
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/pecoff.c
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/posix.c
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/print.c
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/read.c
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/sort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/state.c
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/stest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/test-driver
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/test_format.c
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/testlib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/testlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ttest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/unittest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/unknown.c
--rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/xcoff.c
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/xztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/regenerate_libbacktrace.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 17:01:54.000000 memray-1.9.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.659533 memray-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 22:54:31.000000 memray-1.9.1/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 22:54:31.000000 memray-1.9.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-01 22:54:31.000000 memray-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-01 22:54:31.000000 memray-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-01 22:54:31.000000 memray-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-08-01 22:54:31.000000 memray-1.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-08-01 22:54:31.000000 memray-1.9.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-08-01 22:54:47.659533 memray-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-08-01 22:54:31.000000 memray-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   529986 2023-08-01 22:54:32.000000 memray-1.9.1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-01 22:54:32.000000 memray-1.9.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 22:54:32.000000 memray-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:54:47.659533 memray-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-08-01 22:54:32.000000 memray-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.615533 memray-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.619533 memray-1.9.1/src/memray/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.623533 memray-1.9.1/src/memray/_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_ipython/flamegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.631533 memray-1.9.1/src/memray/_memray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/algorithm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/alloc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/compat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/elf_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/elf_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/frame_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/hooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/hooks.h
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/hooks.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/inject.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/linker_shenanigans.h
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/lz4_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/macho_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/macho_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/native_resolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/native_resolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/native_resolver.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/pthread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/python_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/python_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_reader.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/record_writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/records.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/records.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/records.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/sink.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/sink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/sink.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34716 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/snapshot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17955 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/snapshot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/snapshot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/socket_reader_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/socket_reader_thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/socket_reader_thread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/source.h
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    37129 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/tracking_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/tracking_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray/tracking_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54611 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_memray_test_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_test_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.635533 memray-1.9.1/src/memray/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/_attach.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/_attach.lldb
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/commands/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.635533 memray-1.9.1/src/memray/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.639533 memray-1.9.1/src/memray/reporters/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/common.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/frame_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.639533 memray-1.9.1/src/memray/reporters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.639533 memray-1.9.1/src/memray/reporters/templates/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/flamegraph.css
+-rw-r--r--   0 runner    (1001) docker     (123)    78020 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73346 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)    72863 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    81214 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/classic_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/templates/temporal_flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-08-01 22:54:32.000000 memray-1.9.1/src/memray/reporters/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.623533 memray-1.9.1/src/memray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 22:54:47.000000 memray-1.9.1/src/memray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.643533 memray-1.9.1/src/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.655533 memray-1.9.1/src/vendor/libbacktrace/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/aclocal.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/allocfail.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/allocfail.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/atomic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/backtrace-supported.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/backtrace.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/backtrace.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/btest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:47.659533 memray-1.9.1/src/vendor/libbacktrace/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/enable.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/lead-dot.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/multi.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/override.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/unwind_ipinfo.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config/warnings.m4
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config.guess
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/config.sub
+-rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/configure
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/debuginfod_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/dwarf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/edtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/edtest2.c
+-rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/elf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/fileline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/filenames.h
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/filetype.awk
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/install-sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/instrumented_alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ltmain.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/macho.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/missing
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/mmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/mmapio.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/move-if-change
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/mtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/nounwind.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/pecoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/posix.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/print.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/read.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/sort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/stest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/test-driver
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/test_format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/testlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/testlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ttest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/unittest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/unknown.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/xcoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/xztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace/ztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-08-01 22:54:32.000000 memray-1.9.1/src/vendor/regenerate_libbacktrace.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 22:54:32.000000 memray-1.9.1/webpack.config.js
```

### Comparing `memray-1.9.0/.pre-commit-config.yaml` & `memray-1.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/LICENSE` & `memray-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/MANIFEST.in` & `memray-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/Makefile` & `memray-1.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/NEWS.rst` & `memray-1.9.1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,25 @@
     fix problems like typo corrections or such.
 
 Changelog
 =========
 
 .. towncrier release notes start
 
+memray 1.9.1 (2023-08-01)
+-------------------------
+
+Bug Fixes
+~~~~~~~~~
+
+- Fix an issue that stopped Memray's experimental support for ``greenlet`` from working with versions of the ``greenlet`` module older than 1.0. (#432)
+- Fix a bug leading to a deadlock when Memray is used to profile an application that uses the jemalloc implementation of ``malloc``. (#433)
+- Fix a bug causing the ``summary`` reporter to generate empty reports. (#435)
+
+
 memray 1.9.0 (2023-07-28)
 -------------------------
 
 Features
 ~~~~~~~~
 
 - Allow to report the current version of Memray via a ``--version/-V`` command line parameter (#420)
```

### Comparing `memray-1.9.0/PKG-INFO` & `memray-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.9.0
+Version: 1.9.1
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `memray-1.9.0/README.md` & `memray-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/package-lock.json` & `memray-1.9.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/pyproject.toml` & `memray-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/setup.py` & `memray-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     "isort",
     "mypy",
     "check-manifest",
 ]
 
 test_requires = [
     "Cython",
-    "greenlet; python_version < '3.11'",
+    "greenlet; python_version < '3.12'",
     "pytest",
     "pytest-cov",
     "ipython",
     "setuptools; python_version >= '3.12'",
 ]
 
 benchmark_requires = [
```

### Comparing `memray-1.9.0/src/memray/__init__.py` & `memray-1.9.1/src/memray/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/__init__.pyi` & `memray-1.9.1/src/memray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_destination.py` & `memray-1.9.1/src/memray/_destination.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_ipython/flamegraph.py` & `memray-1.9.1/src/memray/_ipython/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/CMakeLists.txt` & `memray-1.9.1/src/memray/_memray/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/alloc.pxd` & `memray-1.9.1/src/memray/_memray/alloc.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/compat.cpp` & `memray-1.9.1/src/memray/_memray/compat.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/compat.h` & `memray-1.9.1/src/memray/_memray/compat.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/elf_shenanigans.cpp` & `memray-1.9.1/src/memray/_memray/elf_shenanigans.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/elf_utils.h` & `memray-1.9.1/src/memray/_memray/elf_utils.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/frame_tree.h` & `memray-1.9.1/src/memray/_memray/frame_tree.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/hooks.cpp` & `memray-1.9.1/src/memray/_memray/hooks.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -162,31 +162,40 @@
 }
 
 void*
 malloc(size_t size) noexcept
 {
     assert(hooks::malloc);
 
-    void* ptr = hooks::malloc(size);
-    tracking_api::Tracker::trackAllocation(ptr, size, hooks::Allocator::MALLOC);
+    void* ptr;
+    {
+        tracking_api::RecursionGuard guard;
+        ptr = hooks::malloc(size);
+    }
+    if (ptr) {
+        tracking_api::Tracker::trackAllocation(ptr, size, hooks::Allocator::MALLOC);
+    }
     return ptr;
 }
 
 void
 free(void* ptr) noexcept
 {
     assert(hooks::free);
 
     // We need to call our API before we call the real free implementation
     // to make sure that the pointer is not reused in-between.
     if (ptr != nullptr) {
         tracking_api::Tracker::trackDeallocation(ptr, 0, hooks::Allocator::FREE);
     }
 
-    hooks::free(ptr);
+    {
+        tracking_api::RecursionGuard guard;
+        hooks::free(ptr);
+    }
 }
 
 void*
 realloc(void* ptr, size_t size) noexcept
 {
     assert(hooks::realloc);
 
@@ -220,36 +229,51 @@
     return ret;
 }
 
 void*
 mmap(void* addr, size_t length, int prot, int flags, int fd, off_t offset) noexcept
 {
     assert(hooks::mmap);
-    void* ptr = hooks::mmap(addr, length, prot, flags, fd, offset);
-    tracking_api::Tracker::trackAllocation(ptr, length, hooks::Allocator::MMAP);
+    void* ptr;
+    {
+        tracking_api::RecursionGuard guard;
+        ptr = hooks::mmap(addr, length, prot, flags, fd, offset);
+    }
+    if (ptr != MAP_FAILED) {
+        tracking_api::Tracker::trackAllocation(ptr, length, hooks::Allocator::MMAP);
+    }
     return ptr;
 }
 
 #if defined(__GLIBC__)
 void*
 mmap64(void* addr, size_t length, int prot, int flags, int fd, off64_t offset) noexcept
 {
     assert(hooks::mmap64);
-    void* ptr = hooks::mmap64(addr, length, prot, flags, fd, offset);
-    tracking_api::Tracker::trackAllocation(ptr, length, hooks::Allocator::MMAP);
+    void* ptr;
+    {
+        tracking_api::RecursionGuard guard;
+        ptr = hooks::mmap64(addr, length, prot, flags, fd, offset);
+    }
+    if (ptr != MAP_FAILED) {
+        tracking_api::Tracker::trackAllocation(ptr, length, hooks::Allocator::MMAP);
+    }
     return ptr;
 }
 #endif
 
 int
 munmap(void* addr, size_t length) noexcept
 {
     assert(hooks::munmap);
     tracking_api::Tracker::trackDeallocation(addr, length, hooks::Allocator::MUNMAP);
-    return hooks::munmap(addr, length);
+    {
+        tracking_api::RecursionGuard guard;
+        return hooks::munmap(addr, length);
+    }
 }
 
 void*
 valloc(size_t size) noexcept
 {
     assert(hooks::valloc);
 
@@ -287,27 +311,33 @@
     void* ret;
     {
         tracking_api::RecursionGuard guard;
         ret = hooks::dlopen(filename, flag);
     }
     if (ret) {
         tracking_api::Tracker::invalidate_module_cache();
-        if (filename && nullptr != strstr(filename, "/_greenlet.")) {
+        if (filename
+            && (nullptr != strstr(filename, "/_greenlet.") || nullptr != strstr(filename, "/greenlet.")))
+        {
             tracking_api::Tracker::beginTrackingGreenlets();
         }
     }
     return ret;
 }
 
 int
 dlclose(void* handle) noexcept
 {
     assert(hooks::dlclose);
 
-    int ret = hooks::dlclose(handle);
+    int ret;
+    {
+        tracking_api::RecursionGuard guard;
+        ret = hooks::dlclose(handle);
+    }
     tracking_api::NativeTrace::flushCache();
     if (!ret) tracking_api::Tracker::invalidate_module_cache();
     return ret;
 }
 
 void*
 aligned_alloc(size_t alignment, size_t size) noexcept
@@ -345,15 +375,19 @@
 
 #    if defined(__GLIBC__)
 void*
 pvalloc(size_t size) noexcept
 {
     assert(hooks::pvalloc);
 
-    void* ret = hooks::pvalloc(size);
+    void* ret;
+    {
+        tracking_api::RecursionGuard guard;
+        ret = hooks::pvalloc(size);
+    }
     if (ret) {
         tracking_api::Tracker::trackAllocation(ret, size, hooks::Allocator::PVALLOC);
     }
     return ret;
 }
 #    endif
```

### Comparing `memray-1.9.0/src/memray/_memray/hooks.h` & `memray-1.9.1/src/memray/_memray/hooks.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/inject.cpp` & `memray-1.9.1/src/memray/_memray/inject.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/logging.cpp` & `memray-1.9.1/src/memray/_memray/logging.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/logging.h` & `memray-1.9.1/src/memray/_memray/logging.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/lz4_stream.h` & `memray-1.9.1/src/memray/_memray/lz4_stream.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/macho_shenanigans.cpp` & `memray-1.9.1/src/memray/_memray/macho_shenanigans.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/macho_utils.h` & `memray-1.9.1/src/memray/_memray/macho_utils.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/native_resolver.cpp` & `memray-1.9.1/src/memray/_memray/native_resolver.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/native_resolver.h` & `memray-1.9.1/src/memray/_memray/native_resolver.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/pthread.pxd` & `memray-1.9.1/src/memray/_memray/pthread.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/python_helpers.cpp` & `memray-1.9.1/src/memray/_memray/python_helpers.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/record_reader.cpp` & `memray-1.9.1/src/memray/_memray/record_reader.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/record_reader.h` & `memray-1.9.1/src/memray/_memray/record_reader.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/record_reader.pxd` & `memray-1.9.1/src/memray/_memray/record_reader.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/record_writer.cpp` & `memray-1.9.1/src/memray/_memray/record_writer.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/record_writer.h` & `memray-1.9.1/src/memray/_memray/record_writer.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/records.cpp` & `memray-1.9.1/src/memray/_memray/records.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/records.h` & `memray-1.9.1/src/memray/_memray/records.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/records.pxd` & `memray-1.9.1/src/memray/_memray/records.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/sink.cpp` & `memray-1.9.1/src/memray/_memray/sink.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/sink.h` & `memray-1.9.1/src/memray/_memray/sink.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/snapshot.cpp` & `memray-1.9.1/src/memray/_memray/snapshot.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/snapshot.h` & `memray-1.9.1/src/memray/_memray/snapshot.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/snapshot.pxd` & `memray-1.9.1/src/memray/_memray/snapshot.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/socket_reader_thread.cpp` & `memray-1.9.1/src/memray/_memray/socket_reader_thread.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/socket_reader_thread.h` & `memray-1.9.1/src/memray/_memray/socket_reader_thread.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/source.cpp` & `memray-1.9.1/src/memray/_memray/source.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/source.h` & `memray-1.9.1/src/memray/_memray/source.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/tracking_api.cpp` & `memray-1.9.1/src/memray/_memray/tracking_api.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,19 @@
     }
 
     // Borrowed reference
     // Look directly at `sys.modules` since we only want to do something if
     // `greenlet._greenlet` has already been imported.
     PyObject* _greenlet = PyDict_GetItemString(modules, "greenlet._greenlet");
     if (!_greenlet) {
-        return;
+        // Before greenlet 1.0, the extension module was just named "greenlet"
+        _greenlet = PyDict_GetItemString(modules, "greenlet");
+        if (!_greenlet) {
+            return;
+        }
     }
 
     // Borrowed reference
     PyObject* _memray = PyDict_GetItemString(modules, "memray._memray");
     if (!_memray) {
         return;
     }
```

### Comparing `memray-1.9.0/src/memray/_memray/tracking_api.h` & `memray-1.9.1/src/memray/_memray/tracking_api.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray/tracking_api.pxd` & `memray-1.9.1/src/memray/_memray/tracking_api.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray.pyi` & `memray-1.9.1/src/memray/_memray.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_memray.pyx` & `memray-1.9.1/src/memray/_memray.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,15 @@
             raise RuntimeError("Attempting to use stale output handle")
         writer = move(self._writer)
 
         self._previous_profile_func = sys.getprofile()
         self._previous_thread_profile_func = threading._profile_hook
         threading.setprofile(start_thread_trace)
 
-        if "greenlet._greenlet" in sys.modules:
+        if "greenlet" in sys.modules:
             NativeTracker.beginTrackingGreenlets()
 
         NativeTracker.createTracker(
             move(writer),
             self._native_traces,
             self._memory_interval_ms,
             self._follow_fork,
```

### Comparing `memray-1.9.0/src/memray/_memray_test_utils.pyx` & `memray-1.9.1/src/memray/_memray_test_utils.pyx`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_test.py` & `memray-1.9.1/src/memray/_test.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/_test_utils.pyi` & `memray-1.9.1/src/memray/_test_utils.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/__init__.py` & `memray-1.9.1/src/memray/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/_attach.gdb` & `memray-1.9.1/src/memray/commands/_attach.gdb`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/_attach.lldb` & `memray-1.9.1/src/memray/commands/_attach.lldb`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/attach.py` & `memray-1.9.1/src/memray/commands/attach.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/common.py` & `memray-1.9.1/src/memray/commands/common.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/flamegraph.py` & `memray-1.9.1/src/memray/commands/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/live.py` & `memray-1.9.1/src/memray/commands/live.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/parse.py` & `memray-1.9.1/src/memray/commands/parse.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/run.py` & `memray-1.9.1/src/memray/commands/run.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/stats.py` & `memray-1.9.1/src/memray/commands/stats.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/summary.py` & `memray-1.9.1/src/memray/commands/summary.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/transform.py` & `memray-1.9.1/src/memray/commands/transform.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/commands/tree.py` & `memray-1.9.1/src/memray/commands/tree.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/common.js` & `memray-1.9.1/src/memray/reporters/assets/common.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/common.test.js` & `memray-1.9.1/src/memray/reporters/assets/common.test.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/flamegraph.js` & `memray-1.9.1/src/memray/reporters/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/flamegraph_common.js` & `memray-1.9.1/src/memray/reporters/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/table.js` & `memray-1.9.1/src/memray/reporters/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/assets/temporal_flamegraph.js` & `memray-1.9.1/src/memray/reporters/assets/temporal_flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/flamegraph.py` & `memray-1.9.1/src/memray/reporters/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/frame_tools.py` & `memray-1.9.1/src/memray/reporters/frame_tools.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/stats.py` & `memray-1.9.1/src/memray/reporters/stats.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/summary.py` & `memray-1.9.1/src/memray/reporters/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class SummaryReporter:
     N_COLUMNS = len(TUI.KEY_TO_COLUMN_NAME)
 
     def __init__(self, data: Iterable[AllocationRecord], native: bool):
         super().__init__()
         self.data = data
         self._tui = TUI(pid=None, cmd_line=None, native=native)
-        self._tui.update_snapshot(data)
+        self._tui.update_snapshot(tuple(data))
 
     @classmethod
     def from_snapshot(
         cls, allocations: Iterable[AllocationRecord], native: bool = False
     ) -> "SummaryReporter":
         return cls(allocations, native=native)
```

### Comparing `memray-1.9.0/src/memray/reporters/table.py` & `memray-1.9.1/src/memray/reporters/table.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/__init__.py` & `memray-1.9.1/src/memray/reporters/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.css` & `memray-1.9.1/src/memray/reporters/templates/assets/flamegraph.css`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.js` & `memray-1.9.1/src/memray/reporters/templates/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph_common.js` & `memray-1.9.1/src/memray/reporters/templates/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/assets/table.js` & `memray-1.9.1/src/memray/reporters/templates/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/assets/temporal_flamegraph.js` & `memray-1.9.1/src/memray/reporters/templates/assets/temporal_flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/base.html` & `memray-1.9.1/src/memray/reporters/templates/base.html`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/classic_base.html` & `memray-1.9.1/src/memray/reporters/templates/classic_base.html`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/flamegraph.html` & `memray-1.9.1/src/memray/reporters/templates/flamegraph.html`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/table.html` & `memray-1.9.1/src/memray/reporters/templates/table.html`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/templates/temporal_flamegraph.html` & `memray-1.9.1/src/memray/reporters/templates/temporal_flamegraph.html`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/transform.py` & `memray-1.9.1/src/memray/reporters/transform.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/tree.py` & `memray-1.9.1/src/memray/reporters/tree.py`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray/reporters/tui.py` & `memray-1.9.1/src/memray/reporters/tui.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from math import ceil
 from typing import DefaultDict
 from typing import Deque
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
+from typing import Sequence
 from typing import Set
 from typing import Tuple
 
 from rich.layout import Layout
 from rich.markup import escape
 from rich.panel import Panel
 from rich.progress_bar import ProgressBar
@@ -422,15 +423,15 @@
         self.layout["header"].update(self.get_header())
         self.layout["heap_size"].update(self.get_heap_size())
         self.layout["table"].update(self.get_body())
         self.layout["message"].update(self.message)
         self.layout["footer"].update(self.footer())
         return self.layout
 
-    def update_snapshot(self, snapshot: Iterable[AllocationRecord]) -> None:
+    def update_snapshot(self, snapshot: Sequence[AllocationRecord]) -> None:
         for record in snapshot:
             if record.tid in self._seen_threads:
                 continue
             if self._threads is self._DUMMY_THREAD_LIST:
                 self._threads = []
             self._threads.append(record.tid)
             self._seen_threads.add(record.tid)
```

### Comparing `memray-1.9.0/src/memray.egg-info/PKG-INFO` & `memray-1.9.1/src/memray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.9.0
+Version: 1.9.1
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `memray-1.9.0/src/memray.egg-info/SOURCES.txt` & `memray-1.9.1/src/memray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/memray.egg-info/requires.txt` & `memray-1.9.1/src/memray.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 bump2version
 sphinx
 furo
 sphinx-argparse
 towncrier
 asv
 
-[dev:python_version < "3.11"]
+[dev:python_version < "3.12"]
 greenlet
 
 [dev:python_version >= "3.12"]
 setuptools
 
 [docs]
 IPython
@@ -48,12 +48,12 @@
 
 [test]
 Cython
 pytest
 pytest-cov
 ipython
 
-[test:python_version < "3.11"]
+[test:python_version < "3.12"]
 greenlet
 
 [test:python_version >= "3.12"]
 setuptools
```

### Comparing `memray-1.9.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt` & `memray-1.9.1/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/LICENSE` & `memray-1.9.1/src/vendor/libbacktrace/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/Makefile.am` & `memray-1.9.1/src/vendor/libbacktrace/Makefile.am`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/Makefile.in` & `memray-1.9.1/src/vendor/libbacktrace/Makefile.in`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/README.md` & `memray-1.9.1/src/vendor/libbacktrace/README.md`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/aclocal.m4` & `memray-1.9.1/src/vendor/libbacktrace/aclocal.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/alloc.c` & `memray-1.9.1/src/vendor/libbacktrace/alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/allocfail.c` & `memray-1.9.1/src/vendor/libbacktrace/allocfail.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/allocfail.sh` & `memray-1.9.1/src/vendor/libbacktrace/allocfail.sh`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/atomic.c` & `memray-1.9.1/src/vendor/libbacktrace/atomic.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/backtrace-supported.h.in` & `memray-1.9.1/src/vendor/libbacktrace/backtrace-supported.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/backtrace.c` & `memray-1.9.1/src/vendor/libbacktrace/backtrace.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/backtrace.h` & `memray-1.9.1/src/vendor/libbacktrace/backtrace.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/btest.c` & `memray-1.9.1/src/vendor/libbacktrace/btest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/compile` & `memray-1.9.1/src/vendor/libbacktrace/compile`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/enable.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/enable.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/lead-dot.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/lead-dot.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/libtool.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/ltoptions.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/ltsugar.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/ltversion.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/lt~obsolete.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/multi.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/multi.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/override.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/override.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/unwind_ipinfo.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config/warnings.m4` & `memray-1.9.1/src/vendor/libbacktrace/config/warnings.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config.guess` & `memray-1.9.1/src/vendor/libbacktrace/config.guess`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config.h.in` & `memray-1.9.1/src/vendor/libbacktrace/config.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/config.sub` & `memray-1.9.1/src/vendor/libbacktrace/config.sub`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/configure` & `memray-1.9.1/src/vendor/libbacktrace/configure`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/configure.ac` & `memray-1.9.1/src/vendor/libbacktrace/configure.ac`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/debuginfod_support.h` & `memray-1.9.1/src/vendor/libbacktrace/debuginfod_support.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/dwarf.c` & `memray-1.9.1/src/vendor/libbacktrace/dwarf.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/edtest.c` & `memray-1.9.1/src/vendor/libbacktrace/edtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/edtest2.c` & `memray-1.9.1/src/vendor/libbacktrace/edtest2.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/elf.c` & `memray-1.9.1/src/vendor/libbacktrace/elf.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/fileline.c` & `memray-1.9.1/src/vendor/libbacktrace/fileline.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/filenames.h` & `memray-1.9.1/src/vendor/libbacktrace/filenames.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/filetype.awk` & `memray-1.9.1/src/vendor/libbacktrace/filetype.awk`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in` & `memray-1.9.1/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/install-sh` & `memray-1.9.1/src/vendor/libbacktrace/install-sh`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/instrumented_alloc.c` & `memray-1.9.1/src/vendor/libbacktrace/instrumented_alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/internal.h` & `memray-1.9.1/src/vendor/libbacktrace/internal.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/libtool.m4` & `memray-1.9.1/src/vendor/libbacktrace/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ltmain.sh` & `memray-1.9.1/src/vendor/libbacktrace/ltmain.sh`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ltoptions.m4` & `memray-1.9.1/src/vendor/libbacktrace/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ltsugar.m4` & `memray-1.9.1/src/vendor/libbacktrace/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ltversion.m4` & `memray-1.9.1/src/vendor/libbacktrace/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/lt~obsolete.m4` & `memray-1.9.1/src/vendor/libbacktrace/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/macho.c` & `memray-1.9.1/src/vendor/libbacktrace/macho.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/missing` & `memray-1.9.1/src/vendor/libbacktrace/missing`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/mmap.c` & `memray-1.9.1/src/vendor/libbacktrace/mmap.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/mmapio.c` & `memray-1.9.1/src/vendor/libbacktrace/mmapio.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/move-if-change` & `memray-1.9.1/src/vendor/libbacktrace/move-if-change`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/mtest.c` & `memray-1.9.1/src/vendor/libbacktrace/mtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/nounwind.c` & `memray-1.9.1/src/vendor/libbacktrace/nounwind.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/pecoff.c` & `memray-1.9.1/src/vendor/libbacktrace/pecoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/posix.c` & `memray-1.9.1/src/vendor/libbacktrace/posix.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/print.c` & `memray-1.9.1/src/vendor/libbacktrace/print.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/read.c` & `memray-1.9.1/src/vendor/libbacktrace/read.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/simple.c` & `memray-1.9.1/src/vendor/libbacktrace/simple.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/sort.c` & `memray-1.9.1/src/vendor/libbacktrace/sort.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/state.c` & `memray-1.9.1/src/vendor/libbacktrace/state.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/stest.c` & `memray-1.9.1/src/vendor/libbacktrace/stest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/test-driver` & `memray-1.9.1/src/vendor/libbacktrace/test-driver`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/test_format.c` & `memray-1.9.1/src/vendor/libbacktrace/test_format.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/testlib.c` & `memray-1.9.1/src/vendor/libbacktrace/testlib.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/testlib.h` & `memray-1.9.1/src/vendor/libbacktrace/testlib.h`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ttest.c` & `memray-1.9.1/src/vendor/libbacktrace/ttest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/unittest.c` & `memray-1.9.1/src/vendor/libbacktrace/unittest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/unknown.c` & `memray-1.9.1/src/vendor/libbacktrace/unknown.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/xcoff.c` & `memray-1.9.1/src/vendor/libbacktrace/xcoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/xztest.c` & `memray-1.9.1/src/vendor/libbacktrace/xztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace/ztest.c` & `memray-1.9.1/src/vendor/libbacktrace/ztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff` & `memray-1.9.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff` & `memray-1.9.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/src/vendor/regenerate_libbacktrace.sh` & `memray-1.9.1/src/vendor/regenerate_libbacktrace.sh`

 * *Files identical despite different names*

### Comparing `memray-1.9.0/webpack.config.js` & `memray-1.9.1/webpack.config.js`

 * *Files identical despite different names*

