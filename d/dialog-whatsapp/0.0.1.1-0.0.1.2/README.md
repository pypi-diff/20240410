# Comparing `tmp/dialog_whatsapp-0.0.1.1.tar.gz` & `tmp/dialog_whatsapp-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_whatsapp-0.0.1.1.tar", max compression
+gzip compressed data, was "dialog_whatsapp-0.0.1.2.tar", max compression
```

## Comparing `dialog_whatsapp-0.0.1.1.tar` & `dialog_whatsapp-0.0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      442 2024-02-19 02:49:52.841907 dialog_whatsapp-0.0.1.1/README.md
--rw-r--r--   0        0        0     5273 2024-02-19 02:49:52.841907 dialog_whatsapp-0.0.1.1/dialog_whatsapp/__init__.py
--rw-r--r--   0        0        0     1916 2024-02-19 02:49:52.841907 dialog_whatsapp-0.0.1.1/dialog_whatsapp/responses.py
--rw-r--r--   0        0        0     1465 2024-02-19 02:49:52.841907 dialog_whatsapp-0.0.1.1/dialog_whatsapp/settings.py
--rw-r--r--   0        0        0      349 2024-02-19 02:49:52.841907 dialog_whatsapp-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      442 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/dialog_whatsapp/__init__.py
+-rw-r--r--   0        0        0     5273 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/dialog_whatsapp/plugin.py
+-rw-r--r--   0        0        0     1916 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/dialog_whatsapp/responses.py
+-rw-r--r--   0        0        0     1465 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/dialog_whatsapp/settings.py
+-rw-r--r--   0        0        0      408 2024-04-09 21:44:03.323806 dialog_whatsapp-0.0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.2/PKG-INFO
```

### Comparing `dialog_whatsapp-0.0.1.1/dialog_whatsapp/__init__.py` & `dialog_whatsapp-0.0.1.2/dialog_whatsapp/plugin.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.1/dialog_whatsapp/responses.py` & `dialog_whatsapp-0.0.1.2/dialog_whatsapp/responses.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.1/dialog_whatsapp/settings.py` & `dialog_whatsapp-0.0.1.2/dialog_whatsapp/settings.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.1/PKG-INFO` & `dialog_whatsapp-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-whatsapp
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: 
 Author: Vinicius Mesel
 Author-email: 4984147+vmesel@users.noreply.github.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

