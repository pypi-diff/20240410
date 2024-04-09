# Comparing `tmp/matchlib-0.2.2.tar.gz` & `tmp/matchlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchlib-0.2.2.tar", last modified: Fri Aug 18 20:17:53 2023, max compression
+gzip compressed data, was "matchlib-0.2.3.tar", last modified: Tue Apr  9 22:16:30 2024, max compression
```

## Comparing `matchlib-0.2.2.tar` & `matchlib-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2023-08-18 20:17:53.812365 matchlib-0.2.2/
--rw-r--r--   0 fortunatov   (501) staff       (20)     1074 2023-08-18 19:39:15.000000 matchlib-0.2.2/LICENSE
--rw-r--r--   0 fortunatov   (501) staff       (20)     3352 2023-08-18 20:17:53.812734 matchlib-0.2.2/PKG-INFO
--rw-r--r--   0 fortunatov   (501) staff       (20)     2914 2023-08-18 19:39:15.000000 matchlib-0.2.2/README.md
-drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2023-08-18 20:17:53.808708 matchlib-0.2.2/matchlib/
--rw-r--r--   0 fortunatov   (501) staff       (20)      117 2023-08-18 19:39:15.000000 matchlib-0.2.2/matchlib/__init__.py
--rw-r--r--   0 fortunatov   (501) staff       (20)     2387 2023-08-18 19:48:18.000000 matchlib-0.2.2/matchlib/main.py
-drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2023-08-18 20:17:53.811117 matchlib-0.2.2/matchlib.egg-info/
--rw-r--r--   0 fortunatov   (501) staff       (20)     3352 2023-08-18 20:17:53.000000 matchlib-0.2.2/matchlib.egg-info/PKG-INFO
--rw-r--r--   0 fortunatov   (501) staff       (20)      225 2023-08-18 20:17:53.000000 matchlib-0.2.2/matchlib.egg-info/SOURCES.txt
--rw-r--r--   0 fortunatov   (501) staff       (20)        1 2023-08-18 20:17:53.000000 matchlib-0.2.2/matchlib.egg-info/dependency_links.txt
--rw-r--r--   0 fortunatov   (501) staff       (20)        9 2023-08-18 20:17:53.000000 matchlib-0.2.2/matchlib.egg-info/top_level.txt
--rw-r--r--   0 fortunatov   (501) staff       (20)       79 2023-08-18 20:17:53.814890 matchlib-0.2.2/setup.cfg
--rw-r--r--   0 fortunatov   (501) staff       (20)      627 2023-08-18 20:11:50.000000 matchlib-0.2.2/setup.py
-drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2023-08-18 20:17:53.811758 matchlib-0.2.2/tests/
--rw-r--r--   0 fortunatov   (501) staff       (20)     9549 2023-08-18 20:16:43.000000 matchlib-0.2.2/tests/test_matching.py
+drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2024-04-09 22:16:30.346278 matchlib-0.2.3/
+-rw-r--r--   0 fortunatov   (501) staff       (20)     1074 2023-08-18 19:39:15.000000 matchlib-0.2.3/LICENSE
+-rw-r--r--   0 fortunatov   (501) staff       (20)     3352 2024-04-09 22:16:30.346462 matchlib-0.2.3/PKG-INFO
+-rw-r--r--   0 fortunatov   (501) staff       (20)     2914 2023-08-18 19:39:15.000000 matchlib-0.2.3/README.md
+drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2024-04-09 22:16:30.343045 matchlib-0.2.3/matchlib/
+-rw-r--r--   0 fortunatov   (501) staff       (20)      117 2024-04-09 21:49:10.000000 matchlib-0.2.3/matchlib/__init__.py
+-rw-r--r--   0 fortunatov   (501) staff       (20)     2730 2024-04-09 22:13:51.000000 matchlib-0.2.3/matchlib/main.py
+drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2024-04-09 22:16:30.344873 matchlib-0.2.3/matchlib.egg-info/
+-rw-r--r--   0 fortunatov   (501) staff       (20)     3352 2024-04-09 22:16:30.000000 matchlib-0.2.3/matchlib.egg-info/PKG-INFO
+-rw-r--r--   0 fortunatov   (501) staff       (20)      225 2024-04-09 22:16:30.000000 matchlib-0.2.3/matchlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fortunatov   (501) staff       (20)        1 2024-04-09 22:16:30.000000 matchlib-0.2.3/matchlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fortunatov   (501) staff       (20)        9 2024-04-09 22:16:30.000000 matchlib-0.2.3/matchlib.egg-info/top_level.txt
+-rw-r--r--   0 fortunatov   (501) staff       (20)       79 2024-04-09 22:16:30.347052 matchlib-0.2.3/setup.cfg
+-rw-r--r--   0 fortunatov   (501) staff       (20)      627 2024-04-09 22:14:56.000000 matchlib-0.2.3/setup.py
+drwxr-xr-x   0 fortunatov   (501) staff       (20)        0 2024-04-09 22:16:30.345259 matchlib-0.2.3/tests/
+-rw-r--r--   0 fortunatov   (501) staff       (20)     9321 2024-04-09 21:49:11.000000 matchlib-0.2.3/tests/test_matching.py
```

### Comparing `matchlib-0.2.2/LICENSE` & `matchlib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matchlib-0.2.2/PKG-INFO` & `matchlib-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for partial comparison of (nested) data structures
 Home-page: https://github.com/qweeze/matchlib
 Author: qweeze
 Author-email: qweeeze@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `matchlib-0.2.2/README.md` & `matchlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `matchlib-0.2.2/matchlib/main.py` & `matchlib-0.2.3/matchlib/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
-from typing import Union
+import typing as t
 
 
-Matchable = Union[dict, list, set, tuple]
+Matchable = t.Union[t.Dict[t.Any, t.Any], t.List[t.Any], t.Set[t.Any], t.Tuple[t.Any]]
 
 
 def matches(obj: Matchable, partial: Matchable) -> bool:
     """Matches a given object against another
     which can contain "wildcard" elements (`...`)
     :return: bool
     """
@@ -34,26 +34,25 @@
 
     elif isinstance(partial, set) and isinstance(obj, set):
         if ... in partial:
             return (partial - {...}).issubset(obj)
         else:
             return partial == obj
 
-    elif (
-        (isinstance(partial, list) and isinstance(obj, list)) or
-        (isinstance(partial, tuple) and isinstance(obj, tuple))
+    elif (isinstance(partial, list) and isinstance(obj, list)) or (
+        isinstance(partial, tuple) and isinstance(obj, tuple)
     ):
         obj_idx = 0
         for idx, el in enumerate(partial):
             if el is ...:
                 if idx == len(partial) - 1:
                     return True
 
                 for i2 in range(obj_idx, len(obj)):
-                    if matches(obj[i2:], partial[idx + 1:]):
+                    if matches(obj[i2:], partial[idx + 1 :]):
                         return True
 
                 return False
 
             if obj_idx >= len(obj) or not matches(obj[obj_idx], el):
                 return False
 
@@ -64,29 +63,33 @@
 
         return True
 
     return partial == obj
 
 
 class Partial:
-    def __init__(self, obj: Union[dict, list]):
+    def __init__(self, obj: t.Union[t.Dict[t.Any, t.Any], t.List[t.Any]]) -> None:
         self.obj = obj
 
-    def __eq__(self, other):
-        return matches(other, self.obj)
-
-    def __ne__(self, other):
-        return not matches(other, self.obj)
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, (dict, list, set, tuple)):
+            return matches(other, self.obj)
+        return super().__eq__(other)
+
+    def __ne__(self, other: object) -> bool:
+        if isinstance(other, (dict, list, set, tuple)):
+            return not matches(other, self.obj)
+        return super().__ne__(other)
 
 
 class Regex:
-    def __init__(self, pattern, flags=0):
+    def __init__(self, pattern: str, flags: int = 0) -> None:
         self._regex = re.compile(pattern, flags=flags)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, str) and self._regex.match(other) is not None
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
 
 Any = ...
```

### Comparing `matchlib-0.2.2/matchlib.egg-info/PKG-INFO` & `matchlib-0.2.3/matchlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for partial comparison of (nested) data structures
 Home-page: https://github.com/qweeze/matchlib
 Author: qweeze
 Author-email: qweeeze@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `matchlib-0.2.2/tests/test_matching.py` & `matchlib-0.2.3/tests/test_matching.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 def test_simple():
     assert matches([], [])
     assert matches({}, {})
     assert matches(None, None)
     assert matches(False, False)
     assert matches(True, True)
     assert matches(42, 42)
-    assert matches('abc', 'abc')
+    assert matches("abc", "abc")
 
     assert matches([1, 2, 3], [1, 2, 3])
-    assert matches({'a': 1, 'b': 2}, {'a': 1, 'b': 2})
+    assert matches({"a": 1, "b": 2}, {"a": 1, "b": 2})
 
-    assert matches({'a': 1, 'b': 2}, {...: ...})
-    assert matches({'a': 1, 'b': 2}, {'a': 1, 'b': ...})
-    assert matches({'a': 1, 'b': 2}, {'a': 1, ...: ...})
-    assert matches({'a': 1, 'b': 2, 'c': 3}, {'a': 1, ...: ...})
-    assert matches({'a': 1, 'b': 2, 'c': 3}, {'a': 1, 'c': 3, ...: ...})
-    assert matches({'a': 1, 'b': 2, 'c': 3}, {'a': ..., 'c': 3, ...: ...})
+    assert matches({"a": 1, "b": 2}, {...: ...})
+    assert matches({"a": 1, "b": 2}, {"a": 1, "b": ...})
+    assert matches({"a": 1, "b": 2}, {"a": 1, ...: ...})
+    assert matches({"a": 1, "b": 2, "c": 3}, {"a": 1, ...: ...})
+    assert matches({"a": 1, "b": 2, "c": 3}, {"a": 1, "c": 3, ...: ...})
+    assert matches({"a": 1, "b": 2, "c": 3}, {"a": ..., "c": 3, ...: ...})
 
     assert matches([1, 2, 3], [..., 2, 3])
     assert matches([1, 2, 3], [1, 2, ...])
     assert matches([1, 2, 3], [1, ..., 3])
 
     assert matches([1, 2, 3], [Any, 2, 3])
     assert matches([1, 2, 3], [1, 2, Any])
@@ -38,38 +38,39 @@
     assert matches([1, 1, 1], [...])
 
     assert matches([1, 2, 3, 4, 5], [1, 2, 3, ..., 4, ...])
     assert matches([1, 2, 3, 4, 5], [1, 2, ..., 4, ..., 5])
     assert matches([1, 2, 3, 4, 5], [..., 1, 2, ..., 5])
     assert matches([1, 2, 3, 4, 5], [..., 2, 3, ...])
 
+
 def test_simple_negative():
     assert not matches([], [42])
     assert not matches([42], [])
-    assert not matches({'a': 1}, {})
-    assert not matches({}, {'a': 1})
+    assert not matches({"a": 1}, {})
+    assert not matches({}, {"a": 1})
     assert not matches(None, 42)
     assert not matches(42, None)
     assert not matches(False, True)
     assert not matches(True, False)
     assert not matches(42, 43)
-    assert not matches('abc', 'abcd')
+    assert not matches("abc", "abcd")
 
     assert not matches([1, 2, 3], [1, 2, 3, 4])
     assert not matches([1, 2, 3, 4], [1, 2, 3])
-    assert not matches({'a': 1, 'b': 2}, {'a': 1, 'b': 42})
-    assert not matches({'a': 1, 'c': 2}, {'a': 1, 'b': 2})
-    assert not matches({'a': 1, 'b': 42}, {'a': 1, 'b': 2})
-
-    assert not matches({'a': 1, 'b': 2}, {'a': 1, 'c': ...})
-    assert not matches({'a': 1, 'b': 2}, {'a': 2, ...: ...})
-    assert not matches({'a': 2, 'b': 2}, {'a': 1, ...: ...})
-    assert not matches({'a': 1, 'b': 2, 'c': 3}, {'a': 1, ...: ..., 'c': 4})
-    assert not matches({'a': 1, 'b': 2, 'c': 4}, {'a': 1, 'c': 3, ...: ...})
-    assert not matches({'a': 1, 'b': 2, 'c': 3}, {'a': ..., 'c': 4, ...: ...})
+    assert not matches({"a": 1, "b": 2}, {"a": 1, "b": 42})
+    assert not matches({"a": 1, "c": 2}, {"a": 1, "b": 2})
+    assert not matches({"a": 1, "b": 42}, {"a": 1, "b": 2})
+
+    assert not matches({"a": 1, "b": 2}, {"a": 1, "c": ...})
+    assert not matches({"a": 1, "b": 2}, {"a": 2, ...: ...})
+    assert not matches({"a": 2, "b": 2}, {"a": 1, ...: ...})
+    assert not matches({"a": 1, "b": 2, "c": 3}, {"a": 1, ...: ..., "c": 4})
+    assert not matches({"a": 1, "b": 2, "c": 4}, {"a": 1, "c": 3, ...: ...})
+    assert not matches({"a": 1, "b": 2, "c": 3}, {"a": ..., "c": 4, ...: ...})
 
     assert not matches([1, 2, 3], [..., 2, 3, 4])
     assert not matches([1, 2, 3], [..., 2, 4, 3])
     assert not matches([1, 2, 3], [0, 1, 2, ...])
     assert not matches([1, 2, 3], [1, 3, 2, ...])
     assert not matches([1, 2, 3], [1, 2, ..., 4])
     assert not matches([1, 2, 3], [2, ..., 3])
@@ -91,14 +92,15 @@
     assert not matches([1, 2, 3, 4, 5], [..., 1, 1, 2, ..., 5])
     assert not matches([1, 2, 3, 4, 5], [..., 2, 3, 3, ...])
 
     assert not matches([1, 1, 2], [..., 1, 2, 2])
     assert not matches([1, 1, 1], [..., 1, 1, ..., 1, 1])
     assert not matches([1, 1, 1], [1, 1, ..., 1, 1])
 
+
 def test_multiple():
     assert matches([1, 3, 5], [..., ..., ..., 5])
     assert not matches([1, 3, 5], [..., ..., ..., 4])
 
     assert matches([1, 3, 5], [..., 3, ...])
     assert not matches([1, 3, 5], [..., 4, ...])
 
@@ -117,249 +119,211 @@
     assert not matches([0, 1, 2, 4, 5, 6, 7, 8, 9], [0, 1, ..., 5, 7, ..., 9])
     assert not matches([0, 1, 2, 4, 5, 6, 7, 8, 9], [0, 1, ..., 5, 7, ..., 8])
 
 
 def test_nested():
 
     obj = {
-        'id': 42,
-        'name': 'John Doe',
-        'email': 'john@gmail.com',
-        'posts': [
+        "id": 42,
+        "name": "John Doe",
+        "email": "john@gmail.com",
+        "posts": [
             {
-                'id': 1,
-                'text': 'some text',
+                "id": 1,
+                "text": "some text",
             },
             {
-                'id': 13,
-                'text': 'Lorem Ipsum...',
-                'likes': [42, 142, 242],
-            }
-        ]
-
+                "id": 13,
+                "text": "Lorem Ipsum...",
+                "likes": [42, 142, 242],
+            },
+        ],
     }
 
     assert matches(
         obj,
+        {"name": "John Doe", "posts": [...], ...: ...},
+    )
+
+    assert obj == Partial({"name": "John Doe", "posts": [...], ...: ...})
+
+    assert obj == Partial(
         {
-            'name': 'John Doe',
-            'posts': [...],
-            ...: ...
-        },
-    )
-
-    assert obj == Partial({
-        'name': 'John Doe',
-        'posts': [...],
-        ...: ...
-    })
-
-    assert obj == Partial({
-        'name': 'John Doe',
-        'posts': [
-            ...,
-            {
-                ...: ...,
-                'likes': [..., 142, ...]
-            },
-            ...
-        ],
-        ...: ...
-    })
+            "name": "John Doe",
+            "posts": [..., {...: ..., "likes": [..., 142, ...]}, ...],
+            ...: ...,
+        }
+    )
 
-    assert obj == Partial({
-        'id': ...,
-        'name': 'John Doe',
-        'email': Regex(r'\w+@gmail.com'),
-        'posts': [...],
-    })
-
-    assert obj == Partial({
-        'id': ...,
-        'name': 'John Doe',
-        'email': Regex(r'\w+@gmail.com'),
-        'posts': [
-            {
-                'id': ...,
-                'text': 'some text',
-            },
-            ...
-        ],
-    })
+    assert obj == Partial(
+        {
+            "id": ...,
+            "name": "John Doe",
+            "email": Regex(r"\w+@gmail.com"),
+            "posts": [...],
+        }
+    )
 
-    assert obj == Partial({
-        'id': 42,
-        ...: ...,
-        'posts': [
-            {
-                'id': 1,
-                ...: ...
-            },
-            {
-                'text': Regex(r'Lorem \w+'),
-                ...: ...
-            }
-        ],
-    })
+    assert obj == Partial(
+        {
+            "id": ...,
+            "name": "John Doe",
+            "email": Regex(r"\w+@gmail.com"),
+            "posts": [
+                {
+                    "id": ...,
+                    "text": "some text",
+                },
+                ...,
+            ],
+        }
+    )
+
+    assert obj == Partial(
+        {
+            "id": 42,
+            ...: ...,
+            "posts": [{"id": 1, ...: ...}, {"text": Regex(r"Lorem \w+"), ...: ...}],
+        }
+    )
+
+    assert [obj] == Partial([{"name": "John Doe", "posts": [...], ...: ...}])
 
-    assert [obj] == Partial([{
-        'name': 'John Doe',
-        'posts': [...],
-        ...: ...
-    }])
-
-    assert [obj, {}] == Partial([
-        {
-            'name': 'John Doe',
-            'posts': [...],
-            ...: ...
-        },
-        ...
-    ])
+    assert [obj, {}] == Partial([{"name": "John Doe", "posts": [...], ...: ...}, ...])
 
 
 def test_nested_negative():
 
     obj = {
-        'id': 42,
-        'name': 'John Doe',
-        'email': 'john@gmail.com',
-        'posts': [
+        "id": 42,
+        "name": "John Doe",
+        "email": "john@gmail.com",
+        "posts": [
             {
-                'id': 1,
-                'text': 'some text',
+                "id": 1,
+                "text": "some text",
             },
             {
-                'id': 13,
-                'text': 'Lorem Ipsum...',
-                'likes': [42, 142, 242],
-            }
-        ]
-
-    }
-
-    assert obj != Partial({
-        'id': ...,
-        'name': 'John Doe',
-        'email': Regex(r'\w+@gmail.com'),
-        'posts': [
-            {
-                'id': ...,
-                'text': 'some text',
+                "id": 13,
+                "text": "Lorem Ipsum...",
+                "likes": [42, 142, 242],
             },
         ],
-    })
+    }
 
-    assert obj != Partial({
-        'email': Regex(r'\w+@gmail.com'),
-        'posts': {...: ...},
-    })
-
-    assert obj != Partial({
-        'email': Regex(r'mail.org'),
-        ...: ...
-    })
-
-    assert obj != Partial({
-        'name': 'John Doe',
-        'posts': [
-            {
-                ...: ...,
-                'likes': [..., 142, ...]
-            },
-        ],
-        ...: ...
-    })
+    assert obj != Partial(
+        {
+            "id": ...,
+            "name": "John Doe",
+            "email": Regex(r"\w+@gmail.com"),
+            "posts": [
+                {
+                    "id": ...,
+                    "text": "some text",
+                },
+            ],
+        }
+    )
 
-    assert obj != Partial({
-        'name': 'John Doe',
-        'posts': [
-            ...,
-            {
-                ...: ...,
-                'likes': [..., 142, ...]
-            },
-            ...
-        ],
-    })
+    assert obj != Partial(
+        {
+            "email": Regex(r"\w+@gmail.com"),
+            "posts": {...: ...},
+        }
+    )
 
-    assert obj != Partial({
-        'name': 'John Doe',
-        'posts': [
-            ...,
-            {
-                ...: ...,
-                'likes': [142, ...]
-            },
-            ...
-        ],
-        ...: ...
-    })
+    assert obj != Partial({"email": Regex(r"mail.org"), ...: ...})
+
+    assert obj != Partial(
+        {
+            "name": "John Doe",
+            "posts": [
+                {...: ..., "likes": [..., 142, ...]},
+            ],
+            ...: ...,
+        }
+    )
+
+    assert obj != Partial(
+        {
+            "name": "John Doe",
+            "posts": [..., {...: ..., "likes": [..., 142, ...]}, ...],
+        }
+    )
+
+    assert obj != Partial(
+        {
+            "name": "John Doe",
+            "posts": [..., {...: ..., "likes": [142, ...]}, ...],
+            ...: ...,
+        }
+    )
 
-    assert [obj, {}] != Partial([{
-        'name': 'John Doe',
-        'posts': [...],
-        ...: ...
-    }])
-
-    assert [obj] != Partial([
-        {
-            'name': 'John Doe',
-            'posts': [...],
-            ...: ...
-        },
-        {}
-    ])
+    assert [obj, {}] != Partial([{"name": "John Doe", "posts": [...], ...: ...}])
+
+    assert [obj] != Partial([{"name": "John Doe", "posts": [...], ...: ...}, {}])
 
 
 def test_sets():
     assert matches(set(), set())
     assert matches({1, 2, 3}, {1, ..., 3})
     assert matches({1, 2, 3}, {1, ...})
     assert matches({1, 2, 3}, {...})
 
     assert not matches({1, 2, 3}, set())
     assert not matches({1, 2, 3}, {0, 1, 2, ...})
 
 
 def test_dict_values():
     obj = {
-        'id': 42,
-        'name': 'John Doe',
-        'email': 'john@gmail.com',
+        "id": 42,
+        "name": "John Doe",
+        "email": "john@gmail.com",
     }
 
-    assert obj == Partial({
-        ...: 42,
-        'name': 'John Doe',
-        'email': 'john@gmail.com',
-    })
-
-    assert obj == Partial({
-        'id': 42,
-        'name': 'John Doe',
-        ...: 'john@gmail.com',
-    })
-
-    assert obj != Partial({
-        'id': 42,
-        ...: 'john@gmail.com',
-    })
-
-    assert obj != Partial({
-        'id': 42,
-        'name': 'John Doe',
-        'posts': [1, 2, 3],
-        ...: 'john@gmail.com',
-    })
-
-    assert obj == Partial({
-        'id': 42,
-        'name': ...,
-        ...: 'john@gmail.com',
-    })
-
-    assert obj == Partial({
-        'id': ...,
-        'name': ...,
-        'email': 'john@gmail.com',
-    })
+    assert obj == Partial(
+        {
+            ...: 42,
+            "name": "John Doe",
+            "email": "john@gmail.com",
+        }
+    )
+
+    assert obj == Partial(
+        {
+            "id": 42,
+            "name": "John Doe",
+            ...: "john@gmail.com",
+        }
+    )
+
+    assert obj != Partial(
+        {
+            "id": 42,
+            ...: "john@gmail.com",
+        }
+    )
+
+    assert obj != Partial(
+        {
+            "id": 42,
+            "name": "John Doe",
+            "posts": [1, 2, 3],
+            ...: "john@gmail.com",
+        }
+    )
+
+    assert obj == Partial(
+        {
+            "id": 42,
+            "name": ...,
+            ...: "john@gmail.com",
+        }
+    )
+
+    assert obj == Partial(
+        {
+            "id": ...,
+            "name": ...,
+            "email": "john@gmail.com",
+        }
+    )
```

