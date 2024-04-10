# Comparing `tmp/expyvalidations-0.0.1.tar.gz` & `tmp/expyvalidations-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expyvalidations-0.0.1.tar", last modified: Sun Mar 31 18:59:43 2024, max compression
+gzip compressed data, was "expyvalidations-0.0.2.tar", last modified: Wed Apr 10 17:22:19 2024, max compression
```

## Comparing `expyvalidations-0.0.1.tar` & `expyvalidations-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1071 2024-03-27 18:40:13.000000 expyvalidations-0.0.1/LICENSE
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      603 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/PKG-INFO
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/expyvalidations/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       64 2024-03-31 16:15:04.000000 expyvalidations-0.0.1/expyvalidations/__init__.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      632 2024-03-31 16:20:05.000000 expyvalidations-0.0.1/expyvalidations/config.py
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/expyvalidations/excel/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-27 18:27:29.000000 expyvalidations-0.0.1/expyvalidations/excel/__init__.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     9904 2024-03-31 17:45:54.000000 expyvalidations-0.0.1/expyvalidations/excel/checks.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)    11332 2024-03-31 17:46:10.000000 expyvalidations-0.0.1/expyvalidations/excel/excel.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     3964 2024-03-31 17:40:55.000000 expyvalidations-0.0.1/expyvalidations/excel/servicos.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     9192 2024-03-31 15:24:36.000000 expyvalidations-0.0.1/expyvalidations/utils.py
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/expyvalidations.egg-info/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      603 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/PKG-INFO
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      468 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/SOURCES.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/dependency_links.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/not-zip-safe
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       56 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/requires.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       16 2024-03-31 18:59:43.000000 expyvalidations-0.0.1/expyvalidations.egg-info/top_level.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       38 2024-03-31 18:59:43.961845 expyvalidations-0.0.1/setup.cfg
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1210 2024-03-31 18:59:29.000000 expyvalidations-0.0.1/setup.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1071 2024-03-27 18:40:13.000000 expyvalidations-0.0.2/LICENSE
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      753 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/PKG-INFO
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       64 2024-04-10 17:22:11.000000 expyvalidations-0.0.2/expyvalidations/__init__.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      631 2024-04-09 22:31:52.000000 expyvalidations-0.0.2/expyvalidations/config.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations/excel/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-27 18:27:29.000000 expyvalidations-0.0.2/expyvalidations/excel/__init__.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     5309 2024-04-09 23:17:48.000000 expyvalidations-0.0.2/expyvalidations/excel/checks.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)    11428 2024-04-09 23:16:18.000000 expyvalidations-0.0.2/expyvalidations/excel/excel.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      763 2024-04-09 23:16:52.000000 expyvalidations-0.0.2/expyvalidations/excel/model.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     3117 2024-04-10 17:20:28.000000 expyvalidations-0.0.2/expyvalidations/excel/servicos.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     9192 2024-04-09 21:58:11.000000 expyvalidations-0.0.2/expyvalidations/utils.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations.egg-info/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      753 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/PKG-INFO
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      499 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-03-31 18:59:43.000000 expyvalidations-0.0.2/expyvalidations.egg-info/not-zip-safe
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       56 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/requires.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       16 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/top_level.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       38 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/setup.cfg
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1357 2024-03-31 19:06:08.000000 expyvalidations-0.0.2/setup.py
```

### Comparing `expyvalidations-0.0.1/LICENSE` & `expyvalidations-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `expyvalidations-0.0.1/PKG-INFO` & `expyvalidations-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: expyvalidations
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sheets data validation
 Home-page: https://github.com/exebixel/expyvalidations
 Author: exebixel
 Author-email: ezequielnat7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `expyvalidations-0.0.1/expyvalidations/config.py` & `expyvalidations-0.0.2/expyvalidations/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def config_bar_excel():
     """ Configuração padrão da barra de progresso os módulos de excel
     """
     config_handler.set_global(bar=None,
                               spinner=False,
-                              receipt=False,
+                              receipt=True,
                               enrich_print=False,
                               stats=False,
                               elapsed=False)
 
 
 class CheckException(Exception):
     """ Exception especifica para algum erro de verificação do modulo de excel
```

### Comparing `expyvalidations-0.0.1/expyvalidations/excel/excel.py` & `expyvalidations-0.0.2/expyvalidations/excel/excel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 import re
-import sys
-from typing import Callable, Any, Literal, Union
+from typing import Callable, Any, Union
 from alive_progress import alive_bar
 
 import pandas as pd
 from expyvalidations import config
 from expyvalidations.config import CheckException
 from expyvalidations.excel.checks import CheckTypes
+from expyvalidations.excel.model import ColumnDefinition, Error, Types, TypeError
 from expyvalidations.utils import string_normalize
 
 
 class ExpyValidations:
 
     def __init__(
         self,
         path_file: str,
         sheet_name: str = "sheet",
-        book: pd.ExcelFile = None,
         header_row: int = 1,
-        verbose: bool = False,
     ):
 
-        self.column_details: list = []
-        self.verbose: bool = verbose
+        self.column_details: list[ColumnDefinition] = []
         self.__book = pd.ExcelFile(path_file)
 
-        self.__errors_list: list = []
-        self.erros: bool = False
+        self.__errors_list: list[Error] = []
         """
         indica se ouve algum erro nas validações da planilha
         se tiver erro o método data_all não deve
         retornar dados
         """
 
         self.excel: pd.DataFrame
         try:
-            excel = pd.read_excel(self.__book, self.sheet_name(sheet_name), header=header_row)
+            excel = pd.read_excel(
+                self.__book, self.sheet_name(sheet_name), header=header_row
+            )
             # retirando linhas e colunas em brando do Data Frame
             excel = excel.dropna(how="all")
             excel.columns = excel.columns.astype("string")
             excel = excel.loc[:, ~excel.columns.str.contains("^Unnamed")]
             excel = excel.astype(object)
             excel = excel.where(pd.notnull(excel), None)
             self.excel = excel
 
         except ValueError as exp:
             raise ValueError(exp)
 
         self.__header_row = header_row
-        self.add_row_column()
 
         self.checks = CheckTypes()
 
     def sheet_name(self, search: str) -> str:
         """
         Função responsável por pesquisa a string do parâmetro 'search'
         nas planilhas (sheets) do 'book' especificado no __init__
@@ -92,27 +89,15 @@
 
     def add_column(
         self,
         key: str,
         name: Union[str, list[str]],
         required: bool = True,
         default: Any = None,
-        types: Literal[
-            "string",
-            "int",
-            "float",
-            "bool",
-            "date",
-            "time",
-            "email",
-            "cel",
-            "cpf",
-            "sex",
-        ] = "string",
-        length: int = 0,
+        types: Types = "string",
         custom_function_before: Callable = None,
         custom_function_after: Callable = None,
     ):
         """
         Função responsável por adicionar as colunas que serão lidas
         da planilha \n
         Parâmetros: \n
@@ -142,35 +127,41 @@
         excel = self.excel
 
         try:
             column_name = self.column_name(name)
         except ValueError as exp:
             if required:
                 print(f"ERROR! Required {exp}")
-                self.erros = True
-            elif self.verbose and not config.NO_WARNING:
+                self.__errors_list.append(
+                    Error(
+                        row=self.__header_row,
+                        column=0,
+                        message=f"Required {exp}",
+                    )
+                )
+            elif config.NO_WARNING:
                 print(f"WARNING! {exp}")
             excel[key] = default
         else:
             excel.rename({column_name: key}, axis="columns", inplace=True)
 
         self.column_details.append(
-            {
-                "key": key,
-                "types": types,
-                "default": default,
-                "length": length,
-                "custom_function_before": custom_function_before,
-                "custom_function_after": custom_function_after,
-            }
+            ColumnDefinition(
+                key=key,
+                types=types,
+                default=default,
+                custom_function_before=custom_function_before,
+                custom_function_after=custom_function_after,
+            )
         )
 
     def check_all(
         self,
-        check_row: Callable = None,
+        check_row_before: Callable = None,
+        check_row_after: Callable = None,
         check_duplicated_keys: list[str] = None,
         checks_final: list[Callable] = None,
     ) -> bool:
         """
         Função responsável por verificar todas as colunas
         da planilha
 
@@ -179,154 +170,152 @@
         checks_final: lista de funções que serão executadas
             considerando todos os dados da planilha
 
         Retorno:
         False se NÃO ouve erros na verificação
         True se ouve erros na verificação
         """
-        if self.erros:
+        if self.__errors_list:
             head = self.__header_row + 1
             print(f"ERROS FOUND! REMENBER HEADER ROW = {head}")
-            sys.exit(1)
+            raise ValueError("ERROS FOUND! REMENBER HEADER ROW = {head}")
 
         excel = self.excel
 
         # configuração padrão da barra de progresso
         config.config_bar_excel()
 
         # verificando todas as colunas
         with alive_bar(
             len(excel.index) * len(self.column_details), title="Checking for columns..."
         ) as pbar:
             # Verificações por coluna
             for column in self.column_details:
                 for index in excel.index:
-                    value = excel.at[index, column["key"]]
-                    invalid = self.check_value(value=value, index=index, **column)
-                    if invalid and not self.erros:
-                        self.erros = True
+                    value = excel.at[index, column.key]
+                    self.check_value(value=value, index=index, **column.model_dump())
                     pbar()
 
         # Verificações por linha
-        with alive_bar(len(excel.index), title="Checking for rows...") as pbar:
-            if check_row is not None:
+        if check_row_after is not None:
+            with alive_bar(len(excel.index), title="Checking for rows...") as pbar:
+                list_colums = list(map(lambda col: col.key, self.column_details))
                 for row in excel.index:
                     try:
-                        data = check_row(excel.at[row, "_row"], excel.loc[row].copy())
+                        data = excel[list_colums].loc[row].to_dict()
+                        data = check_row_after(data)
                         for key, value in data.items():
                             excel.at[row, key] = value
 
-                    except CheckException:
-                        self.erros = True
+                    except CheckException as exp:
+                        self.__errors_list.append(
+                            Error(
+                                row=self.__row(row),
+                                column=None,
+                                message=str(exp),
+                            )
+                        )
                     pbar()
 
         # Verificações totais (duplicação de dados)
         if check_duplicated_keys is not None:
             try:
                 excel = self.checks.check_duplications(
                     data=excel, keys=check_duplicated_keys
                 )
-            except CheckException:
-                self.erros = True
-
-        if checks_final is not None:
-            for check in checks_final:
-                try:
-                    excel = check(excel)
-                except CheckException:
-                    self.erros = True
-                pbar()
+            except CheckException as exp:
+                for error in exp.args[0]:
+                    self.__errors_list.append(
+                        Error(
+                            type=TypeError.DUPLICATED,
+                            row=error["line"],
+                            column=error["column"],
+                            message=error["error"],
+                        )
+                    )
+
+        # if checks_final is not None:
+        #     for check in checks_final:
+        #         try:
+        #             excel = check(excel)
+        #         except CheckException:
+        #             self.erros = True
+        #         pbar()
 
         self.excel = excel
-        return self.erros
+        return True if self.__errors_list else False
 
     def check_value(
         self,
         value: Any,
         key: str,
         types: str,
         index: int,
         default: Any = None,
         length: int = 0,
         custom_function_before: Callable = None,
         custom_function_after: Callable = None,
-    ) -> bool:
+    ) -> None:
         """Executa todas as verificações em um valor especifico,
         retorna True um False para caso as verificações passarem ou não
         """
         excel = self.excel
-        erros = False
-
-        # Pega referencia fa função de verificação padrão
-        check_function = self.checks.get_type_function(types=types)
 
-        # Verificações customizadas que serão feitas antes
-        # das verificações padrões
+        functions = []
         if custom_function_before is not None:
-            try:
-                value = custom_function_before(
-                    value=value, key=key, default=default, row=self.row(index)
-                )
-            except CheckException:
-                erros = True
-
-        # Executa a verificação padrão
-        try:
-            value = check_function(value, key=key, default=default, row=self.row(index))
-        except CheckException:
-            erros = True
-
-        # Verificação de tamanho de string
-        if length not in (0, None):
-            try:
-                value = self.checks.check_length(
-                    value, key=key, row=self.row(index), length=length
-                )
-            except CheckException:
-                erros = True
-
-        # Executa a função de verificações customizada
-        # depois das verificações padrão
+            functions.append(custom_function_before)
+        functions.append(self.checks.get_type_function(types))
         if custom_function_after is not None:
+            functions.append(custom_function_after)
+
+        for func in functions:
             try:
-                value = custom_function_after(
-                    value=value, key=key, default=default, row=self.row(index)
+                value = func(value)
+            except CheckException as exp:
+                self.__errors_list.append(
+                    Error(
+                        row=self.__row(index),
+                        column=key,
+                        message=str(exp),
+                    )
                 )
-            except CheckException:
-                erros = True
+                break
 
         excel.at[index, key] = value
-        return erros
-
-    def clean_columns(self):
-        """
-        Deleta as colunas do data frame que não foram adicionadas pelo
-        'add_column'
-        """
-        columns = list(map(lambda col: col["key"], self.column_details))
-        columns.append("_row")
-        self.excel = self.excel[columns]
 
-    def row(self, index: int) -> int:
+    def __row(self, index: int) -> int:
         """
         Retorna a linha do respectivo index passado
         """
         return index + self.__header_row + 2
 
-    def add_row_column(self):
-        """Adicionar uma columa ao datafreme chamada 'row'
-        com o número de cada linha
-        """
-        excel = self.excel
-        rows = []
-        for i in excel.index:
-            rows.append(self.row(i))
-        excel["_row"] = rows
-
     def data_all(self) -> dict:
         excel = self.excel
         if excel.empty:
             return {}
 
-        excel = excel.drop(columns="_row")
+        list_colums = list(map(lambda col: col.key, self.column_details))
+
         excel = excel.where(pd.notnull(excel), None)
-        return excel.to_dict("records")
+        return excel[list_colums].to_dict("records")
+
+    def print_errors(self):
+        for error in self.__errors_list:
+            if error.column is None:
+                print(f"{error.type.value}! in line {error.row}: {error.message}")
+            else:
+                print(
+                    f"{error.type.value}! in line {error.row}, Column {error.column}: {error.message}"
+                )
+
+    def get_all_errors(self) -> list[dict]:
+        errors = []
+        for error in self.__errors_list:
+            errors.append(
+                {
+                    "type": error.type.value,
+                    "row": error.row,
+                    "column": error.column,
+                    "message": error.message,
+                }
+            )
+        return errors
```

### Comparing `expyvalidations-0.0.1/expyvalidations/excel/servicos.py` & `expyvalidations-0.0.2/expyvalidations/excel/servicos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import json
 import sys
 from typing import Any
 
 # from alive_progress import alive_bar
 from pandas import ExcelFile
+
 # from oneparams.api.gservs import Gservis
 # from oneparams.api.servicos import ApiServicos
 from expyvalidations.config import CheckException
 from expyvalidations.excel.excel import ExpyValidations
 
 
 def servico(book: ExcelFile, header: int = 1, reset: bool = False):
@@ -22,109 +24,85 @@
     """
     # one = ApiServicos()
     print("analyzing spreadsheet")
 
     ex = ExpyValidations(path_file=book, sheet_name="Servico", header_row=header)
 
     ex.add_column(key="flagAtivo", name="ativo", required=False, default=True)
-    ex.add_column(key="descricao",
-                  name="nome",
-                  length=50,
-                  custom_function_after=check_descricao)
-    ex.add_column(key="gservId",
-                  name="grupo",
-                  length=50,
-                  custom_function_after=check_descricao)
+    ex.add_column(key="descricao", name="nome", custom_function_before=check_descricao)
+    ex.add_column(key="gservId", name="grupo", custom_function_after=check_descricao)
     ex.add_column(key="preco", name="valor", default=1, types="float")
-    ex.add_column(key="comissao",
-                  name="comissao",
-                  default=0,
-                  types="float",
-                  custom_function_after=check_comissao)
-    ex.add_column(key="tempoExecucao",
-                  name="execucao",
-                  default="00:30:00",
-                  types="time")
-    ex.add_column(key="custosGerais",
-                  name="custo",
-                  required=False,
-                  default=0,
-                  types="float")
-    ex.add_column(key="intervaloMarcacao",
-                  name="intervalo",
-                  required=False,
-                  default="00:10:00",
-                  types="time")
-    ex.add_column(key="permiteEncaixe",
-                  name="encaixe",
-                  required=False,
-                  default=True,
-                  types="bool")
-    ex.add_column(key="permiteSimultaneidade",
-                  name="simultaneidade",
-                  required=False,
-                  default=True,
-                  types="bool")
-    ex.add_column(key="valPercComissao",
-                  name="tipo comissao",
-                  required=False,
-                  default="P")
-    ex.add_column(key="valPercCustos",
-                  name="tipo custo",
-                  required=False,
-                  default="P")
-    ex.add_column(key="flagMobilidade",
-                  name="mobilidade",
-                  required=False,
-                  default=True,
-                  types="bool")
-    ex.clean_columns()
-
-    invalid = ex.check_all(check_duplicated_keys=["descricao"])
-    if invalid:
-        sys.exit(1)
+    ex.add_column(
+        key="comissao",
+        name="comissao",
+        default=0,
+        types="float",
+        custom_function_after=check_comissao,
+    )
+    ex.add_column(
+        key="tempoExecucao", name="execucao", default="00:30:00", types="time"
+    )
+    ex.add_column(
+        key="custosGerais", name="custo", required=False, default=0, types="float"
+    )
+    ex.add_column(
+        key="intervaloMarcacao",
+        name="intervalo",
+        required=False,
+        default="00:10:00",
+        types="time",
+    )
+    ex.add_column(
+        key="permiteEncaixe", name="encaixe", required=False, default=True, types="bool"
+    )
+    ex.add_column(
+        key="permiteSimultaneidade",
+        name="simultaneidade",
+        required=False,
+        default=True,
+        types="bool",
+    )
+    ex.add_column(
+        key="valPercComissao", name="tipo comissao", required=False, default="P"
+    )
+    ex.add_column(key="valPercCustos", name="tipo custo", required=False, default="P")
+    ex.add_column(
+        key="flagMobilidade",
+        name="mobilidade",
+        required=False,
+        default=True,
+        types="bool",
+    )
+
+    ex.check_all(check_row_before=row_test, check_duplicated_keys=["descricao"])
+    # ex.print_errors()
+    # print(ex.get_all_errors())
 
-    print("creating services")
     data = ex.data_all()
-    print(data)
-
-    # len_data = len(data)
-    # if reset:
-    #     len_data += len(one.items)
-
-    # config_bar_api()
-    # with alive_bar(len_data) as pbar:
-    #     if reset:
-    #         for i in list(one.items):
-    #             one.delete(i)
-    #             pbar()
-
-    #     for row in data:
-    #         one.diff_item(row)
-    #         pbar()
-
-    # with alive_bar() as pbar:
-    #     grupo = Gservis()
-    #     grupo.get_all()
-    #     grupo.clear()
+    print(json.dumps(data, indent=4))
 
 
-def check_descricao(value: Any, key: str, row: int, default: Any) -> Any:
+def check_descricao(value: Any) -> str:
     if value is None:
-        print(f"ERROR! in line {row}, Column {key}, empty value")
-        raise CheckException
+        raise CheckException("Empty value")
     return value
 
 
-def check_comissao(value: Any, key: str, row: int, default: Any) -> float:
+def check_comissao(value: Any) -> float:
     try:
         value = float(value)
-    except ValueError as exp:
-        raise CheckException from exp
+    except (ValueError, TypeError) as exp:
+        raise CheckException(f"Value '{value}' is not a valid number")
 
     if value <= 1:
         value = value * 100
     return value
 
 
+def row_test(data: dict) -> dict:
+    # if data["comissao"] < 50:
+    #     raise CheckException("Comissão menor que 30")
+    return data
+
+
 if __name__ == "__main__":
     servico("Parametrização Sistema One Beleza.xlsx")
```

### Comparing `expyvalidations-0.0.1/expyvalidations/utils.py` & `expyvalidations-0.0.2/expyvalidations/utils.py`

 * *Files identical despite different names*

### Comparing `expyvalidations-0.0.1/expyvalidations.egg-info/PKG-INFO` & `expyvalidations-0.0.2/expyvalidations.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: expyvalidations
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sheets data validation
 Home-page: https://github.com/exebixel/expyvalidations
 Author: exebixel
 Author-email: ezequielnat7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `expyvalidations-0.0.1/setup.py` & `expyvalidations-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     author_email="ezequielnat7@gmail.com",
     url="https://github.com/exebixel/expyvalidations",
     install_requires=requirements,
     python_requires=">=3.7",
     classifiers=[
         "Operating System :: OS Independent",
         "Environment :: Console",
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'License :: OSI Approved :: MIT License',
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     zip_safe=False,
 )
```

