# Comparing `tmp/webwithpy-0.7.4.5.tar.gz` & `tmp/webwithpy-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.4.5.tar", max compression
+gzip compressed data, was "webwithpy-0.7.5.tar", max compression
```

## Comparing `webwithpy-0.7.4.5.tar` & `webwithpy-0.7.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.5/LICENSE
--rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.5/README.md
--rw-r--r--   0        0        0      571 2024-04-10 08:57:10.844320 webwithpy-0.7.4.5/pyproject.toml
--rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.4.5/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/app.py
--rw-r--r--   0        0        0     1567 2024-04-10 08:01:56.351262 webwithpy-0.7.4.5/webwithpy/commands.py
--rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.5/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6088 2024-04-10 08:26:02.365828 webwithpy-0.7.4.5/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5653 2024-04-10 08:28:05.770430 webwithpy-0.7.4.5/webwithpy/routing/router.py
--rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.4.5/webwithpy/tests/__init__.py
--rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.4.5/webwithpy/tests/case.py
--rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.4.5/webwithpy/tests/helper.py
--rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.5/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 webwithpy-0.7.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.5/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.5/README.md
+-rw-r--r--   0        0        0      569 2024-04-10 09:21:25.068023 webwithpy-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.5/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/app.py
+-rw-r--r--   0        0        0     1567 2024-04-10 08:01:56.351262 webwithpy-0.7.5/webwithpy/commands.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.5/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6260 2024-04-10 09:16:23.493948 webwithpy-0.7.5/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5832 2024-04-10 09:03:15.499903 webwithpy-0.7.5/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.5/webwithpy/tests/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.5/webwithpy/tests/case.py
+-rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.5/webwithpy/tests/helper.py
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.5/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 webwithpy-0.7.5/PKG-INFO
```

### Comparing `webwithpy-0.7.4.5/LICENSE` & `webwithpy-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/README.md` & `webwithpy-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/pyproject.toml` & `webwithpy-0.7.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "webwithpy"
 readme = "README.md"
-version = "0.7.4.5"
+version = "0.7.5"
 description = ""
 authors = ["Sven Keimpema"]
 packages = [{include = "webwithpy/**/*.*", format = ["wheel", "sdist"]}]
 
 [tool.poetry.scripts]
 webwithpy = "webwithpy:cli"
```

### Comparing `webwithpy-0.7.4.5/webwithpy/commands.py` & `webwithpy-0.7.5/webwithpy/commands.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.5/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.5/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.5/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/data/ast.py` & `webwithpy-0.7.5/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/forms.py` & `webwithpy-0.7.5/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/lexer.py` & `webwithpy-0.7.5/webwithpy/html/lexer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/parser.py` & `webwithpy-0.7.5/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/pyhtml.py` & `webwithpy-0.7.5/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/html/renderer.py` & `webwithpy-0.7.5/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/http/cookies.py` & `webwithpy-0.7.5/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/http/handler.py` & `webwithpy-0.7.5/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/http/request.py` & `webwithpy-0.7.5/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/http/response.py` & `webwithpy-0.7.5/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/http/urls.py` & `webwithpy-0.7.5/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/auth.py` & `webwithpy-0.7.5/webwithpy/orm/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,18 @@
                 extra_buttons=[login_href_button],
             )
 
         # register user and log him in if the form is validated correctly
         if form.accepted:
             user_data: dict = form.form_data
             user_data.update({"uuid": App.request.cookies.get("session")})
+            if len((self.db.auth_user.email == user_data["email"]).select()) != 0:
+                form.error_msg = "Email already registered"
+                return form
+
             self.db.auth_user.insert(**user_data)
             return Redirect("/")
 
         return form
 
 
 def logged_in():
```

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/core.py` & `webwithpy-0.7.5/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.5/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.5/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.5/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.5/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.5/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.5/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.5/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.5/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/orm/objects/query.py` & `webwithpy-0.7.5/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/persistence.py` & `webwithpy-0.7.5/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/routing/methods.py` & `webwithpy-0.7.5/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/routing/router.py` & `webwithpy-0.7.5/webwithpy/routing/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,28 @@
     def __init__(
         self,
         func: Callable,
         url: str,
         method: str,
         template: Optional[str] = "",
         content_type: Optional[str] = "",
+        test_function: Optional[bool] = False,
     ):
         """
         :param func: function you want to be called whenever a user go to the given url
         :param url: The url you want your function to be called on
         :param method: The method given by the user, e.g. GET, POST, etc. If you want to include all methods use ANY
         :param template: Template that can be sent to the user, result of func will also be given to the template
         """
         self.func = func
         self.url = url
         self.method = method
         self.template = template
         self.content_type = content_type
+        self.test_function = test_function
 
 
 class RouteData:
     def __init__(
         self,
         func,
         url: str,
@@ -99,19 +101,20 @@
     @classmethod
     def add_route(cls, route: Route, **kwargs: Any):
         """
         adds routes to the router
         """
         Router.routes.append(
             RouteData(
-                route.func,
-                route.url,
-                route.method,
-                route.template,
-                route.content_type,
+                func=route.func,
+                url=route.url,
+                method=route.method,
+                template=route.template,
+                content_type=route.content_type,
+                test_function=route.test_function,
                 **kwargs,
             )
         )
 
     @classmethod
     def bulk_add_routes(cls, *routes: Route, **kwargs: Any):
         for route in routes:
```

### Comparing `webwithpy-0.7.4.5/webwithpy/static/form.css` & `webwithpy-0.7.5/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.5/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/tests/helper.py` & `webwithpy-0.7.5/webwithpy/tests/helper.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/webwithpy/webwithpy.py` & `webwithpy-0.7.5/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.5/PKG-INFO` & `webwithpy-0.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.4.5
+Version: 0.7.5
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

