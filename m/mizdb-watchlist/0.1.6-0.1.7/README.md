# Comparing `tmp/mizdb_watchlist-0.1.6.tar.gz` & `tmp/mizdb_watchlist-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb_watchlist-0.1.6.tar", max compression
+gzip compressed data, was "mizdb_watchlist-0.1.7.tar", max compression
```

## Comparing `mizdb_watchlist-0.1.6.tar` & `mizdb_watchlist-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-04-03 06:48:04.367968 mizdb_watchlist-0.1.6/LICENSE
--rw-r--r--   0        0        0    12547 2024-04-09 10:24:36.232562 mizdb_watchlist-0.1.6/README.md
--rw-r--r--   0        0        0     1807 2024-04-09 10:35:00.018513 mizdb_watchlist-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-0.1.6/src/mizdb_watchlist/__init__.py
--rw-r--r--   0        0        0      673 2024-04-03 06:48:04.370968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/actions.py
--rw-r--r--   0        0        0     1882 2024-04-09 10:24:36.232562 mizdb_watchlist-0.1.6/src/mizdb_watchlist/admin.py
--rw-r--r--   0        0        0      135 2024-03-12 07:47:13.602157 mizdb_watchlist-0.1.6/src/mizdb_watchlist/apps.py
--rw-r--r--   0        0        0     1445 2024-04-09 09:11:15.224678 mizdb_watchlist-0.1.6/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2491 2024-04-03 06:48:04.370968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11133 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/manager.py
--rw-r--r--   0        0        0     1426 2024-04-08 09:55:49.339373 mizdb_watchlist-0.1.6/src/mizdb_watchlist/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-0.1.6/src/mizdb_watchlist/migrations/__init__.py
--rw-r--r--   0        0        0      884 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/models.py
--rw-r--r--   0        0        0     1043 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css
--rw-r--r--   0        0        0     3024 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js
--rw-r--r--   0        0        0      365 2024-04-08 10:33:54.259477 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/admin/watchlist.html
--rw-r--r--   0        0        0      455 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/mizdb_watchlist/toggle_button.html
--rw-r--r--   0        0        0     2501 2024-04-08 11:40:49.700933 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html
--rw-r--r--   0        0        0      288 2024-03-11 09:33:17.648399 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_icon.svg
--rw-r--r--   0        0        0      426 2024-03-19 08:44:02.612348 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html
--rw-r--r--   0        0        0        0 2024-03-11 07:55:02.083282 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templatetags/__init__.py
--rw-r--r--   0        0        0     2850 2024-03-19 08:12:44.997279 mizdb_watchlist-0.1.6/src/mizdb_watchlist/templatetags/mizdb_watchlist.py
--rw-r--r--   0        0        0      337 2024-03-19 12:28:14.463165 mizdb_watchlist-0.1.6/src/mizdb_watchlist/urls.py
--rw-r--r--   0        0        0     6395 2024-04-09 10:24:36.232562 mizdb_watchlist-0.1.6/src/mizdb_watchlist/views.py
--rw-r--r--   0        0        0    13275 1970-01-01 00:00:00.000000 mizdb_watchlist-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 06:48:04.367968 mizdb_watchlist-0.1.7/LICENSE
+-rw-r--r--   0        0        0    12422 2024-04-09 10:52:16.608443 mizdb_watchlist-0.1.7/README.md
+-rw-r--r--   0        0        0     1807 2024-04-09 10:55:10.205002 mizdb_watchlist-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-0.1.7/src/mizdb_watchlist/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 06:48:04.370968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/actions.py
+-rw-r--r--   0        0        0     1882 2024-04-09 10:24:36.232562 mizdb_watchlist-0.1.7/src/mizdb_watchlist/admin.py
+-rw-r--r--   0        0        0      135 2024-03-12 07:47:13.602157 mizdb_watchlist-0.1.7/src/mizdb_watchlist/apps.py
+-rw-r--r--   0        0        0     1445 2024-04-09 09:11:15.224678 mizdb_watchlist-0.1.7/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2491 2024-04-03 06:48:04.370968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11133 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/manager.py
+-rw-r--r--   0        0        0     1426 2024-04-08 09:55:49.339373 mizdb_watchlist-0.1.7/src/mizdb_watchlist/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-0.1.7/src/mizdb_watchlist/migrations/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/models.py
+-rw-r--r--   0        0        0     1043 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css
+-rw-r--r--   0        0        0     3024 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js
+-rw-r--r--   0        0        0      365 2024-04-08 10:33:54.259477 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/admin/watchlist.html
+-rw-r--r--   0        0        0      455 2024-04-03 06:48:04.371968 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/mizdb_watchlist/toggle_button.html
+-rw-r--r--   0        0        0     2501 2024-04-08 11:40:49.700933 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html
+-rw-r--r--   0        0        0      288 2024-03-11 09:33:17.648399 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_icon.svg
+-rw-r--r--   0        0        0      426 2024-03-19 08:44:02.612348 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.083282 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templatetags/__init__.py
+-rw-r--r--   0        0        0     2850 2024-03-19 08:12:44.997279 mizdb_watchlist-0.1.7/src/mizdb_watchlist/templatetags/mizdb_watchlist.py
+-rw-r--r--   0        0        0      337 2024-03-19 12:28:14.463165 mizdb_watchlist-0.1.7/src/mizdb_watchlist/urls.py
+-rw-r--r--   0        0        0     6395 2024-04-09 10:24:36.232562 mizdb_watchlist-0.1.7/src/mizdb_watchlist/views.py
+-rw-r--r--   0        0        0    13150 1970-01-01 00:00:00.000000 mizdb_watchlist-0.1.7/PKG-INFO
```

### Comparing `mizdb_watchlist-0.1.6/LICENSE` & `mizdb_watchlist-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/README.md` & `mizdb_watchlist-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 
 Finally, run the migration to add the Watchlist model:
 
 ```commandline
 python manage.py migrate mizdb_watchlist
 ```
 
-NOTE: ensure that Django's SessionMiddleware is [enabled](https://docs.djangoproject.com/en/5.0/topics/http/sessions/).
+> ⚠️️ **Note**:
+>
+> Django's SessionMiddleware must be [enabled](https://docs.djangoproject.com/en/5.0/topics/http/sessions/).
 
 ## Manipulating the watchlist
 
 ### Toggle button
 
 The toggle button adds an item to your watchlist if it is not already on it,
 otherwise it removes the item from the watchlist. If the item is on the watchlist,
@@ -88,19 +90,19 @@
 {% block content %}
   <h5>{{ object }} {% toggle_button view.request object %}</h5>
   ...
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
 
-> ℹ️ **NOTE**:
+> ℹ️ **Note**:
+>
 > The `mizdb_watchlist/js/watchlist.js` javascript drives the toggle button and the
 > buttons that remove items on the watchlist overview. Make sure you include it.
 
-
 The template tag takes the following arguments:
 
 | Argument     | Default value | Description                                                                               |
 |--------------|---------------|-------------------------------------------------------------------------------------------|
 | request      | **required**  | the view's request                                                                        |
 | obj          | **required**  | the model object to add or remove                                                         |
 | text         | `""`          | optional text for the button                                                              |
@@ -256,17 +258,14 @@
 The ModelAdmin provides an admin view for the watchlist overview and adds it
 to the ModelAdmin's URLs with the view name `watchlist`. The URL of the overview
 can be reversed with `reverse(f"{your_admin_site.name}:watchlist")`.
 
 The ModelAdmin itself lets admins inspect and modify the (model) watchlists of
 other users, while the overview displays the watchlist items of the current admin user.
 
-The ModelAdmin adds the `add_to_watchlist` action that lets you select items on
-the changelist page and add them to your watchlist via admin actions.
-
 The ModelAdmin is hooked up to Django's default admin site.
 If you are not using the default admin site, make sure to register the ModelAdmin
 with your site:
 
 ```python
 from mizdb_watchlist.admin import WatchlistAdmin
 from mizdb_watchlist.models import Watchlist
@@ -308,15 +307,16 @@
 
 {% block userlinks %}
   {% watchlist_link '<name of your admin site>:watchlist' icon=False %} / {{ block.super }}
 {% endblock %}
 ```
 [comment]: <> (@formatter:on)
 
-> ℹ️
+> ℹ️ **Note**:
+>
 > See [Overriding admin templates](https://docs.djangoproject.com/en/5.0/ref/contrib/admin/#admin-overriding-templates)
 > for more details on how to override admin templates.
 
 ### admin.WatchlistMixin
 
 `admin.WatchlistMixin` is the admin version of `views.WatchlistMixin`. The mixin
 adds annotations and filtering (see [WatchlistMixin](#viewswatchlistmixin)) to
```

### Comparing `mizdb_watchlist-0.1.6/pyproject.toml` & `mizdb_watchlist-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mizdb-watchlist"
-version = "0.1.6"
+version = "0.1.7"
 description = "A watchlist for Django model objects."
 authors = [
   "Philip Becker <yummytea1@gmail.com>" ,
 ]
 readme = "README.md"
 packages = [{include = "mizdb_watchlist", from = "src"}]
 classifiers = [
     "Framework :: Django",
     "Programming Language :: Python :: 3",
 ]
 license = "MIT"
-repository = "https://github.com/Actionb/mizdb-tomselect"
+repository = "https://github.com/Actionb/mizdb-watchlist"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = ">4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
```

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/actions.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/actions.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/admin.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/admin.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/manager.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/manager.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/migrations/0001_initial.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/models.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/models.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/templatetags/mizdb_watchlist.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/templatetags/mizdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/src/mizdb_watchlist/views.py` & `mizdb_watchlist-0.1.7/src/mizdb_watchlist/views.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.6/PKG-INFO` & `mizdb_watchlist-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mizdb-watchlist
-Version: 0.1.6
+Version: 0.1.7
 Summary: A watchlist for Django model objects.
-Home-page: https://github.com/Actionb/mizdb-tomselect
+Home-page: https://github.com/Actionb/mizdb-watchlist
 License: MIT
 Author: Philip Becker
 Author-email: yummytea1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>4)
-Project-URL: Repository, https://github.com/Actionb/mizdb-tomselect
+Project-URL: Repository, https://github.com/Actionb/mizdb-watchlist
 Description-Content-Type: text/markdown
 
 # mizdb-watchlist
 
 Django model and views that implement a watchlist of other Django objects.
 
 This library provides a toggle button for adding individual items, a list view
@@ -82,15 +82,17 @@
 
 Finally, run the migration to add the Watchlist model:
 
 ```commandline
 python manage.py migrate mizdb_watchlist
 ```
 
-NOTE: ensure that Django's SessionMiddleware is [enabled](https://docs.djangoproject.com/en/5.0/topics/http/sessions/).
+> ⚠️️ **Note**:
+>
+> Django's SessionMiddleware must be [enabled](https://docs.djangoproject.com/en/5.0/topics/http/sessions/).
 
 ## Manipulating the watchlist
 
 ### Toggle button
 
 The toggle button adds an item to your watchlist if it is not already on it,
 otherwise it removes the item from the watchlist. If the item is on the watchlist,
@@ -108,19 +110,19 @@
 {% block content %}
   <h5>{{ object }} {% toggle_button view.request object %}</h5>
   ...
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
 
-> ℹ️ **NOTE**:
+> ℹ️ **Note**:
+>
 > The `mizdb_watchlist/js/watchlist.js` javascript drives the toggle button and the
 > buttons that remove items on the watchlist overview. Make sure you include it.
 
-
 The template tag takes the following arguments:
 
 | Argument     | Default value | Description                                                                               |
 |--------------|---------------|-------------------------------------------------------------------------------------------|
 | request      | **required**  | the view's request                                                                        |
 | obj          | **required**  | the model object to add or remove                                                         |
 | text         | `""`          | optional text for the button                                                              |
@@ -276,17 +278,14 @@
 The ModelAdmin provides an admin view for the watchlist overview and adds it
 to the ModelAdmin's URLs with the view name `watchlist`. The URL of the overview
 can be reversed with `reverse(f"{your_admin_site.name}:watchlist")`.
 
 The ModelAdmin itself lets admins inspect and modify the (model) watchlists of
 other users, while the overview displays the watchlist items of the current admin user.
 
-The ModelAdmin adds the `add_to_watchlist` action that lets you select items on
-the changelist page and add them to your watchlist via admin actions.
-
 The ModelAdmin is hooked up to Django's default admin site.
 If you are not using the default admin site, make sure to register the ModelAdmin
 with your site:
 
 ```python
 from mizdb_watchlist.admin import WatchlistAdmin
 from mizdb_watchlist.models import Watchlist
@@ -328,15 +327,16 @@
 
 {% block userlinks %}
   {% watchlist_link '<name of your admin site>:watchlist' icon=False %} / {{ block.super }}
 {% endblock %}
 ```
 [comment]: <> (@formatter:on)
 
-> ℹ️
+> ℹ️ **Note**:
+>
 > See [Overriding admin templates](https://docs.djangoproject.com/en/5.0/ref/contrib/admin/#admin-overriding-templates)
 > for more details on how to override admin templates.
 
 ### admin.WatchlistMixin
 
 `admin.WatchlistMixin` is the admin version of `views.WatchlistMixin`. The mixin
 adds annotations and filtering (see [WatchlistMixin](#viewswatchlistmixin)) to
```

