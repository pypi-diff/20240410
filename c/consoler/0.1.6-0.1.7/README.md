# Comparing `tmp/consoler-0.1.6.tar.gz` & `tmp/consoler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoler-0.1.6.tar", max compression
+gzip compressed data, was "consoler-0.1.7.tar", max compression
```

## Comparing `consoler-0.1.6.tar` & `consoler-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-04 08:32:45.868780 consoler-0.1.6/LICENSE
--rw-r--r--   0        0        0     1495 2024-04-04 15:04:02.836146 consoler-0.1.6/README.md
--rw-r--r--   0        0        0       88 2024-04-04 08:32:45.869096 consoler-0.1.6/consoler/__init__.py
--rw-r--r--   0        0        0     2420 2024-04-04 11:22:39.483403 consoler-0.1.6/consoler/colours.py
--rw-r--r--   0        0        0     7430 2024-04-04 15:53:53.300225 consoler-0.1.6/consoler/console.py
--rw-r--r--   0        0        0      507 2024-04-04 08:32:45.869519 consoler-0.1.6/consoler/settings.py
--rw-r--r--   0        0        0     1136 2024-04-04 15:54:28.003786 consoler-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 consoler-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-10 12:25:28.276641 consoler-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1495 2024-04-10 12:25:28.276773 consoler-0.1.7/README.md
+-rw-r--r--   0        0        0       88 2024-04-10 12:25:28.276924 consoler-0.1.7/consoler/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-10 12:25:28.277031 consoler-0.1.7/consoler/colours.py
+-rw-r--r--   0        0        0     7350 2024-04-10 12:34:07.896637 consoler-0.1.7/consoler/console.py
+-rw-r--r--   0        0        0      507 2024-04-10 12:25:28.277320 consoler-0.1.7/consoler/settings.py
+-rw-r--r--   0        0        0     1136 2024-04-10 12:35:12.436782 consoler-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 consoler-0.1.7/PKG-INFO
```

### Comparing `consoler-0.1.6/LICENSE` & `consoler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `consoler-0.1.6/README.md` & `consoler-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `consoler-0.1.6/consoler/colours.py` & `consoler-0.1.7/consoler/colours.py`

 * *Files identical despite different names*

### Comparing `consoler-0.1.6/consoler/console.py` & `consoler-0.1.7/consoler/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,12 +230,11 @@
         return val.decode('utf-8')
     except Exception:
         try:
             return val.decode('latin-1')
         except Exception:
             try:
                 return val.decode('ascii')
-            except Exception:
-                if USE_GURU and settings.DEBUG is False:
-                    guru.error(f'Failed to decode {val}')
+            except Exception:  # noqa: S110
+                pass
 
     return val
```

### Comparing `consoler-0.1.6/pyproject.toml` & `consoler-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "consoler"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Hactar <systems@hactar.is>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hactar-is/consoler"
 repository = "https://github.com/hactar-is/consoler"
```

### Comparing `consoler-0.1.6/PKG-INFO` & `consoler-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoler
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/hactar-is/consoler
 License: MIT
 Keywords: console,terminal,logging
 Author: Hactar
 Author-email: systems@hactar.is
 Requires-Python: >=3.6,<4.0
```

