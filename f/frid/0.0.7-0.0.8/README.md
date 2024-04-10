# Comparing `tmp/frid-0.0.7.tar.gz` & `tmp/frid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.7.tar", last modified: Mon Apr  8 22:01:28 2024, max compression
+gzip compressed data, was "frid-0.0.8.tar", last modified: Tue Apr  9 20:55:19 2024, max compression
```

## Comparing `frid-0.0.7.tar` & `frid-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.7/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 22:01:28.912291 frid-0.0.7/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.7/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.7/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.7/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-08 21:10:44.000000 frid-0.0.7/frid/autils.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.7/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.7/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.7/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8575 2024-04-08 19:51:11.000000 frid-0.0.7/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.7/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.7/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.7/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.7/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2351 2024-04-08 20:00:06.000000 frid-0.0.7/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.7/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-08 22:01:04.000000 frid-0.0.7/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-08 22:01:28.912291 frid-0.0.7/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.8/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-09 20:55:19.842771 frid-0.0.8/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.8/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.8/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24852 2024-04-09 15:23:14.000000 frid-0.0.8/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-08 21:10:44.000000 frid-0.0.8/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.8/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.8/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2839 2024-04-09 20:53:28.000000 frid-0.0.8/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8575 2024-04-08 19:51:11.000000 frid-0.0.8/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.8/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24329 2024-04-09 15:21:21.000000 frid-0.0.8/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.8/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.8/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2351 2024-04-09 20:53:51.000000 frid-0.0.8/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11564 2024-04-09 20:53:16.000000 frid-0.0.8/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-09 20:55:19.842771 frid-0.0.8/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-09 20:55:19.000000 frid-0.0.8/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-09 20:55:13.000000 frid-0.0.8/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-09 20:55:19.842771 frid-0.0.8/setup.cfg
```

### Comparing `frid-0.0.7/LICENSE` & `frid-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/PKG-INFO` & `frid-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.7/README.md` & `frid-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/__init__.py` & `frid-0.0.8/frid/__init__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/__main__.py` & `frid-0.0.8/frid/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,14 +496,26 @@
         math.nan, math.inf, -math.inf, dateonly.today(), b"1234", {3: 4}, object(),
     ]
     def test_negative_json_dump(self):
         for i, k in enumerate(self.negative_json_dump_cases):
             with self.assertRaises(ValueError, msg=f"[{i}]: {k}"):
                 dump_into_str(k, json_level=True)
 
+    comment_cases = {
+        "\n123": 123, "\n[\n123,\n\n 456,]": [123, 456],
+        "123 # 456": 123, "123 # 456\n": 123, "// abc\n456": 456, "/* abc */ 123": 123,
+        "[123, #456,\n789]": [123, 789], "[1,/*1,\n3,*/ 4 // 5,\n # 6\n, 7]": [1,4,7],
+    }
+
+    def test_comments(self):
+        for i, (k, v) in enumerate(self.comment_cases.items()):
+            w = load_from_str(k, comments=[("#", "\n"), ("//", "\n"), ("/*", "*/")])
+            self.assertEqual(v, w, msg=f"[{i}]: {k}")
+
+
 if __name__ == '__main__':
     if _cov is not None:
         unittest.main(exit=False)
         _cov.stop()
         _cov.save()
         print("Generating HTML converage report ...")
         _cov.html_report()
```

### Comparing `frid-0.0.7/frid/autils.py` & `frid-0.0.8/frid/autils.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/chrono.py` & `frid-0.0.8/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/dumper.py` & `frid-0.0.8/frid/dumper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/errors.py` & `frid-0.0.8/frid/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from collections.abc import Sequence
 import traceback
 from types import TracebackType
 
-from .typing import FridMixin
+from .typing import FridMixin, FridValue
+from .helper import get_type_name
 from .guards import is_text_list_like
 
 FRID_ERROR_VENUE = os.getenv('FRID_ERROR_VENUE')
 
 class FridError(FridMixin, Exception):
     """The base class of errors that is compatible with Frid.
     The error can be constructed in three ways:
@@ -39,15 +40,16 @@
     def frid_from(cls, name: str, *args, error: str, trace: Sequence[str]|None=None,
                   cause: str|None=None, **kwds):
         # The `trace` and `cause` are not accepting TrackbackType and BaseException;
         # and `error` is passed as the first argument.
         assert name in cls.frid_keys()
         return FridError(error, trace=trace, **kwds)
 
-    def frid_repr(self) -> dict[str,str|int|list[str]]:
+    def frid_dict(self) -> dict[str,str|int|list[str]]:
+        """Convert the error into a dictionary"""
         out: dict[str,str|int|list[str]] = {'error': str(self)}
         trace = []
         if self.trace is not None:
             trace.extend(self.trace)
             trace.append("")
         trace.extend(traceback.format_exception(self))
         if self.__cause__:
@@ -60,7 +62,10 @@
         if trace:
             out['trace'] = trace
         if self.notes:
             out['notes'] = self.notes
         if FRID_ERROR_VENUE is not None:
             out['venue'] = FRID_ERROR_VENUE
         return out
+
+    def frid_repr(self) -> tuple[str,Sequence[FridValue],dict[str,str|int|list[str]]]:
+        return (get_type_name(self), (), self.frid_dict())
```

### Comparing `frid-0.0.7/frid/guards.py` & `frid-0.0.8/frid/guards.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/helper.py` & `frid-0.0.8/frid/helper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/loader.py` & `frid-0.0.8/frid/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import math, base64
-from collections.abc import Callable, Iterator, Mapping, Set
+import math, types, base64
+from collections.abc import Callable, Iterator, Mapping, Sequence, Set
 from typing import  Any, Literal, NoReturn, TextIO, TypeVar
 
 from .typing import BlobTypes, DateTypes, FridArray, FridMixin, FridPrime, FridValue, StrKeyMap
 from .guards import is_frid_identifier, is_frid_prime, is_frid_quote_free, is_quote_free_char
 from .errors import FridError
 from .strops import str_find_any, StringEscapeDecode
 from .chrono import parse_datetime
 from .dumper import EXTRA_ESCAPE_PAIRS
 
-NO_QUOTE_CHARS = "~!?@#$%^&*/"
+NO_QUOTE_CHARS = "~!?@$%^&"   # Extra no quote chars; not including/ * # for potential comments
 ALLOWED_QUOTES = "'`\""
 
 T = TypeVar('T')
 
 class ParseError(FridError):
     def __init__(self, s: str, index: int, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -56,25 +56,29 @@
     - `parse_misc`: Callback to parse any unparsable data; must return a Frid
       compatible type. The function accepts an additional path parameter for path
       in the tree.
     """
     def __init__(
             self, buffer: str|None=None, length: int|None=None, offset: int=0, /,
             *, json_level: Literal[0,1,5]=0, escape_seq: str|None=None,
+            comments: Sequence[tuple[str,str]]=(),
             frid_mixin: Mapping[str,type[FridMixin]]|Iterator[type[FridMixin]]|None=None,
             parse_real: Callable[[str],int|float|None]|None=None,
             parse_date: Callable[[str],DateTypes|None]|None=None,
             parse_blob: Callable[[str],BlobTypes|None]|None=None,
             parse_expr: Callable[[str,str],FridMixin]|None=None,
             parse_misc: Callable[[str,str],FridValue]|None=None,
     ):
         self.buffer = buffer or ""
         self.offset = offset
         self.length = length if length is not None else 1<<62 if buffer is None else len(buffer)
         self.anchor: int|None = None   # A place where the location is marked
+        if not all(opening and closing for opening, closing in comments):
+            raise ValueError(f"Invalid comments configuration: {comments}")
+        self.comments: Sequence[tuple[str,str]] = comments
         # The following are all constants
         self.json_level = json_level
         self.escape_seq = escape_seq
         self.parse_real = parse_real
         self.parse_date = parse_date
         self.parse_blob = parse_blob
         self.parse_expr = parse_expr
@@ -186,57 +190,82 @@
                 pass
             try:
                 return float(s)
             except Exception:
                 pass
         return default
 
+    def peek_fixed_size(self, index: int, path: str, nchars: int) -> str:
+        """Peeks a string with a fixed size given by `nchars`.
+        - Returns the string with these number of chars, or shorter if end of
+          stream is reached.
+        """
+        while len(self.buffer) < min(index + nchars, self.length):
+            index = self.fetch(index, path)
+        while True:
+            try:
+                if index >= self.length:
+                    return ''
+                if index + nchars > self.length:
+                    return self.buffer[index:self.length]
+                return self.buffer[index:(index + nchars)]
+            except IndexError:
+                index = self.fetch(index, path)
+
     def skip_fixed_size(self, index: int, path: str, nchars: int) -> int:
         """Skips a number of characters without checking the content."""
         index += nchars
         if index > self.length:
             self.error(self.length, f"Trying to pass beyound the EOS at {index}: {path=}")
         return index
 
+    def skip_comments(self, index: int, path: str) -> int:
+        """Skip the comments in pairs."""
+        for opening, closing in self.comments:
+            if self.peek_fixed_size(index, path, len(opening)) != opening:
+                continue
+            index = self.skip_fixed_size(index, path, len(opening))
+            while True:
+                end_idx = self.buffer.find(closing, index)
+                if end_idx >= 0:
+                    assert end_idx >= index
+                    return end_idx + len(closing)
+                if len(self.buffer) >= self.length:
+                    if closing.isspace():
+                        # If the closing is a space (like newline), it is optional at end
+                        return self.length
+                    self.error(index, f"Expecting '{closing}' after {opening}")
+                index = self.fetch(index, path)
+            break
+        return index
+
     def skip_whitespace(self, index: int, path: str) -> int:
         """Skips the all following whitespaces."""
         while True:
             try:
                 while index < self.length and self.buffer[index].isspace():
                     index += 1
-                break
+                new_idx = self.skip_comments(index, path)
+                if index >= self.length:
+                    return index
+                if new_idx <= index: # No progress
+                    break
+                index = new_idx
             except IndexError:
                 index = self.fetch(index, path)
         return index
 
     def skip_prefix_str(self, index: int, path: str, prefix: str) -> int:
         """Skips the `prefix` if it matches, or raise an ParseError."""
         while len(self.buffer) < min(index + len(prefix), self.length):
             index = self.fetch(index, path)
         if not self.buffer.startswith(prefix, index):
             self.error(index, f"Stream ends while expecting '{prefix}'")
         return index + len(prefix)
 
-    def peek_fixed_size(self, index: int, path: str, nchars: int) -> str:
-        """Peeks a string with a fixed size given by `nchars`.
-        - Returns the string with these number of chars, or shorter if end of
-          stream is reached.
-        """
-        while len(self.buffer) < min(index + nchars, self.length):
-            index = self.fetch(index, path)
-        while True:
-            try:
-                if index >= self.length:
-                    return ''
-                if index + nchars > self.length:
-                    return self.buffer[index:self.length]
-                return self.buffer[index:(index + nchars)]
-            except IndexError:
-                index = self.fetch(index, path)
-
     def scan_prime_data(self, index: int, path: str, /, empty: Any='',
                         accept=NO_QUOTE_CHARS) -> tuple[int,FridValue]:
         """Scans the unquoted data that are identifier chars plus the est given by `accept`."""
         while True:
             start = index
             try:
                 while index < self.length:
@@ -283,29 +312,33 @@
                 break
             except IndexError:
                 index = self.fetch(index, path)
             except ValueError as exc:
                 self.error(index, exc)
         return (index + count, value)
 
-    def scan_quoted_seq(self, index: int, path: str, /, quotes: str) -> tuple[int,FridPrime]:
+    def scan_quoted_seq(
+            self, index: int, path: str, /, quotes: str
+    ) -> tuple[int,FridPrime|types.EllipsisType]:
         """Scan a continuationm of quoted string after the first quoted str."""
         out = []
         while True:
             index = self.skip_whitespace(index, path)
             c = self.peek_fixed_size(index, path, 1)
             if not c or c not in quotes:
                 break
             index = self.skip_fixed_size(index, path, len(c))
             (index, value) = self.scan_escape_str(index, path, c)
             out.append(value)
             index = self.skip_prefix_str(index, path, c)
         data = ''.join(out)
         if self.escape_seq and data.startswith(self.escape_seq):
             data = data[len(self.escape_seq):]
+            if not data:
+                return (index,...)
             if (out := self.parse_prime_str(data, ...)) is not ...:
                 return (index, out)
         return (index, data)
 
     def scan_naked_list(self, index: int, path: str,
                         /, stop: str='', sep: str=',') -> tuple[int,FridArray]:
         out = []
@@ -407,15 +440,17 @@
             /, name: str,  args: list[FridValue], kwds: dict[str,FridValue]
     ) -> tuple[int,FridValue]:
         mixin = self.frid_mixin.get(name)
         if mixin is None:
             self.error(start, f"Cannot find constructor called {name}")
         return (index, mixin.frid_from(name, *args, **kwds))
 
-    def scan_frid_value(self, index: int, path: str, /, empty: Any='') -> tuple[int,FridValue]:
+    def scan_frid_value(
+            self, index: int, path: str, /, empty: Any=''
+    ) -> tuple[int,FridValue|types.EllipsisType]:
         """Load the text representation."""
         index = self.skip_whitespace(index, path)
         if index >= self.length:
             return (index, empty)
         c = self.peek_fixed_size(index, path, 1)
         if c == '[':
             index = self.skip_fixed_size(index, path, 1)
@@ -467,17 +502,18 @@
                 raise ValueError(f"Invalid input {type}")
         if index < 0:
             self.error(0, f"Failed to parse data: {path=}")
         if index < self.length:
             index = self.skip_whitespace(index, path)
             if index < self.length:
                 self.error(index, f"Trailing data at {index} ({path=}): {self.buffer[index:]}")
+        if value is ...:
+            self.error(index, "Dummy is only supported for map values")
         return value
 
-
 class FridTextIOLoader(FridLoader):
     def __init__(self, t: TextIO, page: int = 16384, **kwargs):
         super().__init__("", 1<<62, 0, **kwargs)  # Do not pass any positional parameters; using default
         self.file: TextIO|None = t
         self.page: int = page
     def fetch(self, index: int, path: str) -> int:
         if self.file is None:
```

### Comparing `frid-0.0.7/frid/pretty.py` & `frid-0.0.8/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/strops.py` & `frid-0.0.8/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/typing.py` & `frid-0.0.8/frid/typing.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.7/frid/webapp.py` & `frid-0.0.8/frid/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, json
-from collections.abc import AsyncIterable, Iterable, Mapping
+from collections.abc import AsyncIterable, Iterable, Mapping, Sequence
 from typing import Any, Literal
 from urllib.parse import unquote
 
 from .typing import BlobTypes, FridValue
 from .errors import FridError
 from .helper import get_type_name
 from .guards import is_frid_value
@@ -237,16 +237,12 @@
     - The constructor requires the http status code as the first argment
       before the error message.
     - Optionally an HTTP text can be given by `http_text` for construction.
     - Users can also specify `headers` as a dict.
     """
     def __init__(self, ht_status: int, *args, **kwargs):
         super().__init__(*args, ht_status=ht_status, **kwargs)
-    def frid_repr(self) -> dict[str,str|int|list[str]]:
-        out = super().frid_repr()
-        out['ht_status'] = self.ht_status
-        return out
     def set_response(self) -> 'HttpError':
-        self.http_data = self.frid_repr()
+        self.http_data = self.frid_dict()  # Only show the keyword part of this error
         super().set_response()
         return self
```

### Comparing `frid-0.0.7/frid.egg-info/PKG-INFO` & `frid-0.0.8/frid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.7/pyproject.toml` & `frid-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

