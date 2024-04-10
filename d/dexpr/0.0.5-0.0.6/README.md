# Comparing `tmp/dexpr-0.0.5.tar.gz` & `tmp/dexpr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexpr-0.0.5.tar", last modified: Sun Mar 10 21:52:16 2024, max compression
+gzip compressed data, was "dexpr-0.0.6.tar", last modified: Wed Apr 10 08:41:36 2024, max compression
```

## Comparing `dexpr-0.0.5.tar` & `dexpr-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:52:16.907500 dexpr-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-10 21:52:08.000000 dexpr-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-10 21:52:16.907500 dexpr-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-10 21:52:08.000000 dexpr-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:52:16.907500 dexpr-0.0.5/dexpr/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/dataclassex.py
--rw-r--r--   0 runner    (1001) docker     (127)    23025 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/dgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    25318 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-10 21:52:08.000000 dexpr-0.0.5/dexpr/tenor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:52:16.907500 dexpr-0.0.5/dexpr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-10 21:52:16.000000 dexpr-0.0.5/dexpr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-10 21:52:16.000000 dexpr-0.0.5/dexpr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 21:52:16.000000 dexpr-0.0.5/dexpr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-10 21:52:16.000000 dexpr-0.0.5/dexpr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-10 21:52:16.000000 dexpr-0.0.5/dexpr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-10 21:52:08.000000 dexpr-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 21:52:16.907500 dexpr-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:41:36.979160 dexpr-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 08:41:32.000000 dexpr-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-10 08:41:36.975160 dexpr-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-10 08:41:32.000000 dexpr-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:41:36.975160 dexpr-0.0.6/dexpr/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23575 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/dgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/exprclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 08:41:32.000000 dexpr-0.0.6/dexpr/tenor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:41:36.975160 dexpr-0.0.6/dexpr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-10 08:41:36.000000 dexpr-0.0.6/dexpr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 08:41:36.000000 dexpr-0.0.6/dexpr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:41:36.000000 dexpr-0.0.6/dexpr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 08:41:36.000000 dexpr-0.0.6/dexpr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 08:41:36.000000 dexpr-0.0.6/dexpr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 08:41:32.000000 dexpr-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:41:36.979160 dexpr-0.0.6/setup.cfg
```

### Comparing `dexpr-0.0.5/LICENSE` & `dexpr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dexpr-0.0.5/PKG-INFO` & `dexpr-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexpr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Libraries for capturing and using expressions in python
 Author-email: wukrur <wukrur@github.com>
 License: MIT
 Keywords: expressions,date generators,extended dataclass
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -87,22 +87,48 @@
     shipping_time: Tenor
     expected_delivery_date: date = lambda self: self.order_date + self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
-adding Op expressoins:
+adding Op expressions:
 
 ```python
 Self = ParameterOp(_name='Self')
 
 @dataclassex
 class OrderWithOp:
+    Self: 'OrderWithOp'
+    
     order_date: date
     shipping_time: Tenor
     expected_delivery_date: date = Self.order_date + Self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
+Note the `Self` member - it is there for enable autocomplete in the IDE when writing the expressions and is removed from
+processed annotations
+
+There are two other variants of syntax supported for declaring dataclasses with support for Ops and lambdas:
+
+```python
+@dataclass
+@exprclass
+class OrderWithOp:
+    ...
+```
+
+And
+
+```python
+@dataclass
+class OrderWithOp(ExprClass):
+    ...
+```
+
+They exist for cases when the developer wants to keep the @dataclass annotations as is 
+to use PyCharm's built in support for it hence enabling autocompletion and other IDE functionality
+
+
```

### Comparing `dexpr-0.0.5/README.md` & `dexpr-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -74,22 +74,48 @@
     shipping_time: Tenor
     expected_delivery_date: date = lambda self: self.order_date + self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
-adding Op expressoins:
+adding Op expressions:
 
 ```python
 Self = ParameterOp(_name='Self')
 
 @dataclassex
 class OrderWithOp:
+    Self: 'OrderWithOp'
+    
     order_date: date
     shipping_time: Tenor
     expected_delivery_date: date = Self.order_date + Self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
+Note the `Self` member - it is there for enable autocomplete in the IDE when writing the expressions and is removed from
+processed annotations
+
+There are two other variants of syntax supported for declaring dataclasses with support for Ops and lambdas:
+
+```python
+@dataclass
+@exprclass
+class OrderWithOp:
+    ...
+```
+
+And
+
+```python
+@dataclass
+class OrderWithOp(ExprClass):
+    ...
+```
+
+They exist for cases when the developer wants to keep the @dataclass annotations as is 
+to use PyCharm's built in support for it hence enabling autocompletion and other IDE functionality
+
+
```

### Comparing `dexpr-0.0.5/dexpr/calendar.py` & `dexpr-0.0.6/dexpr/calendar.py`

 * *Files identical despite different names*

### Comparing `dexpr-0.0.5/dexpr/dataclassex.py` & `dexpr-0.0.6/dexpr/exprclass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import abstractmethod
 from dataclasses import dataclass
+from datetime import date
 from inspect import isfunction, signature
 
-from dexpr.magic import calc, Op
+from dexpr import make_date, is_dgen
+from dexpr.magic import calc, Op, Expression, is_op
 
-
-__all__ = ("dataclassex", 'DataclassEx')
+__all__ = ("dataclassex", 'exprclass', 'ExprClass')
 
 
 class _BaseExDescriptor:
     def __init__(self, expr):
         self.expr = expr
 
     def __get__(self, instance, owner = None):
@@ -34,42 +35,72 @@
                 raise AttributeError(f'field {self.name} in {instance} is readonly')
 
     def __set_name__(self, owner, name):
         self.name = name
         self.cache_name = f'__cache_{self.name or id(self)}__'
 
 
-class OpDescriptor(_BaseExDescriptor):
+class CallableDescriptor(_BaseExDescriptor):
     def __calc__(self, instance):
-        return calc(self.expr, instance)
+        return self.expr(instance)
+
 
-class LambdaDescriptor(_BaseExDescriptor):
+class DateDescriptor(_BaseExDescriptor):
     def __calc__(self, instance):
-        return self.expr(instance)
+        r = self.expr(instance)
+        if isinstance(r, date):
+            return r
+        elif is_dgen(r):
+            return next(r())
+        else:
+            return make_date(r)
+
+
+class DateListDescriptor(_BaseExDescriptor):
+    def __calc__(self, instance):
+        r = self.expr(instance)
+        if isinstance(r, date):
+            return [r]
+        elif is_dgen(r):
+            return tuple(r())
+        else:
+            return make_date(r)
 
 
 def _process_ops_and_lambdas(cls):
     cls.__annotations__.pop('Self', None)
 
     for k, a in cls.__annotations__.items():
         if (op := getattr(cls, k, None)) is not None:
-            if isinstance(op, Op) and not issubclass(a, Op):
-                descriptor = OpDescriptor(op)
+
+            if a == date:  # special treatment for dates
+                descriptor_type = DateDescriptor
+            elif a == list[date] or a == tuple[date]:
+                descriptor_type = DateListDescriptor
+            else:
+                descriptor_type = CallableDescriptor
+
+            if isinstance(op, Op) and not is_op(a):
+                descriptor = descriptor_type(Expression(op))
                 descriptor.__set_name__(cls, k)
                 setattr(cls, k, descriptor)
             elif isfunction(op) and op.__name__ == '<lambda>':
                 if len(signature(op).parameters) == 1:
-                    descriptor = LambdaDescriptor(op)
+                    descriptor = descriptor_type(op)
                     descriptor.__set_name__(cls, k)
                     setattr(cls, k, descriptor)
 
     return cls
 
 
-class DataclassEx:
+class ExprClass:
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         _process_ops_and_lambdas(cls)
 
 
 def dataclassex(cls):
     return dataclass(_process_ops_and_lambdas(cls))
+
+
+def exprclass(cls):
+    return _process_ops_and_lambdas(cls)
```

### Comparing `dexpr-0.0.5/dexpr/dgen.py` & `dexpr-0.0.6/dexpr/dgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, timedelta
 from itertools import islice
 from typing import cast
 
 from dexpr.calendar import Calendar
-from dexpr.magic import Item
+from dexpr.magic import Item, const, Op
 from dexpr.tenor import Tenor
 
 __all__ = ('is_dgen', 'make_date', 'make_dgen', 'years', 'months', 'weeks', 'weekdays', 'weekends', 'days',
            'business_days', 'roll_fwd', 'roll_bwd')
 
 
 def is_dgen(obj):
@@ -42,15 +42,15 @@
         or item.stop is not None and item.stop < 0 \
         or item.step is not None and item.step < 0
 
 
 class DGen(Item):
     def __call__(self, input_date=None, start: date = date.min, end: date = date.max, after: date = date.min,
                  before: date = date.max, calendar: Calendar = None):
-        return self.__invoke__(start, end, after, before, calendar)
+        return self.__invoke__(make_date(start), make_date(end), make_date(after), make_date(before), calendar)
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
                    calendar: Calendar = None):
         raise StopIteration
 
     def is_single_date_gen(self):
         return False
@@ -83,14 +83,16 @@
 
     def __lt__(self, other):
         if is_dgen(other) and self.is_single_date_gen():
             return other.__ge__(self)
         else:
             if lhs := getattr(self, '__compared__', None):
                 return BeforeDGen(lhs, make_date(other))
+            if self.__expression__ is not None:
+                return self.__expression__ < other
             return BeforeDGen(self, make_date(other))
 
     def __ge__(self, other):
         if not is_dgen(other):
             return AfterOrOnDGen(self, make_date(other))
         elif other.is_single_date_gen():
             return AfterOrOnDGen(self, other)
@@ -99,14 +101,16 @@
 
     def __le__(self, other):
         if is_dgen(other) and self.is_single_date_gen():
             return other.__gt__(self)
         else:
             if lhs := getattr(self, '__compared__', None):
                 return BeforeOrOnDGen(lhs, make_date(other))
+            if self.__expression__ is not None:
+                return self.__expression__ <= other
             return BeforeOrOnDGen(self, make_date(other))
 
     def __add__(self, other):
         return AddTenorDGen(self, Tenor(other))
 
     def __sub__(self, other):
         try:
@@ -133,14 +137,16 @@
                 return SliceDGen(self, slice(item, item + 1))
             else:
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
         if isinstance(item, slice):
             if is_negative_slice(item):
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
             return SliceDGen(self, item)
+        if isinstance(item, Op):
+            return const(self)[item]
 
     def over(self, calendar: Calendar):
         return WithCalendarDGen(self, calendar)
 
 
 class ConstDGen(DGen):
     def __init__(self, date):
@@ -174,15 +180,17 @@
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
                    calendar: Calendar = None):
         if is_dgen(self.date):
             after = self.date(start, end, after, before, calendar)
         else:
             after = self.date
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d > after)
+        after = after + timedelta(days=1)
+
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d >= after)
 
     def __bool__(self):
         if is_dgen(self.date):
             self.date.__compared__ = self
         self.gen.__compared__ = self
         return True
 
@@ -240,15 +248,17 @@
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
                    calendar: Calendar = None):
         if is_dgen(self.date):
             before = self.date(start, end, after, before, calendar)
         else:
             before = self.date
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d <= before)
+        before = before + timedelta(days=1)
+
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d < before)
 
 
 class EveryDayDGen(DGen):
     def cadence(self):
         return Tenor('1d')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
@@ -579,26 +589,28 @@
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
                    calendar: Calendar = None):
         for begin in self.main_sequence.__invoke__(start, end, after, before, calendar):
             end = self.main_sequence.cadence().add_to(begin)
             sub_sequence = cast(DGen, begin <= self.sub_sequence < end)
             if self.slice is None:
-                yield from sub_sequence()
+                yield from (d for d in sub_sequence() if d < before)
             else:
                 if is_negative_slice(self.slice):
-                    yield from [d for d in sub_sequence()][self.slice]
+                    yield from [d for d in sub_sequence() if d < before][self.slice]
                 else:
-                    yield from islice(sub_sequence(), self.slice.start, self.slice.stop, self.slice.step)
+                    yield from (d for d in islice(sub_sequence(), self.slice.start, self.slice.stop, self.slice.step) if d < before)
 
     def __getitem__(self, item):
         if isinstance(item, int):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, slice(item, item + 1))
         if isinstance(item, slice):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, item)
+        if isinstance(item, Op):
+            return const(self)[item]
 
 class DaysOfMonthDGen(DGen):
     def __init__(self, months, days):
         self.months = months
         self.days = days
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
```

### Comparing `dexpr-0.0.5/dexpr/magic.py` & `dexpr-0.0.6/dexpr/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         obj = self._obj.__invoke__(*args, **kwargs)
         if isinstance(obj, FailedOp):
             return obj
 
         lhs = self._lhs.__invoke__(*args, **kwargs, **{self._parameter._name: obj})
         if isinstance(lhs, FailedOp):
             return lhs
-        if lhs is False:
+        if bool(lhs) is False:
             return lhs
 
         return self._rhs.__invoke__(*args, **kwargs, **{self._parameter._name: obj})
 
     def __repr__(self):
         lhs = repr(self._lhs if self._lhs._rhs is self._parameter else self._lhs.__reverse__())
         rhs = repr(self._rhs if self._rhs._lhs is self._parameter else self._rhs.__reverse__())
```

### Comparing `dexpr-0.0.5/dexpr/tenor.py` & `dexpr-0.0.6/dexpr/tenor.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
     def is_neg(self):
         return sum(self.ymwd_b) < 0
 
     def __neg__(self):
         return Tenor(tuple(-i for i in self.ymwd_b))
 
+    def __radd__(self, other):
+        if isinstance(other, date):
+            return self.add_to(other)
+        else:
+            return other.__add__(self)
+
     def add_to(self, dt, calendar = None):
         if self.is_neg():
             return self.__neg__().sub_from(dt, calendar)
 
         if self.ymwd_b[-1] == 0: # not a business days tenor
             y, m, w, d, _ = self.ymwd_b
             year, month, day = dt.year, dt.month, dt.day
```

### Comparing `dexpr-0.0.5/dexpr.egg-info/PKG-INFO` & `dexpr-0.0.6/dexpr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexpr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Libraries for capturing and using expressions in python
 Author-email: wukrur <wukrur@github.com>
 License: MIT
 Keywords: expressions,date generators,extended dataclass
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -87,22 +87,48 @@
     shipping_time: Tenor
     expected_delivery_date: date = lambda self: self.order_date + self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
-adding Op expressoins:
+adding Op expressions:
 
 ```python
 Self = ParameterOp(_name='Self')
 
 @dataclassex
 class OrderWithOp:
+    Self: 'OrderWithOp'
+    
     order_date: date
     shipping_time: Tenor
     expected_delivery_date: date = Self.order_date + Self.shipping_time
 
 o = OrderWithLambda(order_date=make_date('2020-02-02'), shipping_time=Tenor('3d'))
 assert o.expected_delivery_date == make_date('2020-02-05')
 ```
 
+Note the `Self` member - it is there for enable autocomplete in the IDE when writing the expressions and is removed from
+processed annotations
+
+There are two other variants of syntax supported for declaring dataclasses with support for Ops and lambdas:
+
+```python
+@dataclass
+@exprclass
+class OrderWithOp:
+    ...
+```
+
+And
+
+```python
+@dataclass
+class OrderWithOp(ExprClass):
+    ...
+```
+
+They exist for cases when the developer wants to keep the @dataclass annotations as is 
+to use PyCharm's built in support for it hence enabling autocompletion and other IDE functionality
+
+
```

### Comparing `dexpr-0.0.5/pyproject.toml` & `dexpr-0.0.6/pyproject.toml`

 * *Files identical despite different names*

