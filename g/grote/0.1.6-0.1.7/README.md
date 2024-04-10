# Comparing `tmp/grote-0.1.6.tar.gz` & `tmp/grote-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grote-0.1.6.tar", max compression
+gzip compressed data, was "grote-0.1.7.tar", max compression
```

## Comparing `grote-0.1.6.tar` & `grote-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.6/LICENSE
--rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.6/README.md
--rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.6/grote/__init__.py
--rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.6/grote/app.py
--rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.6/grote/collections/__init__.py
--rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.6/grote/collections/base.py
--rw-r--r--   0        0        0     1218 2024-04-10 21:30:35.209116 grote-0.1.6/grote/collections/config.yaml
--rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.6/grote/collections/load.py
--rw-r--r--   0        0        0     8298 2024-04-10 21:30:05.986989 grote-0.1.6/grote/collections/translate.py
--rw-r--r--   0        0        0     2451 2024-04-10 21:36:18.537577 grote-0.1.6/grote/config.py
--rw-r--r--   0        0        0      299 2024-04-10 21:31:45.750995 grote-0.1.6/grote/config.yaml
--rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.6/grote/event_logging.py
--rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.6/grote/functions/__init__.py
--rw-r--r--   0        0        0     5543 2024-04-10 21:18:52.959276 grote-0.1.6/grote/functions/load.py
--rw-r--r--   0        0        0     3529 2024-04-10 21:35:57.692323 grote-0.1.6/grote/functions/translate.py
--rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.6/grote/style.py
--rw-r--r--   0        0        0     3659 2024-04-10 21:37:15.973066 grote-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.7/README.md
+-rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.7/grote/__init__.py
+-rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.7/grote/app.py
+-rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.7/grote/collections/__init__.py
+-rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.7/grote/collections/base.py
+-rw-r--r--   0        0        0     1218 2024-04-10 21:30:35.209116 grote-0.1.7/grote/collections/config.yaml
+-rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.7/grote/collections/load.py
+-rw-r--r--   0        0        0     8298 2024-04-10 21:30:05.986989 grote-0.1.7/grote/collections/translate.py
+-rw-r--r--   0        0        0     2455 2024-04-10 21:45:48.308514 grote-0.1.7/grote/config.py
+-rw-r--r--   0        0        0      299 2024-04-10 21:31:45.750995 grote-0.1.7/grote/config.yaml
+-rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.7/grote/event_logging.py
+-rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.7/grote/functions/__init__.py
+-rw-r--r--   0        0        0     5543 2024-04-10 21:18:52.959276 grote-0.1.7/grote/functions/load.py
+-rw-r--r--   0        0        0     3529 2024-04-10 21:35:57.692323 grote-0.1.7/grote/functions/translate.py
+-rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.7/grote/style.py
+-rw-r--r--   0        0        0     3659 2024-04-10 21:47:05.732519 grote-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.7/PKG-INFO
```

### Comparing `grote-0.1.6/LICENSE` & `grote-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/README.md` & `grote-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/app.py` & `grote-0.1.7/grote/app.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/collections/base.py` & `grote-0.1.7/grote/collections/base.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/collections/config.yaml` & `grote-0.1.7/grote/collections/config.yaml`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/collections/load.py` & `grote-0.1.7/grote/collections/load.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/collections/translate.py` & `grote-0.1.7/grote/collections/translate.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/config.py` & `grote-0.1.7/grote/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,11 +53,11 @@
         self.login_codes = self.init_list(self.login_codes)
         self.allowed_tags = self.init_list(self.allowed_tags)
         self.tag_labels = self.init_list(self.tag_labels)
         self.tag_colors = self.init_list(self.tag_colors)
 
 
 # Priority: environment variables > config.yaml
-CONFIG = GroteConfig(
+CONFIG = GroteConfig(**{
     **yaml.safe_load(open(Path(__file__).parent / "config.yaml", encoding="utf8")),
     **{k.lower(): v for k, v in os.environ.items() if k.lower() in [f.name.lower() for f in fields(GroteConfig)]},
-)
+})
```

### Comparing `grote-0.1.6/grote/event_logging.py` & `grote-0.1.7/grote/event_logging.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/functions/__init__.py` & `grote-0.1.7/grote/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/functions/load.py` & `grote-0.1.7/grote/functions/load.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/functions/translate.py` & `grote-0.1.7/grote/functions/translate.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/grote/style.py` & `grote-0.1.7/grote/style.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.6/pyproject.toml` & `grote-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "grote"
-version = "0.1.6"
+version = "0.1.7"
 description = "Groningen Translation Environment"
 readme = "README.md"
 authors = ["Gabriele Sarti"]
 maintainers = ["Gabriele Sarti <gabriele.sarti996@gmail.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/gsarti/grote"
 homepage = "https://github.com/gsarti/grote"
```

### Comparing `grote-0.1.6/PKG-INFO` & `grote-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grote
-Version: 0.1.6
+Version: 0.1.7
 Summary: Groningen Translation Environment
 Home-page: https://github.com/gsarti/grote
 License: Apache Software License 2.0
 Keywords: translation environment,gradio
 Author: Gabriele Sarti
 Maintainer: Gabriele Sarti
 Maintainer-email: gabriele.sarti996@gmail.com
```

