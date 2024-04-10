# Comparing `tmp/GeneralSQL-1.2.0.tar.gz` & `tmp/GeneralSQL-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeneralSQL-1.2.0.tar", last modified: Wed Mar 13 05:17:07 2024, max compression
+gzip compressed data, was "GeneralSQL-1.3.0.tar", last modified: Wed Apr 10 10:06:08 2024, max compression
```

## Comparing `GeneralSQL-1.2.0.tar` & `GeneralSQL-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/GeneralSQL/
--rw-r--r--   0 joker     (1000) joker     (1000)     2321 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/Error.py
--rw-r--r--   0 joker     (1000) joker     (1000)    35149 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/LICENSE
--rw-r--r--   0 joker     (1000) joker     (1000)     1368 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/README.md
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/GeneralSQL/Template/
--rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/Template/__init__.py
--rw-r--r--   0 joker     (1000) joker     (1000)     3024 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/Template/base.py
--rw-r--r--   0 joker     (1000) joker     (1000)     2119 2024-03-13 05:09:42.000000 GeneralSQL-1.2.0/GeneralSQL/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/GeneralSQL/db/
--rw-r--r--   0 joker     (1000) joker     (1000)    16057 2024-03-13 05:10:00.000000 GeneralSQL-1.2.0/GeneralSQL/db/Jmysql.py
--rw-r--r--   0 joker     (1000) joker     (1000)       57 2023-11-19 09:55:51.000000 GeneralSQL-1.2.0/GeneralSQL/db/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/GeneralSQL.egg-info/
--rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-03-13 05:17:06.000000 GeneralSQL-1.2.0/GeneralSQL.egg-info/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      347 2024-03-13 05:17:06.000000 GeneralSQL-1.2.0/GeneralSQL.egg-info/SOURCES.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2024-03-13 05:17:06.000000 GeneralSQL-1.2.0/GeneralSQL.egg-info/dependency_links.txt
--rw-r--r--   0 joker     (1000) joker     (1000)       11 2024-03-13 05:17:06.000000 GeneralSQL-1.2.0/GeneralSQL.egg-info/top_level.txt
--rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/PKG-INFO
--rwxrwxrwx   0 joker     (1000) joker     (1000)      717 2023-12-25 09:51:11.000000 GeneralSQL-1.2.0/pyproject.toml
--rw-r--r--   0 joker     (1000) joker     (1000)       38 2024-03-13 05:17:06.998255 GeneralSQL-1.2.0/setup.cfg
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.117930 GeneralSQL-1.3.0/GeneralSQL/
+-rw-r--r--   0 joker     (1000) joker     (1000)     2321 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/Error.py
+-rw-r--r--   0 joker     (1000) joker     (1000)    35149 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/LICENSE
+-rw-r--r--   0 joker     (1000) joker     (1000)     1368 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/README.md
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL/Template/
+-rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/Template/__init__.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2994 2024-04-10 09:59:53.000000 GeneralSQL-1.3.0/GeneralSQL/Template/base.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2119 2024-04-10 09:50:57.000000 GeneralSQL-1.3.0/GeneralSQL/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL/db/
+-rw-r--r--   0 joker     (1000) joker     (1000)    16294 2024-04-10 10:04:52.000000 GeneralSQL-1.3.0/GeneralSQL/db/Jmysql.py
+-rw-r--r--   0 joker     (1000) joker     (1000)       57 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/db/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL.egg-info/
+-rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)      347 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)        1 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)       11 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/top_level.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/PKG-INFO
+-rwxrwxrwx   0 joker     (1000) joker     (1000)      717 2023-12-25 09:51:11.000000 GeneralSQL-1.3.0/pyproject.toml
+-rw-r--r--   0 joker     (1000) joker     (1000)       38 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/setup.cfg
```

### Comparing `GeneralSQL-1.2.0/GeneralSQL/Error.py` & `GeneralSQL-1.3.0/GeneralSQL/Error.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.2.0/GeneralSQL/LICENSE` & `GeneralSQL-1.3.0/GeneralSQL/LICENSE`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.2.0/GeneralSQL/README.md` & `GeneralSQL-1.3.0/GeneralSQL/README.md`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.2.0/GeneralSQL/Template/__init__.py` & `GeneralSQL-1.3.0/GeneralSQL/Template/__init__.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.2.0/GeneralSQL/Template/base.py` & `GeneralSQL-1.3.0/GeneralSQL/Template/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return res
 
 def filter_format(func, check: str, **kwargs) -> str:
     # template 't'
     # 变量对照检查
     t = '{_logic} {_not} {_t_as:.}`{field}` {symbl} {value}'
     print(t)
-    return 
+    return
 
 """
 基本 模型
 
 DB 数据库管理
 
 Sql 基本 sql 方法对象
@@ -65,41 +65,41 @@
 
 
 class Sql:
     """Sql 数据类型
     """
 
     def __init__(self):
-        # type: query/ affairs
+        # query | affairs
         self.__type = None
         self.__value = None
 
     def get_sql(self):
         return self.__value
-    
+
     def set_sql(self, v):
         self.__value = v
-    
+
     def get_type(self):
         return self.__type
-    
+
     def set_type(self, t):
         self.__type = t
 
 
 class Tab:
 
     def __init__(self):
         self.table = None
 
     def set_where(self):
         # check 当对象没有该属性无法使用方法
         if not hasattr(self, 'where'):
             raise Error.UseError(200001)
-    
+
     def get_where(self):
         # check 当对象没有该属性无法获取
         if not hasattr(self, 'where'):
             raise Error.UseError(200002)
 
 class Insert(Tab):
 
@@ -111,25 +111,25 @@
         self.data = None
 
 class Delete(Tab):
 
     def __init__(self):
         Tab.__init__(self)
         self.where = None
-    
+
     def get_where(self):
         Tab.get_where(self)
         return self.where
 
 class Update(Tab):
 
     def __init__(self):
         Tab.__init__(self)
         self.where = None
-    
+
     def get_where(self):
         Tab.get_where(self)
         return self.where
 
 class Select(Tab):
 
     def __init__(self):
```

### Comparing `GeneralSQL-1.2.0/GeneralSQL/__init__.py` & `GeneralSQL-1.3.0/GeneralSQL/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import functools
 from . import db
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 
 __cls__ = db.__all__
 
 
 def SeniorDB(t):
     if t in __cls__:
         __db = getattr(db, t).DB
```

### Comparing `GeneralSQL-1.2.0/GeneralSQL/db/Jmysql.py` & `GeneralSQL-1.3.0/GeneralSQL/db/Jmysql.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,61 +38,86 @@
         res = [f'`{i}`' for i in list(field)]
     else:
         raise Error.ParamsError(400001)
     return res
 
 def _filter_format(filter_data:dict) -> str:
     # 检查
-    if set(filter_data.keys()) >= set(['symbol', 'field', 'value']):
-        # check symbol
-        field, val = f"{filter_data.get('field')}", filter_data.get('value')
-        symbol = filter_data.get('symbol')
-
-        symbol_list = ['=', '<=', '>=', '!=', '<>', '<', '>', 'IN', 'LIKE', 'BETWEEN', 'ISNULL']
-        if symbol.upper() in symbol_list:
-            result = ''
-            # 表 as 名称替换 field
-            if filter_data.get('table_as'):
-                field = f"{filter_data.get('table_as')}.{field}"
-            # symbol 格式化
-            if symbol.upper() == 'IN':
-                if filter_data.get('not'):
-                    symbol = 'NOT IN'
-                result = f"{field} {symbol} ({','.join([repr(str(i)) for i in val])})"
-            elif symbol.upper() == 'LIKE':
-                if filter_data.get('not'):
-                    symbol = 'NOT LIKE'
-                result = f"{field} {symbol} {repr(f'{str(val)}')}"
-            elif symbol.upper() == 'ISNULL':
-                symbol = 'IS NULL'
-                if filter_data.get('not'):
-                    symbol = 'IS NOT NULL'
-                result = f'{field} {symbol}'
-            elif symbol.upper() == 'BETWEEN':
-                if filter_data.get('not'):
-                    symbol = 'NOT BETWEEN'
-                result = f'{field} {symbol} {repr(val.get("start"))} AND {repr(val.get("end"))}'
-                if filter_data.get('not'):
-                    symbol = 'NOT BETWEEN'
-                result = f'{field} {symbol} {repr(val.get("start"))} AND {repr(val.get("end"))}'
-            else:
-                result = f'{field} {symbol} {repr(val)}'
-                if filter_data.get('not'):
-                    result = f'NOT {result}'
-            # 关系
-            if factor := filter_data.get('factor'):
-                if factor.upper() in ['AND', 'OR']:
-                    result = f'{factor.upper()} {result}'
-                else:
-                    raise Error.ParamsError(400004)
-            return result
+    if not set(filter_data.keys()) >= set(['symbol', 'field', 'value']): raise Error.ParamsError(400003, 'Params miss in [symbol, field, value]')
+
+    symbol_list = ['=', '<=', '>=', '!=', '<>', '<', '>', 'IN', 'LIKE', 'BETWEEN', 'ISNULL']
+    result = ''
+    factor_list = ['AND', 'OR', 'NOT']
+    # check symbol
+    symbol, field, val = str(filter_data.get('symbol')).upper(), f"{filter_data.get('field')}", filter_data.get('value')
+
+    # 条件逻辑处理
+    symbol:str = filter_data.get('symbol').upper()
+    if symbol == None: raise Error.ParamsError(400003, 'Params miss in [symbol, field, value]')
+    if symbol not in symbol_list: raise Error.ParamsError(400004)
+    symbol = symbol.upper()
+    # 关系逻辑处理
+    # factor = filter_data.get('factor', None)
+    # if factor and factor.upper() not in factor_list: raise Error.ParamsError(400004)
+    # if factor:
+    #     factor = factor.upper()
+    #     result += factor
+    # 表 as 名称替换 field
+    if filter_data.get('table_as'):
+        field = f"{filter_data.get('table_as')}.{repr(field)}"
+
+
+    # 自定义 value 处理
+    if filter_data.get('val_format'):
+        val = filter_data.get('val_format')(val)
+    else:
+        # 默认 value 处理
+        if isinstance(val, (dict)) and val.get('start') and val.get('end'):
+            val = f'{repr(val.get("start"))} AND {repr(val.get("end"))}'
+        elif isinstance(val, (tuple, list)) and symbol == 'IN':
+            val = ','.join([repr(str(i)) for i in val])
         else:
-            raise Error.ParamsError(400004)
+            val = repr(val)
+
+    if symbol == 'ISNULL':
+        return f'{result} {symbol}({field})'
     else:
-        raise Error.ParamsError(400003, 'Params miss in [symbol, field, value]')
+        return f'{result} {field} {symbol} ({val})'
+
+class SqlWhere:
+
+    def __init__(self):
+        self.where = None
+
+    # 设置条件
+    def set_where(self, *filters):
+        self.where = []
+        if len(filters) < 1: raise Error.ParamsError(400002)
+        factor_list = ['AND', 'OR', 'NOT']
+        filters = list(filter(lambda x: isinstance(x, dict), filters))
+        if isinstance(filters[0], dict) and filters[0].get('factor'):
+            filters[0].pop('factor')
+
+        gl_index = []
+        for i, v in enumerate(filters):
+            if v.get('val_factor') and i > 0:
+                self.where[i - 1] += f' {v.get("val_factor")}{_filter_format(v)}'
+                continue
+            gl_index.append(i)
+            self.where.append(_filter_format(v))
+        for i, v in enumerate(self.where):
+            if gl_index[i]:
+                if filters[gl_index[i]].get('factor', '').upper() in factor_list:
+                    tmp_factor = str(filters[gl_index[i]].get('factor', '')).upper()
+                    self.where[i] = f'{tmp_factor} ({v})'
+                else:
+                    raise Error.ParamsError(400003, 'factor not in ["AND", "OR", "NOT"]')
+            else:
+                self.where[i] = f'({v})'
+        self.where = f'WHERE {" ".join(self.where)}'
 
 class DB(TDB):
 
     def __init__(self):
         TDB.__init__(self)
         self.db_type = 'mysql'
         self.db_info = {
@@ -225,93 +250,77 @@
             if self.update:
                 # 重复更新
                 res.append(f"{self.__base[0]} {self.table} ({field}) {self.__base[1]} {','.join(tmp)} {self.__base[2]} {','.join(format_update)}")
             else:
                 res.append(f"{self.__base[0]} {self.table} ({field}) {self.__base[1]} {','.join(tmp)}")
         self.set_sql(res)
 
-class Update(TUpdate):
+class Update(TUpdate, SqlWhere):
 
     def __init__(self, table, data):
         TUpdate.__init__(self, table, data)
+        SqlWhere.__init__(self)
         self.__base = ['UPDATE', 'SET']
 
     def data_decode(self):
         if hasattr(self, 'data'):
             if isinstance(self.data, dict):
                 self.value = [f'`{k}` = {v}' for k, v in self.data.items()]
             else:
                 raise Error.ParamsError(400001)
         else:
             raise Error.UseError(200002)
 
     def set_where(self, *filters):
-        if len(filters) > 0:
-            self.where = []
-            for i in filters:
-                self.where.append(_filter_format(i))
-            self.where = f'WHERE {" ".join(self.where)}'
-        else:
-            raise Error.ParamsError(400002)
+        return SqlWhere.set_where(self, *filters)
 
     def format_sql(self):
         self.data_decode()
         str_data = ','.join(self.value)
         sql = f'{self.__base[0]} {self.table} {self.__base[1]} {str_data}'
         if self.where:
             sql = f'{sql} {self.where}'
         self.set_sql(sql)
 
-class Delete(TDelete):
+class Delete(TDelete, SqlWhere):
 
     def __init__(self, table):
         TDelete.__init__(self, table)
+        SqlWhere.__init__(self)
         self.__base = ['DELETE FROM']
 
     def set_where(self, *filters):
-        if len(filters) > 0:
-            self.where = []
-            for i in filters:
-                self.where.append(_filter_format(i))
-            self.where = f'WHERE {" ".join(self.where)}'
-        else:
-            raise Error.ParamsError(400002)
+        return SqlWhere.set_where(self, *filters)
 
     def format_sql(self):
         sql = f'{self.__base[0]} {self.table}'
         if self.where:
             sql = f'{sql} {self.where}'
         self.set_sql(sql)
 
-class Select(TSelect):
+class Select(TSelect, SqlWhere):
 
     def __init__(self, **kwargs):
         TSelect.__init__(self, **kwargs)
+        SqlWhere.__init__(self)
         self.__base = ['SELECT', 'FROM']
         if kwargs.get('fields'):
             if isinstance(kwargs.get('fields'), (list, tuple, dict)):
                 self.fields = _format_field(kwargs.get('fields'))
         else:
             self.fields = '*'
 
     def set_fields(self, *fields):
         if len(fields) < 1:
             raise Error.ParamsError(400002)
         for i in fields:
             self.fields = _format_field(i)
 
-    # 设置条件
     def set_where(self, *filters):
-        if len(filters) > 0:
-            self.where = []
-            for i in filters:
-                self.where.append(_filter_format(i))
-            self.where = f'WHERE {" ".join(self.where)}'
-        else:
-            raise Error.ParamsError(400002)
+        return SqlWhere.set_where(self, *filters)
 
     # 设置分组
     def set_group(self, *fields):
         '''
         Set up groups
             *fields: table field
                 [field] or [table]__[field]
```

### Comparing `GeneralSQL-1.2.0/GeneralSQL.egg-info/PKG-INFO` & `GeneralSQL-1.3.0/GeneralSQL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeneralSQL
-Version: 1.2.0
+Version: 1.3.0
 Summary: Sql generator tool.
 Author-email: joker-zzp <joker_zzp@qq.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `GeneralSQL-1.2.0/PKG-INFO` & `GeneralSQL-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeneralSQL
-Version: 1.2.0
+Version: 1.3.0
 Summary: Sql generator tool.
 Author-email: joker-zzp <joker_zzp@qq.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `GeneralSQL-1.2.0/pyproject.toml` & `GeneralSQL-1.3.0/pyproject.toml`

 * *Files identical despite different names*

