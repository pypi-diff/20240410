# Comparing `tmp/abi3info-2024.3.26.tar.gz` & `tmp/abi3info-2024.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2024.3.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3info-2024.4.10.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `abi3info-2024.3.26.tar` & `abi3info-2024.4.10.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2024-03-26 13:02:59.233643 abi3info-2024.3.26/LICENSE
--rw-r--r--   0        0        0     1915 2024-03-26 13:02:59.233643 abi3info-2024.3.26/README.md
--rw-r--r--   0        0        0     1038 2024-03-26 13:02:59.233643 abi3info-2024.3.26/abi3info/__init__.py
--rw-r--r--   0        0        0   196630 2024-03-26 13:02:59.233643 abi3info-2024.3.26/abi3info/_internal.py
--rw-r--r--   0        0        0     7769 2024-03-26 13:02:59.233643 abi3info-2024.3.26/abi3info/models.py
--rw-r--r--   0        0        0     1922 2024-03-26 13:02:59.233643 abi3info-2024.3.26/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 abi3info-2024.3.26/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-04-10 14:16:11.215559 abi3info-2024.4.10/LICENSE
+-rw-r--r--   0        0        0     1915 2024-04-10 14:16:11.215559 abi3info-2024.4.10/README.md
+-rw-r--r--   0        0        0     1038 2024-04-10 14:16:11.215559 abi3info-2024.4.10/abi3info/__init__.py
+-rw-r--r--   0        0        0   227441 2024-04-10 14:16:11.215559 abi3info-2024.4.10/abi3info/_internal.py
+-rw-r--r--   0        0        0     8034 2024-04-10 14:16:11.215559 abi3info-2024.4.10/abi3info/models.py
+-rw-r--r--   0        0        0     1922 2024-04-10 14:16:11.215559 abi3info-2024.4.10/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 abi3info-2024.4.10/PKG-INFO
```

### Comparing `abi3info-2024.3.26/LICENSE` & `abi3info-2024.4.10/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2024.3.26/README.md` & `abi3info-2024.4.10/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2024.3.26/abi3info/__init__.py` & `abi3info-2024.4.10/abi3info/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2024.03.26"
+__version__ = "2024.04.10"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2024.3.26/abi3info/models.py` & `abi3info-2024.4.10/abi3info/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Literal, Union
 
+# values taken from the GCC/Clang manual.
+Visibility = Literal["default", "hidden", "internal", "protected"]
+
 
 @dataclass(frozen=True, eq=False, unsafe_hash=True)
 class Symbol:
     """
     Represents a linker symbol, which may or may not point to some kind of object
     (function, struct, constant, etc.).
 
@@ -20,14 +23,19 @@
     """
 
     name: str
     """
     The symbol's underlying name. This may not correspond to an actual symbol
     in a binary without platform-specific normalization.
     """
+    visibility: Visibility | None = None
+    """
+    The symbol's visibility in the shared object file, or None if it could not
+    be determined.
+    """
 
     @property
     def macos(self) -> str:
         """
         Returns a macOS-style symbol for the underlying symbol.
         """
         return f"_{self.name}"
```

### Comparing `abi3info-2024.3.26/pyproject.toml` & `abi3info-2024.4.10/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2024.3.26/PKG-INFO` & `abi3info-2024.4.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2024.3.26
+Version: 2024.4.10
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

