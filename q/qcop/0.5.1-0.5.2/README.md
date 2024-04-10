# Comparing `tmp/qcop-0.5.1.tar.gz` & `tmp/qcop-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcop-0.5.1.tar", max compression
+gzip compressed data, was "qcop-0.5.2.tar", max compression
```

## Comparing `qcop-0.5.1.tar` & `qcop-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-03-29 23:58:36.983945 qcop-0.5.1/LICENSE
--rw-r--r--   0        0        0     7283 2024-03-29 23:58:36.983945 qcop-0.5.1/README.md
--rw-r--r--   0        0        0     1820 2024-03-29 23:58:36.987945 qcop-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      248 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/__init__.py
--rw-r--r--   0        0        0      318 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/__init__.py
--rw-r--r--   0        0        0    12380 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/base.py
--rw-r--r--   0        0        0     1487 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/file.py
--rw-r--r--   0        0        0    11141 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/geometric.py
--rw-r--r--   0        0        0     2111 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/qcengine.py
--rw-r--r--   0        0        0     4662 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/terachem.py
--rw-r--r--   0        0        0     7899 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/utils.py
--rw-r--r--   0        0        0      164 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/adapters/xtb.py
--rw-r--r--   0        0        0     3639 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/exceptions.py
--rw-r--r--   0        0        0     3134 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/main.py
--rw-r--r--   0        0        0        0 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/py.typed
--rw-r--r--   0        0        0     3295 2024-03-29 23:58:36.987945 qcop-0.5.1/qcop/utils.py
--rw-r--r--   0        0        0     8300 1970-01-01 00:00:00.000000 qcop-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-10 16:39:47.807119 qcop-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7283 2024-04-10 16:39:47.807119 qcop-0.5.2/README.md
+-rw-r--r--   0        0        0     1818 2024-04-10 16:39:47.807119 qcop-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/__init__.py
+-rw-r--r--   0        0        0    12380 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/base.py
+-rw-r--r--   0        0        0     1487 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/file.py
+-rw-r--r--   0        0        0    11141 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/geometric.py
+-rw-r--r--   0        0        0     2111 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/qcengine.py
+-rw-r--r--   0        0        0     4662 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/terachem.py
+-rw-r--r--   0        0        0     7899 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/utils.py
+-rw-r--r--   0        0        0     4122 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/xtb.py
+-rw-r--r--   0        0        0     3639 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/exceptions.py
+-rw-r--r--   0        0        0     3134 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/main.py
+-rw-r--r--   0        0        0        0 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/py.typed
+-rw-r--r--   0        0        0     3363 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/utils.py
+-rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.2/PKG-INFO
```

### Comparing `qcop-0.5.1/LICENSE` & `qcop-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/README.md` & `qcop-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/pyproject.toml` & `qcop-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "qcop"
-version = "0.5.1"
+version = "0.5.2"
 description = "A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-qcio = ">=0.8.1"
-qcparse = ">=0.5.2"
+qcio = "^0.8.2"
+qcparse = "^0.5.2"
 
 # A list of all of the optional dependencies, some of which are included in the below
 # `extras`. They can be opted into by apps.
 qcelemental = { version = ">=0.26.0", optional = true }
 qcengine = { version = ">=0.27.0", optional = true }
 geometric = { version = ">=1.0.1", optional = true }
```

### Comparing `qcop-0.5.1/qcop/adapters/base.py` & `qcop-0.5.2/qcop/adapters/base.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/adapters/file.py` & `qcop-0.5.2/qcop/adapters/file.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/adapters/geometric.py` & `qcop-0.5.2/qcop/adapters/geometric.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/adapters/qcengine.py` & `qcop-0.5.2/qcop/adapters/qcengine.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/adapters/terachem.py` & `qcop-0.5.2/qcop/adapters/terachem.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/adapters/utils.py` & `qcop-0.5.2/qcop/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/exceptions.py` & `qcop-0.5.2/qcop/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/main.py` & `qcop-0.5.2/qcop/main.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.1/qcop/utils.py` & `qcop-0.5.2/qcop/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         raise ModuleNotFoundError(
             "QCEngine not installed. To use qcengine as a fallback, "
             "install it by running 'python -m pip install "
             "'qcop[qcengine]'."
         ) from e
 
     try:
+        # NOTE: This call adds >1s of overhead to execution time!!!
         get_program(program)
     except InputError as e:  # Raised by QCEngine if program not registered
         raise AdapterNotFoundError(program) from e
     # Raised by QCEngine if program not installed on system
     # IndexError insulates from .pyenv/shims not covered in qcng
     except (ResourceError, IndexError):
         raise ProgramNotFoundError(program)
```

### Comparing `qcop-0.5.1/PKG-INFO` & `qcop-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcop
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: geometric
 Provides-Extra: qcengine
 Requires-Dist: geometric (>=1.0.1) ; extra == "geometric"
 Requires-Dist: qcelemental (>=0.26.0) ; extra == "qcengine"
 Requires-Dist: qcengine (>=0.27.0) ; extra == "qcengine"
-Requires-Dist: qcio (>=0.8.1)
-Requires-Dist: qcparse (>=0.5.2)
+Requires-Dist: qcio (>=0.8.2,<0.9.0)
+Requires-Dist: qcparse (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # Quantum Chemistry Operate
 
 A package for operating Quantum Chemistry programs using [qcio](https://github.com/coltonbh/qcio) standardized data structures. Compatible with `TeraChem`, `psi4`, `QChem`, `NWChem`, `ORCA`, `Molpro`, `geomeTRIC` and many more.
 
 [![image](https://img.shields.io/pypi/v/qcop.svg)](https://pypi.python.org/pypi/qcop)
```

