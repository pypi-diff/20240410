# Comparing `tmp/webwithpy-0.7.4.2.tar.gz` & `tmp/webwithpy-0.7.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.4.2.tar", max compression
+gzip compressed data, was "webwithpy-0.7.4.3.tar", max compression
```

## Comparing `webwithpy-0.7.4.2.tar` & `webwithpy-0.7.4.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.2/LICENSE
--rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.2/README.md
--rw-r--r--   0        0        0      503 2024-04-09 09:19:41.823248 webwithpy-0.7.4.2/pyproject.toml
--rw-r--r--   0        0        0       99 2024-04-09 09:19:41.819248 webwithpy-0.7.4.2/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/app.py
--rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4418 2024-04-09 09:13:10.442038 webwithpy-0.7.4.2/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6057 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5317 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/routing/router.py
--rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.2/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.3/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.3/README.md
+-rw-r--r--   0        0        0      503 2024-04-09 09:26:12.465690 webwithpy-0.7.4.3/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-04-09 09:19:41.819248 webwithpy-0.7.4.3/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/app.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.3/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6057 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5317 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.3/PKG-INFO
```

### Comparing `webwithpy-0.7.4.2/LICENSE` & `webwithpy-0.7.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/README.md` & `webwithpy-0.7.4.3/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.4.3/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.4.3/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.4.3/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/html/data/ast.py` & `webwithpy-0.7.4.3/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/html/forms.py` & `webwithpy-0.7.4.3/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/html/lexer.py` & `webwithpy-0.7.4.3/webwithpy/html/lexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,15 @@
             # make it so that everything outside the brackets is also parsed
             # append left
             tokens.append(Token(data=line[0:l_bracket], method=Methods.HTML))
             # append middle
             middle_line = self.__filter_pyht(line=line[l_bracket + 2 : r_bracket])
             tokens.append(self.get_token_by_line(middle_line))
 
-            file_data[idx] = (
-                file_data[idx][:l_bracket] + file_data[idx][r_bracket + 2 :]
-            )
+            file_data[idx] = file_data[idx][r_bracket + 2 :]
 
             if "{{" in line:
                 continue
 
             # append right side of code
             tokens.append(
                 Token(data=line[r_bracket + 2 : len(line)], method=Methods.HTML)
```

### Comparing `webwithpy-0.7.4.2/webwithpy/html/parser.py` & `webwithpy-0.7.4.3/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/html/pyhtml.py` & `webwithpy-0.7.4.3/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/html/renderer.py` & `webwithpy-0.7.4.3/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/http/cookies.py` & `webwithpy-0.7.4.3/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/http/handler.py` & `webwithpy-0.7.4.3/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/http/request.py` & `webwithpy-0.7.4.3/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/http/response.py` & `webwithpy-0.7.4.3/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/http/urls.py` & `webwithpy-0.7.4.3/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/auth.py` & `webwithpy-0.7.4.3/webwithpy/orm/auth.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/core.py` & `webwithpy-0.7.4.3/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.4.3/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.4.3/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.4.3/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.4.3/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.4.3/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.4.3/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.4.3/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.4.3/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/orm/objects/query.py` & `webwithpy-0.7.4.3/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/persistence.py` & `webwithpy-0.7.4.3/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/routing/methods.py` & `webwithpy-0.7.4.3/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/routing/router.py` & `webwithpy-0.7.4.3/webwithpy/routing/router.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/static/form.css` & `webwithpy-0.7.4.3/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.4.3/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/webwithpy/webwithpy.py` & `webwithpy-0.7.4.3/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.2/PKG-INFO` & `webwithpy-0.7.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.4.2
+Version: 0.7.4.3
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

