# Comparing `tmp/sqlfactory-1.0.1.tar.gz` & `tmp/sqlfactory-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfactory-1.0.1.tar", max compression
+gzip compressed data, was "sqlfactory-1.0.2.tar", max compression
```

## Comparing `sqlfactory-1.0.1.tar` & `sqlfactory-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1069 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/LICENSE
--rw-r--r--   0        0        0     7889 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/README.md
--rw-r--r--   0        0        0     1293 2024-04-02 08:21:29.563271 sqlfactory-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/__init__.py
--rw-r--r--   0        0        0      324 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/__init__.py
--rw-r--r--   0        0        0     5049 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/base.py
--rw-r--r--   0        0        0     1787 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/between.py
--rw-r--r--   0        0        0     4920 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/in_condition.py
--rw-r--r--   0        0        0     1274 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/like.py
--rw-r--r--   0        0        0     5510 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/condition/simple.py
--rw-r--r--   0        0        0       68 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/delete/__init__.py
--rw-r--r--   0        0        0     1951 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/delete/delete.py
--rw-r--r--   0        0        0     7691 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/entities.py
--rw-r--r--   0        0        0     7543 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/execute.py
--rw-r--r--   0        0        0        0 2024-04-02 08:21:28.687281 sqlfactory-1.0.1/sqlfactory/func/__init__.py
--rw-r--r--   0        0        0     2148 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/agg.py
--rw-r--r--   0        0        0      987 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/base.py
--rw-r--r--   0        0        0      979 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/control.py
--rw-r--r--   0        0        0    15497 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/datetime.py
--rw-r--r--   0        0        0     4359 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/enc.py
--rw-r--r--   0        0        0     4726 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/info.py
--rw-r--r--   0        0        0     4601 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/misc.py
--rw-r--r--   0        0        0     7156 2024-04-02 08:21:28.659282 sqlfactory-1.0.1/sqlfactory/func/numeric.py
--rw-r--r--   0        0        0     7741 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/func/str.py
--rw-r--r--   0        0        0       95 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/insert/__init__.py
--rw-r--r--   0        0        0     6349 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/insert/insert.py
--rw-r--r--   0        0        0      601 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/insert/values.py
--rw-r--r--   0        0        0      115 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/logger.py
--rw-r--r--   0        0        0      271 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/mixins/__init__.py
--rw-r--r--   0        0        0     3822 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/mixins/limit.py
--rw-r--r--   0        0        0     2498 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/mixins/order.py
--rw-r--r--   0        0        0      824 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/mixins/where.py
--rw-r--r--   0        0        0      244 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/select/__init__.py
--rw-r--r--   0        0        0     1200 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/select/aliased.py
--rw-r--r--   0        0        0     2119 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/select/column_list.py
--rw-r--r--   0        0        0     1846 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/select/join.py
--rw-r--r--   0        0        0     7224 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/select/select.py
--rw-r--r--   0        0        0     3861 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/statement.py
--rw-r--r--   0        0        0       68 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/update/__init__.py
--rw-r--r--   0        0        0     4858 2024-04-02 08:21:28.663282 sqlfactory-1.0.1/sqlfactory/update/update.py
--rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/LICENSE
+-rw-r--r--   0        0        0     7889 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/README.md
+-rw-r--r--   0        0        0     1293 2024-04-10 11:43:13.914416 sqlfactory-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/__init__.py
+-rw-r--r--   0        0        0     5049 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/base.py
+-rw-r--r--   0        0        0     1787 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/between.py
+-rw-r--r--   0        0        0     4920 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/in_condition.py
+-rw-r--r--   0        0        0     1274 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/like.py
+-rw-r--r--   0        0        0     5510 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/condition/simple.py
+-rw-r--r--   0        0        0       68 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/delete/__init__.py
+-rw-r--r--   0        0        0     1951 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/delete/delete.py
+-rw-r--r--   0        0        0     7691 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/entities.py
+-rw-r--r--   0        0        0     7543 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/execute.py
+-rw-r--r--   0        0        0        0 2024-04-10 11:43:13.082426 sqlfactory-1.0.2/sqlfactory/func/__init__.py
+-rw-r--r--   0        0        0     2148 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/agg.py
+-rw-r--r--   0        0        0      987 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/base.py
+-rw-r--r--   0        0        0      979 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/control.py
+-rw-r--r--   0        0        0    15497 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/datetime.py
+-rw-r--r--   0        0        0     4359 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/enc.py
+-rw-r--r--   0        0        0     4726 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/info.py
+-rw-r--r--   0        0        0     4601 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/misc.py
+-rw-r--r--   0        0        0     7156 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/numeric.py
+-rw-r--r--   0        0        0     7741 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/func/str.py
+-rw-r--r--   0        0        0       95 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/insert/__init__.py
+-rw-r--r--   0        0        0     6349 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/insert/insert.py
+-rw-r--r--   0        0        0      601 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/insert/values.py
+-rw-r--r--   0        0        0      115 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/logger.py
+-rw-r--r--   0        0        0      271 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/mixins/__init__.py
+-rw-r--r--   0        0        0     3822 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/mixins/limit.py
+-rw-r--r--   0        0        0     2498 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/mixins/order.py
+-rw-r--r--   0        0        0      824 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/mixins/where.py
+-rw-r--r--   0        0        0      244 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/select/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/select/aliased.py
+-rw-r--r--   0        0        0     2119 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/select/column_list.py
+-rw-r--r--   0        0        0     1846 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/select/join.py
+-rw-r--r--   0        0        0     7224 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/select/select.py
+-rw-r--r--   0        0        0     3861 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/statement.py
+-rw-r--r--   0        0        0       68 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/update/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-10 11:43:13.054427 sqlfactory-1.0.2/sqlfactory/update/update.py
+-rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.0.2/PKG-INFO
```

### Comparing `sqlfactory-1.0.1/LICENSE` & `sqlfactory-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/README.md` & `sqlfactory-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/pyproject.toml` & `sqlfactory-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlfactory"
-version = "v1.0.1"
+version = "v1.0.2"
 description = "Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible."
 authors = ["Michal Kuchta <niximor@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlfactory"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `sqlfactory-1.0.1/sqlfactory/condition/base.py` & `sqlfactory-1.0.2/sqlfactory/condition/base.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/condition/between.py` & `sqlfactory-1.0.2/sqlfactory/condition/between.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/condition/in_condition.py` & `sqlfactory-1.0.2/sqlfactory/condition/in_condition.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/condition/like.py` & `sqlfactory-1.0.2/sqlfactory/condition/like.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/condition/simple.py` & `sqlfactory-1.0.2/sqlfactory/condition/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/delete/delete.py` & `sqlfactory-1.0.2/sqlfactory/delete/delete.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/entities.py` & `sqlfactory-1.0.2/sqlfactory/entities.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/execute.py` & `sqlfactory-1.0.2/sqlfactory/execute.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/agg.py` & `sqlfactory-1.0.2/sqlfactory/func/agg.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/base.py` & `sqlfactory-1.0.2/sqlfactory/func/base.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/control.py` & `sqlfactory-1.0.2/sqlfactory/func/control.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/datetime.py` & `sqlfactory-1.0.2/sqlfactory/func/datetime.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/enc.py` & `sqlfactory-1.0.2/sqlfactory/func/enc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/info.py` & `sqlfactory-1.0.2/sqlfactory/func/info.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/misc.py` & `sqlfactory-1.0.2/sqlfactory/func/misc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/numeric.py` & `sqlfactory-1.0.2/sqlfactory/func/numeric.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/func/str.py` & `sqlfactory-1.0.2/sqlfactory/func/str.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/insert/insert.py` & `sqlfactory-1.0.2/sqlfactory/insert/insert.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/insert/values.py` & `sqlfactory-1.0.2/sqlfactory/insert/values.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/mixins/limit.py` & `sqlfactory-1.0.2/sqlfactory/mixins/limit.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/mixins/order.py` & `sqlfactory-1.0.2/sqlfactory/mixins/order.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/mixins/where.py` & `sqlfactory-1.0.2/sqlfactory/mixins/where.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/select/aliased.py` & `sqlfactory-1.0.2/sqlfactory/select/aliased.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/select/column_list.py` & `sqlfactory-1.0.2/sqlfactory/select/column_list.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/select/join.py` & `sqlfactory-1.0.2/sqlfactory/select/join.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/select/select.py` & `sqlfactory-1.0.2/sqlfactory/select/select.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/statement.py` & `sqlfactory-1.0.2/sqlfactory/statement.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.1/sqlfactory/update/update.py` & `sqlfactory-1.0.2/sqlfactory/update/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """UPDATE statement builder."""
 
 from __future__ import annotations
+
 from typing import Any, Optional
 
+from ..condition.base import ConditionBase
 from ..entities import ColumnArg, Column, Table
 from ..execute import ExecutableStatementWithArgs, ConditionalExecutableStatement
 from ..mixins.limit import WithLimit, Limit
 from ..mixins.where import WithWhere
 from ..statement import StatementWithArgs, Statement
-from ..condition.base import Condition
 
 
 class UpdateColumn(StatementWithArgs):
     """
     Represents one field that should be updated.
     """
     def __init__(self, column: ColumnArg, value: Statement | Any):
@@ -59,15 +60,15 @@
     >>> t = Table("table")
     >>> Update(t).set(t.column1, 1).where(t.column2 == 2)
     """
     def __init__(
             self,
             table: Table | str,
             *fields: UpdateColumn,
-            where: Optional[Condition] = None,
+            where: Optional[ConditionBase] = None,
             limit: Optional[Limit] = None
     ):
         """
         :param table: Table to update.
         :param fields: List of UpdateColumn instances containing columns to be updated. This is not very pleasant way
             to create the statement, use set() method instead.
         :param where: WHERE condition
```

### Comparing `sqlfactory-1.0.1/PKG-INFO` & `sqlfactory-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfactory
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible.
 Author: Michal Kuchta
 Author-email: niximor@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

