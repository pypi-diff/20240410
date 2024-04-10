# Comparing `tmp/zon-1.0.0.tar.gz` & `tmp/zon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zon-1.0.0.tar", last modified: Fri Nov 24 14:20:41 2023, max compression
+gzip compressed data, was "zon-1.1.0.tar", last modified: Wed Apr 10 11:17:55 2024, max compression
```

## Comparing `zon-1.0.0.tar` & `zon-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2023-11-24 14:20:41.912309 zon-1.0.0/
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1069 2023-11-22 19:49:29.000000 zon-1.0.0/LICENSE
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1364 2023-11-24 14:20:41.912309 zon-1.0.0/PKG-INFO
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)      862 2023-11-24 14:16:13.000000 zon-1.0.0/README.md
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)      608 2023-11-24 14:05:16.000000 zon-1.0.0/pyproject.toml
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)       38 2023-11-24 14:20:41.912309 zon-1.0.0/setup.cfg
-drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2023-11-24 14:20:41.912309 zon-1.0.0/zon/
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     2648 2023-11-24 14:16:34.000000 zon-1.0.0/zon/__init__.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     4269 2023-11-24 14:17:38.000000 zon-1.0.0/zon/base.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1444 2023-11-24 14:17:52.000000 zon-1.0.0/zon/bool.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)      653 2023-11-24 14:17:43.000000 zon-1.0.0/zon/error.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     2186 2023-11-24 14:15:54.000000 zon-1.0.0/zon/list.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1262 2023-11-24 14:14:29.000000 zon-1.0.0/zon/record.py
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)      615 2023-11-24 14:14:51.000000 zon-1.0.0/zon/union.py
-drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2023-11-24 14:20:41.912309 zon-1.0.0/zon.egg-info/
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1364 2023-11-24 14:20:41.000000 zon-1.0.0/zon.egg-info/PKG-INFO
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)      232 2023-11-24 14:20:41.000000 zon-1.0.0/zon.egg-info/SOURCES.txt
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)        1 2023-11-24 14:20:41.000000 zon-1.0.0/zon.egg-info/dependency_links.txt
--rw-r--r--   0 naapperas  (1000) naapperas  (1000)        4 2023-11-24 14:20:41.000000 zon-1.0.0/zon.egg-info/top_level.txt
+drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2024-04-10 11:17:55.408442 zon-1.1.0/
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1069 2024-04-10 10:21:01.000000 zon-1.1.0/LICENSE
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     4551 2024-04-10 11:17:55.408442 zon-1.1.0/PKG-INFO
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     4050 2024-04-10 10:21:01.000000 zon-1.1.0/README.md
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      608 2024-04-10 11:15:15.000000 zon-1.1.0/pyproject.toml
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)       38 2024-04-10 11:17:55.408442 zon-1.1.0/setup.cfg
+drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2024-04-10 11:17:55.405109 zon-1.1.0/zon/
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     3095 2024-04-10 10:21:01.000000 zon-1.1.0/zon/__init__.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      318 2024-04-10 10:21:01.000000 zon-1.1.0/zon/any.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     5535 2024-04-10 11:15:15.000000 zon-1.1.0/zon/base.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1444 2024-04-10 10:21:01.000000 zon-1.1.0/zon/bool.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      653 2024-04-10 10:21:01.000000 zon-1.1.0/zon/error.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      480 2024-04-10 10:21:01.000000 zon-1.1.0/zon/none.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     1262 2024-04-10 10:21:01.000000 zon-1.1.0/zon/record.py
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      615 2024-04-10 10:21:01.000000 zon-1.1.0/zon/union.py
+drwxr-xr-x   0 naapperas  (1000) naapperas  (1000)        0 2024-04-10 11:17:55.405109 zon-1.1.0/zon.egg-info/
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)     4551 2024-04-10 11:17:55.000000 zon-1.1.0/zon.egg-info/PKG-INFO
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)      243 2024-04-10 11:17:55.000000 zon-1.1.0/zon.egg-info/SOURCES.txt
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)        1 2024-04-10 11:17:55.000000 zon-1.1.0/zon.egg-info/dependency_links.txt
+-rw-r--r--   0 naapperas  (1000) naapperas  (1000)        4 2024-04-10 11:17:55.000000 zon-1.1.0/zon.egg-info/top_level.txt
```

### Comparing `zon-1.0.0/LICENSE` & `zon-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zon-1.0.0/pyproject.toml` & `zon-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zon"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Nuno Pereira", email="nunoafonso2002@gmail.com" },
 ]
 description = "A Zod-like validation library for Python"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `zon-1.0.0/zon/__init__.py` & `zon-1.1.0/zon/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Nuno Pereira"
 
 from zon.number.float import ZonFloat
 from zon.number.int import ZonInteger
 from zon.base import Zon
 from zon.bool import ZonBoolean
-from zon.list import ZonList
+from zon.element_list import ZonList
 from zon.str import ZonString
 from zon.union import ZonUnion
 from zon.record import ZonRecord
+from zon.any import ZonAny
+from zon.none import ZonNone
 
 
 def string() -> "ZonString":
     """Creates a new Zon that validates that the data is a string.
 
     Returns:
         ZonString: a new validator that validates that the data is a string.
@@ -88,7 +90,25 @@
         properties (dict[str, Zon]): the properties of the object to be validated.
 
     Returns:
         ZonRecord: a new validator that validates that the data is
         an object with the specified properties.
     """
     return ZonRecord(properties)
+
+
+def none() -> "ZonNone":
+    """Creates a new Zon that validates that the data is None.
+
+    Returns:
+        ZonNone: a new validator that validates that the data is None.
+    """
+    return ZonNone()
+
+
+def anything() -> "ZonAny":
+    """Creates a new Zon that validates anything.
+
+    Returns:
+        ZonAny: a new validator that validates anything.
+    """
+    return ZonAny()
```

### Comparing `zon-1.0.0/zon/base.py` & `zon-1.1.0/zon/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 from .error import ValidationError
 
 T = TypeVar("T")
 ValidationRule = Callable[[T], bool]
 
 
+class AggregateValidator:
+    """A validator that aggregates multiple validation calls"""
+
+
 class Zon(ABC):
     """Base class for all Zons.
     A Zon is the basic unit of validation in Zon.
     It is used to validate data, and can be composed with other Zons
     to create more complex validations.
     """
 
@@ -93,14 +97,48 @@
             the data is valid for both this Zon and the supplied Zon.
         """
         return ZonAnd(self, zon)
 
     def __and__(self, zon: "Zon") -> "ZonAnd":
         return self.and_also(zon)
 
+    def refine(self, refinement: Callable[[T], bool]) -> "Self":
+        """Creates a new Zon that validates the data with the supplied refinement.
+
+        A refinement is a function that takes a piece of data and returns True if the data is valid or throws otherwise.
+
+        Args:
+            refinement (Callable[[T], bool]): the refinement to be applied.
+
+        Returns:
+            ZonRefined: a new validator that validates the data with the supplied refinement.
+        """
+        _clone = self._clone()
+
+        def _refinement_validate(data):
+            try:
+                return refinement(data)
+            except ValidationError as e:
+                _clone._add_error(e)
+                return False
+
+        if "_refined_" not in _clone.validators:
+            _clone.validators["_refined_"] = _refinement_validate
+        else:
+            current_refinement = _clone.validators["_refined_"]
+
+            def _refined_validator(data):
+                return current_refinement(data) and _refinement_validate(
+                    data
+                )
+
+            _clone.validators["_refined_"] = _refined_validator
+
+        return _clone
+
 
 def optional(zon: Zon) -> "ZonOptional":
     """Marks this validation chain as optional, making it so the data supplied need not be defined.
 
     Args:
         zon (Zon): the validator to be marked as optional.
 
@@ -125,15 +163,15 @@
             return True
         return self.zon.validate(data)
 
 
 class ZonAnd(Zon):
     """A Zon that validates that the data is valid for both this Zon and the supplied Zon."""
 
-    def __init__(self, zon1, zon2):
+    def __init__(self, zon1: Zon, zon2: Zon):
         super().__init__()
         self.zon1 = zon1
         self.zon2 = zon2
 
     def _setup(self):
         self.validators["_default_"] = self._default_validate
```

### Comparing `zon-1.0.0/zon/bool.py` & `zon-1.1.0/zon/bool.py`

 * *Files identical despite different names*

### Comparing `zon-1.0.0/zon/error.py` & `zon-1.1.0/zon/error.py`

 * *Files identical despite different names*

### Comparing `zon-1.0.0/zon/record.py` & `zon-1.1.0/zon/record.py`

 * *Files identical despite different names*

### Comparing `zon-1.0.0/zon/union.py` & `zon-1.1.0/zon/union.py`

 * *Files identical despite different names*

