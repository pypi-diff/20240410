# Comparing `tmp/imbue-0.1.0.tar.gz` & `tmp/imbue-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbue-0.1.0.tar", max compression
+gzip compressed data, was "imbue-1.0.0.tar", max compression
```

## Comparing `imbue-0.1.0.tar` & `imbue-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,24 @@
--rw-r--r--   0        0        0     1064 2024-03-12 08:19:42.008490 imbue-0.1.0/LICENSE
--rw-r--r--   0        0        0       59 2024-03-12 08:22:57.364486 imbue-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-12 08:39:09.337395 imbue-0.1.0/imbue/__init__.py
--rw-r--r--   0        0        0      870 2024-03-12 08:21:25.276488 imbue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 imbue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-10 17:52:04.806052 imbue-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5047 2024-04-10 17:52:04.806052 imbue-1.0.0/README.md
+-rw-r--r--   0        0        0      565 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/abc.py
+-rw-r--r--   0        0        0     5928 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/container.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/__init__.py
+-rw-r--r--   0        0        0     3046 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/abc.py
+-rw-r--r--   0        0        0     1782 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/application.py
+-rw-r--r--   0        0        0     4199 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/base.py
+-rw-r--r--   0        0        0      461 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/factory.py
+-rw-r--r--   0        0        0      587 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/task.py
+-rw-r--r--   0        0        0     1188 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/thread.py
+-rw-r--r--   0        0        0     1237 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/dependency.py
+-rw-r--r--   0        0        0      288 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/exceptions.py
+-rw-r--r--   0        0        0      964 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/package.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/abc.py
+-rw-r--r--   0        0        0     1728 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/common.py
+-rw-r--r--   0        0        0     2036 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/function.py
+-rw-r--r--   0        0        0     3333 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/instance.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/py.typed
+-rw-r--r--   0        0        0     4172 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/utils.py
+-rw-r--r--   0        0        0      870 2024-04-10 17:52:04.806052 imbue-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5738 1970-01-01 00:00:00.000000 imbue-1.0.0/PKG-INFO
```

### Comparing `imbue-0.1.0/LICENSE` & `imbue-1.0.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Gabriel
+Copyright (c) 2024 Gabriel Pajot
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `imbue-0.1.0/pyproject.toml` & `imbue-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imbue"
-version = "0.1.0"
+version = "1.0.0"
 description = "Type based python dependency injection framework."
 authors = ["Gabriel Pajot <gab@lescactus.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/imbue"
 include = ["imbue/py.typed"]
```

