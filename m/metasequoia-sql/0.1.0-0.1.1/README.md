# Comparing `tmp/metasequoia-sql-0.1.0.tar.gz` & `tmp/metasequoia-sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.1.0.tar", last modified: Sun Apr  7 00:15:14 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.1.1.tar", last modified: Tue Apr  9 23:19:48 2024, max compression
```

## Comparing `metasequoia-sql-0.1.0.tar` & `metasequoia-sql-0.1.1.tar`

### file list

```diff
@@ -1,59 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.623823 metasequoia-sql-0.1.0/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5756 2024-04-07 00:15:14.622823 metasequoia-sql-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5087 2024-04-07 00:13:47.000000 metasequoia-sql-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.581827 metasequoia-sql-0.1.0/auto_test/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/auto_test/__init__.py
--rw-rw-rw-   0        0        0    96622 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/auto_test/sql_basic_tutorial.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.582827 metasequoia-sql-0.1.0/metasequoia_sql/
--rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.585827 metasequoia-sql-0.1.0/metasequoia_sql/ast/
--rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/__init__.py
--rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/functions.py
--rw-rw-rw-   0        0        0    17093 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/nodes.py
--rw-rw-rw-   0        0        0     8458 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.586827 metasequoia-sql-0.1.0/metasequoia_sql/common/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0     3089 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/text_scanner.py
--rw-rw-rw-   0        0        0     8206 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/token_scanner.py
--rw-rw-rw-   0        0        0      665 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.588827 metasequoia-sql-0.1.0/metasequoia_sql/objects/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/__init__.py
--rw-rw-rw-   0        0        0     8175 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/common.py
--rw-rw-rw-   0        0        0    53603 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/core.py
--rw-rw-rw-   0        0        0      114 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/data_source.py
--rw-rw-rw-   0        0        0     2927 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/hive.py
--rw-rw-rw-   0        0        0    10343 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/mysql.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.589827 metasequoia-sql-0.1.0/metasequoia_sql/parser/
--rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/__init__.py
--rw-rw-rw-   0        0        0    69957 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/common.py
--rw-rw-rw-   0        0        0    13123 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/mysql_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.590827 metasequoia-sql-0.1.0/metasequoia_sql/statements/
--rw-rw-rw-   0        0        0        0 2024-04-06 23:27:57.000000 metasequoia-sql-0.1.0/metasequoia_sql/statements/__init__.py
--rw-rw-rw-   0        0        0       45 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/statements/mysql.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.591827 metasequoia-sql-0.1.0/metasequoia_sql/static/
--rw-rw-rw-   0        0        0      183 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/common.py
--rw-rw-rw-   0        0        0     2571 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/mysql.py
--rw-rw-rw-   0        0        0     3824 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/other.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.619826 metasequoia-sql-0.1.0/metasequoia_sql/translate/
--rw-rw-rw-   0        0        0      101 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/__init__.py
--rw-rw-rw-   0        0        0     3399 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/from_mysql.py
--rw-rw-rw-   0        0        0     5343 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/full_statement.py
--rw-rw-rw-   0        0        0     1222 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/to_hive.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.622823 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     5756 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1392 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.620825 metasequoia-sql-0.1.0/scripts/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.621823 metasequoia-sql-0.1.0/scripts/demo/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/__init__.py
--rw-rw-rw-   0        0        0    67081 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/sql_basic_tutorial.py
--rw-rw-rw-   0        0        0     2024 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/with_demo.py
--rw-rw-rw-   0        0        0      278 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/temp_test.py
--rw-rw-rw-   0        0        0     4882 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/unittest_maker.py
--rw-rw-rw-   0        0        0       42 2024-04-07 00:15:14.623823 metasequoia-sql-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-04-07 00:14:06.000000 metasequoia-sql-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.397704 metasequoia-sql-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6183 2024-04-09 23:19:48.396703 metasequoia-sql-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5514 2024-04-09 23:19:02.000000 metasequoia-sql-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.385703 metasequoia-sql-0.1.1/metasequoia_sql/
+-rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.388703 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0        0 2024-04-09 23:10:25.000000 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-04-09 23:10:25.000000 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/consanguinity.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.390704 metasequoia-sql-0.1.1/metasequoia_sql/ast/
+-rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/__init__.py
+-rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/functions.py
+-rw-rw-rw-   0        0        0    17093 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/nodes.py
+-rw-rw-rw-   0        0        0     8463 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.392703 metasequoia-sql-0.1.1/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0        0 2024-04-09 23:06:06.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/base_scanner.py
+-rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      150 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/text_scanner.py
+-rw-rw-rw-   0        0        0     5712 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/token_scanner.py
+-rw-rw-rw-   0        0        0      665 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.392703 metasequoia-sql-0.1.1/metasequoia_sql/objects/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/objects/__init__.py
+-rw-rw-rw-   0        0        0    75855 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/objects/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.393704 metasequoia-sql-0.1.1/metasequoia_sql/parser/
+-rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/parser/__init__.py
+-rw-rw-rw-   0        0        0    83932 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/parser/common.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.395704 metasequoia-sql-0.1.1/metasequoia_sql/static/
+-rw-rw-rw-   0        0        0      183 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/common.py
+-rw-rw-rw-   0        0        0     2571 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/mysql.py
+-rw-rw-rw-   0        0        0     3824 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/other.py
+drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.396703 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     6183 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 23:19:48.397704 metasequoia-sql-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2024-04-09 23:17:20.000000 metasequoia-sql-0.1.1/setup.py
```

### Comparing `metasequoia-sql-0.1.0/LICENSE` & `metasequoia-sql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/PKG-INFO` & `metasequoia-sql-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: metasequoia-sql
-Version: 0.1.0
-Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
-Home-page: https://github.com/ChangxingJiang/metasequoia-sql
-Author: changxing
-Author-email: 1278729001@qq.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sql-tree：SQL 解析器
 
 ## 安装方法
 
 ```bash
 pip install metasequoia-sql
 ```
@@ -37,29 +19,30 @@
 ```
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
-from metasequoia_sql.parser.mysql_parser import parse_mysql_create_table_statement
+from metasequoia_sql.parser.common import parse_create_table_statement
+from metasequoia_sql.common.token_scanner import build_token_scanner
 
-statement = parse_mysql_create_table_statement("your sql")
+statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
-from metasequoia_sql.parser.mysql_parser import parse_mysql_create_table_statement
+from metasequoia_sql.parser.common import parse_create_table_statement
 from metasequoia_sql.translate import *
+from metasequoia_sql.common.token_scanner import build_token_scanner
 
-statement = ddl_create_table_statement_to_hive(
-    ddl_create_table_statement_from_mysql(parse_mysql_create_table_statement("your sql")))
+statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
@@ -127,15 +110,29 @@
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
 ## 修改记录
 
+#### 0.1.0 > 0.1.1
+
+新增：
+- `INSERT` 语句解析逻辑
+- 一次性解析多条 SQL 语句
+
+优化：
+- 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
+- 清理多余对象
+- TokenScanner 使用方法
+
+修复：
+- `WITH` 语句解析报错的 Bug 修复
+
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
 
-- 新增 CREATE TABLE 语句解析逻辑
+- 新增 CREATE TABLE 语句解析逻辑
```

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/ast/functions.py` & `metasequoia-sql-0.1.1/metasequoia_sql/ast/functions.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/ast/nodes.py` & `metasequoia-sql-0.1.1/metasequoia_sql/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/ast/parser.py` & `metasequoia-sql-0.1.1/metasequoia_sql/ast/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         状态机状态
     _cache : List[str]
         当前正在缓存的词语
     """
 
     def __init__(self, text: str):
         self._stack: List[List[AST]] = [[]]
-        self._scanner: TextScanner = TextScanner(text.replace("\r\n", "\n"))
+        self._scanner: TextScanner = TextScanner(list(text.replace("\r\n", "\n")))
         self._status: AstParseStatus = AstParseStatus.WAIT_TOKEN
         self._cache: List[str] = []
 
     # ------------------------------ 上下文管理器属性 ------------------------------
 
     @property
     def stack(self) -> List[List[AST]]:
@@ -69,15 +69,15 @@
     def now_ch(self) -> str:
         """当前指针位置的字符"""
         return self._scanner.now
 
     @property
     def next_ch(self) -> str:
         """当前指针位置的下一个字符"""
-        return self._scanner.next
+        return self._scanner.next1
 
     @property
     def is_finish(self) -> bool:
         """若当前上下文已匹配结束则返回 True，否则返回 False"""
         return self._scanner.is_finish
 
     # ------------------------------ 当前缓存词语的相关方法 ------------------------------
@@ -105,23 +105,23 @@
         self.cache_reset()
         return result
 
     # ------------------------------ 状态变化方法 ------------------------------
 
     def handle_left_parenthesis(self) -> None:
         """【移动指针】处理当前指针位置的左括号"""
-        self.scanner.move()
+        self.scanner.pop()
         self.stack.append([])
 
     def handle_right_parenthesis(self) -> None:
         """【移动指针】处理当前指针位置的右括号"""
         if len(self.stack) <= 1:
             raise AstParseError(f"当前 ')' 数量大于 '(': pos={self.scanner.pos}")
 
-        self.scanner.move()
+        self.scanner.pop()
         tokens = self.stack.pop()
         self.stack[-1].append(ASTParenthesis(tokens, "(", ")"))
 
     def handle_end_word(self) -> None:
         """【不移动指针】处理在当前指针位置的前一个字符结束的缓存词语（即当前指针位置是下一个词语的第一个字符）
 
         1. 获取并重置缓存词语
```

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/common/text_scanner.py` & `metasequoia-sql-0.1.1/metasequoia_sql/common/base_scanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""文本扫描器"""
+"""基础扫描器"""
 
-from typing import Optional
+from typing import TypeVar, Generic, List, Optional
 
 from metasequoia_sql.errors import ScannerError
 
+T = TypeVar('T')  # 兼容 Python 3.10 及以下版本的泛型
 
-class TextScanner:
+
+class BaseScanner(Generic[T]):
     """文本扫描器"""
 
-    def __init__(self, elements: str, pos: int = 0):
+    def __init__(self, elements: List[T], pos: int = 0):
         """
 
-        指针允许到字符串长度的位置，但在该位置不允许获取。
+        指针允许到 len(elements) 长度的位置，但在该位置不允许 get()。
 
         Parameters
         ----------
-        elements : str
+        elements : Any
             扫描的文本
         pos : int, default = 0
             当前指针位置
         """
         if pos < 0:
             raise ScannerError(f"初始化的指针小于 0: pos={pos}")
         if pos > len(elements):
@@ -28,71 +30,83 @@
         self._elements = elements
         self._pos = pos
         self._len = len(elements)
 
         self._last = elements[pos - 1] if pos > 0 else None  # 上一个元素
 
     @property
-    def elements(self) -> str:
+    def elements(self) -> List[T]:
         return self._elements
 
     @property
     def pos(self) -> int:
         return self._pos
 
     @property
-    def last(self) -> Optional[str]:
+    def last(self) -> Optional[T]:
         """当前指针位置的上一个字符"""
         return self._last
 
     @property
-    def now(self) -> Optional[str]:
+    def now(self) -> Optional[T]:
         """当前指针位置的字符"""
         return self.get()
 
     @property
-    def next(self) -> Optional[str]:
+    def next1(self) -> Optional[T]:
         """当前指针位置的下一个字符"""
-        return self.get_next()
+        return self._get_by_offset(1)
+
+    @property
+    def next2(self) -> Optional[T]:
+        """设当前指针位置为 idx，则返回 idx+2 位置的元素"""
+        return self._get_by_offset(2)
+
+    @property
+    def next3(self) -> Optional[T]:
+        """设当前指针位置为 idx，则返回 idx+2 位置的元素"""
+        return self._get_by_offset(3)
+
+    @property
+    def next4(self) -> Optional[T]:
+        """设当前指针位置为 idx，则返回 idx+2 位置的元素"""
+        return self._get_by_offset(4)
 
-    def get(self) -> Optional[str]:
+    def get(self) -> Optional[T]:
         """获取当前指针位置元素，但不移动指针
 
         - 如果指针已到达字符串末尾，则返回 None
         - 如果指针超出字符串长度，则抛出异常
         """
-        if self._pos > self._len:
-            raise ScannerError(f"要获取的指针大于等于字符串长度: len={self._len}, pos={self._pos}")
-        if self._pos == self._len:
+        if self.pos > self._len:
+            raise ScannerError(f"要获取的指针大于等于字符串长度: len={self._len}, pos={self.pos}")
+        if self.pos == self._len:
             return None
         return self._elements[self._pos]
 
-    def get_next(self) -> Optional[str]:
-        """获取当前指针下一个位置的元素，但不一定指针
-        """
-        if self._pos + 1 > self._len:
-            raise ScannerError(f"要获取的指针大于等于字符串长度: len={self._len}, pos={self._pos + 1}")
-        if self._pos + 1 == self._len:
-            return None
-        return self._elements[self._pos + 1]
-
-    def pop(self) -> str:
+    def pop(self) -> T:
         """获取当前指针位置元素，并移动指针
 
         - 如果要移动到的指针位置超出字符串长度，则抛出异常
         """
-        if self._pos >= self._len:
-            raise ScannerError(f"要移动到的指针下标大于字符串长度: len={self._len}, pos={self._pos + 1}")
+        if self.pos >= self._len:
+            raise ScannerError(f"要移动到的指针下标大于字符串长度: len={self._len}, pos={self.pos + 1} {self}")
 
         self._last = self.get()  # 更新上一个元素
-        result = self._elements[self._pos]
+        result = self._elements[self.pos]
         self._pos += 1  # 移动指针
         return result
 
-    def move(self) -> None:
-        """移动指针"""
-        self._pos += 1
+    def _get_by_offset(self, idx: int) -> Optional[T]:
+        """获取当前指针位置 + idx 位置的元素，但不一定指针
+        """
+        if self.pos + idx >= self._len:
+            return None
+        return self._elements[self.pos + idx]
 
     @property
     def is_finish(self) -> bool:
         """返回当前是否已匹配结束"""
-        return self._pos == self._len
+        return self.pos == self._len
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} tokens={self.elements[self.pos:]}, pos={self.pos}>"
```

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/errors.py` & `metasequoia-sql-0.1.1/metasequoia_sql/errors.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/parser/common.py` & `metasequoia-sql-0.1.1/metasequoia_sql/parser/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 基础元素的解析逻辑
 
 TODO 使用 search 替代直接使用 now 判断
 TODO 整理各种函数的共同规律
 """
 
 from metasequoia_sql import ast
-from metasequoia_sql.common.token_scanner import TokenScanner, build_scanner
+from metasequoia_sql.common.token_scanner import TokenScanner, build_token_scanner
 from metasequoia_sql.objects.core import *
 
 
 def maybe_compute_operator(scanner: TokenScanner) -> bool:
     """检查是否可能为计算运算符
 
     Examples
@@ -368,18 +368,18 @@
 
 def parse_cast_function_expression(scanner: TokenScanner) -> SQLCastFunctionExpression:
     """解析 CAST 函数表达式"""
     column_expression = parse_general_expression(scanner)
     scanner.match("AS")
     signed = scanner.search_and_move("SIGNED")
     cast_type = parse_cast_data_type(scanner)
-    if not scanner.is_finish and scanner.now.is_parenthesis:
+    if not scanner.is_finish and scanner.now_is_parenthesis:
         parenthesis_scanner = scanner.pop_as_children_scanner()
         cast_params: Optional[List[SQLGeneralExpression]] = []
-        for param_scanner in parenthesis_scanner.split_by_comma():
+        for param_scanner in parenthesis_scanner.split_by(","):
             cast_params.append(parse_general_expression(param_scanner))
             if not param_scanner.is_finish:
                 raise SqlParseError(f"无法解析函数参数: {param_scanner}")
     else:
         cast_params = None
     if not scanner.is_finish:
         raise SqlParseError(f"无法解析CAST函数参数: {scanner}")
@@ -397,37 +397,37 @@
     return SQLExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
 
 
 def parse_if_function_expression(parenthesis_scanner: TokenScanner) -> SQLFunctionExpression:
     """解析 IF 函数表达式"""
     function_params: List[SQLGeneralExpression] = []
     first_param = True
-    for param_scanner in parenthesis_scanner.split_by_comma():
+    for param_scanner in parenthesis_scanner.split_by(","):
         if first_param is True:
             function_params.append(parse_condition_expression(param_scanner))
             first_param = False
         else:
             function_params.append(parse_general_expression(param_scanner))
         if not param_scanner.is_finish:
             raise SqlParseError(f"无法解析函数参数: {param_scanner}")
     return SQLFunctionExpression(schema_name=None, function_name="IF", function_params=function_params)
 
 
 def _parse_function_name(scanner: TokenScanner) -> Tuple[Optional[str], str]:
     """解析函数表达式函数的 schema 名和 function 名"""
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_parenthesis):
-        return None, scanner.pop().source
+        return None, scanner.pop_as_source()
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_name and
             scanner.next3 is not None and scanner.next3.is_parenthesis):
-        schema_name = scanner.pop().source
+        schema_name = scanner.pop_as_source()
         scanner.pop()
-        return schema_name, scanner.pop().source
+        return schema_name, scanner.pop_as_source()
     raise SqlParseError(f"无法解析为函数表达式: {scanner}")
 
 
 def parse_function_expression(scanner: TokenScanner) -> SQLFunctionExpression:
     """解析函数表达式
 
     Examples
@@ -465,15 +465,15 @@
 
     is_distinct = False
     if function_name.upper() in {"COUNT", "SUM", "MIN", "MAX", "AVG"} and parenthesis_scanner.now.equals("DISTINCT"):
         parenthesis_scanner.pop()
         is_distinct = True
 
     function_params: List[SQLGeneralExpression] = []
-    for param_scanner in parenthesis_scanner.split_by_comma():
+    for param_scanner in parenthesis_scanner.split_by(","):
         function_params.append(parse_general_expression(param_scanner))
         if not param_scanner.is_finish:
             raise SqlParseError(f"无法解析函数参数: {param_scanner}")
 
     if schema_name is None and function_name.upper() in {"COUNT", "SUM", "MIN", "MAX", "AVG"}:
         return SQLAggregationFunctionExpression(function_name=function_name,
                                                 function_params=function_params,
@@ -540,22 +540,22 @@
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
     >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("coumn_name WHERE"), ignore_space=True))
     <SQLColumnNameExpression source=coumn_name>
     """
     if (scanner.now.is_maybe_name and
             (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
-        return SQLColumnNameExpression(None, scanner.pop().source)
+        return SQLColumnNameExpression(None, scanner.pop_as_source())
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_name and
             (scanner.next3 is None or not scanner.next3.is_parenthesis)):
-        table_name = scanner.pop().source
+        table_name = scanner.pop_as_source()
         scanner.pop()
-        column_name = scanner.pop().source
+        column_name = scanner.pop_as_source()
         return SQLColumnNameExpression(table_name, column_name)
     raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
 
 def maybe_case_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为 CASE 表达式
 
@@ -570,20 +570,20 @@
 
 
 def parse_case_expression(scanner: TokenScanner) -> Union[SQLCaseExpression, SQLCaseValueExpression]:
     """解析 CASE 表达式
 
     Examples
     --------
-    >>> parse_case_expression(build_scanner("CASE WHEN 2 THEN 3 ELSE 4 END"))
+    >>> parse_case_expression(build_token_scanner("CASE WHEN 2 THEN 3 ELSE 4 END"))
     <SQLCaseExpression source=CASE
         WHEN <SQLLiteralExpression source=2> THEN <SQLLiteralExpression source=3>
         ELSE <SQLLiteralExpression source=4>
     END>
-    >>> parse_case_expression(build_scanner("3 + 5"))
+    >>> parse_case_expression(build_token_scanner("3 + 5"))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为CASE表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=1>
     """
     scanner.match("CASE")
     if scanner.search("WHEN"):
         # 第 1 种格式的 CASE 表达式
@@ -620,17 +620,17 @@
 
 
 def maybe_window_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为窗口函数
 
     Examples
     --------
-    >>> maybe_window_expression(build_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
+    >>> maybe_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
     True
-    >>> maybe_window_expression(build_scanner("3 + 5"))
+    >>> maybe_window_expression(build_token_scanner("3 + 5"))
     False
     """
     return not scanner.is_finish and (
             scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
             scanner.next1 is not None and scanner.next1.is_parenthesis and
             scanner.next2 is not None and scanner.next2.equals("OVER") and
             scanner.next3 is not None and scanner.next3.is_parenthesis)
@@ -639,17 +639,17 @@
 def parse_window_expression(scanner: TokenScanner) -> SQLWindowExpression:
     """解析窗口函数
 
     TODO 支持 ROW BETWEEN 的语法
 
     Examples
     --------
-    >>> parse_window_expression(build_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
+    >>> parse_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
     <SQLWindowExpression source=<SQLFunctionExpression source=ROW_NUMBER()> OVER (PARTITION BY <SQLColumnNameExpression source=column1>ORDER BY <SQLColumnNameExpression source=column2>)>
-    >>> parse_window_expression(build_scanner("3 + 5"))
+    >>> parse_window_expression(build_token_scanner("3 + 5"))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=0>
     """
     window_function = parse_function_expression(scanner)
     partition_by = None
     order_by = None
@@ -671,15 +671,15 @@
         return parse_window_expression(scanner)
     if maybe_function_expression(scanner):
         return parse_function_expression(scanner)
     if maybe_literal_expression(scanner):
         return parse_literal_expression(scanner)
     if maybe_column_name_expression(scanner):
         return parse_column_name_expression(scanner)
-    if scanner.now.is_parenthesis:
+    if scanner.now_is_parenthesis:
         return parse_general_parenthesis(scanner)
     if maybe_wildcard_expression(scanner):
         return parse_wildcard_expression(scanner)
     raise SqlParseError(f"未知的一般表达式元素: {scanner}")
 
 
 def parse_general_expression(scanner: TokenScanner, maybe_window: bool = True) -> SQLGeneralExpression:
@@ -695,60 +695,60 @@
 
 
 def parse_table_name_expression(scanner: TokenScanner) -> Union[SQLTableNameExpression, SQLSubQueryExpression]:
     """解析表名表达式或子查询表达式
 
     Examples
     --------
-    >>> parse_table_name_expression(build_scanner("table1.column1 AS t1"))
+    >>> parse_table_name_expression(build_token_scanner("table1.column1 AS t1"))
     <SQLTableNameExpression source=table1.column1>
     """
     if (scanner.now.is_maybe_name and
             (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
-        return SQLTableNameExpression(None, scanner.pop().source)
+        return SQLTableNameExpression(None, scanner.pop_as_source())
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_name and
             (scanner.next3 is None or not scanner.next3.is_parenthesis)):
-        schema_name = scanner.pop().source
+        schema_name = scanner.pop_as_source()
         scanner.pop()
-        table_name = scanner.pop().source
+        table_name = scanner.pop_as_source()
         return SQLTableNameExpression(schema_name, table_name)
     if is_sub_query_parenthesis(scanner):
         return parse_sub_query_parenthesis(scanner)
     raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
 
 def parse_bool_expression(scanner: TokenScanner) -> SQLBoolExpression:
     """解析布尔值表达式
 
     Examples
     --------
-    >>> parse_bool_expression(build_scanner("column1 > 3"))
+    >>> parse_bool_expression(build_token_scanner("column1 > 3"))
     <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_scanner("t2.column1 > 3"))
+    >>> parse_bool_expression(build_token_scanner("t2.column1 > 3"))
     <SQLBoolCompareExpression source=<SQLColumnNameExpression source=t2.column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_scanner("t2.column1 + 3 > 3"))
+    >>> parse_bool_expression(build_token_scanner("t2.column1 + 3 > 3"))
     <SQLBoolCompareExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=t2.column1> <SQLPlus> <SQLLiteralExpression source=3>> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_scanner("column1 BETWEEN 3 AND 4"))
+    >>> parse_bool_expression(build_token_scanner("column1 BETWEEN 3 AND 4"))
     <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column1> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
-    >>> parse_bool_expression(build_scanner("column1 + 3 BETWEEN 3 AND 4"))
+    >>> parse_bool_expression(build_token_scanner("column1 + 3 BETWEEN 3 AND 4"))
     <SQLBoolBetweenExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=column1> <SQLPlus> <SQLLiteralExpression source=3>> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
     """
     if scanner.search_and_move("EXISTS"):
         after_value = parse_sub_query_parenthesis(scanner)
         return SQLBoolExistsExpression(is_not=False, after_value=after_value)
     if scanner.search_and_move("NOT", "EXISTS"):
         after_value = parse_sub_query_parenthesis(scanner)
         return SQLBoolExistsExpression(is_not=True, after_value=after_value)
     before_value = parse_general_expression(scanner)
     if scanner.search_and_move("BETWEEN"):
         # "... BETWEEN ... AND ..."
         from_value = parse_general_expression(scanner)
-        if not scanner.pop().equals("AND"):
+        if not scanner.search_and_move("AND"):
             raise SqlParseError(f"无法解析为 BETWEEN 布尔值表达式: {scanner}")
         to_value = parse_general_expression(scanner)
         return SQLBoolBetweenExpression(before_value=before_value, from_value=from_value, to_value=to_value)
     if scanner.search_and_move("IS"):
         # ".... IS ...." 或 "... IS NOT ..."
         if scanner.search_and_move("NOT"):
             is_not = True
@@ -778,61 +778,61 @@
 
 
 def maybe_alias_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为别名表达式
 
     Examples
     --------
-    >>> maybe_alias_expression(build_scanner("t1"))
+    >>> maybe_alias_expression(build_token_scanner("t1"))
     True
-    >>> maybe_alias_expression(build_scanner("AS t1"))
+    >>> maybe_alias_expression(build_token_scanner("AS t1"))
     True
-    >>> maybe_alias_expression(build_scanner("WHERE"))
+    >>> maybe_alias_expression(build_token_scanner("WHERE"))
     False
     """
     return not scanner.is_finish and (scanner.now.equals("AS") or scanner.now.is_maybe_name)
 
 
 def parse_alias_expression(scanner: TokenScanner) -> SQLAlisaExpression:
     """解析别名表达式
 
     Examples
     --------
-    >>> parse_alias_expression(build_scanner("t1"))
+    >>> parse_alias_expression(build_token_scanner("t1"))
     <SQLAlisaExpression source=AS t1>
-    >>> parse_alias_expression(build_scanner("AS t1"))
+    >>> parse_alias_expression(build_token_scanner("AS t1"))
     <SQLAlisaExpression source=AS t1>
-    >>> parse_alias_expression(build_scanner("WHERE"))
+    >>> parse_alias_expression(build_token_scanner("WHERE"))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为别名表达式: <TokenScanner tokens=[<ASTCommon source=WHERE>], pos=0>
     """
     scanner.search_and_move("AS")
     if not scanner.now.is_maybe_name:
         raise SqlParseError(f"无法解析为别名表达式: {scanner}")
-    return SQLAlisaExpression(alias_name=scanner.pop().source)
+    return SQLAlisaExpression(alias_name=scanner.pop_as_source())
 
 
 def parse_condition_expression(scanner: TokenScanner) -> SQLConditionExpression:
     """解析条件表达式
 
     Examples
     --------
-    >>> parse_condition_expression(build_scanner("column1 > 3 AND column2 > 2 WHERE"))
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 AND column2 > 2 WHERE"))
     <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_scanner("column1 > 3 OR column2 > 2 WHERE"))
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 > 2 WHERE"))
     <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_scanner("column1 > 3 OR column2 BETWEEN 2 AND 4 WHERE"))
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 BETWEEN 2 AND 4 WHERE"))
     <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>
     """
 
     def parse_single():
         if scanner.search("NOT"):
             elements.append(parse_logical_operator(scanner))
-        if scanner.now.is_parenthesis:
+        if scanner.now_is_parenthesis:
             elements.append(parse_condition_expression(scanner.pop_as_children_scanner()))  # 插入语，子句也应该是一个条件表达式
         else:
             elements.append(parse_bool_expression(scanner))
 
     elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
     parse_single()  # 解析第 1 个表达式元素
     while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
@@ -843,30 +843,30 @@
 
 
 def parse_join_on_expression(scanner: TokenScanner) -> SQLJoinOnExpression:
     """解析 ON 关联表达式
 
     Examples
     --------
-    >>> parse_join_on_expression(build_scanner("ON t1.column1 = t2.column2"))
+    >>> parse_join_on_expression(build_token_scanner("ON t1.column1 = t2.column2"))
     <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column2>>>>
     """
-    if not scanner.pop().equals("ON"):
+    if not scanner.search_and_move("ON"):
         raise SqlParseError(f"无法解析为 ON 关联表达式: {scanner}")
     return SQLJoinOnExpression(condition=parse_condition_expression(scanner))
 
 
 def parse_join_using_expression(scanner: TokenScanner) -> SQLJoinUsingExpression:
     """解析 USING 关联表达式
 
     Examples
     --------
-    >>> parse_join_using_expression(build_scanner("USING(column1, column2)"))
+    >>> parse_join_using_expression(build_token_scanner("USING(column1, column2)"))
     <SQLJoinUsingExpression source=<SQLFunctionExpression source=USING(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    >>> parse_join_using_expression(build_scanner("using(column1, column2)"))
+    >>> parse_join_using_expression(build_token_scanner("using(column1, column2)"))
     <SQLJoinUsingExpression source=<SQLFunctionExpression source=using(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
     """
     if not scanner.now.equals("USING"):
         raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
     return SQLJoinUsingExpression(using_function=parse_function_expression(scanner))
 
 
@@ -876,128 +876,150 @@
 
 
 def parse_join_expression(scanner: TokenScanner) -> SQLJoinExpression:
     """解析关联表达式
 
     Examples
     --------
-    >>> parse_join_on_expression(build_scanner("ON t1.column1 = t2.column2"))
+    >>> parse_join_on_expression(build_token_scanner("ON t1.column1 = t2.column2"))
     <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column2>>>>
-    >>> parse_join_using_expression(build_scanner("USING(column1, column2)"))
+    >>> parse_join_using_expression(build_token_scanner("USING(column1, column2)"))
     <SQLJoinUsingExpression source=<SQLFunctionExpression source=USING(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    >>> parse_join_using_expression(build_scanner("using(column1, column2)"))
+    >>> parse_join_using_expression(build_token_scanner("using(column1, column2)"))
     <SQLJoinUsingExpression source=<SQLFunctionExpression source=using(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
     """
     if scanner.search("ON"):
         return parse_join_on_expression(scanner)
     if scanner.search("USING"):
         return parse_join_using_expression(scanner)
     raise SqlParseError(f"无法解析为关联表达式: {scanner}")
 
 
 def maybe_wildcard_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为通配符表达式
 
     Examples
     --------
-    >>> maybe_wildcard_expression(build_scanner("*"))
+    >>> maybe_wildcard_expression(build_token_scanner("*"))
     True
-    >>> maybe_wildcard_expression(build_scanner("t1.*"))
+    >>> maybe_wildcard_expression(build_token_scanner("t1.*"))
     True
     """
     return not scanner.is_finish and (scanner.now.is_maybe_wildcard or
                                       (scanner.now.is_maybe_name and
                                        scanner.next1 is not None and scanner.next1.is_dot and
                                        scanner.next2 is not None and scanner.next2.is_maybe_wildcard))
 
 
 def parse_wildcard_expression(scanner: TokenScanner) -> SQLWildcardExpression:
     """解析通配符表达式
 
     Examples
     --------
-    >>> parse_wildcard_expression(build_scanner("*"))
+    >>> parse_wildcard_expression(build_token_scanner("*"))
     <SQLWildcardExpression source=*>
-    >>> parse_wildcard_expression(build_scanner("t1.*"))
+    >>> parse_wildcard_expression(build_token_scanner("t1.*"))
     <SQLWildcardExpression source=t1.*>
     """
     if scanner.now.is_maybe_wildcard:
         scanner.pop()
         return SQLWildcardExpression(schema=None)
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_wildcard):
-        schema_name = scanner.pop().source
+        schema_name = scanner.pop_as_source()
         scanner.pop()
         scanner.pop()
         return SQLWildcardExpression(schema=schema_name)
     raise SqlParseError("无法解析为通配符表达式")
 
 
 def parse_table_expression(scanner: TokenScanner) -> SQLTableExpression:
     """解析表名表达式
 
     Examples
     --------
-    >>> parse_table_expression(build_scanner("schema1.table1 AS t1"))
+    >>> parse_table_expression(build_token_scanner("schema1.table1 AS t1"))
     <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>
     """
     table_name_expression = parse_table_name_expression(scanner)
     alias_expression = parse_alias_expression(scanner) if maybe_alias_expression(scanner) else None
     return SQLTableExpression(table=table_name_expression, alias=alias_expression)
 
 
 def parse_column_expression(scanner: TokenScanner) -> SQLColumnExpression:
     """解析列名表达式
 
     Examples
     --------
-    >>> parse_column_expression(build_scanner("table1.column1 AS t1"))
+    >>> parse_column_expression(build_token_scanner("table1.column1 AS t1"))
     <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
-    >>> parse_column_expression(build_scanner("3 + 5 AS t1"))
+    >>> parse_column_expression(build_token_scanner("3 + 5 AS t1"))
     <SQLColumnExpression source=<SQLComputeExpression source=<SQLLiteralExpression source=3> <SQLPlus> <SQLLiteralExpression source=5>> AS <SQLAlisaExpression source=AS t1>>
-    >>> parse_column_expression(build_scanner("TRIM(column1) AS t1"))
+    >>> parse_column_expression(build_token_scanner("TRIM(column1) AS t1"))
     <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
     """
     general_expression = parse_general_expression(scanner)
     alias_expression = parse_alias_expression(scanner) if maybe_alias_expression(scanner) else None
     return SQLColumnExpression(column=general_expression, alias=alias_expression)
 
 
 def parse_value_expression(scanner: TokenScanner) -> SQLValueExpression:
     """解析值表达式"""
     values = []
-    for value_scanner in scanner.pop_as_children_scanner_list_split_by_comma():
+    for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
         values.append(parse_general_expression(value_scanner))
     return SQLValueExpression(values=values)
 
 
+def parse_equal_expression(scanner: TokenScanner) -> SQLEqualExpression:
+    """解析等式表达式"""
+    before_value = parse_general_expression(scanner)
+    scanner.match("=")
+    after_value = parse_general_expression(scanner)
+    return SQLEqualExpression(before_value=before_value, after_value=after_value)
+
+
+def is_partition_expression(scanner: TokenScanner) -> bool:
+    """判断是否可能为分区表达式"""
+    return scanner.search("PARTITION")
+
+
+def parse_partition_expression(scanner: TokenScanner) -> SQLPartitionExpression:
+    """解析分区表达式"""
+    scanner.match("PARTITION")
+    partition_list = []
+    for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+        partition_list.append(parse_equal_expression(partition_scanner))
+    return SQLPartitionExpression(partition_list=partition_list)
+
+
 def maybe_limit_clause(scanner: TokenScanner) -> bool:
     """是否可能为 LIMIT 子句
 
     Examples
     --------
-    >>> maybe_limit_clause(build_scanner("LIMIT 2, 5"))
+    >>> maybe_limit_clause(build_token_scanner("LIMIT 2, 5"))
     True
-    >>> maybe_limit_clause(build_scanner("LIMIT 5 OFFSET 2"))
+    >>> maybe_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
     True
-    >>> maybe_limit_clause(build_scanner("ORDER BY column1"))
+    >>> maybe_limit_clause(build_token_scanner("ORDER BY column1"))
     False
     """
     return scanner.search("LIMIT")
 
 
 def parse_limit_clause(scanner: TokenScanner) -> SQLLimitClause:
     """解析 LIMIT 子句
 
     Examples
     --------
-    >>> parse_limit_clause(build_scanner("LIMIT 2, 5"))
+    >>> parse_limit_clause(build_token_scanner("LIMIT 2, 5"))
     <SQLLimitClause source=LIMIT 2, 5>
-    >>> parse_limit_clause(build_scanner("LIMIT 5 OFFSET 2"))
+    >>> parse_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
     <SQLLimitClause source=LIMIT 2, 5>
     """
     if not scanner.search_and_move("LIMIT"):
         raise SqlParseError("无法解析为 LIMIT 子句")
     cnt_1 = parse_literal_expression(scanner).as_int()
     mark = scanner.pop()
     if mark.is_comma:
@@ -1013,36 +1035,36 @@
 
 
 def maybe_order_by_clause(scanner: TokenScanner) -> bool:
     """是否可能为 ORDER BY 子句
 
     Examples
     --------
-    >>> maybe_order_by_clause(build_scanner("ORDER BY column1, column2"))
+    >>> maybe_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
     True
-    >>> maybe_order_by_clause(build_scanner("ORDER BY column1, column2 DESC"))
+    >>> maybe_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
     True
-    >>> maybe_order_by_clause(build_scanner("ORDER BY trim(column1) ASC, column2"))
+    >>> maybe_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
     True
-    >>> maybe_order_by_clause(build_scanner("WHERE trim(column1) IS NOT NULL"))
+    >>> maybe_order_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
     False
     """
     return scanner.search("ORDER", "BY")
 
 
 def parse_order_by_clause(scanner: TokenScanner) -> SQLOrderByClause:
     """解析 ORDER BY 子句
 
     Examples
     --------
-    >>> parse_order_by_clause(build_scanner("ORDER BY column1, column2"))
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
     <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_order_by_clause(build_scanner("ORDER BY column1, column2 DESC"))
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
     <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2> DESC>
-    >>> parse_order_by_clause(build_scanner("ORDER BY trim(column1) ASC, column2"))
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
     <SQLOrderByClause source=ORDER BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
     """
 
     def parse_single():
         column = parse_general_expression(scanner)
         if not scanner.is_finish and scanner.search_and_move("DESC"):
             order = SQLEnumOrderType.DESC
@@ -1061,77 +1083,77 @@
 
 
 def maybe_having_clause(scanner: TokenScanner) -> bool:
     """是否可能为 HAVING 子句
 
     Examples
     --------
-    >>> maybe_having_clause(build_scanner("HAVING column1 > 3 AND column2 > 2"))
+    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
     True
-    >>> maybe_having_clause(build_scanner("HAVING column1 > 3 OR column2 > 2"))
+    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
     True
-    >>> maybe_having_clause(build_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
     True
-    >>> maybe_having_clause(build_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> maybe_having_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     False
     """
     return scanner.search("HAVING")
 
 
 def parse_having_clause(scanner: TokenScanner) -> SQLHavingClause:
     """解析 HAVING 子句
 
     Examples
     --------
-    >>> parse_having_clause(build_scanner("HAVING column1 > 3 AND column2 > 2"))
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
     <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_scanner("HAVING column1 > 3 OR column2 > 2"))
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
     <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
     <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
     """
     scanner.match("HAVING")
     return SQLHavingClause(condition=parse_condition_expression(scanner))
 
 
 def maybe_group_by_clause(scanner: TokenScanner) -> bool:
     """判断是否可能为 GROUP BY 子句
 
     Examples
     --------
-    >>> maybe_group_by_clause(build_scanner("GROUP BY column1, column2"))
+    >>> maybe_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
     True
-    >>> maybe_group_by_clause(build_scanner("GROUP BY column1, column2 DESC"))
+    >>> maybe_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
     True
-    >>> maybe_group_by_clause(build_scanner("GROUP BY trim(column1) ASC, column2"))
+    >>> maybe_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
     True
-    >>> maybe_group_by_clause(build_scanner("WHERE trim(column1) IS NOT NULL"))
+    >>> maybe_group_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
     False
     """
     return scanner.search("GROUP", "BY")
 
 
 def parse_group_by_clause(scanner: TokenScanner) -> SQLGroupByClause:
     """解析 GROUP BY 子句
 
     Examples
     --------
-    >>> parse_group_by_clause(build_scanner("GROUP BY column1, column2"))
+    >>> parse_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
     <SQLGroupByClause source=GROUP BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_group_by_clause(build_scanner("GROUP BY column1, column2 DESC"))
+    >>> parse_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
     <SQLGroupByClause source=GROUP BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_group_by_clause(build_scanner("GROUP BY trim(column1) ASC, column2"))
+    >>> parse_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
     <SQLGroupByClause source=GROUP BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
     """
     scanner.match("GROUP", "BY")
     if scanner.search_and_move("GROUPING", "SETS"):
         grouping_list = []
-        for grouping_scanner in scanner.pop_as_children_scanner_list_split_by_comma():
-            if grouping_scanner.now.is_parenthesis:
-                parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by_comma()
+        for grouping_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            if grouping_scanner.now_is_parenthesis:
+                parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by(",")
                 columns_list = [parse_general_expression(parenthesis_scanner)
                                 for parenthesis_scanner in parenthesis_scanner_list]
                 grouping_list.append(columns_list)
             else:
                 grouping_list.append([parse_general_expression(grouping_scanner)])
         return SQLGroupingSetsGroupByClause(grouping_list=grouping_list)
     else:
@@ -1146,52 +1168,52 @@
 
 
 def maybe_where_clause(scanner: TokenScanner) -> bool:
     """判断是否可能为 WHERE 子句
 
     Examples
     --------
-    >>> maybe_where_clause(build_scanner("WHERE column1 > 3 AND column2 > 2"))
+    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
     True
-    >>> maybe_where_clause(build_scanner("WHERE column1 > 3 OR column2 > 2"))
+    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
     True
-    >>> maybe_where_clause(build_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     True
-    >>> maybe_where_clause(build_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> maybe_where_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
     False
     """
     return scanner.search("WHERE")
 
 
 def parse_where_clause(scanner: TokenScanner) -> SQLWhereClause:
     """解析 WHERE 子句
 
     Examples
     --------
-    >>> parse_where_clause(build_scanner("WHERE column1 > 3 AND column2 > 2"))
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
     <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_scanner("WHERE column1 > 3 OR column2 > 2"))
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
     <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
     """
     scanner.match("WHERE")
     return SQLWhereClause(condition=parse_condition_expression(scanner))
 
 
 def maybe_join_clause(scanner: TokenScanner) -> bool:
     """判断是否为 JOIN 子句
 
     Examples
     --------
-    >>> maybe_join_clause(build_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> maybe_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
     True
-    >>> maybe_join_clause(build_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> maybe_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
     True
-    >>> maybe_join_clause(build_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> maybe_join_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     False
     """
     return (scanner.search("JOIN") or
             scanner.search("INNER", "JOIN") or
             scanner.search("LEFT", "JOIN") or
             scanner.search("LEFT", "OUTER", "JOIN") or
             scanner.search("RIGHT", "JOIN") or
@@ -1225,17 +1247,17 @@
 
 
 def parse_join_clause(scanner: TokenScanner) -> SQLJoinClause:
     """解析 JOIN 子句
 
     Examples
     --------
-    >>> parse_join_clause(build_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> parse_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
     <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
-    >>> parse_join_clause(build_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> parse_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
     <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
     """
     join_type = _parse_join_type(scanner)
     table_expression = parse_table_expression(scanner)
     if is_join_expression(scanner):
         join_rule = parse_join_expression(scanner)
     else:
@@ -1244,32 +1266,32 @@
 
 
 def maybe_from_clause(scanner: TokenScanner) -> bool:
     """判断是否为 FROM 子句
 
     Examples
     --------
-    >>> maybe_from_clause(build_scanner("FROM schema1.table1 AS t1"))
+    >>> maybe_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
     True
-    >>> maybe_from_clause(build_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
+    >>> maybe_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
     True
-    >>> maybe_from_clause(build_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> maybe_from_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
     False
     """
     return scanner.search("FROM")
 
 
 def parse_from_clause(scanner: TokenScanner) -> SQLFromClause:
     """解析 FROM 子句
 
     Examples
     --------
-    >>> parse_from_clause(build_scanner("FROM schema1.table1 AS t1"))
+    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
     <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>>
-    >>> parse_from_clause(build_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
+    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
     <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>, <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>>>
     """
     scanner.match("FROM")
     tables = [parse_table_expression(scanner)]
     while not scanner.is_finish and scanner.now.is_comma:
         scanner.pop()
         tables.append(parse_table_expression(scanner))
@@ -1277,33 +1299,33 @@
 
 
 def maybe_select_clause(scanner: TokenScanner) -> bool:
     """判断是否为 SELECT 子句
 
     Examples
     --------
-    >>> maybe_from_clause(build_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
+    >>> maybe_from_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
     True
-    >>> maybe_from_clause(build_scanner("SELECT column1 AS c1"))
+    >>> maybe_from_clause(build_token_scanner("SELECT column1 AS c1"))
     True
-    >>> maybe_from_clause(build_scanner("FROM table1"))
+    >>> maybe_from_clause(build_token_scanner("FROM table1"))
     False
     """
     return scanner.search("SELECT")
 
 
 def parse_select_clause(scanner: TokenScanner) -> SQLSelectClause:
     """解析 SELECT 子句
 
     Examples
     --------
-    >>> parse_select_clause(build_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
+    >>> parse_select_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
     <SQLSelectClause source=SELECT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>,
     <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column2>)> AS <SQLAlisaExpression source=AS c2>>>
-    >>> parse_select_clause(build_scanner("SELECT DISTINCT column1 AS c1"))
+    >>> parse_select_clause(build_token_scanner("SELECT DISTINCT column1 AS c1"))
     <SQLSelectClause source=SELECT DISTINCT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>>
     """
 
     scanner.match("SELECT")
     distinct = scanner.search_and_move("DISTINCT")
     columns = [parse_column_expression(scanner)]
     while not scanner.is_finish and scanner.now.is_comma:
@@ -1318,20 +1340,22 @@
     scanner.match("AS")
     table_statement = parse_select_statement(scanner.pop_as_children_scanner(), with_clause=SQLWithClause.empty())
     return table_name, table_statement
 
 
 def parse_with_clause(scanner: TokenScanner) -> Optional[SQLWithClause]:
     """解析 WITH 子句"""
-    scanner.match("WITH")
-    tables = [_parse_single_with_table(scanner)]
-    while scanner.search_and_move(","):
-        table_statement = _parse_single_with_table(scanner)
-        tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
-    return SQLWithClause(tables=tables)
+    if scanner.search_and_move("WITH"):
+        tables = [_parse_single_with_table(scanner)]
+        while scanner.search_and_move(","):
+            table_statement = _parse_single_with_table(scanner)
+            tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
+        return SQLWithClause(tables=tables)
+    else:
+        return SQLWithClause.empty()
 
 
 def maybe_select_statement(scanner: TokenScanner) -> bool:
     """判断是否可能为 SELECT 语句"""
     return scanner.search("SELECT")
 
 
@@ -1372,37 +1396,112 @@
         group_by_clause=group_by_clause,
         having_clause=having_clause,
         order_by_clause=order_by_clause,
         limit_clause=limit_clause
     )
 
 
+def is_select_statement(scanner: TokenScanner) -> bool:
+    """判断是否为 SELECT 语句（已匹配过 WITH 语句后才可以调用）"""
+    return scanner.search("SELECT")
+
+
 def parse_select_statement(scanner: TokenScanner,
                            with_clause: Optional[SQLWithClause] = None) -> SQLSelectStatement:
     """解析 SELECT 语句"""
     if with_clause is None:
         with_clause = parse_with_clause(scanner)
     result = [parse_single_select_statement(scanner, with_clause=with_clause)]
     while not scanner.is_finish:
         for union_type in SQLEnumUnionType:
             if scanner.search_and_move(*union_type.value):
                 result.append(SQLUnionKeyword(union_type=union_type))
                 result.append(parse_single_select_statement(scanner, with_clause=with_clause))
                 break
         else:
             break
+    scanner.search_and_move(";")
     if not scanner.is_finish:
         raise SqlParseError(f"没有解析完成: {scanner}")
 
     if len(result) > 1:
         return SQLUnionSelectStatement(with_clause=with_clause, elements=result)
     else:
         return result[0]
 
 
+def is_insert_statement(scanner: TokenScanner) -> bool:
+    """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
+    return scanner.search("INSERT")
+
+
+def parse_insert_statement(scanner: TokenScanner, with_clause: SQLWithClause) -> SQLInsertStatement:
+    """解析 INSERT 表达式"""
+    scanner.match("INSERT")
+
+    # 解析 INSERT 类型
+    if scanner.search_and_move("INTO"):
+        insert_type = SQLInsertType.INSERT_INTO
+    elif scanner.search_and_move("OVERWRITE"):
+        insert_type = SQLInsertType.INSERT_OVERWRITE
+    else:
+        raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
+
+    # 匹配可能包含的 TABLE 关键字
+    has_table_keyword = scanner.search_and_move("TABLE")
+
+    # 匹配表名
+    table_name = parse_table_name_expression(scanner)
+
+    # 匹配分区表达式
+    if is_partition_expression(scanner):
+        partition = parse_partition_expression(scanner)
+    else:
+        partition = None
+
+    # 匹配列名列表
+    if scanner.now_is_parenthesis:
+        columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            columns.append(parse_column_name_expression(column_scanner))
+            if not column_scanner.is_finish:
+                raise SqlParseError(f"未解析完成的列名: {column_scanner}")
+    else:
+        columns = None
+
+    # 匹配 VALUES 类型
+    if scanner.search_and_move("VALUES"):
+        values = []
+        while scanner.now_is_parenthesis:
+            values.append(parse_value_expression(scanner))
+            scanner.search_and_move(",")
+
+        return SQLInsertValuesStatement(
+            with_clause=with_clause,
+            insert_type=insert_type,
+            has_table_keyword=has_table_keyword,
+            table_name=table_name,
+            partition=partition,
+            columns=columns,
+            values=values
+        )
+
+    if scanner.search("SELECT"):
+        select_statement = parse_select_statement(scanner, with_clause=SQLWithClause.empty())
+        return SQLInsertSelectStatement(
+            with_clause=with_clause,
+            insert_type=insert_type,
+            has_table_keyword=has_table_keyword,
+            table_name=table_name,
+            partition=partition,
+            columns=columns,
+            select_statement=select_statement
+        )
+
+
 def is_sub_query_parenthesis(scanner: TokenScanner) -> bool:
     """判断是否为子查询的插入语"""
     parenthesis_scanner: TokenScanner = scanner.get_as_children_scanner()
     return maybe_select_statement(parenthesis_scanner)
 
 
 def parse_sub_query_parenthesis(scanner: TokenScanner) -> SQLSubQueryExpression:
@@ -1420,20 +1519,260 @@
 def parse_in_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
     """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
     if is_sub_query_parenthesis(scanner):
         return parse_sub_query_parenthesis(scanner)
     return parse_value_expression(scanner)
 
 
-def parse_sql_column_type(scanner: TokenScanner) -> SQLColumnType:
-    """解析字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
+def parse_ddl_column_type_expression(scanner: TokenScanner) -> DDLColumnTypeExpression:
+    """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
     # 解析字段类型名称
-    function_name: str = scanner.pop().source
+    function_name: str = scanner.pop_as_source()
 
     # 解析字段类型参数
-    if not scanner.is_finish and scanner.now.is_parenthesis:
+    if not scanner.is_finish and scanner.now_is_parenthesis:
         function_params: List[SQLGeneralExpression] = []
-        for param_scanner in scanner.pop_as_children_scanner_list_split_by_comma():
+        for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             function_params.append(parse_general_expression(param_scanner))
-        return SQLColumnType(function_name, function_params)
+        return DDLColumnTypeExpression(function_name, function_params)
     else:
-        return SQLColumnType(function_name, [])
+        return DDLColumnTypeExpression(function_name, [])
+
+
+def parse_ddl_column_expression(scanner: TokenScanner) -> DDLColumnExpression:
+    """解析 DDL 的字段表达式"""
+    # 解析顺序固定的信息
+    column_name = scanner.pop_as_source()
+    column_type = parse_ddl_column_type_expression(scanner)
+
+    # 解析顺序可能不定的字段信息
+    comment: Optional[str] = None
+    is_unsigned: bool = False
+    is_zerofill: bool = False
+    character_set: Optional[str] = None
+    collate: Optional[str] = None
+    is_allow_null: bool = False
+    is_not_null: bool = False
+    is_auto_increment: bool = False
+    default: Optional[SQLGeneralExpression] = None
+    on_update: Optional[SQLGeneralExpression] = None
+    while not scanner.is_finish:
+        if scanner.search_and_move("NOT", "NULL"):
+            is_not_null = True
+        elif scanner.search_and_move("NULL"):
+            is_allow_null = True
+        elif scanner.search_and_move("CHARACTER", "SET"):
+            character_set = scanner.pop_as_source()
+        elif scanner.search_and_move("COLLATE"):
+            collate = scanner.pop_as_source()
+        elif scanner.search_and_move("DEFAULT"):
+            default = parse_general_expression(scanner)
+        elif scanner.search_and_move("COMMENT"):
+            comment = scanner.pop_as_source()
+        elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
+            on_update = parse_general_expression(scanner)
+        elif scanner.search_and_move("AUTO_INCREMENT"):
+            is_auto_increment = True
+        elif scanner.search_and_move("UNSIGNED"):
+            is_unsigned = True
+        elif scanner.search_and_move("ZEROFILL"):
+            is_zerofill = True
+        else:
+            raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
+
+    # 构造 DDL 字段表达式对象
+    return DDLColumnExpression(
+        column_name=column_name,
+        column_type=column_type,
+        comment=comment,
+        is_unsigned=is_unsigned,
+        is_zerofill=is_zerofill,
+        character_set=character_set,
+        collate=collate,
+        is_allow_null=is_allow_null,
+        is_not_null=is_not_null,
+        is_auto_increment=is_auto_increment,
+        default=default,
+        on_update=on_update
+    )
+
+
+def is_ddl_primary_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为主键表达式"""
+    return scanner.search("PRIMARY", "KEY")
+
+
+def parse_ddl_primary_index_expression(scanner: TokenScanner) -> DDLPrimaryIndexExpression:
+    """解析主键表达式"""
+    scanner.match("PRIMARY", "KEY")
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return DDLPrimaryIndexExpression(columns=columns)
+
+
+def is_ddl_unique_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为唯一键表达式"""
+    return scanner.search("UNIQUE", "KEY")
+
+
+def parse_ddl_unique_index_expression(scanner: TokenScanner) -> DDLUniqueIndexExpression:
+    """解析唯一键表达式"""
+    scanner.match("UNIQUE", "KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return DDLUniqueIndexExpression(name=name, columns=columns)
+
+
+def is_ddl_normal_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为一般索引表达式"""
+    return scanner.search("KEY")
+
+
+def parse_ddl_normal_index_expression(scanner: TokenScanner) -> DDLNormalIndexExpression:
+    """解析一般索引表达式"""
+    scanner.match("KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return DDLNormalIndexExpression(name=name, columns=columns)
+
+
+def is_ddl_fulltext_expression(scanner: TokenScanner) -> bool:
+    """判断是否为全文索引表达式"""
+    return scanner.search("FULLTEXT", "KEY")
+
+
+def parse_ddl_fulltext_expression(scanner: TokenScanner) -> DDLFulltextIndexExpression:
+    """解析全文索引表达式"""
+    scanner.match("FULLTEXT", "KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return DDLFulltextIndexExpression(name=name, columns=columns)
+
+
+def is_ddl_foreign_key_expression(scanner: TokenScanner) -> bool:
+    """判断是否为外键表达式"""
+    return scanner.search("CONSTRAINT")
+
+
+def parse_dll_foreign_key_expression(scanner: TokenScanner) -> DDLForeignKeyExpression:
+    """解析外键表达式"""
+    scanner.match("CONSTRAINT")
+    constraint_name = scanner.pop_as_source()
+    scanner.match("FOREIGN", "KEY")
+    slave_columns = [column_scanner.pop_as_source()
+                     for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    scanner.match("REFERENCES")
+    master_table_name = scanner.pop_as_source()
+    master_columns = [column_scanner.pop_as_source()
+                      for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return DDLForeignKeyExpression(
+        constraint_name=constraint_name,
+        slave_columns=slave_columns,
+        master_table_name=master_table_name,
+        master_columns=master_columns
+    )
+
+
+def parse(scanner: TokenScanner) -> List[SQLStatement]:
+    """解析一段 SQL 语句，返回表达式的列表
+
+    Examples
+    --------
+    >>> parse(build_token_scanner("SELECT a FROM b; SELECT c FROM d"))
+    [<SQLSingleSelectStatement source=SELECT a
+    FROM b>, <SQLSingleSelectStatement source=SELECT c
+    FROM d>]
+    """
+    statement_list = []
+    for statement_scanner in scanner.split_by(";"):
+        # 先尝试解析 WITH 语句
+        with_clause = parse_with_clause(statement_scanner)
+
+        if is_select_statement(statement_scanner):
+            statement_list.append(parse_select_statement(statement_scanner, with_clause=with_clause))
+        else:
+            raise SqlParseError(f"未知语句类型: {statement_scanner}")
+
+    return statement_list
+
+
+def parse_create_table_statement(scanner: TokenScanner) -> DDLCreateTableStatement:
+    # 解析字段、索引括号前的部分
+    scanner.match("CREATE", "TABLE")
+    if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
+    table_name = scanner.pop_as_source().strip("`")  # TODO 待改为 TableNameExpression，并支持 schema_name
+
+    # 解析字段和索引
+    columns: List[DDLColumnExpression] = []
+    primary_key: Optional[DDLPrimaryIndexExpression] = None
+    unique_key: List[DDLUniqueIndexExpression] = []
+    key: List[DDLNormalIndexExpression] = []
+    fulltext_key: List[DDLFulltextIndexExpression] = []
+    foreign_key: List[DDLForeignKeyExpression] = []
+    for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+        if is_ddl_primary_index_expression(group_scanner):
+            primary_key = parse_ddl_primary_index_expression(group_scanner)
+        elif is_ddl_unique_index_expression(group_scanner):
+            unique_key.append(parse_ddl_unique_index_expression(group_scanner))
+        elif is_ddl_normal_index_expression(group_scanner):
+            key.append(parse_ddl_normal_index_expression(group_scanner))
+        elif is_ddl_fulltext_expression(group_scanner):
+            fulltext_key.append(parse_ddl_fulltext_expression(group_scanner))
+        elif is_ddl_foreign_key_expression(group_scanner):
+            foreign_key.append(parse_dll_foreign_key_expression(group_scanner))
+        else:
+            columns.append(parse_ddl_column_expression(group_scanner))
+
+    # 解析表属性
+    comment: Optional[str] = None
+    engine: Optional[str] = None
+    auto_increment: Optional[int] = None
+    default_charset: Optional[str] = None
+    collate: Optional[str] = None
+    row_format: Optional[str] = None
+    states_persistent: Optional[str] = None
+    while not scanner.is_finish:
+        if scanner.search_and_move("ENGINE"):
+            scanner.search_and_move("=")
+            engine = scanner.pop_as_source()
+        elif scanner.search_and_move("AUTO_INCREMENT"):
+            scanner.match("=")
+            auto_increment = int(scanner.pop_as_source())
+        elif scanner.search_and_move("DEFAULT", "CHARSET"):
+            scanner.match("=")
+            default_charset = scanner.pop_as_source()
+        elif scanner.search_and_move("ROW_FORMAT"):
+            scanner.match("=")
+            row_format = scanner.pop_as_source()
+        elif scanner.search_and_move("COLLATE"):
+            scanner.match("=")
+            collate = scanner.pop_as_source()
+        elif scanner.search_and_move("COMMENT"):
+            scanner.match("=")
+            comment = scanner.pop_as_source()
+        elif scanner.search_and_move("STATS_PERSISTENT"):
+            scanner.match("=")
+            states_persistent = scanner.pop_as_source()
+        else:
+            raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
+    scanner.search_and_move(";")
+
+    return DDLCreateTableStatement(
+        table_name=table_name,
+        comment=comment,
+        if_not_exists=if_not_exists,
+        columns=columns,
+        primary_key=primary_key,
+        unique_key=unique_key,
+        key=key,
+        fulltext_key=fulltext_key,
+        foreign_key=foreign_key,
+        engine=engine,
+        auto_increment=auto_increment,
+        default_charset=default_charset,
+        collate=collate,
+        row_format=row_format,
+        states_persistent=states_persistent
+    )
```

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/static/mysql.py` & `metasequoia-sql-0.1.1/metasequoia_sql/static/mysql.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql/static/other.py` & `metasequoia-sql-0.1.1/metasequoia_sql/static/other.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql.egg-info/PKG-INFO` & `metasequoia-sql-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.1.0
+Version: 0.1.1
 Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
@@ -37,29 +37,30 @@
 ```
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
-from metasequoia_sql.parser.mysql_parser import parse_mysql_create_table_statement
+from metasequoia_sql.parser.common import parse_create_table_statement
+from metasequoia_sql.common.token_scanner import build_token_scanner
 
-statement = parse_mysql_create_table_statement("your sql")
+statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
-from metasequoia_sql.parser.mysql_parser import parse_mysql_create_table_statement
+from metasequoia_sql.parser.common import parse_create_table_statement
 from metasequoia_sql.translate import *
+from metasequoia_sql.common.token_scanner import build_token_scanner
 
-statement = ddl_create_table_statement_to_hive(
-    ddl_create_table_statement_from_mysql(parse_mysql_create_table_statement("your sql")))
+statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
@@ -127,14 +128,28 @@
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
 ## 修改记录
 
+#### 0.1.0 > 0.1.1
+
+新增：
+- `INSERT` 语句解析逻辑
+- 一次性解析多条 SQL 语句
+
+优化：
+- 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
+- 清理多余对象
+- TokenScanner 使用方法
+
+修复：
+- `WITH` 语句解析报错的 Bug 修复
+
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
```

### Comparing `metasequoia-sql-0.1.0/metasequoia_sql.egg-info/SOURCES.txt` & `metasequoia-sql-0.1.1/metasequoia_sql.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 LICENSE
 README.md
 setup.py
-auto_test/__init__.py
-auto_test/sql_basic_tutorial.py
 metasequoia_sql/__init__.py
 metasequoia_sql/errors.py
 metasequoia_sql.egg-info/PKG-INFO
 metasequoia_sql.egg-info/SOURCES.txt
 metasequoia_sql.egg-info/dependency_links.txt
 metasequoia_sql.egg-info/top_level.txt
+metasequoia_sql/analyzer/__init__.py
+metasequoia_sql/analyzer/consanguinity.py
 metasequoia_sql/ast/__init__.py
 metasequoia_sql/ast/functions.py
 metasequoia_sql/ast/nodes.py
 metasequoia_sql/ast/parser.py
 metasequoia_sql/common/__init__.py
+metasequoia_sql/common/base_scanner.py
 metasequoia_sql/common/basic.py
 metasequoia_sql/common/text_scanner.py
 metasequoia_sql/common/token_scanner.py
 metasequoia_sql/objects/__init__.py
-metasequoia_sql/objects/common.py
 metasequoia_sql/objects/core.py
-metasequoia_sql/objects/data_source.py
-metasequoia_sql/objects/hive.py
-metasequoia_sql/objects/mysql.py
 metasequoia_sql/parser/__init__.py
 metasequoia_sql/parser/common.py
-metasequoia_sql/parser/mysql_parser.py
-metasequoia_sql/statements/__init__.py
-metasequoia_sql/statements/mysql.py
 metasequoia_sql/static/__init__.py
 metasequoia_sql/static/common.py
 metasequoia_sql/static/mysql.py
-metasequoia_sql/static/other.py
-metasequoia_sql/translate/__init__.py
-metasequoia_sql/translate/from_mysql.py
-metasequoia_sql/translate/full_statement.py
-metasequoia_sql/translate/to_hive.py
-scripts/__init__.py
-scripts/temp_test.py
-scripts/unittest_maker.py
-scripts/demo/__init__.py
-scripts/demo/sql_basic_tutorial.py
-scripts/demo/with_demo.py
+metasequoia_sql/static/other.py
```

### Comparing `metasequoia-sql-0.1.0/setup.py` & `metasequoia-sql-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.1.0",
+    version="0.1.1",
     description="SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
     license="MIT License",
-    packages=find_packages(),
+    packages=[package for package in find_packages() if package.startswith("metasequoia_sql")],
     platforms=["all"],
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

