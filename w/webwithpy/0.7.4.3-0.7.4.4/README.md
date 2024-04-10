# Comparing `tmp/webwithpy-0.7.4.3.tar.gz` & `tmp/webwithpy-0.7.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.4.3.tar", max compression
+gzip compressed data, was "webwithpy-0.7.4.4.tar", max compression
```

## Comparing `webwithpy-0.7.4.3.tar` & `webwithpy-0.7.4.4.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.3/LICENSE
--rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.3/README.md
--rw-r--r--   0        0        0      503 2024-04-09 09:26:12.465690 webwithpy-0.7.4.3/pyproject.toml
--rw-r--r--   0        0        0       99 2024-04-09 09:19:41.819248 webwithpy-0.7.4.3/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/app.py
--rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.3/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6057 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5317 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/routing/router.py
--rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.3/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.4/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.4/README.md
+-rw-r--r--   0        0        0      554 2024-04-10 08:45:48.815584 webwithpy-0.7.4.4/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-10 07:14:22.692581 webwithpy-0.7.4.4/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/app.py
+-rw-r--r--   0        0        0     1567 2024-04-10 08:01:56.351262 webwithpy-0.7.4.4/webwithpy/commands.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4357 2024-04-09 09:26:12.477690 webwithpy-0.7.4.4/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6088 2024-04-10 08:26:02.365828 webwithpy-0.7.4.4/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5653 2024-04-10 08:28:05.770430 webwithpy-0.7.4.4/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0       63 2024-04-10 08:42:40.770674 webwithpy-0.7.4.4/webwithpy/tests/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-10 08:42:07.174512 webwithpy-0.7.4.4/webwithpy/tests/case.py
+-rw-r--r--   0        0        0      557 2024-04-10 08:29:49.054933 webwithpy-0.7.4.4/webwithpy/tests/helper.py
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.4/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.4/PKG-INFO
```

### Comparing `webwithpy-0.7.4.3/LICENSE` & `webwithpy-0.7.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/README.md` & `webwithpy-0.7.4.4/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.4.4/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.4.4/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.4.4/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/data/ast.py` & `webwithpy-0.7.4.4/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/forms.py` & `webwithpy-0.7.4.4/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/lexer.py` & `webwithpy-0.7.4.4/webwithpy/html/lexer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/parser.py` & `webwithpy-0.7.4.4/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/pyhtml.py` & `webwithpy-0.7.4.4/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/html/renderer.py` & `webwithpy-0.7.4.4/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/http/cookies.py` & `webwithpy-0.7.4.4/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/http/handler.py` & `webwithpy-0.7.4.4/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/http/request.py` & `webwithpy-0.7.4.4/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/http/response.py` & `webwithpy-0.7.4.4/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/http/urls.py` & `webwithpy-0.7.4.4/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/auth.py` & `webwithpy-0.7.4.4/webwithpy/orm/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,20 +116,22 @@
                 extra_buttons=[login_href_button],
             )
 
         # logic if form is accepted
         if form.accepted:
             user: dict = (
                 self.db.auth_user.email == form.form_data.get("email")
-            ).select(fields=["id", "password"])[0]
+            ).select(fields=["id", "password"])
 
-            if not user:
+            if len(user) == 0:
                 form.error_msg = "Email not found!"
                 return form
 
+            user = user[0]
+
             from_pass = form.form_data.get("password").encode()
 
             if bcrypt.checkpw(from_pass, user["password"]):
                 (self.db.auth_user.id == user["id"]).update(
                     uuid=App.request.cookies.get("session")
                 )
```

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/core.py` & `webwithpy-0.7.4.4/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.4.4/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.4.4/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.4.4/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.4.4/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.4.4/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.4.4/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.4.4/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.4.4/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/orm/objects/query.py` & `webwithpy-0.7.4.4/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/persistence.py` & `webwithpy-0.7.4.4/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/routing/methods.py` & `webwithpy-0.7.4.4/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/routing/router.py` & `webwithpy-0.7.4.4/webwithpy/routing/router.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,24 +35,26 @@
     def __init__(
         self,
         func,
         url: str,
         method: str,
         template: Optional[Union[str, PathLike, None]] = "",
         content_type: Optional[str] = "text/html",
+        test_function: Optional[bool] = False,
         *args,
         **kwargs,
     ):
         self.func = func
         self.url = url
         self.method = method
         self.html_template = template
         self.args = args
         self.kwargs = kwargs
         self.content_type = content_type
+        self.test_function = test_function
 
     async def call_func(self, _async: bool):
         """
         calls function and returns necessary data to turn it into a http request
         """
         if _async:
             return (
@@ -67,15 +69,19 @@
             self.content_type,
         )
 
     def get_route(self):
         # getter for url
         return self.url
 
-    def eq(self, url: str, method: str) -> bool:
+    def eq(self, url: str, method: str, testing: bool) -> bool:
+        # if we are not testing then we are NOT allowed to call these functions
+        if testing is False and self.test_function:
+            return False
+
         # checks if url and method is equal to current routed data
         return self.url == url and (
             self.method.lower() == method.lower() or self.method.lower() == "any"
         )
 
     def __str__(self):
         # if routed_data is printed it will print the method and url instead of its memory location
@@ -84,14 +90,15 @@
     def __repr__(self):
         return self.__str__()
 
 
 class Router:
     # python hack for static vars
     routes: list[RouteData] = []
+    testing: bool = False
 
     @classmethod
     def add_route(cls, route: Route, **kwargs: Any):
         """
         adds routes to the router
         """
         Router.routes.append(
@@ -115,29 +122,32 @@
         """
         gets the routed data by route
 
         :param url: http url like '/route'
         :param method: method used by http
         """
         for route in Router.routes:
-            if route.eq(url, method):
+            if route.eq(url, method, Router.testing):
                 return route
 
         return None
 
     @classmethod
     def _get_route(cls, route: str):
         """
         gets the routed data by route
 
         :param route: route is simple an url in this case: '/route'
         """
-        for Router_route in Router.routes:
-            if Router_route.get_route() == route:
-                return Router_route
+        for router_route in Router.routes:
+            if router_route.get_route() == route:
+                if not Router.testing and router_route.test_function:
+                    return None
+
+                return router_route
         return None
 
     @classmethod
     def _static_file_by_route(cls, route: str):
         path = Path(f"{os.getcwd()}/static{route}")
 
         if path.exists():
@@ -171,11 +181,10 @@
 
             raise ServerError("Server Error!")
 
     @classmethod
     async def _handle_static_file(cls, route: str, method: str):
         if (file := Router._static_file_by_route(route)) is not None:
             return file, "", f"text/{Router._parse_suffix(Path(route).suffix)}"
-        elif route == "/favicon.ico":
-            file = pkgutil.get_data(__name__, "../static/favicon.ico")
+        elif "favicon.ico" in route:
             return "", "", ""
         raise RouteNotFound(route, method)
```

### Comparing `webwithpy-0.7.4.3/webwithpy/static/form.css` & `webwithpy-0.7.4.4/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.4.4/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/webwithpy/webwithpy.py` & `webwithpy-0.7.4.4/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4.3/PKG-INFO` & `webwithpy-0.7.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.4.3
+Version: 0.7.4.4
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

