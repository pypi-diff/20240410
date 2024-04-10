# Comparing `tmp/webwithpy-0.7.4.4.tar.gz` & `tmp/webwithpy-0.7.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.4.4.tar", max compression
+gzip compressed data, was "webwithpy-0.7.4.5.tar", max compression
```

## Comparing `webwithpy-0.7.4.4.tar` & `webwithpy-0.7.4.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.4/LICENSE
--rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.4/README.md
--rw-r--r--   0        0        0      554 2024-04-10 08:45:48.815584 webwithpy-0.7.4.4/pyproject.toml
--rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.4.4/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/app.py
--rw-r--r--   0        0        0     1567 2024-04-10 08:01:56.351262 webwithpy-0.7.4.4/webwithpy/commands.py
--rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.4/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6088 2024-04-10 08:26:02.365828 webwithpy-0.7.4.4/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5653 2024-04-10 08:28:05.770430 webwithpy-0.7.4.4/webwithpy/routing/router.py
--rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.4.4/webwithpy/tests/__init__.py
--rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.4.4/webwithpy/tests/case.py
--rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.4.4/webwithpy/tests/helper.py
--rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.5/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.5/README.md
+-rw-r--r--   0        0        0      571 2024-04-10 08:57:10.844320 webwithpy-0.7.4.5/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.4.5/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/app.py
+-rw-r--r--   0        0        0     1567 2024-04-10 08:01:56.351262 webwithpy-0.7.4.5/webwithpy/commands.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.5/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6088 2024-04-10 08:26:02.365828 webwithpy-0.7.4.5/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5653 2024-04-10 08:28:05.770430 webwithpy-0.7.4.5/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.4.5/webwithpy/tests/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.4.5/webwithpy/tests/case.py
+-rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.4.5/webwithpy/tests/helper.py
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 webwithpy-0.7.4.5/PKG-INFO
```

### Comparing `webwithpy-0.7.4.4/LICENSE` & `webwithpy-0.7.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/README.md` & `webwithpy-0.7.4.5/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/pyproject.toml` & `webwithpy-0.7.4.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "webwithpy"
 readme = "README.md"
-version = "0.7.4.4"
+version = "0.7.4.5"
 description = ""
 authors = ["Sven Keimpema"]
 packages = [{include = "webwithpy/**/*.*", format = ["wheel", "sdist"]}]
 
 [tool.poetry.scripts]
 webwithpy = "webwithpy:cli"
 
@@ -14,11 +14,12 @@
 asyncio = "^3.4.3"
 pyjwt = "^2.8.0"
 cython = "^3.0.5"
 bcrypt = "^3.2.0"
 setuptools = "^69.0.2"
 mysql-connector-python = "^8.3.0"
 requests-toolbelt = "^1.0.0"
+click = "^8.1.7"
 
 [build-system]
 requires = ["poetry-core", "cython", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `webwithpy-0.7.4.4/webwithpy/commands.py` & `webwithpy-0.7.4.5/webwithpy/commands.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.4.5/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.4.5/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.4.5/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/data/ast.py` & `webwithpy-0.7.4.5/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/forms.py` & `webwithpy-0.7.4.5/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/lexer.py` & `webwithpy-0.7.4.5/webwithpy/html/lexer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/parser.py` & `webwithpy-0.7.4.5/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/pyhtml.py` & `webwithpy-0.7.4.5/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/html/renderer.py` & `webwithpy-0.7.4.5/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/http/cookies.py` & `webwithpy-0.7.4.5/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/http/handler.py` & `webwithpy-0.7.4.5/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/http/request.py` & `webwithpy-0.7.4.5/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/http/response.py` & `webwithpy-0.7.4.5/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/http/urls.py` & `webwithpy-0.7.4.5/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/auth.py` & `webwithpy-0.7.4.5/webwithpy/orm/auth.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/core.py` & `webwithpy-0.7.4.5/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.4.5/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.4.5/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.4.5/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.4.5/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.4.5/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.4.5/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.4.5/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.4.5/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/orm/objects/query.py` & `webwithpy-0.7.4.5/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/persistence.py` & `webwithpy-0.7.4.5/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/routing/methods.py` & `webwithpy-0.7.4.5/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/routing/router.py` & `webwithpy-0.7.4.5/webwithpy/routing/router.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/static/form.css` & `webwithpy-0.7.4.5/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.4.5/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/tests/helper.py` & `webwithpy-0.7.4.5/webwithpy/tests/helper.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/webwithpy/webwithpy.py` & `webwithpy-0.7.4.5/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.4/PKG-INFO` & `webwithpy-0.7.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.4.4
+Version: 0.7.4.5
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bcrypt (>=3.2.0,<4.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cython (>=3.0.5,<4.0.0)
 Requires-Dist: mysql-connector-python (>=8.3.0,<9.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Description-Content-Type: text/markdown
```

