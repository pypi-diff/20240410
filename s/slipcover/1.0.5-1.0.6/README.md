# Comparing `tmp/slipcover-1.0.5.tar.gz` & `tmp/slipcover-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-1.0.5.tar", last modified: Thu Apr  4 17:45:02 2024, max compression
+gzip compressed data, was "slipcover-1.0.6.tar", last modified: Tue Apr  9 23:43:54 2024, max compression
```

## Comparing `slipcover-1.0.5.tar` & `slipcover-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.368946 slipcover-1.0.5/
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-04-04 17:44:35.000000 slipcover-1.0.5/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-04 17:44:35.000000 slipcover-1.0.5/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-04 17:45:02.368286 slipcover-1.0.5/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     8234 2024-04-04 17:44:35.000000 slipcover-1.0.5/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 17:45:02.369047 slipcover-1.0.5/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     4329 2024-04-04 17:44:35.000000 slipcover-1.0.5/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.358121 slipcover-1.0.5/src/
--rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/probe.cxx
--rw-r--r--   0 runner     (501) staff       (20)      865 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/pyptr.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.361526 slipcover-1.0.5/src/slipcover/
--rw-r--r--   0 runner     (501) staff       (20)      168 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8340 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     6472 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/branch.py
--rw-r--r--   0 runner     (501) staff       (20)    21990 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/fuzz.py
--rw-r--r--   0 runner     (501) staff       (20)     9302 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/importer.py
--rw-r--r--   0 runner     (501) staff       (20)    24920 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/slipcover.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.367767 slipcover-1.0.5/src/slipcover.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      669 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.367355 slipcover-1.0.5/tests/
--rw-r--r--   0 runner     (501) staff       (20)    15690 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_branch.py
--rw-r--r--   0 runner     (501) staff       (20)    22245 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)    26932 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_coverage.py
--rw-r--r--   0 runner     (501) staff       (20)     9264 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_importer.py
--rw-r--r--   0 runner     (501) staff       (20)    17743 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_instrumentation.py
--rw-r--r--   0 runner     (501) staff       (20)     1313 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-class.py
--rw-r--r--   0 runner     (501) staff       (20)     1422 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-inner.py
--rw-r--r--   0 runner     (501) staff       (20)     1279 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-partial.py
--rw-r--r--   0 runner     (501) staff       (20)     1269 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-09 23:43:54.489617 slipcover-1.0.6/
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-04-09 23:43:32.000000 slipcover-1.0.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-09 23:43:32.000000 slipcover-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-09 23:43:54.489101 slipcover-1.0.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8234 2024-04-09 23:43:32.000000 slipcover-1.0.6/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-09 23:43:54.489703 slipcover-1.0.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     4329 2024-04-09 23:43:32.000000 slipcover-1.0.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-09 23:43:54.476605 slipcover-1.0.6/src/
+-rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/probe.cxx
+-rw-r--r--   0 runner     (501) staff       (20)      865 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/pyptr.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-09 23:43:54.480694 slipcover-1.0.6/src/slipcover/
+-rw-r--r--   0 runner     (501) staff       (20)      168 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9556 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6472 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/branch.py
+-rw-r--r--   0 runner     (501) staff       (20)    21990 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/bytecode.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/fuzz.py
+-rw-r--r--   0 runner     (501) staff       (20)     9302 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/importer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2171 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/isolate.py
+-rw-r--r--   0 runner     (501) staff       (20)    25234 2024-04-09 23:43:32.000000 slipcover-1.0.6/src/slipcover/slipcover.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-09 23:43:54.488608 slipcover-1.0.6/src/slipcover.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      716 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-09 23:43:54.000000 slipcover-1.0.6/src/slipcover.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-09 23:43:54.488158 slipcover-1.0.6/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    15690 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_branch.py
+-rw-r--r--   0 runner     (501) staff       (20)    22245 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_bytecode.py
+-rw-r--r--   0 runner     (501) staff       (20)    28458 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_coverage.py
+-rw-r--r--   0 runner     (501) staff       (20)     9528 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_importer.py
+-rw-r--r--   0 runner     (501) staff       (20)    17743 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_instrumentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     5065 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/test_isolate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1313 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/testme-class.py
+-rw-r--r--   0 runner     (501) staff       (20)     1422 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/testme-inner.py
+-rw-r--r--   0 runner     (501) staff       (20)     1279 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/testme-partial.py
+-rw-r--r--   0 runner     (501) staff       (20)     1269 2024-04-09 23:43:32.000000 slipcover-1.0.6/tests/testme.py
```

### Comparing `slipcover-1.0.5/LICENSE` & `slipcover-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/PKG-INFO` & `slipcover-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.5
+Version: 1.0.6
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.5/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.6/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -57,16 +57,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.6/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.6/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -86,15 +86,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.5/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.6/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.5/README.md` & `slipcover-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/setup.py` & `slipcover-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/probe.cxx` & `slipcover-1.0.6/src/probe.cxx`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/pyptr.h` & `slipcover-1.0.6/src/pyptr.h`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/slipcover/__main__.py` & `slipcover-1.0.6/src/slipcover/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 import ast
 import atexit
 import platform
 import functools
 import os
 import tempfile
 import json
+import warnings
 
 # Used for fork() support
 input_tmpfiles = []
 output_tmpfile = None
 
 
-def fork_shim():
+def fork_shim(sci):
     """Shims os.fork(), preparing the child to write its coverage to a temporary file
        and the parent to read from that file, so as to report the full coverage obtained.
     """
     original_fork = os.fork
 
     @functools.wraps(original_fork)
     def wrapper(*pargs, **kwargs):
         global input_tmpfiles, output_tmpfile
 
         tmp_file = tempfile.NamedTemporaryFile(mode="r+", encoding="utf-8", delete=False)
 
         if (pid := original_fork(*pargs, **kwargs)):
             input_tmpfiles.append(tmp_file)
+
         else:
+            sci.signal_child_process()
+            input_tmpfiles.clear()  # to be used by this process' children, if any
             output_tmpfile = tmp_file
 
         return pid
 
     return wrapper
 
 
@@ -46,26 +50,26 @@
     if input_tmpfiles:
         for f in input_tmpfiles:
             try:
                 fname = f.name
                 f.seek(0)
                 sc.merge_coverage(cov, json.load(f))
             except json.JSONDecodeError as e:
-                print(f"Error reading {fname}: {e}")
+                warnings.warn(f"Error reading {fname}: {e}")
             finally:
                 f.close()
                 try:
                     os.remove(fname)
                 except FileNotFoundError:
                     pass
 
     return cov
 
 
-def exit_shim(args, sci):
+def exit_shim(sci):
     """Shims os._exit(), so a previously forked child process writes its coverage to
        a temporary file read by the parent.
     """
     original_exit = os._exit
 
     @functools.wraps(original_exit)
     def wrapper(*pargs, **kwargs):
@@ -78,34 +82,35 @@
         original_exit(*pargs, **kwargs)
 
     return wrapper
 
 
 def merge_files(args):
     """Merges coverage files."""
+
     try:
         with args.merge[0].open() as jf:
             merged = json.load(jf)
     except Exception as e:
-        print(f"Error reading in {args.merge[0]}: {e}")
+        warnings.warn(f"Error reading in {args.merge[0]}: {e}")
         return 1
 
     try:
         for f in args.merge[1:]:
             with f.open() as jf:
                 sc.merge_coverage(merged, json.load(jf))
     except Exception as e:
-        print(f"Error merging in {f}: {e}")
+        warnings.warn(f"Error merging in {f}: {e}")
         return 1
 
     try:
         with args.out.open("w", encoding='utf-8') as jf:
             json.dump(merged, jf)
     except Exception as e:
-        print(e)
+        warnings.warn(e)
         return 1
 
     return 0
 
 
 def main():
     import argparse
@@ -129,14 +134,18 @@
                     help=(argparse.SUPPRESS if platform.python_implementation() == "PyPy" else "request immediate de-instrumentation"))
     ap.add_argument('--skip-covered', action='store_true', help="omit fully covered files (from text, non-JSON output)")
     ap.add_argument('--fail-under', type=float, default=0, help="fail execution with RC 2 if the overall coverage lays lower than this")
     ap.add_argument('--threshold', type=int, default=50, metavar="T",
                     help="threshold for de-instrumentation (if not immediate)")
     ap.add_argument('--missing-width', type=int, default=80, metavar="WIDTH", help="maximum width for `missing' column")
 
+    ap.add_argument('--isolate-tests', default=False,
+                    action=(argparse.BooleanOptionalAction if sys.version_info[0:2] >= (3,9) else 'store_true'),
+                    help=argparse.SUPPRESS) #'run pytest tests in isolation, to try to work around state pollution')
+
     # intended for slipcover development only
     ap.add_argument('--silent', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--dis', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--debug', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--dont-wrap-pytest', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--version', action='version',
                     version=f"%(prog)s v{sc.VERSION} (Python {'.'.join(map(str, sys.version_info[:3]))})")
@@ -150,14 +159,30 @@
     if '-m' in sys.argv: # work around exclusive group not handled properly
         minus_m = sys.argv.index('-m')
         args = ap.parse_args(sys.argv[1:minus_m+2])
         args.script_or_module_args = sys.argv[minus_m+2:]
     else:
         args = ap.parse_args(sys.argv[1:])
 
+    if args.isolate_tests:
+        if platform.system() == 'Windows':
+            ap.error('--isolate-tests is only supported on Unix')
+
+        if args.module != ['pytest']:
+            ap.error('--isolate-tests must be used with -m pytest')
+
+        args.module = ['slipcover.isolate']
+
+        try:
+            import pytest_forked
+            if pytest_forked.__file__ is None:
+                # 'import pytest_forked' may work, but the plugin may still not be there...
+                raise ImportError("pytest-forked not installed")
+        except ImportError:
+            ap.error('--isolate-tests requires pytest-forked  (fix with "pip install pytest-forked")')
 
     if args.merge:
         if not args.out: ap.error("--out is required with --merge")
         return merge_files(args)
 
 
     base_path = Path(args.script).resolve().parent if args.script \
@@ -184,16 +209,16 @@
 
 
     if not args.dont_wrap_pytest:
         sc.wrap_pytest(sci, file_matcher)
 
 
     if platform.system() != 'Windows':
-        os.fork = fork_shim()
-        os._exit = exit_shim(args, sci)
+        os.fork = fork_shim(sci)
+        os._exit = exit_shim(sci)
 
     def sci_atexit():
         global output_tmpfile
 
         def printit(coverage, outfile):
             if args.json:
                 print(json.dumps(coverage, indent=(4 if args.pretty_print else None)), file=outfile)
@@ -215,27 +240,30 @@
         # python 'globals' for the script being executed
         script_globals: Dict[Any, Any] = dict()
 
         # needed so that the script being invoked behaves like the main one
         script_globals['__name__'] = '__main__'
         script_globals['__file__'] = args.script
 
-        sys.argv = [args.script, *args.script_or_module_args]
+        sys.argv = [str(args.script), *args.script_or_module_args]
 
         # the 1st item in sys.path is always the main script's directory
         sys.path.pop(0)
         sys.path.insert(0, str(base_path))
 
         with open(args.script, "r") as f:
             t = ast.parse(f.read())
-            if args.branch:
+            if args.branch and file_matcher.matches(args.script):
                 t = br.preinstrument(t)
             code = compile(t, str(Path(args.script).resolve()), "exec")
 
-        code = sci.instrument(code)
+
+        if file_matcher.matches(args.script):
+            code = sci.instrument(code)
+
         with sc.ImportManager(sci, file_matcher):
             exec(code, script_globals)
 
     else:
         import runpy
         sys.argv = [*args.module, *args.script_or_module_args]
         with sc.ImportManager(sci, file_matcher):
```

### Comparing `slipcover-1.0.5/src/slipcover/branch.py` & `slipcover-1.0.6/src/slipcover/branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/slipcover/bytecode.py` & `slipcover-1.0.6/src/slipcover/bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/slipcover/importer.py` & `slipcover-1.0.6/src/slipcover/importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/src/slipcover/slipcover.py` & `slipcover-1.0.6/src/slipcover/slipcover.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if sys.version_info[0:2] < (3,12):
     from . import probe
     from . import bytecode as bc
 
 from pathlib import Path
 from . import branch as br
 
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 
 # FIXME provide __all__
 
 # Counter.total() is new in 3.10
 if sys.version_info[0:2] < (3,10):
     def counter_total(self: Counter) -> int:
         return sum([self[n] for n in self])
@@ -82,14 +82,17 @@
     return ", ".join(find_ranges())
 
 
 def print_coverage(coverage, *, outfile=sys.stdout, missing_width=None, skip_covered=False) -> None:
     """Prints coverage information for human consumption."""
     from tabulate import tabulate
 
+    if not coverage.get('files', None): # includes empty coverage['files']
+        return
+
     branch_coverage = coverage.get('meta', {}).get('branch_coverage', False)
 
     def table():
         for f, f_info in sorted(coverage['files'].items()):
             exec_l = len(f_info['executed_lines'])
             miss_l = len(f_info['missing_lines'])
 
@@ -523,14 +526,21 @@
             'version': VERSION,
             'timestamp': datetime.datetime.now().isoformat(),
             'branch_coverage': branch_coverage,
             'show_contexts': False
         }
 
 
+    def signal_child_process(self):
+        self.source = None  # only the parent process needs to run _add_unseen_source_files
+        with self.lock:
+            self._get_newly_seen()
+            self.all_seen.clear()
+
+
     def get_coverage(self):
         """Returns coverage information collected."""
 
         with self.lock:
             # FIXME calling _get_newly_seen will prevent de-instrumentation if still running!
             newly_seen = self._get_newly_seen()
```

### Comparing `slipcover-1.0.5/src/slipcover.egg-info/PKG-INFO` & `slipcover-1.0.6/src/slipcover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.5
+Version: 1.0.6
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.5/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.6/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -57,16 +57,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.6/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.6/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -86,15 +86,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.5/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.6/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.5/src/slipcover.egg-info/SOURCES.txt` & `slipcover-1.0.6/src/slipcover.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 src/pyptr.h
 src/slipcover/__init__.py
 src/slipcover/__main__.py
 src/slipcover/branch.py
 src/slipcover/bytecode.py
 src/slipcover/fuzz.py
 src/slipcover/importer.py
+src/slipcover/isolate.py
 src/slipcover/slipcover.py
 src/slipcover.egg-info/PKG-INFO
 src/slipcover.egg-info/SOURCES.txt
 src/slipcover.egg-info/dependency_links.txt
 src/slipcover.egg-info/entry_points.txt
 src/slipcover.egg-info/requires.txt
 src/slipcover.egg-info/top_level.txt
 tests/test_branch.py
 tests/test_bytecode.py
 tests/test_coverage.py
 tests/test_importer.py
 tests/test_instrumentation.py
+tests/test_isolate.py
 tests/testme-class.py
 tests/testme-inner.py
 tests/testme-partial.py
 tests/testme.py
```

### Comparing `slipcover-1.0.5/tests/test_branch.py` & `slipcover-1.0.6/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/test_bytecode.py` & `slipcover-1.0.6/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/test_coverage.py` & `slipcover-1.0.6/tests/test_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,21 @@
     exec(code, g, g)
     sci.print_coverage(sys.stdout)
     output = capsys.readouterr()[0]
     output = output.splitlines()
     assert re.match(f'^foo\\.py +{"1" if PYTHON_VERSION < (3,11) else "0"} +0{" +0 +0 +0" if do_branch else ""} +100', output[3])
 
 
+@pytest.mark.parametrize("do_branch", [True, False])
+def test_print_coverage_no_coverage(capsys, do_branch):
+    sci = sc.Slipcover(branch=do_branch)
+    cov = sci.get_coverage()
+    sc.print_coverage(cov)
+
+
 def test_print_coverage_skip_covered():
     p = subprocess.run(f"{sys.executable} -m slipcover --skip-covered tests/importer.py".split(),
                        check=True, capture_output=True)
     output = str(p.stdout)
     print(output)
     assert '__init__.py' in output
     assert 'importer.py' not in output
@@ -640,14 +647,17 @@
 
     subprocess.run((f"{sys.executable} -m slipcover --branch --json --out {out_file} " +\
                     f"--source tests/imported tests/importer.py").split(),
                    check=True)
     with open(out_file, "r") as f:
         cov = json.load(f)
 
+    assert 'tests/importer.py' not in cov['files']
+    assert str(Path('tests/importer.py').resolve()) not in cov['files']
+
     init_file = str(Path('tests') / 'imported' / '__init__.py')
     foo_file = str(Path('tests') / 'imported' / 'foo.py')
     baz_file = str(Path('tests') / 'imported' / 'subdir' / 'baz.PY')
 
     assert init_file in cov['files']
     assert [1,2,3,4,5,6,8] == cov['files'][init_file]['executed_lines']
     assert [9] == cov['files'][init_file]['missing_lines']
@@ -856,14 +866,58 @@
     assert test_file in cov['files']
     assert {test_file} == set(cov['files'].keys())
     cov = cov['files'][test_file]
     assert [1, 2, 3, 4, 5, 6, 8, 9, 10, 11, 13, 14] == cov['executed_lines']
     assert [] == cov['missing_lines']
 
 
+@pytest.mark.skipif(sys.platform == 'win32', reason='fork() and pytest-forked are Unix-specific')
+def test_forked_twice(tmp_path, monkeypatch):
+    source = (Path('tests') / 'pyt.py').resolve()
+    out = tmp_path / "out.json"
+    script = tmp_path / "foo.py"
+
+    monkeypatch.chdir(tmp_path)
+    test_file = 't.py'
+    Path(test_file).write_text(source.read_text())
+
+    script.write_text(f"""\
+import os
+import sys
+import pytest
+
+if (pid := os.fork()):
+    pid, status = os.waitpid(pid, 0)
+    if status:
+        if os.WIFSIGNALED(status):
+            exitstatus = os.WTERMSIG(status) + 128
+        else:
+            exitstatus = os.WEXITSTATUS(status)
+    else:
+        exitstatus = 0
+
+    sys.exit(exitstatus)
+else:
+    print(os.getpid(), "calling pytest")
+    os._exit(pytest.main(['--forked', '{test_file}']))
+""")
+
+    subprocess.run([sys.executable, '-m', 'slipcover', '--debug', '--json', '--out', str(out), script])
+
+    with out.open() as f:
+        cov = json.load(f)
+
+    check_summaries(cov)
+
+    assert test_file in cov['files']
+    cov = cov['files'][test_file]
+    assert [1, 2, 3, 4, 5, 6, 8, 9, 10, 11, 13, 14] == cov['executed_lines']
+    assert [] == cov['missing_lines']
+
+
 def test_merge_flag(cov_merge_fixture):
     subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
                     '--json', '--out', "a.json", "t.py"], check=True)
     subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
                     '--json', '--out', "b.json", "t.py", "X"], check=True)
 
     subprocess.run([sys.executable, '-m', 'slipcover', '--merge',
```

### Comparing `slipcover-1.0.5/tests/test_importer.py` & `slipcover-1.0.6/tests/test_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 import slipcover.importer as im
 from pathlib import Path
+import subprocess
 
 import sys
 
 
 def test_filematcher_defaults(tmp_path, monkeypatch):
     base = tmp_path / "foo"
     base.mkdir()
@@ -272,7 +273,17 @@
 
     cov = sci.get_coverage()
     assert any(str(Path('pip/__init__.py')) in k for k in cov['files'].keys())
 """)
 
     p = subprocess.run([sys.executable, "-m", "slipcover", "--silent", "-m", "pytest", "-vv", cmdfile])
     assert p.returncode == 0
+
+
+def test_run_script_argv_is_str(tmp_path):
+    cmdfile = tmp_path / "t.py"
+    cmdfile.write_text("""
+import sys
+assert isinstance(sys.argv[0], str)
+""")
+
+    subprocess.run([sys.executable, "-m", "slipcover", "--silent", cmdfile], check=True)
```

### Comparing `slipcover-1.0.5/tests/test_instrumentation.py` & `slipcover-1.0.6/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/testme-class.py` & `slipcover-1.0.6/tests/testme-class.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/testme-inner.py` & `slipcover-1.0.6/tests/testme-inner.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/testme-partial.py` & `slipcover-1.0.6/tests/testme-partial.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.5/tests/testme.py` & `slipcover-1.0.6/tests/testme.py`

 * *Files identical despite different names*

