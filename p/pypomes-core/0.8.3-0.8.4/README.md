# Comparing `tmp/pypomes_core-0.8.3.tar.gz` & `tmp/pypomes_core-0.8.4.tar.gz`

## Comparing `pypomes_core-0.8.3.tar` & `pypomes_core-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.4/PKG-INFO
```

### Comparing `pypomes_core-0.8.3/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.4/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/__init__.py` & `pypomes_core-0.8.4/src/pypomes_core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     json_normalize_dict, json_normalize_iterable,
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .str_pomes import (
-    str_sanitize, str_between, str_split_on_mark, str_find_whitespace,
+    str_sanitize, str_split_on_mark, str_find_whitespace, str_get_between, str_get_positional,
 )
 from .validation_msgs import (
     validate_add_msgs, validate_set_msgs
 )
 from .validation_pomes import (
     VALIDATE_MSG_LANGUAGE, VALIDATE_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
@@ -77,15 +77,15 @@
     "file_from_request", "file_get_data",
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
     # list_pomes
     "list_compare", "list_flatten", "list_unflatten",
     "list_find_coupled", "list_elem_starting_with", "list_transform",
     # str_pomes
-    "str_sanitize", "str_between", "str_split_on_mark", "str_find_whitespace",
+    "str_sanitize", "str_split_on_mark", "str_find_whitespace", "str_get_between", "str_get_positional",
     # validation_msgs
     "validate_add_msgs", "validate_set_msgs",
     # validation_pomes
     "VALIDATE_MSG_LANGUAGE", "VALIDATE_MSG_PREFIX",
     "validate_value", "validate_bool", "validate_int", "validate_float", "validate_str",
     "validate_date", "validate_datetime", "validate_ints", "validate_strs",
     "validate_format_error", "validate_format_errors", "validate_unformat_errors",
```

### Comparing `pypomes_core-0.8.3/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/str_pomes.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,21 +16,21 @@
                              .replace("\n", " ") \
                              .replace("\t", " ")
     return " ".join(cleaned.split())
 
 
 def str_split_on_mark(source: str, mark: str) -> list[str]:
     """
-    Extrai, de *source*, os segmentos de texto separados por *mark*, e os retorna em uma lista.
+    Extract from *source* the text segments separated by *mark*, and return them in a *list*.
 
-    Os segmentos retornados não contem o separador.
+    The separator itself will not be in the returned list.
 
-    :param source: o texto de referência
-    :param mark: o separador
-    :return: a lista de segmentos de texto obtidos
+    :param source: the string to be inspected
+    :param mark: the separator
+    :return: the list of text segments extracted
     """
     # inicializa a variável de retorno
     result: list[str] = []
 
     pos: int = 0
     skip: int = len(mark)
     after: int = source.find(mark)
@@ -42,50 +42,69 @@
         result.append(source[pos:])
     else:
         result.append("")
 
     return result
 
 
-def str_between(source: str, from_str: str, to_str: str) -> str:
+def str_find_whitespace(source: str) -> int:
+    """
+    Locate and return the position of the first occurence of a *whitespace* character in *source*.
+
+    :param source: the string to be inspected
+    :return: the position of the first whitespace character, or -1 if none was found
     """
-    Extrai e retorna a *substring* em *source* localizada entre os delimitadores *from_st* e *to_str*.
+    # inicializa a variável de retorno
+    result: int = -1
+
+    # busca por whitespace
+    for inx, char in enumerate(source):
+        if char.isspace():
+            result = inx
+            break
+
+    return result
 
-    Retorna *None* se essa extração não for possível.
 
-    :param source: a string a ser pesquisada
-    :param from_str: o delimitador inicial
-    :param to_str: o delimitador final
-    :return: a substring procurada
+def str_get_between(source: str, from_str: str, to_str: str) -> str:
+    """
+    Extract and return the *substring* in *source* located between the delimiters *from_str* and *to_str*.
+
+    :param source: the string to be inspected
+    :param from_str: the initial delimiter
+    :param to_str: the final delimiter
+    :return: the extracted substring, or None if no substring was obtained
     """
     # inicializa a variável de retorno
     result: str | None = None
 
     pos1: int = source.find(from_str)
     if pos1 >= 0:
         pos1 += len(from_str)
         pos2: int = source.find(to_str, pos1)
         if pos2 >= pos1:
             result = source[pos1:pos2]
 
     return result
 
 
-def str_find_whitespace(source: str) -> int:
+def str_get_positional(source: str, list_origin: list[str], list_dest: list[str]) -> str:
     """
-    Localiza e retorna a posição da primeira ocorrência de *whitespace* em *source*.
+    Locate the position of *source* within *list_origin*, and return the element in the same position in *list_dest*.
 
-    Retorna *-1* se nenhum *whitespace* for encontrado.
+    :param source: the source string
+    :param list_origin: the list to be inspected
+    :param list_dest: the list containing the positionally corresponding values
+    :return: the value positionally corresponding to the source string, or None if not found
+    """
+    # declare the return variable
+    result: str | None
+
+    try:
+        pos: int = list_origin.index(source)
+        result = list_dest[pos]
+    except ValueError:
+        result = None
 
-    :param source: a string a ser pesquisada
-    :return: a posição do primeiro whitespace encontrado
-    """
-    # inicializa a variável de retorno
-    result: int = -1
+    return result
 
-    # busca por whitespace
-    for inx, char in enumerate(source):
-        if char.isspace():
-            result = inx
-            break
 
-    return result
```

### Comparing `pypomes_core-0.8.3/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.4/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.4/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/LICENSE` & `pypomes_core-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.3/pyproject.toml` & `pypomes_core-0.8.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.3/PKG-INFO` & `pypomes_core-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.3
+Version: 0.8.4
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

