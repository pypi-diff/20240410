# Comparing `tmp/arrow_mssql-0.0.7.tar.gz` & `tmp/arrow_mssql-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_mssql-0.0.7.tar", max compression
+gzip compressed data, was "arrow_mssql-0.0.8.tar", max compression
```

## Comparing `arrow_mssql-0.0.7.tar` & `arrow_mssql-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0      130 2024-03-23 22:01:58.725215 arrow_mssql-0.0.7/arrow_mssql/__init__.py
--rw-r--r--   0        0        0     1328 2024-03-23 21:59:39.992092 arrow_mssql-0.0.7/arrow_mssql/connector.py
--rw-r--r--   0        0        0     2553 2024-03-16 23:14:01.023608 arrow_mssql-0.0.7/arrow_mssql/datatypes.py
--rw-r--r--   0        0        0     3602 2024-03-23 22:00:36.433610 arrow_mssql-0.0.7/arrow_mssql/export.py
--rw-r--r--   0        0        0     3433 2024-03-23 22:01:52.803234 arrow_mssql-0.0.7/arrow_mssql/schemas.py
--rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.7/arrow_mssql/utils.py
--rw-r--r--   0        0        0      690 2024-03-23 22:02:38.473846 arrow_mssql-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1291 2024-03-17 00:30:08.927273 arrow_mssql-0.0.7/README.md
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 arrow_mssql-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-04-10 18:46:31.679270 arrow_mssql-0.0.8/arrow_mssql/__init__.py
+-rw-r--r--   0        0        0     1355 2024-04-02 19:24:19.265370 arrow_mssql-0.0.8/arrow_mssql/connector.py
+-rw-r--r--   0        0        0     3609 2024-04-02 19:13:05.501619 arrow_mssql-0.0.8/arrow_mssql/export.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.8/arrow_mssql/input/__init__.py
+-rw-r--r--   0        0        0     3608 2024-04-10 18:24:20.692624 arrow_mssql-0.0.8/arrow_mssql/input/datatypes.py
+-rw-r--r--   0        0        0     1514 2024-04-10 15:01:16.386256 arrow_mssql-0.0.8/arrow_mssql/input/schema.py
+-rw-r--r--   0        0        0     1288 2024-04-10 18:36:45.564350 arrow_mssql-0.0.8/arrow_mssql/iport.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.8/arrow_mssql/output/__init__.py
+-rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.8/arrow_mssql/output/datatypes.py
+-rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.8/arrow_mssql/output/schemas.py
+-rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.8/arrow_mssql/utils.py
+-rw-r--r--   0        0        0      753 2024-04-10 18:43:07.395117 arrow_mssql-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1594 2024-04-10 18:46:28.079048 arrow_mssql-0.0.8/README.md
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 arrow_mssql-0.0.8/PKG-INFO
```

### Comparing `arrow_mssql-0.0.7/arrow_mssql/connector.py` & `arrow_mssql-0.0.8/arrow_mssql/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,33 +29,33 @@
         frac // 1000,
         datetime.timezone(datetime.timedelta(hours=tz_hour, minutes=tz_minutes)),
     )
 
 
 def do_connect(
     *args,
-    **kwargs: Any,
+    **kwargs: Any
 ) -> None:
     
     con = odbc.connect(
         *args,
         **kwargs,
     )
 
     con.add_output_converter(
         -155, 
         datetimeoffset_to_datetime
     )
     
-    # with(nolock) ativado
-    con.execute(
-        'set transaction '
-        'isolation level '
-        'read uncommitted;'
-    )
+    if 'autocommit' not in kwargs:
+        con.execute(
+            'set transaction '
+            'isolation level '
+            'read uncommitted;'
+        )
 
     with closing(con.cursor()) as cur:
         cur.execute("SET DATEFIRST 1")
 
     return con
```

### Comparing `arrow_mssql-0.0.7/arrow_mssql/datatypes.py` & `arrow_mssql-0.0.8/arrow_mssql/output/datatypes.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.7/arrow_mssql/export.py` & `arrow_mssql-0.0.8/arrow_mssql/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pyarrow as pa
 from .connector import raw_sql
 from textwrap import dedent
 from typing import (
     Iterable, 
 )
-from .schemas import get_schema
+from .output.schemas import get_schema
 from .utils import is_query
 import sqlglot as sg
 
 
 def cursor_arrow(
     driver: str,
     name: str,
```

### Comparing `arrow_mssql-0.0.7/arrow_mssql/schemas.py` & `arrow_mssql-0.0.8/arrow_mssql/output/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pyarrow as pa
-from .connector import raw_sql
+from ..connector import raw_sql
 from textwrap import dedent
 from typing import (
     Any, 
     Literal, 
     Callable
 )
 from .datatypes import map_typs
 from operator import itemgetter
 import sqlglot as sg
 import sqlglot.expressions as sge
-from .utils import (
+from ..utils import (
     is_query,
     rename_col
 )
 
 
 def schema_query_or_table(
     driver: str,
```

### Comparing `arrow_mssql-0.0.7/arrow_mssql/utils.py` & `arrow_mssql-0.0.8/arrow_mssql/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.7/pyproject.toml` & `arrow_mssql-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arrow-mssql"
-version = "0.0.07"
-description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv"
+version = "0.0.08"
+description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server"
 authors = ["Marcus Holanda <mvsh777@hotmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Natural Language :: Portuguese (Brazilian)",
     "Programming Language :: PL/SQL",
     "Programming Language :: Python :: 3.11"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `arrow_mssql-0.0.7/README.md` & `arrow_mssql-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 ## O que é o Arrow-mssql ?
 
 é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
 
+Agora é possível importar um arquivo *.parquet* para uma tabela do sql server.
+
 ## Instalação
 
 ```bash
 pip install arrow-mssql
 ```
 
 ## Conexão
@@ -52,8 +54,17 @@
     DRIVER, 
     'SELECT N1, N2 FROM NOME_TABELA WHERE N1 = 0', 
     schema='dbo',
     database='seu_banco', 
     path='destino.parquet'
 )
 
+# IMPORTAR .parquet para tabela temporaria do ssms
+# o retornor é um cursor referente a conexao com o banco de dados
+with write_parquet(
+    DRIVER, 
+    '##teste', 
+    path='origem.parquet'
+) as C:
+
+    ...
 ```
```

### Comparing `arrow_mssql-0.0.7/PKG-INFO` & `arrow_mssql-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: arrow-mssql
-Version: 0.0.7
-Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv
+Version: 0.0.8
+Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server
 Author: Marcus Holanda
 Author-email: mvsh777@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: PL/SQL
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,16 @@
 ## O que é o Arrow-mssql ?
 
 é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
 
+Agora é possível importar um arquivo *.parquet* para uma tabela do sql server.
+
 ## Instalação
 
 ```bash
 pip install arrow-mssql
 ```
 
 ## Conexão
@@ -71,8 +73,17 @@
     DRIVER, 
     'SELECT N1, N2 FROM NOME_TABELA WHERE N1 = 0', 
     schema='dbo',
     database='seu_banco', 
     path='destino.parquet'
 )
 
+# IMPORTAR .parquet para tabela temporaria do ssms
+# o retornor é um cursor referente a conexao com o banco de dados
+with write_parquet(
+    DRIVER, 
+    '##teste', 
+    path='origem.parquet'
+) as C:
+
+    ...
 ```
```

