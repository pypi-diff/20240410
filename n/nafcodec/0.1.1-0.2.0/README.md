# Comparing `tmp/nafcodec-0.1.1.tar.gz` & `tmp/nafcodec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nafcodec-0.1.1.tar", last modified: Sun Oct  8 19:09:24 2023, max compression
+gzip compressed data, was "nafcodec-0.2.0.tar", last modified: Wed Apr 10 09:41:36 2024, max compression
```

## Comparing `nafcodec-0.1.1.tar` & `nafcodec-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-10-08 19:09:18.000000 nafcodec-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-10-08 19:09:18.000000 nafcodec-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-08 19:09:18.000000 nafcodec-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2023-10-08 19:09:24.953657 nafcodec-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-10-08 19:09:18.000000 nafcodec-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.949657 nafcodec-0.1.1/nafcodec/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-10-08 19:09:18.000000 nafcodec-0.1.1/nafcodec/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/data.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec/src/decoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/decoder/ioslice.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15180 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/decoder/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/decoder/parser.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/decoder/reader.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/tests/dna.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/tests/fastq.rs
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec/tests/protein.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.949657 nafcodec-0.1.1/nafcodec-py/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec-py/nafcodec/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-10-08 19:09:18.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/LuxC.naf
--rw-r--r--   0 runner    (1001) docker     (127)  1331207 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/NZ_AAEN01000029.naf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/masked.naf
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/phix.naf
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-08 19:09:19.000000 nafcodec-0.1.1/nafcodec-py/nafcodec/tests/unittest.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:09:24.953657 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2023-10-08 19:09:24.000000 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-08 19:09:24.000000 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 19:09:24.000000 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-08 19:09:24.000000 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 19:09:24.000000 nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-08 19:09:24.000000 nafcodec-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-10-08 19:09:24.957657 nafcodec-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-10-08 19:09:19.000000 nafcodec-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 09:41:32.000000 nafcodec-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 09:41:32.000000 nafcodec-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 09:41:32.000000 nafcodec-0.2.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 09:41:32.000000 nafcodec-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-10 09:41:36.225393 nafcodec-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-10 09:41:32.000000 nafcodec-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.221392 nafcodec-0.2.0/nafcodec/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/data.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec/src/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/decoder/ioslice.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/decoder/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/decoder/parser.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/decoder/reader.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec/src/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/encoder/counter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/encoder/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/encoder/storage.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/encoder/writer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec/tests/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/tests/decoder/dna.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/tests/decoder/fastq.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/tests/decoder/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/tests/decoder/protein.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec/tests/encoder.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.221392 nafcodec-0.2.0/nafcodec-py/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.221392 nafcodec-0.2.0/nafcodec-py/nafcodec/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/pyfile.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.221392 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.225393 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    26342 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/CP040672.naf
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/LuxC.naf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/masked.naf
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/phix.naf
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-10 09:41:32.000000 nafcodec-0.2.0/nafcodec-py/nafcodec/tests/unittest.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:41:36.221392 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-10 09:41:36.000000 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-10 09:41:36.000000 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:41:36.000000 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 09:41:36.000000 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:41:36.000000 nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 09:41:36.000000 nafcodec-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 09:41:36.225393 nafcodec-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-10 09:41:32.000000 nafcodec-0.2.0/setup.py
```

### Comparing `nafcodec-0.1.1/COPYING` & `nafcodec-0.2.0/COPYING`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Martin Larralde <martin.larralde@embl.de>
+Copyright (c) 2023-2024 Martin Larralde <martin.larralde@embl.de>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nafcodec-0.1.1/PKG-INFO` & `nafcodec-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nafcodec
-Version: 0.1.1
+Version: 0.2.0
 Summary: PyO3 bindings and Python interface to nafcodec, an encoder/decoder for Nucleotide Archive Format (NAF) files.
 Home-page: https://github.com/althonos/nafcodec
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/nafcodec/issues
 Project-URL: Changelog, https://github.com/althonos/nafcodec/blob/master/CHANGELOG.md
@@ -20,29 +20,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 📦🧬 `nafcodec` [![Stars](https://img.shields.io/github/stars/althonos/nafcodec.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/nafcodec/stargazers)
 
 *Rust coder/decoder for [Nucleotide Archive Format (NAF)](https://github.com/KirillKryukov/naf) files*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/nafcodec/python.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/nafcodec/actions)
-[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/nafcodec/)
+[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://app.codecov.io/gh/althonos/nafcodec)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Docs](https://img.shields.io/readthedocs/nafcodec/latest?style=flat-square&maxAge=600)](https://nafcodec.readthedocs.io)
 [![Crate](https://img.shields.io/crates/v/nafcodec-py.svg?maxAge=600&style=flat-square)](https://crates.io/crates/nafcodec-py)
 [![PyPI](https://img.shields.io/pypi/v/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec)
 [![Wheel](https://img.shields.io/pypi/wheel/nafcodec.svg?style=flat-square&maxAge=2678400)](https://pypi.org/project/nafcodec/#files)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/nafcodec?style=flat-square&maxAge=3600)](https://anaconda.org/bioconda/nafcodec)
 [![Python Versions](https://img.shields.io/pypi/pyversions/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec/#files)
@@ -65,35 +66,36 @@
 
 This library provides [PyO3](https://pyo3.rs) bindings to the `nafcodec` crate,
 a Rust implementation of a NAF decoder using [`nom`](https://crates.io/crates/nom) 
 for parsing the binary format, and [`zstd`](https://crates.io/crates/zstd) for 
 handling Zstandard decompression. It provides a complete API that allows 
 iterating over the contents of a NAF file.
 
-*This is the Python version, there is a [Rust crate](https://crates.io/crate/nafcodec) available as well.*
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/nafcodec) available as well.*
 
 ### 📋 Features
 
 - **streaming decoder**: The decoder is implemented using different readers
   each accessing a region of the compressed file, allowing to stream records
   without having to decode full blocks.
+- **file-like decoding**: Allow the decoder to read from a file-like object
+  instead of expecting a path.
 
 The following features are planned:
 
-- **file-like decoding**: Allow the decoder to read from a file-like object
-  instead of expecting a path.
 - **optional decoding**: Allow the decoder to skip the decoding of certains
   fields, such as ignoring quality strings when they are not needed.
 - **encoder**: Implement an encoder as well, using either in-memory buffers
   or temporary files to grow the archive.
 
 ### 🔌 Usage
 
-Use `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive Format,
-reading from the given path
+Use a `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive 
+Format, reading from the given [path-like](https://docs.python.org/3/glossary.html#term-path-like-object)
+or [file-like](https://docs.python.org/3/glossary.html#term-file-object) object:
 
 ```python
 import nafcodec
 
 decoder = nafcodec.Decoder("../data/LuxC.naf")
 for record in decoder:
     print(record.id)
```

### Comparing `nafcodec-0.1.1/README.md` & `nafcodec-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 📦🧬 `nafcodec` [![Stars](https://img.shields.io/github/stars/althonos/nafcodec.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/nafcodec/stargazers)
 
 *Rust coder/decoder for [Nucleotide Archive Format (NAF)](https://github.com/KirillKryukov/naf) files*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/nafcodec/rust.yml?branch=main&style=flat-square&maxAge=600)](https://github.com/althonos/nafcodec/actions)
-[![Codecov](https://img.shields.io/codecov/c/gh/althonos/nafcodec/master.svg?style=flat-square&maxAge=600)](https://codecov.io/gh/althonos/nafcodec)
+[![Codecov](https://img.shields.io/codecov/c/gh/althonos/nafcodec/master.svg?style=flat-square&maxAge=600)](https://app.codecov.io/gh/althonos/nafcodec)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/nafcodec)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/nafcodec/)
 [![Crate](https://img.shields.io/crates/v/nafcodec.svg?maxAge=600&style=flat-square)](https://crates.io/crates/nafcodec)
 [![Documentation](https://img.shields.io/badge/docs.rs-latest-4d76ae.svg?maxAge=2678400&style=flat-square)](https://docs.rs/nafcodec)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/nafcodec/blob/master/CHANGELOG.md)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/nafcodec.svg?style=flat-square&maxAge=600)](https://github.com/althonos/nafcodec/issues)
@@ -33,68 +33,69 @@
 ### 📋 Features
 
 - **streaming decoder**: The decoder is implemented using different readers
   each accessing a region of the compressed file, allowing to stream records
   without having to decode full blocks.
 - **optional decoding**: Allow the decoder to skip the decoding of certains
   fields, such as ignoring quality strings when they are not needed.
-
-The following features are planned:
-
-- **encoder**: Implement an encoder as well, using either in-memory buffers
-  or temporary files to grow the archive.
+- **flexible encoder**: The encoder is implemented using an abstract storage
+  interface for temporary data, which allows to keep sequence in memory or
+  inside a temporary folder.
 
 ### 🔌 Usage
 
-Use `nafcodec::Decoder` to iterate over the contents of a Nucleotide Archive Format,
+Use a [`Decoder`](https://docs.rs/nafcodec/latest/nafcodec/struct.Decoder.html) 
+to iterate over the contents of a Nucleotide Archive Format,
 reading from any [`BufRead`](https://doc.rust-lang.org/nightly/std/io/trait.BufRead.html) +
 [`Seek`](https://doc.rust-lang.org/nightly/std/io/trait.Seek.html) implementor:
 
 ```rust
 let mut decoder = nafcodec::Decoder::from_path("../data/LuxC.naf")
-  .expect("failed to open nucleotide archive");
+    .expect("failed to open nucleotide archive");
 
 for result in decoder {
     let record = result.unwrap();
     // .. do something with the record .. //
 }
 ```
 
-All fields of the obtained `Record` are optional, and actually depend on the
-kind of data that was compressed. The decoder can be configured through
-a `DecoderBuilder` to ignore some fields to make decompression faster,
-even if they are present in the source archive:
+All fields of the obtained [`Record`](https://docs.rs/nafcodec/latest/nafcodec/data/struct.Record.html) 
+are optional, and actually depend on the kind of data that was compressed. 
+The decoder can be configured through a 
+[`DecoderBuilder`](https://docs.rs/nafcodec/latest/nafcodec/struct.DecoderBuilder.html) 
+to ignore some fields to make decompression faster, even if they are present 
+in the source archive:
 
 ```rust
 let mut decoder = nafcodec::DecoderBuilder::new()
     .quality(false)
-    .from_path("../data/phix.naf")
+    .with_path("../data/phix.naf")
     .expect("failed to open nucleotide archive");
 
 // the archive contains quality strings...
-assert!(decoder.header().flags().has_quality());
+assert!(decoder.header().flags().test(nafcodec::Flag::Quality));
 
 // ... but we configured the decoder to ignore them
 for result in decoder {
     let record = result.unwrap();
     assert!(record.quality.is_none())
 }
 ```
 
 <!-- ## 🔍 See Also -->
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
 
-Found a bug ? Have an enhancement request ? Head over to the [GitHub issue
-tracker](https://github.com/althonos/nafcodec/issues) if you need to report
-or ask something. If you are filing in on a bug, please include as much
-information as you can about the issue, and try to recreate the same bug
-in a simple, easily reproducible situation.
+Found a bug ? Have an enhancement request ? Head over to the 
+[GitHub issue tracker](https://github.com/althonos/nafcodec/issues) if you 
+need to report or ask something. If you are filing in on a bug, please include 
+as much information as you can about the issue, and try to recreate the same 
+bug in a simple, easily reproducible situation.
 
 <!-- ### 🏗️ Contributing
 
 Contributions are more than welcome! See [`CONTRIBUTING.md`](https://github.com/althonos/nafcodec/blob/master/CONTRIBUTING.md) for more details. -->
 
 
 ## 📋 Changelog
```

### Comparing `nafcodec-0.1.1/nafcodec/README.md` & `nafcodec-0.2.0/nafcodec/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 📦🧬 `nafcodec` [![Stars](https://img.shields.io/github/stars/althonos/nafcodec.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/nafcodec/stargazers)
 
 *Rust coder/decoder for [Nucleotide Archive Format (NAF)](https://github.com/KirillKryukov/naf) files*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/nafcodec/rust.yml?branch=main&style=flat-square&maxAge=600)](https://github.com/althonos/nafcodec/actions)
-[![Codecov](https://img.shields.io/codecov/c/gh/althonos/nafcodec/master.svg?style=flat-square&maxAge=600)](https://codecov.io/gh/althonos/nafcodec)
+[![Codecov](https://img.shields.io/codecov/c/gh/althonos/nafcodec/master.svg?style=flat-square&maxAge=600)](https://app.codecov.io/gh/althonos/nafcodec)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/nafcodec)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/nafcodec/)
 [![Crate](https://img.shields.io/crates/v/nafcodec.svg?maxAge=600&style=flat-square)](https://crates.io/crates/nafcodec)
 [![Documentation](https://img.shields.io/badge/docs.rs-latest-4d76ae.svg?maxAge=2678400&style=flat-square)](https://docs.rs/nafcodec)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/nafcodec/blob/master/CHANGELOG.md)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/nafcodec.svg?style=flat-square&maxAge=600)](https://github.com/althonos/nafcodec/issues)
@@ -33,68 +33,69 @@
 ### 📋 Features
 
 - **streaming decoder**: The decoder is implemented using different readers
   each accessing a region of the compressed file, allowing to stream records
   without having to decode full blocks.
 - **optional decoding**: Allow the decoder to skip the decoding of certains
   fields, such as ignoring quality strings when they are not needed.
-
-The following features are planned:
-
-- **encoder**: Implement an encoder as well, using either in-memory buffers
-  or temporary files to grow the archive.
+- **flexible encoder**: The encoder is implemented using an abstract storage
+  interface for temporary data, which allows to keep sequence in memory or
+  inside a temporary folder.
 
 ### 🔌 Usage
 
-Use `nafcodec::Decoder` to iterate over the contents of a Nucleotide Archive Format,
+Use a [`Decoder`](https://docs.rs/nafcodec/latest/nafcodec/struct.Decoder.html) 
+to iterate over the contents of a Nucleotide Archive Format,
 reading from any [`BufRead`](https://doc.rust-lang.org/nightly/std/io/trait.BufRead.html) +
 [`Seek`](https://doc.rust-lang.org/nightly/std/io/trait.Seek.html) implementor:
 
 ```rust
 let mut decoder = nafcodec::Decoder::from_path("../data/LuxC.naf")
-  .expect("failed to open nucleotide archive");
+    .expect("failed to open nucleotide archive");
 
 for result in decoder {
     let record = result.unwrap();
     // .. do something with the record .. //
 }
 ```
 
-All fields of the obtained `Record` are optional, and actually depend on the
-kind of data that was compressed. The decoder can be configured through
-a `DecoderBuilder` to ignore some fields to make decompression faster,
-even if they are present in the source archive:
+All fields of the obtained [`Record`](https://docs.rs/nafcodec/latest/nafcodec/data/struct.Record.html) 
+are optional, and actually depend on the kind of data that was compressed. 
+The decoder can be configured through a 
+[`DecoderBuilder`](https://docs.rs/nafcodec/latest/nafcodec/struct.DecoderBuilder.html) 
+to ignore some fields to make decompression faster, even if they are present 
+in the source archive:
 
 ```rust
 let mut decoder = nafcodec::DecoderBuilder::new()
     .quality(false)
-    .from_path("../data/phix.naf")
+    .with_path("../data/phix.naf")
     .expect("failed to open nucleotide archive");
 
 // the archive contains quality strings...
-assert!(decoder.header().flags().has_quality());
+assert!(decoder.header().flags().test(nafcodec::Flag::Quality));
 
 // ... but we configured the decoder to ignore them
 for result in decoder {
     let record = result.unwrap();
     assert!(record.quality.is_none())
 }
 ```
 
 <!-- ## 🔍 See Also -->
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
 
-Found a bug ? Have an enhancement request ? Head over to the [GitHub issue
-tracker](https://github.com/althonos/nafcodec/issues) if you need to report
-or ask something. If you are filing in on a bug, please include as much
-information as you can about the issue, and try to recreate the same bug
-in a simple, easily reproducible situation.
+Found a bug ? Have an enhancement request ? Head over to the 
+[GitHub issue tracker](https://github.com/althonos/nafcodec/issues) if you 
+need to report or ask something. If you are filing in on a bug, please include 
+as much information as you can about the issue, and try to recreate the same 
+bug in a simple, easily reproducible situation.
 
 <!-- ### 🏗️ Contributing
 
 Contributions are more than welcome! See [`CONTRIBUTING.md`](https://github.com/althonos/nafcodec/blob/master/CONTRIBUTING.md) for more details. -->
 
 
 ## 📋 Changelog
```

### Comparing `nafcodec-0.1.1/nafcodec/src/decoder/mod.rs` & `nafcodec-0.2.0/nafcodec/src/decoder/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,175 @@
 use std::fmt::Debug;
 use std::fs::File;
 use std::io::BufRead;
 use std::io::BufReader;
+use std::io::Cursor;
 use std::io::Seek;
 use std::io::SeekFrom;
 use std::iter::FusedIterator;
 use std::path::Path;
 use std::sync::RwLock;
 
 mod ioslice;
 mod parser;
 mod reader;
 
 use self::ioslice::IoSlice;
-use self::reader::*;
+use self::reader::CStringReader;
+use self::reader::LengthReader;
+use self::reader::MaskReader;
+use self::reader::SequenceReader;
+use super::Rc;
+use crate::data::Flag;
+use crate::data::Flags;
 use crate::data::Header;
 use crate::data::MaskUnit;
 use crate::data::Record;
 use crate::data::SequenceType;
 use crate::error::Error;
 
-/// The reference counter type used to share the stream.
-#[cfg(feature = "arc")]
-type Rc<T> = std::sync::Arc<T>;
-#[cfg(not(feature = "arc"))]
-type Rc<T> = std::rc::Rc<T>;
-
 /// The wrapper used to decode Zstandard stream.
-type ZstdDecoder<'z, R> = BufReader<zstd::stream::read::Decoder<'z, BufReader<IoSlice<R>>>>;
+type ZstdDecoder<'z, R> = BufReader<zstd::Decoder<'z, BufReader<IoSlice<R>>>>;
 
-/// A builder to configure and initialize a [`Decoder`](./struct.Decoder.html).
+/// A builder to configure and initialize a [`Decoder`].
+///
+/// The fields to decode are *opt-out*: by default, the [`Decoder`] will
+/// extract all available fields found in the archive into each [`Record`].
+/// Use the provided methods to avoid decoding uneeded fields.
 ///
-/// Use the provided methods to avoid decoding uneeded fields. For instance,
-/// to read a nucleotide archive and only extract sequences names:
+/// For instance, to read a nucleotide archive and only extract
+/// sequences names, skipping decoding of sequences:
 /// ```rust
 /// let decoder = nafcodec::DecoderBuilder::new()
 ///     .sequence(false)
 ///     .quality(false)
-///     .from_path("../data/phix.naf")
+///     .with_path("../data/phix.naf")
 ///     .unwrap();
 /// for record in decoder.map(Result::unwrap) {
 ///     println!(">{}", record.id.unwrap());
 /// }
 /// ```
 #[derive(Debug, Clone)]
 pub struct DecoderBuilder {
     buffer_size: usize,
-    quality: bool,
+    id: bool,
+    comment: bool,
     sequence: bool,
+    quality: bool,
     mask: bool,
 }
 
 impl DecoderBuilder {
     /// Create a new decoder builder with default parameters.
+    ///
+    /// By default, all fields are extracted if they are available in
+    /// the header.
     pub fn new() -> Self {
         Self {
             buffer_size: 4096,
-            quality: true,
+            id: true,
+            comment: true,
             sequence: true,
+            quality: true,
             mask: true,
         }
     }
 
-    /// Build a decoder with this configuration that reads data from the given file path.
-    pub fn from_path<'z, P: AsRef<Path>>(
+    /// Create a new decoder builder from the given flags.
+    ///
+    /// This constructor can be used as a shortcut to setup decoding
+    /// of a subset of supported fields. For instance, to read only the
+    /// sequence identifiers and quality lines from an archive:
+    /// ```
+    /// # use nafcodec::{DecoderBuilder, Flag};
+    /// let mut decoder = DecoderBuilder::from_flags(Flag::Id | Flag::Quality)
+    ///     .with_path("../data/phix.naf")
+    ///     .unwrap();
+    ///
+    /// let record = decoder.next().unwrap().unwrap();
+    /// assert!(record.sequence.is_none());
+    /// assert!(record.quality.is_some());
+    /// ```
+    pub fn from_flags<F: Into<Flags>>(flags: F) -> Self {
+        let flags = flags.into();
+        let mut builder = Self::new();
+        builder.quality(flags.test(Flag::Quality));
+        builder.sequence(flags.test(Flag::Sequence));
+        builder.mask(flags.test(Flag::Mask));
+        builder.comment(flags.test(Flag::Comment));
+        builder
+    }
+
+    /// The buffer size to use while reading.
+    ///
+    /// Note that [`Decoder`] uses a lot of buffered I/O, and that more than
+    /// one buffer will be created. Nevertheless, a higher value will reduce
+    /// the necessity to seek the reader while reading the different blocks.
+    ///
+    /// By default, a buffer size of 4KiB is used for each internal buffer.
+    pub fn buffer_size(&mut self, buffer_size: usize) -> &mut Self {
+        self.buffer_size = buffer_size;
+        self
+    }
+
+    /// Whether or not to decode the sequence identifiers if available.
+    #[inline]
+    pub fn id(&mut self, id: bool) -> &mut Self {
+        self.id = id;
+        self
+    }
+
+    /// Whether or not to decode the sequence comment if available.
+    #[inline]
+    pub fn comment(&mut self, comment: bool) -> &mut Self {
+        self.comment = comment;
+        self
+    }
+
+    /// Whether or not to decode the sequence string if available.
+    #[inline]
+    pub fn sequence(&mut self, sequence: bool) -> &mut Self {
+        self.sequence = sequence;
+        self
+    }
+
+    /// Whether or not to decode the quality string if available.
+    #[inline]
+    pub fn quality(&mut self, quality: bool) -> &mut Self {
+        self.quality = quality;
+        self
+    }
+
+    /// Whether or not to perform region masking in the output sequence.
+    #[inline]
+    pub fn mask(&mut self, mask: bool) -> &mut Self {
+        self.mask = mask;
+        self
+    }
+
+    /// Consume the builder to get a decoder reading data from the given buffer.
+    pub fn with_bytes<'data, 'z>(
+        &self,
+        bytes: &'data [u8],
+    ) -> Result<Decoder<'z, BufReader<Cursor<&'data [u8]>>>, Error> {
+        self.with_reader(BufReader::new(Cursor::new(bytes)))
+    }
+
+    /// Consume the builder to get a decoder reading a file at the given path.
+    pub fn with_path<'z, P: AsRef<Path>>(
         &self,
         path: P,
     ) -> Result<Decoder<'z, BufReader<File>>, Error> {
         File::open(path.as_ref())
             .map_err(Error::from)
-            .and_then(|f| self.from_reader(std::io::BufReader::new(f)))
+            .and_then(|f| self.with_reader(std::io::BufReader::new(f)))
     }
 
-    /// Build a decoder with this configuration that reads data from `reader`.
-    pub fn from_reader<'z, R: BufRead + Seek>(
+    /// Consume the builder to get a decoder reading data from `reader`.
+    pub fn with_reader<'z, R: BufRead + Seek>(
         &self,
         mut reader: R,
     ) -> Result<Decoder<'z, R>, Error> {
         let buffer = reader.fill_buf()?;
         let header = match self::parser::header(buffer) {
             Ok((i, header)) => {
                 let consumed = buffer.len() - i.len();
@@ -91,30 +183,30 @@
                 )));
             }
             Err(nom::Err::Error(e) | nom::Err::Failure(e)) => {
                 return Err(Error::from(e));
             }
         };
 
-        if header.flags().has_title() {
+        if header.flags().test(Flag::Title) {
             let buf = reader.fill_buf()?;
             let (i, _title) = self::parser::title(buf)?;
             let consumed = buf.len() - i.len();
             reader.consume(consumed);
         }
 
         let rc = Rc::new(RwLock::new(reader));
         macro_rules! setup_block {
-            ($flag:expr, $use_block:expr, $rc:ident, $block:ident) => {
+            ($flags:expr, $flag:ident, $use_block:expr, $rc:ident, $block:ident) => {
                 let _length: u64;
-                setup_block!($flag, $use_block, $rc, $block, _length);
+                setup_block!($flags, $flag, $use_block, $rc, $block, _length);
             };
-            ($flag:expr, $use_block:expr, $rc:ident, $block:ident, $block_length:ident) => {
+            ($flags:expr, $flag:ident, $use_block:expr, $rc:ident, $block:ident, $block_length:ident) => {
                 let $block;
-                if $flag {
+                if $flags.test(Flag::$flag) {
                     // create a local copy of the reader that we can access
                     let tee = $rc.clone();
                     let mut handle = $rc.write().unwrap();
                     // decode the block size
                     let buf = handle.fill_buf()?;
                     let (i, original_size) = self::parser::variable_u64(buf)?;
                     let (i, compressed_size) = self::parser::variable_u64(i)?;
@@ -137,135 +229,115 @@
                     $block = None;
                 }
             };
         }
 
         let flags = header.flags();
         let mut seqlen = 0;
-        setup_block!(flags.has_ids(), true, rc, ids_block);
-        setup_block!(flags.has_comments(), true, rc, com_block);
-        setup_block!(flags.has_lengths(), true, rc, len_block);
-        setup_block!(flags.has_mask(), self.mask, rc, mask_block);
-        setup_block!(flags.has_sequence(), self.sequence, rc, seq_block, seqlen);
-        setup_block!(flags.has_quality(), self.quality, rc, quality_block);
+        setup_block!(flags, Id, self.id, rc, ids_block);
+        setup_block!(flags, Comment, self.comment, rc, com_block);
+        setup_block!(flags, Length, true, rc, len_block);
+        setup_block!(flags, Mask, self.mask, rc, mask_block);
+        setup_block!(flags, Sequence, self.sequence, rc, seq_block, seqlen);
+        setup_block!(flags, Quality, self.quality, rc, quality_block);
 
         Ok(Decoder {
             ids: ids_block.map(CStringReader::new),
             com: com_block.map(CStringReader::new),
             len: len_block.map(LengthReader::new),
             seq: seq_block.map(|x| SequenceReader::new(x, header.sequence_type())),
             qual: quality_block.map(|x| SequenceReader::new(x, SequenceType::Text)),
             mask: mask_block.map(|x| MaskReader::new(x, seqlen)),
             n: 0,
             header,
             reader: rc,
             unit: MaskUnit::Unmasked(0),
         })
     }
-
-    /// The buffer size to use while reading.
-    ///
-    /// Note that `Decoder` uses a lot of buffered I/O, and that more than
-    /// one buffer will be created. Nevertheless, a higher value will reduce
-    /// the necessity to seek the reader while reading the different blocks.
-    pub fn buffer_size(&mut self, buffer_size: usize) -> &mut Self {
-        self.buffer_size = buffer_size;
-        self
-    }
-
-    /// Whether or not to decode the sequence string if available.
-    pub fn sequence(&mut self, sequence: bool) -> &mut Self {
-        self.sequence = sequence;
-        self
-    }
-
-    /// Whether or not to decode the quality string if available.
-    pub fn quality(&mut self, quality: bool) -> &mut Self {
-        self.quality = quality;
-        self
-    }
-
-    /// Whether or not to perform region masking in the output sequence.
-    pub fn mask(&mut self, mask: bool) -> &mut Self {
-        self.mask = mask;
-        self
-    }
 }
 
 impl Default for DecoderBuilder {
     fn default() -> Self {
         Self::new()
     }
 }
 
 /// A decoder for Nucleotide Archive Format files.
 ///
 /// The internal reader is shared and accessed non-sequentially to read the
 /// different block components of the archive. This means that the internal
-/// file heavily make use of [`seek`](https://doc.rust-lang.org/std/io/trait.Seek.html#tymethod.seek),
-/// so make sure that the actual type has a fast seeking implementation.
+/// file heavily make use of [`Seek::seek`], so make sure that the actual
+/// type has a fast seeking implementation.
+///
+/// By default, the decoder will decode all available fields, which may not
+/// be needed. Use a [`DecoderBuilder`] to configure decoding of individual
+/// fields.
 ///
 /// # Thread safety
 ///
 /// By default, `Decoder` objects are not [`Send`] because they use reference
 /// counting to share the reader between the different block parsers. Compile
 /// the crate with the *arc* feature to use [`Arc`] instead of [`Rc`], making
 /// the decoder [`Send`].
 ///
-/// [`Send`]: https://doc.rust-lang.org/nightly/std/marker/trait.Send.html
 /// [`Rc`]: https://doc.rust-lang.org/nightly/std/rc/struct.Rc.html
 /// [`Arc`]: https://doc.rust-lang.org/nightly/std/sync/struct.Arc.html
 pub struct Decoder<'z, R: BufRead + Seek> {
     header: Header,
-
     reader: Rc<RwLock<R>>,
-
     ids: Option<CStringReader<ZstdDecoder<'z, R>>>,
     com: Option<CStringReader<ZstdDecoder<'z, R>>>,
     len: Option<LengthReader<ZstdDecoder<'z, R>>>,
     seq: Option<SequenceReader<ZstdDecoder<'z, R>>>,
     qual: Option<SequenceReader<ZstdDecoder<'z, R>>>,
     mask: Option<MaskReader<ZstdDecoder<'z, R>>>,
-
     n: usize,
     unit: MaskUnit,
 }
 
 impl Decoder<'_, BufReader<File>> {
     /// Create a new decoder from the given path.
     ///
     /// This constructor is a shortcut for `DecoderBuilder::new().from_path(path)`.
     /// Use [`DecoderBuilder`](./struct.DecoderBuilder.html) to configure a decoder
     /// with more options.
     pub fn from_path<P: AsRef<Path>>(path: P) -> Result<Self, Error> {
-        DecoderBuilder::new().from_path(path)
+        DecoderBuilder::new().with_path(path)
     }
 }
 
 impl<R: BufRead + Seek> Decoder<'_, R> {
     /// Create a new decoder from the given reader.
     ///
-    /// This constructor is a shortcut for `DecoderBuilder::new().from_reader(reader)`.
+    /// This constructor is a shortcut for `DecoderBuilder::new().with_reader(reader)`.
     /// Use [`DecoderBuilder`](./struct.DecoderBuilder.html) to configure a
     /// decoder with more options.
     pub fn new(reader: R) -> Result<Self, Error> {
-        DecoderBuilder::new().from_reader(reader)
+        DecoderBuilder::new().with_reader(reader)
     }
 
     /// Get the header extracted from the archive.
     ///
     /// The NAF header contains useful metadata which are decoded before
     /// starting to decode the rest of the archive, such as the total number
     /// of sequences (useful for building a progress bar) or the line length
     /// (useful for writing the decoded sequences in FASTA format).
     #[inline]
     pub fn header(&self) -> &Header {
         &self.header
     }
 
+    /// Get the type of sequence in the archive being decoded.
+    ///
+    /// This method is a shortcut for `self.header().sequence_type()`.
+    #[inline]
+    pub fn sequence_type(&self) -> SequenceType {
+        self.header().sequence_type()
+    }
+
     /// Extract the internal reader.
     ///
     /// Note that the internal reader may have been advanced even if no
     /// records were obtained from the decoder yet, since at least the header
     /// needs to be decoded to obtain a working decoder.
     pub fn into_inner(self) -> R {
         let reader = self.reader.clone();
@@ -280,24 +352,24 @@
     ///
     /// This function expects that a record is available; use `Decoder::next`
     /// to check beforehand whether all sequences were read from the archive.
     fn next_record(&mut self) -> Result<Record, Error> {
         let id = self
             .ids
             .as_mut()
-            .map(|r| r.next())
+            .and_then(|r| r.next())
             .transpose()?
             .map(|id| id.into_string().expect("TODO"));
         let comment = self
             .com
             .as_mut()
-            .map(|r| r.next())
+            .and_then(|r| r.next())
             .transpose()?
             .map(|com| com.into_string().expect("TODO"));
-        let length = self.len.as_mut().map(|r| r.next()).transpose()?;
+        let length = self.len.as_mut().and_then(|r| r.next()).transpose()?;
 
         let mut sequence = None;
         let mut quality = None;
         if let Some(l) = length {
             sequence = self.seq.as_mut().map(|r| r.next(l)).transpose()?;
             quality = self.qual.as_mut().map(|r| r.next(l)).transpose()?;
             if let Some(mut seq) = sequence.as_mut() {
@@ -365,24 +437,25 @@
             return None;
         }
         Some(self.next_record())
     }
 
     fn size_hint(&self) -> (usize, Option<usize>) {
         let remaining = self.header.number_of_sequences() as usize - self.n;
-        (0, Some(remaining))
+        (remaining, Some(remaining))
     }
 }
 
+impl<R: BufRead + Seek> ExactSizeIterator for Decoder<'_, R> {}
+
 impl<R: BufRead + Seek> FusedIterator for Decoder<'_, R> {}
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use crate::data::MaskUnit;
 
     const ARCHIVE: &[u8] = include_bytes!("../../../data/LuxC.naf");
 
     #[test]
     fn error_empty() {
         match Decoder::new(std::io::Cursor::new(b"")) {
             Ok(_decoder) => panic!("unexpected success"),
@@ -419,14 +492,14 @@
         );
     }
 
     #[test]
     fn skip_sequence() {
         let decoder = DecoderBuilder::new()
             .sequence(false)
-            .from_reader(std::io::Cursor::new(ARCHIVE))
+            .with_reader(std::io::Cursor::new(ARCHIVE))
             .unwrap();
         for record in decoder.map(Result::unwrap) {
             assert!(record.sequence.is_none());
         }
     }
 }
```

### Comparing `nafcodec-0.1.1/nafcodec/src/decoder/parser.rs` & `nafcodec-0.2.0/nafcodec/src/decoder/parser.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use nom::IResult;
 
+use crate::data::Flag;
 use crate::data::Flags;
 use crate::data::FormatVersion;
 use crate::data::Header;
 use crate::data::SequenceType;
 
 fn is_printable(&byte: &u8) -> bool {
     (0x20..=0x7E).contains(&byte)
@@ -66,15 +67,23 @@
         Ok((i, 2)) => Ok((i, SequenceType::Protein)),
         Ok((i, 3)) => Ok((i, SequenceType::Text)),
         _ => unreachable!(),
     }
 }
 
 pub fn flags(i: &[u8]) -> IResult<&[u8], Flags> {
-    self::byte(i).map(|(i, x)| (i, Flags::new(x)))
+    self::byte(i).map(|(i, x)| {
+        let mut flags = Flags::new();
+        for flag in Flag::values() {
+            if x & flag.as_byte() != 0 {
+                flags.set(*flag);
+            }
+        }
+        (i, flags)
+    })
 }
 
 pub fn name_separator(i: &[u8]) -> IResult<&[u8], char> {
     nom::combinator::verify(self::byte, self::is_printable)(i).map(|(i, c)| (i, c as char))
 }
 
 pub fn line_length(i: &[u8]) -> IResult<&[u8], u64> {
@@ -91,15 +100,15 @@
     let (i, seqty) = match fmt {
         FormatVersion::V1 => (i, SequenceType::Dna),
         FormatVersion::V2 => sequence_type(i)?,
     };
     let (i, f) = flags(i)?;
     let (i, sep) = name_separator(i)?;
     let (i, ll) = line_length(i)?;
-    let (i, nseq) = line_length(i)?;
+    let (i, nseq) = number_of_sequences(i)?;
     Ok((
         i,
         Header {
             format_version: fmt,
             sequence_type: seqty,
             flags: f,
             name_separator: sep,
@@ -107,16 +116,24 @@
             number_of_sequences: nseq,
         },
     ))
 }
 
 pub fn title(i: &[u8]) -> IResult<&[u8], &str> {
     let (i, size) = self::variable_u64(i)?;
-    let (i, text) =
-        nom::combinator::map_res(nom::bytes::streaming::take(size), std::str::from_utf8)(i)?;
+    if size > (usize::MAX as u64) {
+        return IResult::Err(nom::Err::Failure(nom::error::Error::new(
+            i,
+            nom::error::ErrorKind::TooLarge,
+        )));
+    }
+    let (i, text) = nom::combinator::map_res(
+        nom::bytes::streaming::take(size as usize),
+        std::str::from_utf8,
+    )(i)?;
     Ok((i, text))
 }
 
 mod tests {
 
     #[test]
     fn header() {
```

### Comparing `nafcodec-0.1.1/nafcodec/src/decoder/reader.rs` & `nafcodec-0.2.0/nafcodec/src/decoder/reader.rs`

 * *Files 7% similar despite different names*

```diff
@@ -11,48 +11,63 @@
     reader: R,
 }
 
 impl<R: BufRead> CStringReader<R> {
     pub fn new(reader: R) -> Self {
         Self { reader }
     }
+}
 
-    pub fn next(&mut self) -> Result<CString, std::io::Error> {
+impl<R: BufRead> Iterator for CStringReader<R> {
+    type Item = Result<CString, std::io::Error>;
+    fn next(&mut self) -> Option<Self::Item> {
         let mut buffer = Vec::new();
-        self.reader.read_until(0, &mut buffer)?;
-        Ok(CString::from_vec_with_nul(buffer).expect("buffer should contain a single nul byte"))
+        match self.reader.read_until(0, &mut buffer) {
+            Ok(0) => None,
+            Err(e) => Some(Err(e)),
+            Ok(_) => Some(Ok(CString::from_vec_with_nul(buffer)
+                .expect("buffer should contain a single nul byte"))),
+        }
     }
 }
 
 // --- LengthReader ------------------------------------------------------------
 
 #[derive(Debug)]
 pub struct LengthReader<R: BufRead> {
     reader: R,
 }
 
 impl<R: BufRead> LengthReader<R> {
     pub fn new(reader: R) -> Self {
         Self { reader }
     }
+}
 
-    pub fn next(&mut self) -> Result<u64, std::io::Error> {
+impl<R: BufRead> Iterator for LengthReader<R> {
+    type Item = Result<u64, std::io::Error>;
+    fn next(&mut self) -> Option<Self::Item> {
         let mut n = 0u64;
         let mut x = u32::MAX;
         let mut buffer = [0u8; 4];
 
         while x == u32::MAX {
-            self.reader.read_exact(&mut buffer[..])?;
+            if let Err(e) = self.reader.read_exact(&mut buffer[..]) {
+                match e.kind() {
+                    std::io::ErrorKind::UnexpectedEof => return None,
+                    _ => return Some(Err(e)),
+                }
+            }
             x = nom::number::complete::le_u32::<&[u8], nom::error::Error<&[u8]>>(&buffer[..])
                 .unwrap()
                 .1;
             n += x as u64;
         }
 
-        Ok(n)
+        Some(Ok(n))
     }
 }
 
 // --- SequenceReader ----------------------------------------------------------
 
 #[derive(Debug)]
 pub struct SequenceReader<R: BufRead> {
@@ -172,16 +187,19 @@
         Self {
             reader,
             total,
             current: 0,
             mask: false,
         }
     }
+}
 
-    pub fn next(&mut self) -> Option<Result<MaskUnit, std::io::Error>> {
+impl<R: BufRead> Iterator for MaskReader<R> {
+    type Item = Result<MaskUnit, std::io::Error>;
+    fn next(&mut self) -> Option<Self::Item> {
         if self.current >= self.total {
             return None;
         }
 
         let mut n = 0u64;
         loop {
             let mut i = 0;
```

### Comparing `nafcodec-0.1.1/nafcodec/tests/dna.rs` & `nafcodec-0.2.0/nafcodec/tests/decoder/dna.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use nafcodec::data::SequenceType;
 use nafcodec::Decoder;
 use nafcodec::DecoderBuilder;
+use nafcodec::SequenceType;
 
-const GENOME: &[u8] = include_bytes!("../../data/NZ_AAEN01000029.naf");
-const MASKED: &[u8] = include_bytes!("../../data/masked.naf");
+const GENOME: &[u8] = include_bytes!("../../../data/NZ_AAEN01000029.naf");
+const MASKED: &[u8] = include_bytes!("../../../data/masked.naf");
 
 #[test]
 fn decode() {
     let c = std::io::Cursor::new(GENOME);
     let mut decoder = Decoder::new(c).unwrap();
 
     assert_eq!(decoder.header().name_separator(), ' ');
@@ -60,16 +60,18 @@
     assert!(seq[720..733].chars().all(|x| x.is_lowercase()));
 
     assert!(decoder.next().is_none());
 }
 
 #[test]
 fn force_nomask() {
-    let c = std::io::Cursor::new(MASKED);
-    let mut decoder = DecoderBuilder::new().mask(false).from_reader(c).unwrap();
+    let mut decoder = DecoderBuilder::new()
+        .mask(false)
+        .with_bytes(MASKED)
+        .unwrap();
 
     assert_eq!(decoder.header().name_separator(), ' ');
     assert_eq!(decoder.header().number_of_sequences(), 2);
     assert_eq!(decoder.header().line_length(), 50);
     assert_eq!(decoder.header().sequence_type(), SequenceType::Dna);
 
     let r1 = decoder.next().unwrap().unwrap();
```

### Comparing `nafcodec-0.1.1/nafcodec/tests/protein.rs` & `nafcodec-0.2.0/nafcodec/tests/decoder/protein.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use nafcodec::data::SequenceType;
 use nafcodec::Decoder;
+use nafcodec::SequenceType;
 
 #[test]
 fn decode() {
-    const ARCHIVE: &[u8] = include_bytes!("../../data/LuxC.naf");
+    const ARCHIVE: &[u8] = include_bytes!("../../../data/LuxC.naf");
 
     let c = std::io::Cursor::new(ARCHIVE);
     let mut decoder = Decoder::new(c).unwrap();
 
     assert_eq!(decoder.header().name_separator(), ' ');
     assert_eq!(decoder.header().number_of_sequences(), 12);
     assert_eq!(decoder.header().line_length(), 60);
```

### Comparing `nafcodec-0.1.1/nafcodec-py/Cargo.toml` & `nafcodec-0.2.0/nafcodec-py/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [package]
 name = "nafcodec-py"
-version = "0.1.1"
+version = "0.2.0"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 edition = "2021"
 license = "MIT"
 description = "PyO3 bindings and Python interface to the nafcodec crate."
 repository = "https://github.com/althonos/nafcodec"
 homepage = "https://github.com/althonos/nafcodec"
 readme = "README.md"
 keywords = ["nucleotide", "archive", "biology", "bioinformatics"]
 categories = ["science", "parser-implementations", "compression"]
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 path = "nafcodec/lib.rs"
+doctest = false
 
 [dependencies.nafcodec]
 path = "../nafcodec"
-version = "0.1.1"
+version = "0.2.0"
 features = ["arc"]
 [dependencies]
-pyo3 = "0.18.3"
+pyo3 = "0.21.1"
 
 [features]
 default = []
 extension-module = ["pyo3/extension-module"]
 nightly = ["pyo3/nightly"]
 
 [[test]]
```

### Comparing `nafcodec-0.1.1/nafcodec-py/README.md` & `nafcodec-0.2.0/nafcodec-py/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 📦🧬 `nafcodec` [![Stars](https://img.shields.io/github/stars/althonos/nafcodec.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/nafcodec/stargazers)
 
 *Rust coder/decoder for [Nucleotide Archive Format (NAF)](https://github.com/KirillKryukov/naf) files*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/nafcodec/python.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/nafcodec/actions)
-[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/nafcodec/)
+[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://app.codecov.io/gh/althonos/nafcodec)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Docs](https://img.shields.io/readthedocs/nafcodec/latest?style=flat-square&maxAge=600)](https://nafcodec.readthedocs.io)
 [![Crate](https://img.shields.io/crates/v/nafcodec-py.svg?maxAge=600&style=flat-square)](https://crates.io/crates/nafcodec-py)
 [![PyPI](https://img.shields.io/pypi/v/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec)
 [![Wheel](https://img.shields.io/pypi/wheel/nafcodec.svg?style=flat-square&maxAge=2678400)](https://pypi.org/project/nafcodec/#files)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/nafcodec?style=flat-square&maxAge=3600)](https://anaconda.org/bioconda/nafcodec)
 [![Python Versions](https://img.shields.io/pypi/pyversions/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec/#files)
@@ -30,35 +30,36 @@
 
 This library provides [PyO3](https://pyo3.rs) bindings to the `nafcodec` crate,
 a Rust implementation of a NAF decoder using [`nom`](https://crates.io/crates/nom) 
 for parsing the binary format, and [`zstd`](https://crates.io/crates/zstd) for 
 handling Zstandard decompression. It provides a complete API that allows 
 iterating over the contents of a NAF file.
 
-*This is the Python version, there is a [Rust crate](https://crates.io/crate/nafcodec) available as well.*
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/nafcodec) available as well.*
 
 ### 📋 Features
 
 - **streaming decoder**: The decoder is implemented using different readers
   each accessing a region of the compressed file, allowing to stream records
   without having to decode full blocks.
+- **file-like decoding**: Allow the decoder to read from a file-like object
+  instead of expecting a path.
 
 The following features are planned:
 
-- **file-like decoding**: Allow the decoder to read from a file-like object
-  instead of expecting a path.
 - **optional decoding**: Allow the decoder to skip the decoding of certains
   fields, such as ignoring quality strings when they are not needed.
 - **encoder**: Implement an encoder as well, using either in-memory buffers
   or temporary files to grow the archive.
 
 ### 🔌 Usage
 
-Use `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive Format,
-reading from the given path
+Use a `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive 
+Format, reading from the given [path-like](https://docs.python.org/3/glossary.html#term-path-like-object)
+or [file-like](https://docs.python.org/3/glossary.html#term-file-object) object:
 
 ```python
 import nafcodec
 
 decoder = nafcodec.Decoder("../data/LuxC.naf")
 for record in decoder:
     print(record.id)
```

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/LuxC.naf` & `nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/LuxC.naf`

 * *Files identical despite different names*

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/masked.naf` & `nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/masked.naf`

 * *Files identical despite different names*

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec/tests/data/phix.naf` & `nafcodec-0.2.0/nafcodec-py/nafcodec/tests/data/phix.naf`

 * *Files identical despite different names*

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec/tests/test_decoder.py` & `nafcodec-0.2.0/nafcodec-py/nafcodec/tests/test_encoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import gzip
+import io
 import os
 import tempfile
 import unittest
 
 import nafcodec
 from . import data
 
@@ -10,66 +11,76 @@
     try:
         from importlib.resources import files
     except ImportError:
         from importlib_resources import files  # type: ignore
 except ImportError:
     files = None  # type: ignore
 
-class TestDecoder(unittest.TestCase):
 
-    def test_error_filenotfound(self):
-        with self.assertRaises(FileNotFoundError):
-            decoder = nafcodec.Decoder("")
-        
-    @unittest.skipIf(os.name == "nt", "Windows error codes differ")
-    def test_error_isadirectory(self):
-        with self.assertRaises(IsADirectoryError):
-            decoder = nafcodec.Decoder(os.path.dirname(__file__))
-
-    @unittest.skipUnless(files, "importlib.resources not found")
-    def test_fastq(self):
-        path = files(data).joinpath("phix.naf")
-        decoder = nafcodec.Decoder(path)
-        records = list(decoder)
-        self.assertEqual(len(records), 42)
-        self.assertEqual(records[0].id, "SRR1377138.1")
-        self.assertEqual(records[0].sequence[:36], "NGCTCTTAAACCTGCTATTGAGGCTTGTGGCATTTC")
-        self.assertEqual(records[0].quality[:31], "#8CCCGGGGGGGGGGGGGGGGGGGGGGGGGG")
-
-    @unittest.skipUnless(files, "importlib.resources not found")
-    def test_dna(self):
-        path = files(data).joinpath("NZ_AAEN01000029.naf")
-        decoder = nafcodec.Decoder(path)
-        records = list(decoder)
-        self.assertEqual(len(records), 30)
-        self.assertEqual(records[0].id, "NZ_AAEN01000029.1")
-        self.assertEqual(records[0].sequence.count('A'), 62115)
-        self.assertEqual(records[0].sequence.count('C'), 28747)
-        self.assertEqual(records[0].sequence.count('G'), 30763)
-        self.assertEqual(records[0].sequence.count('T'), 61152)
-        self.assertIs(records[0].quality, None)
-
-    @unittest.skipUnless(files, "importlib.resources not found")
-    def test_protein(self):
-        path = files(data).joinpath("LuxC.naf")
-        decoder = nafcodec.Decoder(path)
+class TestEncoder(unittest.TestCase):
+
+    def test_invalid_sequence(self):
+        buffer = io.BytesIO()
+        with self.assertRaises(ValueError):
+            encoder = nafcodec.Encoder(buffer, sequence_type="dna", sequence=True)
+            encoder.write(nafcodec.Record(sequence="hello world?!"))
+
+    def test_missing_field(self):
+        buffer = io.BytesIO()
+        with self.assertRaises(ValueError):
+            encoder = nafcodec.Encoder(buffer, sequence_type="dna", sequence=True)
+            encoder.write(nafcodec.Record())
+        with self.assertRaises(ValueError):
+            encoder = nafcodec.Encoder(buffer, sequence_type="dna", sequence=True)
+            encoder.write(nafcodec.Record(id="r1"))
+
+    def test_dna_records(self):
+        buffer = io.BytesIO()
+
+        with nafcodec.Encoder(buffer, sequence_type="dna", id=True, sequence=True) as f:
+            f.write(nafcodec.Record(id="r1", sequence="ATTATTAGACAGAGC"))
+            f.write(nafcodec.Record(id="r2", sequence="CTATTG"))
+            f.write(nafcodec.Record(id="r3", sequence="TTAGTNNNNN"))
+
+        buffer.seek(0)
+        decoder = nafcodec.Decoder(buffer)
         records = list(decoder)
-        self.assertEqual(len(records), 12)
-        self.assertEqual(records[0].id, "sp|P19841|LUXC_PHOPO")
-        self.assertEqual(records[0].sequence[:25], "MCNAEFKGDCMIKKIPMIIGGAERD")
-        self.assertIs(records[0].quality, None)
-        self.assertEqual(records[5].id, "sp|P29236|LUXC2_PHOLE")
-        self.assertEqual(records[5].sequence[:25], "MIKKIPMIIGGVVQNTSGYGMRELT")
-        self.assertIs(records[5].quality, None)
-
-    @unittest.skipUnless(files, "importlib.resources not found")
-    def test_dna_masked(self):
-        path = files(data).joinpath("masked.naf")
-        decoder = nafcodec.Decoder(path)
+
+        self.assertEqual(len(records), 3)
+        self.assertEqual(records[0].id, "r1")
+        self.assertEqual(records[1].id, "r2")
+        self.assertEqual(records[2].id, "r3")
+        self.assertEqual(records[0].sequence, "ATTATTAGACAGAGC")
+        self.assertEqual(records[1].sequence, "CTATTG")
+        self.assertEqual(records[2].sequence, "TTAGTNNNNN")
+
+        for i in range(3):
+            self.assertIs(records[i].quality, None)
+            self.assertIs(records[i].comment, None)
+
+    def test_fastq_records(self):
+        buffer = io.BytesIO()
+
+        with nafcodec.Encoder(
+            buffer, sequence_type="rna", id=True, sequence=True, quality=True
+        ) as f:
+            f.write(nafcodec.Record(id="r1", sequence="AUUAU", quality="GGGGG"))
+            f.write(nafcodec.Record(id="r2", sequence="CUAUU", quality="#8A@C"))
+            f.write(nafcodec.Record(id="r3", sequence="UUAGU", quality="CCGGG"))
+
+        buffer.seek(0)
+        decoder = nafcodec.Decoder(buffer)
         records = list(decoder)
-        self.assertEqual(len(records), 2)
-        self.assertEqual(records[0].id, "test1")
-        self.assertTrue(records[0].sequence[:657].isupper())
-        self.assertTrue(records[0].sequence[657:676].islower())
-        self.assertTrue(records[0].sequence[676:1311].isupper())
-        self.assertTrue(records[0].sequence[1311:1350].islower())
-        self.assertIs(records[0].quality, None)
+
+        self.assertEqual(len(records), 3)
+        self.assertEqual(records[0].id, "r1")
+        self.assertEqual(records[1].id, "r2")
+        self.assertEqual(records[2].id, "r3")
+        self.assertEqual(records[0].sequence, "AUUAU")
+        self.assertEqual(records[1].sequence, "CUAUU")
+        self.assertEqual(records[2].sequence, "UUAGU")
+        self.assertEqual(records[0].quality, "GGGGG")
+        self.assertEqual(records[1].quality, "#8A@C")
+        self.assertEqual(records[2].quality, "CCGGG")
+
+        for i in range(3):
+            self.assertIs(records[i].comment, None)
```

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec/tests/unittest.rs` & `nafcodec-0.2.0/nafcodec-py/nafcodec/tests/unittest.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 extern crate nafcodec_py;
 extern crate pyo3;
 
 use std::path::Path;
 
-use pyo3::prelude::PyResult;
+use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use pyo3::types::PyList;
-use pyo3::types::PyModule;
-use pyo3::Python;
 
 pub fn main() -> PyResult<()> {
     // get the relative path to the project folder
     let folder = Path::new(file!())
         .parent()
         .unwrap()
         .parent()
@@ -22,32 +20,32 @@
         .unwrap();
 
     // spawn a Python interpreter
     pyo3::prepare_freethreaded_python();
     Python::with_gil(|py| {
         // insert the project folder in `sys.modules` so that
         // the main module can be imported by Python
-        let sys = py.import("sys")?;
+        let sys = py.import_bound("sys")?;
         sys.getattr("path")?
             .downcast::<PyList>()?
             .insert(0, folder)?;
 
         // create a Python module from our rust code with debug symbols
-        let module = PyModule::new(py, "nafcodec.lib")?;
+        let module = PyModule::new_bound(py, "nafcodec.lib")?;
         nafcodec_py::init(py, &module).unwrap();
         sys.getattr("modules")?
             .downcast::<PyDict>()?
-            .set_item("nafcodec.lib", module)?;
+            .set_item("nafcodec.lib", &module)?;
 
         // run unittest on the tests
-        let kwargs = PyDict::new(py);
+        let kwargs = PyDict::new_bound(py);
         kwargs.set_item("exit", false).unwrap();
         kwargs.set_item("verbosity", 2u8).unwrap();
-        py.import("unittest").unwrap().call_method(
+        py.import_bound("unittest").unwrap().call_method(
             "TestProgram",
             ("nafcodec.tests",),
-            Some(kwargs),
+            Some(&kwargs),
         )?;
 
         Ok(())
     })
 }
```

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/PKG-INFO` & `nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nafcodec
-Version: 0.1.1
+Version: 0.2.0
 Summary: PyO3 bindings and Python interface to nafcodec, an encoder/decoder for Nucleotide Archive Format (NAF) files.
 Home-page: https://github.com/althonos/nafcodec
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/nafcodec/issues
 Project-URL: Changelog, https://github.com/althonos/nafcodec/blob/master/CHANGELOG.md
@@ -20,29 +20,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 📦🧬 `nafcodec` [![Stars](https://img.shields.io/github/stars/althonos/nafcodec.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/nafcodec/stargazers)
 
 *Rust coder/decoder for [Nucleotide Archive Format (NAF)](https://github.com/KirillKryukov/naf) files*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/nafcodec/python.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/nafcodec/actions)
-[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/nafcodec/)
+[![Coverage](https://img.shields.io/codecov/c/gh/althonos/nafcodec?logo=codecov&style=flat-square&maxAge=3600)](https://app.codecov.io/gh/althonos/nafcodec)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Docs](https://img.shields.io/readthedocs/nafcodec/latest?style=flat-square&maxAge=600)](https://nafcodec.readthedocs.io)
 [![Crate](https://img.shields.io/crates/v/nafcodec-py.svg?maxAge=600&style=flat-square)](https://crates.io/crates/nafcodec-py)
 [![PyPI](https://img.shields.io/pypi/v/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec)
 [![Wheel](https://img.shields.io/pypi/wheel/nafcodec.svg?style=flat-square&maxAge=2678400)](https://pypi.org/project/nafcodec/#files)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/nafcodec?style=flat-square&maxAge=3600)](https://anaconda.org/bioconda/nafcodec)
 [![Python Versions](https://img.shields.io/pypi/pyversions/nafcodec.svg?style=flat-square&maxAge=600)](https://pypi.org/project/nafcodec/#files)
@@ -65,35 +66,36 @@
 
 This library provides [PyO3](https://pyo3.rs) bindings to the `nafcodec` crate,
 a Rust implementation of a NAF decoder using [`nom`](https://crates.io/crates/nom) 
 for parsing the binary format, and [`zstd`](https://crates.io/crates/zstd) for 
 handling Zstandard decompression. It provides a complete API that allows 
 iterating over the contents of a NAF file.
 
-*This is the Python version, there is a [Rust crate](https://crates.io/crate/nafcodec) available as well.*
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/nafcodec) available as well.*
 
 ### 📋 Features
 
 - **streaming decoder**: The decoder is implemented using different readers
   each accessing a region of the compressed file, allowing to stream records
   without having to decode full blocks.
+- **file-like decoding**: Allow the decoder to read from a file-like object
+  instead of expecting a path.
 
 The following features are planned:
 
-- **file-like decoding**: Allow the decoder to read from a file-like object
-  instead of expecting a path.
 - **optional decoding**: Allow the decoder to skip the decoding of certains
   fields, such as ignoring quality strings when they are not needed.
 - **encoder**: Implement an encoder as well, using either in-memory buffers
   or temporary files to grow the archive.
 
 ### 🔌 Usage
 
-Use `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive Format,
-reading from the given path
+Use a `nafcodec.Decoder` to iterate over the contents of a Nucleotide Archive 
+Format, reading from the given [path-like](https://docs.python.org/3/glossary.html#term-path-like-object)
+or [file-like](https://docs.python.org/3/glossary.html#term-file-object) object:
 
 ```python
 import nafcodec
 
 decoder = nafcodec.Decoder("../data/LuxC.naf")
 for record in decoder:
     print(record.id)
```

### Comparing `nafcodec-0.1.1/nafcodec-py/nafcodec.egg-info/SOURCES.txt` & `nafcodec-0.2.0/nafcodec-py/nafcodec.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 CHANGELOG.md
 COPYING
+Cargo.toml
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 nafcodec/Cargo.toml
 nafcodec/README.md
 nafcodec-py/Cargo.toml
 nafcodec-py/README.md
 nafcodec-py/nafcodec/__init__.py
 nafcodec-py/nafcodec/lib.pyi
 nafcodec-py/nafcodec/lib.rs
+nafcodec-py/nafcodec/py.typed
+nafcodec-py/nafcodec/pyfile.rs
 nafcodec-py/nafcodec.egg-info/PKG-INFO
 nafcodec-py/nafcodec.egg-info/SOURCES.txt
 nafcodec-py/nafcodec.egg-info/dependency_links.txt
 nafcodec-py/nafcodec.egg-info/top_level.txt
 nafcodec-py/nafcodec.egg-info/zip-safe
 nafcodec-py/nafcodec/tests/__init__.py
 nafcodec-py/nafcodec/tests/requirements.txt
 nafcodec-py/nafcodec/tests/test_decoder.py
+nafcodec-py/nafcodec/tests/test_doctest.py
+nafcodec-py/nafcodec/tests/test_encoder.py
+nafcodec-py/nafcodec/tests/test_open.py
 nafcodec-py/nafcodec/tests/unittest.rs
+nafcodec-py/nafcodec/tests/data/CP040672.naf
 nafcodec-py/nafcodec/tests/data/LuxC.naf
-nafcodec-py/nafcodec/tests/data/NZ_AAEN01000029.naf
 nafcodec-py/nafcodec/tests/data/__init__.py
 nafcodec-py/nafcodec/tests/data/masked.naf
 nafcodec-py/nafcodec/tests/data/phix.naf
 nafcodec/src/data.rs
 nafcodec/src/error.rs
 nafcodec/src/lib.rs
 nafcodec/src/decoder/ioslice.rs
 nafcodec/src/decoder/mod.rs
 nafcodec/src/decoder/parser.rs
 nafcodec/src/decoder/reader.rs
-nafcodec/tests/dna.rs
-nafcodec/tests/fastq.rs
-nafcodec/tests/protein.rs
+nafcodec/src/encoder/counter.rs
+nafcodec/src/encoder/mod.rs
+nafcodec/src/encoder/storage.rs
+nafcodec/src/encoder/writer.rs
+nafcodec/tests/encoder.rs
+nafcodec/tests/decoder/dna.rs
+nafcodec/tests/decoder/fastq.rs
+nafcodec/tests/decoder/mod.rs
+nafcodec/tests/decoder/protein.rs
```

### Comparing `nafcodec-0.1.1/setup.cfg` & `nafcodec-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Rust
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
 	Bug Tracker = https://github.com/althonos/nafcodec/issues
```

### Comparing `nafcodec-0.1.1/setup.py` & `nafcodec-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     def build_extension(self, ext, target):
         with patch_env("RUSTFLAGS", " ".join(ext.rustc_flags)):
             return _build_rust.build_extension(self, ext, target)
 
     def get_dylib_ext_path(self, ext, module_name):
         ext_path = _build_rust.get_dylib_ext_path(self, ext, module_name)
         if self.inplace:
-            package_dir = self.distribution.package_dir['']
+            package_dir = self.distribution.package_dir[""]
             base = os.path.basename(ext_path)
             folder = os.path.dirname(os.path.realpath(__file__))
             prefix = os.path.sep.join(ext.name.split(".")[:-1])
             ext_path = os.path.join(folder, package_dir, prefix, base)
         return ext_path
```

