# Comparing `tmp/lambda_calculus-3.0.0.tar.gz` & `tmp/lambda_calculus-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_calculus-3.0.0.tar", last modified: Tue Oct  4 16:32:27 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lambda_calculus-3.0.0.tar` & `lambda_calculus-3.1.0.tar`

### file list

```diff
@@ -1,30 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.507832 lambda_calculus-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-10-04 16:32:27.507832 lambda_calculus-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.503832 lambda_calculus-3.0.0/lambda_calculus/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.503832 lambda_calculus-3.0.0/lambda_calculus/terms/
--rw-r--r--   0 runner    (1001) docker     (121)    12574 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/terms/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/terms/combinators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/terms/logic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/terms/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.507832 lambda_calculus-3.0.0/lambda_calculus/visitors/
--rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4487 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/normalisation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.507832 lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/
--rw-r--r--   0 runner    (1001) docker     (121)     4326 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/checked.py
--rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/renaming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/unsafe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/lambda_calculus/visitors/walking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:32:27.503832 lambda_calculus-3.0.0/lambda_calculus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-10-04 16:32:27.000000 lambda_calculus-3.0.0/lambda_calculus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-04 16:32:27.000000 lambda_calculus-3.0.0/lambda_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 16:32:27.000000 lambda_calculus-3.0.0/lambda_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-04 16:32:27.000000 lambda_calculus-3.0.0/lambda_calculus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-10-04 16:32:14.000000 lambda_calculus-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 16:32:27.507832 lambda_calculus-3.0.0/setup.cfg
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/.flake8
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/Makefile
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api.rst
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/conf.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/index.rst
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/installation.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/errors.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms/abc.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms/arithmetic.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms/combinators.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms/logic.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/terms/pairs.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/normalisation.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/substitution.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/walking.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/substitution/checked.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/substitution/renaming.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/docs/api/visitors/substitution/unsafe.rst
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/errors.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/py.typed
+-rw-r--r--   0        0        0    12440 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/abc.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/arithmetic.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/combinators.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/logic.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/terms/pairs.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/__init__.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/normalisation.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/walking.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/__init__.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/checked.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/renaming.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/unsafe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/test_errors.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/test_readme.py
+-rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/__init__.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/test_abc.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/test_arithmetic.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/test_combinators.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/test_logic.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/terms/test_pairs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/__init__.py
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/test_normalisation.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/test_walking.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/substitution/__init__.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/substitution/test_checked.py
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/tests/visitors/substitution/test_renaming.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/LICENSE
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/README.md
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lambda_calculus-3.1.0/PKG-INFO
```

### Comparing `lambda_calculus-3.0.0/LICENSE` & `lambda_calculus-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/PKG-INFO` & `lambda_calculus-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lambda_calculus
-Version: 3.0.0
+Version: 3.1.0
 Summary: Implementation of the Lambda calculus
-Author-email: Eric Niklas Wolf <eric_niklas.wolf@mailbox.tu-dresden.de>
 Project-URL: Repository, https://github.com/Deric-W/lambda_calculus
 Project-URL: Documentation, http://lambda-calculus.readthedocs.io/
 Project-URL: Bugtracker, https://github.com/Deric-W/lambda_calculus/issues
+Author-email: Eric Niklas Wolf <eric_niklas.wolf@mailbox.tu-dresden.de>
+License-File: LICENSE
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Education
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # lambda_calculus
 
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 ![Tests](https://github.com/Deric-W/lambda_calculus/actions/workflows/Tests.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/Deric-W/lambda_calculus/branch/main/graph/badge.svg?token=SU3982mC17)](https://codecov.io/gh/Deric-W/lambda_calculus)
 [![Documentation Status](https://readthedocs.org/projects/lambda-calculus/badge/?version=stable)](https://lambda-calculus.readthedocs.io/en/stable/?badge=stable)
 
 The [`lambda_calculus`](https://pypi.org/project/lambda-calculus/) package contains classes which implement basic operations of the lambda calculus.
 
 To use it, simply import the classes `Variable`, `Abstraction` and `Application` from this package
@@ -107,8 +108,8 @@
 from lambda_calculus import Variable, Application
 from lambda_calculus.visitors.normalisation import BetaNormalisingVisitor
 
 assert BetaNormalisingVisitor().skip_intermediate(term) == Application.with_arguments(
     Variable("+"),
     (Variable("4"), Variable("3"))
 )
-```
+```
```

### Comparing `lambda_calculus-3.0.0/README.md` & `lambda_calculus-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # lambda_calculus
 
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 ![Tests](https://github.com/Deric-W/lambda_calculus/actions/workflows/Tests.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/Deric-W/lambda_calculus/branch/main/graph/badge.svg?token=SU3982mC17)](https://codecov.io/gh/Deric-W/lambda_calculus)
 [![Documentation Status](https://readthedocs.org/projects/lambda-calculus/badge/?version=stable)](https://lambda-calculus.readthedocs.io/en/stable/?badge=stable)
 
 The [`lambda_calculus`](https://pypi.org/project/lambda-calculus/) package contains classes which implement basic operations of the lambda calculus.
 
 To use it, simply import the classes `Variable`, `Abstraction` and `Application` from this package
```

### Comparing `lambda_calculus-3.0.0/lambda_calculus/errors.py` & `lambda_calculus-3.1.0/src/lambda_calculus/errors.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/terms/__init__.py` & `lambda_calculus-3.1.0/src/lambda_calculus/terms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ..visitors.substitution import checked
 
 __all__ = (
     "Term",
     "Variable",
     "Abstraction",
     "Application",
+    "abc",
     "arithmetic",
     "logic",
     "pairs",
     "combinators"
 )
 
 T = TypeVar("T")
@@ -276,27 +277,25 @@
         elif new not in self.body.free_variables():
             return Abstraction(
                 new,
                 self.body.substitute(self.bound, Variable(new))
             )
         raise CollisionError("new variable would bind free variable in body", (new,))
 
-    def eta_reduction(self) -> Term[V]:   # type: ignore[return]
+    def eta_reduction(self) -> Term[V]:
         """
         Remove a useless abstraction.
 
         :raise ValueError: If abstraction is not useless
         :return: new term
         """
         match self.body:
             case Application(f, Variable(x)) if x == self.bound and x not in f.free_variables():
                 return f
             case _:
-                # mypy detects missing returns
-                # because of https://github.com/python/mypy/issues/12534
                 raise ValueError("abstraction is not useless")
 
     def accept(self, visitor: visitors.Visitor[T, V]) -> T:
         """
         Accept a visitor by calling visitors.Visitor.visit_abstraction.
 
         :param visitor: Visitor to accept
```

### Comparing `lambda_calculus-3.0.0/lambda_calculus/terms/arithmetic.py` & `lambda_calculus-3.1.0/src/lambda_calculus/terms/arithmetic.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/terms/combinators.py` & `lambda_calculus-3.1.0/src/lambda_calculus/terms/combinators.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/terms/logic.py` & `lambda_calculus-3.1.0/src/lambda_calculus/terms/logic.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/terms/pairs.py` & `lambda_calculus-3.1.0/src/lambda_calculus/terms/pairs.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/__init__.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/normalisation.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/normalisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
 
     __slots__ = ()
 
     def skip_intermediate(self, term: terms.Term[str]) -> terms.Term[str]:
         """
         Calculate the beta normal form directly.
-        
+
         :param term: term which should be transformed into ist beta normal form
         :return: new term representing the beta normal form if it exists
         """
         result = term
         for _, intermediate in term.accept(self):
             result = intermediate
         return result
@@ -73,15 +73,15 @@
         """
         results = abstraction.body.accept(self)
         return map(lambda s: (s[0], terms.Abstraction(abstraction.bound, s[1])), results)
 
     def beta_reducation(self, abstraction: terms.Abstraction[str], argument: terms.Term[str]) -> Generator[Step, None, terms.Term[str]]:
         """
         Perform beta reduction of an application.
-        
+
         :param abstraction: abstraction of the application
         :param argument: argument of the application
         :return: Generator yielding steps and returning the reduced term
         """
         conversions = CountingSubstitution.from_substitution(abstraction.bound, argument).trace()
         reduced = yield from map(
             lambda body: (
```

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/__init__.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/checked.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/checked.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/renaming.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/renaming.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/substitution/unsafe.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/substitution/unsafe.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/lambda_calculus/visitors/walking.py` & `lambda_calculus-3.1.0/src/lambda_calculus/visitors/walking.py`

 * *Files identical despite different names*

### Comparing `lambda_calculus-3.0.0/pyproject.toml` & `lambda_calculus-3.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lambda_calculus"
-version = "3.0.0"
+version = "3.1.0"
 description = "Implementation of the Lambda calculus"
 requires-python = ">=3.10"
 keywords = []
 classifiers = [
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
@@ -24,31 +24,87 @@
 
 [project.urls]
 Repository = "https://github.com/Deric-W/lambda_calculus"
 Documentation = "http://lambda-calculus.readthedocs.io/"
 Bugtracker = "https://github.com/Deric-W/lambda_calculus/issues"
 
 [build-system]
-requires = ["setuptools >= 61.0.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.setuptools.package-data]
-lambda_calculus = ["py.typed"]
+[tool.hatch.envs.test]
+dependencies = [
+    "coverage[toml] == 7.*"
+]
+
+[tool.hatch.envs.test.scripts]
+test = "python -m unittest discover {args}"
+cov-run = "coverage run -m unittest discover {args}"
+cov-report = [
+    "- coverage combine",
+    "coverage report"
+]
+cov = [
+    "cov-run",
+    "cov-report"
+]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.10", "3.11", "3.12"]
+
+[tool.hatch.envs.lint]
+dependencies = [
+    "mypy >= 1.0.0",
+    "pylint >= 2.12.2",
+    "flake8 >= 5.0.0",
+    "isort >= 5.10.1"
+]
+
+[tool.hatch.envs.lint.scripts]
+lint = [
+    "- flake8 src/lambda_calculus",
+    "- pylint src/lambda_calculus"
+]
+typecheck = "mypy -p lambda_calculus"
+release = [
+    "typecheck"
+]
+
+[tool.hatch.envs.docs]
+dependencies = [
+    "sphinx ~= 5.2.0",
+    "sphinx-pyproject ~= 0.1.0",
+    "sphinx-rtd-theme ~= 1.0.0"
+]
+
+[tool.hatch.envs.docs.scripts]
+build = "sphinx-build {args} docs docs/_build"
+
+[tool.hatch.build.targets.sdist]
+exclude = ["/.github"]
 
 [tool.mypy]
 disallow_any_unimported = true
 disallow_any_generics = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unreachable = true
 
+[tool.pylint]
+max-line-length = 100
+
+[tool.coverage.run]
+source_pkgs = ["lambda_calculus"]
+branch = true
+parallel = true
+
 [tool.sphinx-pyproject]
 project = "lambda_calculus"
 copyright = "2022 Eric Wolf"
 html_theme = "sphinx_rtd_theme"
 extensions = [
     "sphinx.ext.intersphinx",
     "sphinx.ext.autodoc",
```

