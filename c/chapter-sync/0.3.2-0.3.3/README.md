# Comparing `tmp/chapter_sync-0.3.2.tar.gz` & `tmp/chapter_sync-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapter_sync-0.3.2.tar", max compression
+gzip compressed data, was "chapter_sync-0.3.3.tar", max compression
```

## Comparing `chapter_sync-0.3.2.tar` & `chapter_sync-0.3.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      185 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/LICENSE
--rw-r--r--   0        0        0     4725 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/README.md
--rw-r--r--   0        0        0     2328 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/src/chapter_sync/__init__.py
--rw-r--r--   0        0        0       76 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/src/chapter_sync/__main__.py
--rw-r--r--   0        0        0     3793 2024-03-19 14:54:19.045633 chapter_sync-0.3.2/src/chapter_sync/chapter.py
--rw-r--r--   0        0        0       73 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/__init__.py
--rw-r--r--   0        0        0     5309 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/base.py
--rw-r--r--   0        0        0     1895 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/chapter.py
--rw-r--r--   0        0        0      659 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/db.py
--rw-r--r--   0        0        0     4303 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/series.py
--rw-r--r--   0        0        0     1808 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cli/subscriber.py
--rw-r--r--   0        0        0     1933 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/console.py
--rw-r--r--   0        0        0     2434 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/cover.py
--rw-r--r--   0        0        0     1923 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/db.py
--rw-r--r--   0        0        0     1531 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/email.py
--rw-r--r--   0        0        0    14814 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/epub.py
--rw-r--r--   0        0        0      276 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/handlers/__init__.py
--rw-r--r--   0        0        0     1908 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/handlers/base.py
--rw-r--r--   0        0        0     5798 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/handlers/custom.py
--rw-r--r--   0        0        0     3756 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/handlers/royal_road.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/__init__.py
--rw-r--r--   0        0        0      575 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/alembic.ini
--rw-r--r--   0        0        0     1396 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/env.py
--rw-r--r--   0        0        0      635 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/script.py.mako
--rw-r--r--   0        0        0     3886 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/migrations/versions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/py.typed
--rw-r--r--   0        0        0     3085 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/request.py
--rw-r--r--   0        0        0     5169 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/schema.py
--rw-r--r--   0        0        0     6131 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/series.py
--rw-r--r--   0        0        0     3160 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/subscriber.py
--rw-r--r--   0        0        0     4486 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/sync.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/templates/__init__.py
--rw-r--r--   0        0        0    14204 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/templates/base.css
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/__init__.py
--rw-r--r--   0        0        0      123 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/__main__.py
--rw-r--r--   0        0        0     2897 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/chapter.py
--rw-r--r--   0        0        0     2021 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/dependencies.py
--rw-r--r--   0        0        0      592 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/main.py
--rw-r--r--   0        0        0     1661 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/routes.py
--rw-r--r--   0        0        0     2467 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/series.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/static/__init__.py
--rw-r--r--   0        0        0     1033 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/static/app.css
--rw-r--r--   0        0        0     4286 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/static/favicon.ico
--rw-r--r--   0        0        0      392 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/static/icon.svg
--rw-r--r--   0        0        0       59 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/static/styles.css
--rw-r--r--   0        0        0     2999 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/subscriber.py
--rw-r--r--   0        0        0        0 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/__init__.py
--rw-r--r--   0        0        0      854 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/base.html
--rw-r--r--   0        0        0     2004 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/chapter.html
--rw-r--r--   0        0        0     2989 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/header.html
--rw-r--r--   0        0        0     3213 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/index.html
--rw-r--r--   0        0        0     1418 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/macros.html
--rw-r--r--   0        0        0      985 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/series.html
--rw-r--r--   0        0        0     1603 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/subscriber.html
--rw-r--r--   0        0        0     1252 2024-03-19 14:54:19.049633 chapter_sync-0.3.2/src/chapter_sync/web/templates/subscribers.html
--rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 chapter_sync-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      185 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4725 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/README.md
+-rw-r--r--   0        0        0     2328 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/__main__.py
+-rw-r--r--   0        0        0     3793 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/chapter.py
+-rw-r--r--   0        0        0       73 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/cli/__init__.py
+-rw-r--r--   0        0        0     5296 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/base.py
+-rw-r--r--   0        0        0     1895 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/chapter.py
+-rw-r--r--   0        0        0      659 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/db.py
+-rw-r--r--   0        0        0     4303 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/series.py
+-rw-r--r--   0        0        0     1808 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/subscriber.py
+-rw-r--r--   0        0        0     1933 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/console.py
+-rw-r--r--   0        0        0     2434 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cover.py
+-rw-r--r--   0        0        0     1923 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/db.py
+-rw-r--r--   0        0        0     1531 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/email.py
+-rw-r--r--   0        0        0    14814 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/epub.py
+-rw-r--r--   0        0        0      276 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/base.py
+-rw-r--r--   0        0        0     5821 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/custom.py
+-rw-r--r--   0        0        0     3767 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/royal_road.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/alembic.ini
+-rw-r--r--   0        0        0     1396 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/script.py.mako
+-rw-r--r--   0        0        0     3886 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/versions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/py.typed
+-rw-r--r--   0        0        0     3091 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/request.py
+-rw-r--r--   0        0        0     5169 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/schema.py
+-rw-r--r--   0        0        0     6131 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/series.py
+-rw-r--r--   0        0        0     3160 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/subscriber.py
+-rw-r--r--   0        0        0     4235 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/sync.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/templates/__init__.py
+-rw-r--r--   0        0        0    14204 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/templates/base.css
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/__init__.py
+-rw-r--r--   0        0        0      123 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/__main__.py
+-rw-r--r--   0        0        0     2897 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/chapter.py
+-rw-r--r--   0        0        0     2077 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/dependencies.py
+-rw-r--r--   0        0        0      880 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/main.py
+-rw-r--r--   0        0        0     1661 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/routes.py
+-rw-r--r--   0        0        0     2467 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/series.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/__init__.py
+-rw-r--r--   0        0        0     1033 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/app.css
+-rw-r--r--   0        0        0     4286 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/favicon.ico
+-rw-r--r--   0        0        0      392 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/icon.svg
+-rw-r--r--   0        0        0       59 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/styles.css
+-rw-r--r--   0        0        0     2999 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/subscriber.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/base.html
+-rw-r--r--   0        0        0     2004 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/chapter.html
+-rw-r--r--   0        0        0     2989 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/header.html
+-rw-r--r--   0        0        0     3213 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/index.html
+-rw-r--r--   0        0        0     1418 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/macros.html
+-rw-r--r--   0        0        0      985 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/series.html
+-rw-r--r--   0        0        0     1603 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/subscriber.html
+-rw-r--r--   0        0        0     1252 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/subscribers.html
+-rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 chapter_sync-0.3.3/PKG-INFO
```

### Comparing `chapter_sync-0.3.2/LICENSE` & `chapter_sync-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/README.md` & `chapter_sync-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/pyproject.toml` & `chapter_sync-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chapter-sync"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = [
     "Dan Cardin <ddcardin@gmail.com>",
 ]
 license = "Apache-2.0"
 repository = "https://github.com/dancardin/sqlalchemy-declarative-extensions"
 readme = 'README.md'
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/chapter.py` & `chapter_sync-0.3.3/src/chapter_sync/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cli/base.py` & `chapter_sync-0.3.3/src/chapter_sync/cli/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Doc("The name of the database file. Defaults to 'chapter_sync.sqlite'."),
     ] = "chapter_sync.sqlite"
     verbose: Annotated[
         int,
         cappa.Arg(short=True, long=True, action=cappa.ArgAction.count),
         Doc("Increase verbosity."),
     ] = 0
-    tty: Annotated[bool | None, cappa.Arg(long="--tty/--no-tty", hidden=True)] = None
+    tty: Annotated[bool | None, cappa.Arg(long="--tty/--no-tty")] = None
 
 
 @cappa.command(invoke="chapter_sync.sync.sync")
 @dataclass
 class Sync:
     """Sync updates to all series."""
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cli/chapter.py` & `chapter_sync-0.3.3/src/chapter_sync/cli/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cli/db.py` & `chapter_sync-0.3.3/src/chapter_sync/cli/db.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cli/series.py` & `chapter_sync-0.3.3/src/chapter_sync/cli/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cli/subscriber.py` & `chapter_sync-0.3.3/src/chapter_sync/cli/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/console.py` & `chapter_sync-0.3.3/src/chapter_sync/console.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/cover.py` & `chapter_sync-0.3.3/src/chapter_sync/cover.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/db.py` & `chapter_sync-0.3.3/src/chapter_sync/db.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/email.py` & `chapter_sync-0.3.3/src/chapter_sync/email.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/epub.py` & `chapter_sync-0.3.3/src/chapter_sync/epub.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/handlers/base.py` & `chapter_sync-0.3.3/src/chapter_sync/handlers/base.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/handlers/custom.py` & `chapter_sync-0.3.3/src/chapter_sync/handlers/custom.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Generator
 from dataclasses import dataclass
 
 import cappa
 from pendulum import now
 from requests import Session
 
-from chapter_sync.console import Status
+from chapter_sync.console import Console
 from chapter_sync.request import (
     clean_emails,
     clean_namespaced_elements,
     get_soup,
     join_path,
     published_at,
     strip_colors,
@@ -42,32 +42,32 @@
     try:
         return Settings(**raw)
     except Exception as e:
         raise ValueError(f"Invalid settings: {e}")
 
 
 def chapter_handler(
-    requests: Session, series: Series, settings: Settings, status: Status
+    requests: Session, series: Series, settings: Settings, console: Console
 ) -> Generator[Chapter, None, None]:
     if settings.chapter_selector:
-        yield from find_by_chapter(requests, series, settings, status=status)
+        yield from find_by_chapter(requests, series, settings, console=console)
     elif settings.next_selector:
-        yield from find_by_next(requests, series, settings, status=status)
+        yield from find_by_next(requests, series, settings, console=console)
     else:
         raise NotImplementedError()
 
 
 def find_by_chapter(
-    requests: Session, series: Series, settings: Settings, status: Status
+    requests: Session, series: Series, settings: Settings, console: Console
 ) -> Generator[Chapter, None, None]:
     assert settings.chapter_selector
 
     url = series.url
 
-    soup = get_soup(requests, url, status=status)
+    soup = get_soup(requests, url, console=console)
 
     assert soup.head
     base = soup.head.base and soup.head.base.get("href") or False
 
     existing_chapters = {c.url: c for c in series.chapters}
 
     existing_chapter = None
@@ -82,24 +82,24 @@
             chapter_url = join_path(base, chapter_url)
 
         for chapter in _collect_chapter(
             requests,
             series,
             settings,
             chapter_url,
-            status=status,
+            console=console,
             title=chapter_link.string,
             number=existing_chapter.number + 1 if existing_chapter else 1,
         ):
             yield chapter
             existing_chapter = chapter
 
 
 def find_by_next(
-    requests: Session, series: Series, settings: Settings, status: Status
+    requests: Session, series: Series, settings: Settings, console: Console
 ) -> Generator[Chapter, None, None]:
     assert settings.next_selector
 
     last_chapter = None
     if series.chapters:
         last_chapter = series.chapters[-1]
 
@@ -110,23 +110,23 @@
     while next_url:
         if next_url not in existing_urls:
             for chapter in _collect_chapter(
                 requests,
                 series,
                 settings,
                 next_url,
-                status=status,
+                console=console,
                 number=last_chapter.number + 1 if last_chapter else 1,
             ):
                 yield chapter
                 last_chapter = chapter
 
         existing_urls.add(next_url)
 
-        soup = get_soup(requests, next_url, status=status)
+        soup = get_soup(requests, next_url, console=console)
 
         assert soup.head
         base = soup.head.base and soup.head.base.get("href") or False
 
         next_link = soup.select(settings.next_selector)
         if not next_link:
             break
@@ -140,20 +140,20 @@
 
 def _collect_chapter(
     requests: Session,
     series: Series,
     settings: Settings,
     url: str,
     *,
-    status: Status,
+    console: Console,
     title: str | None = None,
     number: int = 1,
 ):
-    status.update(f"Extracting chapter at '{url}'")
-    soup = get_soup(requests, url, status=status)
+    console.trace(f"Extracting chapter at '{url}'")
+    soup = get_soup(requests, url, console=console)
 
     if not soup.select(settings.content_selector):
         return
 
     clean_namespaced_elements(soup)
     clean_emails(soup)
     strip_colors(soup)
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/handlers/royal_road.py` & `chapter_sync-0.3.3/src/chapter_sync/handlers/royal_road.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from collections.abc import Generator
 from dataclasses import dataclass
 
 import pendulum
 from requests import Session
 
-from chapter_sync.console import Status
+from chapter_sync.console import Console
 from chapter_sync.request import (
     clean_emails,
     clean_namespaced_elements,
     get_soup,
     join_path,
     strip_colors,
 )
@@ -42,23 +42,23 @@
     try:
         return Settings(**raw)
     except Exception as e:
         raise ValueError(f"Invalid settings: {e}")
 
 
 def chapter_handler(
-    requests: Session, series: Series, settings: Settings, status: Status
+    requests: Session, series: Series, settings: Settings, console: Console
 ) -> Generator[Chapter, None, None]:
     # TODO: It's likely most kinds of sites can be handled in terms of the "custom" handler
     #       based on TOC. The main drawback would be things like login requirements, or
     #       the below extra cleaning bits. A system of callbacks for cleaning could be the most
     #       straghtforward way. And login could be handled by the requests session input.
     url = series.url
 
-    soup = get_soup(requests, url, status=status)
+    soup = get_soup(requests, url, console=console)
 
     existing_chapters = {c.url: c for c in series.chapters}
 
     chapter_elements = soup.select("#chapters tbody tr[data-url]")
     for number, chapter in enumerate(chapter_elements, start=1):
         chapter_url = join_path(series.url, str(chapter.get("data-url")))
 
@@ -66,31 +66,31 @@
             continue
 
         title = chapter.find("a", href=True).string.strip()  # type: ignore
         yield _collect_chapter(
             requests,
             series,
             chapter_url,
-            status=status,
+            console=console,
             title=title,
             number=number,
         )
 
 
 def _collect_chapter(
     requests: Session,
     series: Series,
     url: str,
     *,
-    status: Status,
+    console: Console,
     title: str | None = None,
     number: int = 1,
 ):
-    status.update(f"Extracting chapter at '{url}'")
-    soup = get_soup(requests, url, status=status)
+    console.trace(f"Extracting chapter at '{url}'")
+    soup = get_soup(requests, url, console=console)
 
     clean_namespaced_elements(soup)
     clean_emails(soup)
     strip_colors(soup)
     strip_spoilers(soup)
 
     content = soup.find("div", class_="chapter-content")
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/migrations/alembic.ini` & `chapter_sync-0.3.3/src/chapter_sync/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/migrations/env.py` & `chapter_sync-0.3.3/src/chapter_sync/migrations/env.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/migrations/script.py.mako` & `chapter_sync-0.3.3/src/chapter_sync/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py` & `chapter_sync-0.3.3/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/request.py` & `chapter_sync-0.3.3/src/chapter_sync/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import urllib.parse
 from typing import cast
 
 import pendulum
 from bs4 import BeautifulSoup, Tag
 from requests import Session
 
-from chapter_sync.console import Status
+from chapter_sync.console import Console
 
 RE_NAMESPACED_ELEMENT = re.compile(r"[a-z]+:[a-z]+")
 
 
 def requests_session():
     return Session()
 
 
 def get_soup(
     session: Session,
     url,
     *,
-    status: Status | None = None,
+    console: Console | None = None,
     method="html5lib",
     retry=3,
     retry_delay=10,
     timeout=30,
 ):
     page = session.get(url, timeout=timeout)
     if not page:
@@ -36,24 +36,24 @@
             raise RuntimeError("Couldn't due to Cloudflare protection", url)
 
         if retry and retry > 0:
             real_delay = retry_delay
             if "Retry-After" in page.headers:
                 real_delay = int(page.headers["Retry-After"])
 
-            if status:
-                status.update(
+            if console:
+                console.trace(
                     f"Load failed: waiting {real_delay} to retry ({page.status_code}: {page.url})",
                 )
             time.sleep(real_delay)
 
             return get_soup(
                 session,
                 url,
-                status=status,
+                console=console,
                 method=method,
                 retry=retry - 1,
                 retry_delay=retry_delay,
                 timeout=timeout,
             )
         raise RuntimeError("Couldn't fetch", url)
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/schema.py` & `chapter_sync-0.3.3/src/chapter_sync/schema.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/series.py` & `chapter_sync-0.3.3/src/chapter_sync/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/subscriber.py` & `chapter_sync-0.3.3/src/chapter_sync/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/sync.py` & `chapter_sync-0.3.3/src/chapter_sync/sync.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import cappa
 import pendulum
 from sqlalchemy import select
 from sqlalchemy.orm import Session, selectinload
 
 from chapter_sync.cli.base import Sync, Watch, console, database, email_client
-from chapter_sync.console import Console, Status
+from chapter_sync.console import Console
 from chapter_sync.email import EmailClient
 from chapter_sync.epub import Epub
 from chapter_sync.handlers import get_chapter_handler, get_settings_handler
 from chapter_sync.request import requests_session
 from chapter_sync.schema import Chapter, Series
 
 
@@ -22,87 +22,77 @@
     database: Annotated[Session, cappa.Dep(database)],
     console: Annotated[Console, cappa.Dep(console)],
     email_client: Annotated[EmailClient, cappa.Dep(email_client)],
 ):
     try:
         with console.status("Syncing series") as status:
             while True:
-                sync(command, database, console, email_client, status)
-                time.sleep(command.interval)
+                sync(command, database, console, email_client)
+
                 status.update("Sleeping")
+                time.sleep(command.interval)
     except KeyboardInterrupt:
         console.info("Stopping")
         return
 
 
 def sync(
     command: Sync,
     database: Annotated[Session, cappa.Dep(database)],
     console: Annotated[Console, cappa.Dep(console)],
     email_client: Annotated[EmailClient, cappa.Dep(email_client)],
-    status: Status | None = None,
 ):
-    requires_status = status is None
-    if status is None:
-        status = console.status("Syncing series")
-        status.start()
-
     query = select(Series).options(selectinload(Series.chapters))
     if command.series:
         query = query.where(Series.id.in_(command.series))
 
     series = database.scalars(query).all()
 
-    status.update(f"Found {len(series)} series")
+    console.info(f"Found {len(series)} series")
 
     for s in series:
         if command.update:
-            update_series(database, s, status)
-            status.update(f"Updated series: '{s.name}'")
+            update_series(database, s, console)
+            console.info(f"Updated series: '{s.name}'")
 
         if command.save:
-            save_series_ebooks(database, s, status)
+            save_series_ebooks(database, s, console)
 
         if command.send:
-            send_series(command, database, s, email_client, status)
-
-    status.update("Done")
-
-    if requires_status:
-        status.stop()
+            send_series(command, database, s, email_client, console)
 
 
-def update_series(database: Session, series: Series, status: Status):
+def update_series(database: Session, series: Series, console: Console):
     settings_handler = get_settings_handler(series.type, load=False)
     settings = settings_handler(series.settings)
 
     requests = requests_session()
     chapter_handler = get_chapter_handler(series.type)
-    for chapter in chapter_handler(requests, series, settings, status):
+    for chapter in chapter_handler(requests, series, settings, console):
         database.add(chapter)
         database.commit()
 
 
-def save_series_ebooks(database: Session, series: Series, status: Status):
+def save_series_ebooks(database: Session, series: Series, console: Console):
     for chapter in series.chapters:
-        status.update(f"Saving chapter: '{chapter.title}'")
+        console.info(f"Saving chapter: '{chapter.title}'")
         if chapter.ebook:
             continue
 
         ebook = Epub.from_series(series, chapter).write_buffer()
         chapter.ebook = ebook.getbuffer()
         database.commit()
 
 
 def send_series(
     command: Sync,
     database: Session,
     series: Series,
     email_client: EmailClient,
-    status: Status,
+    console: Console,
 ):
     subscribers = series.email_subscribers
     unsent_chapters = [c for c in series.chapters if c.sent_at is None]
 
     if command.contiguous_chapters:
         last_chapter = -1
         contiguous_blocks: list[list[Chapter]] = []
@@ -124,22 +114,22 @@
 
             title = chapter.filename()
         else:
             ebook = Epub.from_series(series, *block).write_buffer().read()
             title = f"{series.name} - Chapters {block[0].number} to {block[-1].number}"
 
         titles = ", ".join([chapter.title for chapter in block])
-        status.update(f"Sending chapters: {titles}")
+        console.info(f"Sending chapters: {titles}")
 
         for subscriber in subscribers:
             email_client.send(
                 subject=title,
                 to=subscriber.email,
                 filename=title,
                 attachment=ebook,
             )
 
         for chapter in block:
             chapter.sent_at = pendulum.now("utc")
 
         database.commit()
-        status.update("Chapter(s) sent")
+        console.trace("Chapter(s) sent")
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/templates/base.css` & `chapter_sync-0.3.3/src/chapter_sync/templates/base.css`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/chapter.py` & `chapter_sync-0.3.3/src/chapter_sync/web/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/dependencies.py` & `chapter_sync-0.3.3/src/chapter_sync/web/dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 
 def chapter_sync():
     return base.ChapterSync(None)
 
 
 def database(
     chapter_sync: Annotated[base.ChapterSync, Depends(chapter_sync)],
+    alembic_config=None,
 ) -> Generator[Session, None, None]:
     url = base.database_url(chapter_sync)
-    yield from base.database(url)
+    yield from base.database(url, alembic_config=alembic_config)
 
 
 def console(
     chapter_sync: Annotated[base.ChapterSync, Depends(chapter_sync)],
 ) -> Generator[base.Console, None, None]:
     yield from base.console(chapter_sync)
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/main.py` & `chapter_sync-0.3.3/src/chapter_sync/web/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 import importlib.resources
 import logging
 
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 
+from chapter_sync.cli.base import alembic_config, database_url
+from chapter_sync.web.dependencies import chapter_sync, database
 from chapter_sync.web.routes import routes
 
 
 def create_app(routes=routes):
     logging.basicConfig(level="INFO")
 
+    boostrap_db()
+
     app = FastAPI()
 
     static_dir = importlib.resources.files("chapter_sync.web.static")
     app.mount("/static", StaticFiles(directory=str(static_dir)), name="static")
 
     for route in routes:
         app.add_api_route(
             path=route["path"],
             endpoint=route["endpoint"],
             methods=[route["method"]],
         )
 
     return app
+
+
+def boostrap_db():
+    app = chapter_sync()
+    url = database_url(app)
+    alembic = alembic_config(url)
+    list(database(app, alembic))
```

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/routes.py` & `chapter_sync-0.3.3/src/chapter_sync/web/routes.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/series.py` & `chapter_sync-0.3.3/src/chapter_sync/web/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/static/app.css` & `chapter_sync-0.3.3/src/chapter_sync/web/static/app.css`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/static/favicon.ico` & `chapter_sync-0.3.3/src/chapter_sync/web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/subscriber.py` & `chapter_sync-0.3.3/src/chapter_sync/web/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/base.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/chapter.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/header.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/header.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/index.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/macros.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/macros.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/series.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/series.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/subscriber.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/subscriber.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/src/chapter_sync/web/templates/subscribers.html` & `chapter_sync-0.3.3/src/chapter_sync/web/templates/subscribers.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.2/PKG-INFO` & `chapter_sync-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapter-sync
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/dancardin/sqlalchemy-declarative-extensions
 License: Apache-2.0
 Keywords: chapter,sync,epub,ebook,leech
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.10,<4.0
```

