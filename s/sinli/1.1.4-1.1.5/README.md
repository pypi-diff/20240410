# Comparing `tmp/sinli-1.1.4.tar.gz` & `tmp/sinli-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.4.tar", last modified: Wed Jul 12 10:34:27 2023, max compression
+gzip compressed data, was "sinli-1.1.5.tar", last modified: Wed Apr 10 12:20:30 2024, max compression
```

## Comparing `sinli-1.1.4.tar` & `sinli-1.1.5.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.306263 sinli-1.1.4/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2023-07-12 10:33:18.000000 sinli-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45669 2023-07-12 10:34:27.306263 sinli-1.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5445 2023-07-12 10:33:18.000000 sinli-1.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-12 10:34:17.000000 sinli-1.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:34:27.306263 sinli-1.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     5491 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7418 2023-07-12 10:33:18.000000 sinli-1.1.4/src/sinli/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45669 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-12 10:34:27.000000 sinli-1.1.4/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:34:27.302263 sinli-1.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-12 10:33:18.000000 sinli-1.1.4/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2024-04-10 12:04:33.000000 sinli-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46399 2024-04-10 12:20:30.565737 sinli-1.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6102 2024-04-10 12:04:33.000000 sinli-1.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-10 12:20:20.000000 sinli-1.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:20:30.565737 sinli-1.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3687 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/doctype/devolu/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/devolu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/devolu/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     7418 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/subject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46399 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-10 12:04:33.000000 sinli-1.1.5/tests/test_document.py
```

### Comparing `sinli-1.1.4/LICENSE` & `sinli-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/PKG-INFO` & `sinli-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.4
+Version: 1.1.5
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,14 +666,16 @@
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions==4.3.0
+Requires-Dist: pycountry==22.3.5
 
 # SINLI
 
 ## Introduction and purpose
 
 This package is a libre-free implementation of the [SINLI standard](http://www.fande.es/normalizacion/sinli_indicedocumentos.html).
 It builds on top of email to allow applications to communicate all sort of operations of the book sector in Spain.
@@ -770,14 +772,40 @@
 # SINLI message string
 print(str(catalog))
 
 # Debugging string
 print(repr(catalog))
 ```
 
+Parse a SINLI email subject line
+```python
+from sinli.subject import Subject
+
+subject_line = "ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE"
+subject = Subject.from_str(subject_line)
+
+print(f'Received a SINLI message: {subject.DOCTYPE} ({subject.get_doctype_desc()})')
+# Received a SINLI message: ENVIO (Albarán de envío de distribuidora)
+```
+
+Build a SINLI email subject
+```python
+from sinli.subject import Subject
+
+subject = Subject()
+
+subject.FROM = "L1234567"
+subject.TO = "LIB12345"
+subject.DOCTYPE = "ENVIO"
+subject.VERSION = 8
+
+print(f"Send email with subject '{subject}'")
+# Send email with subject 'ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE'
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.4/README.md` & `sinli-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -97,14 +97,40 @@
 # SINLI message string
 print(str(catalog))
 
 # Debugging string
 print(repr(catalog))
 ```
 
+Parse a SINLI email subject line
+```python
+from sinli.subject import Subject
+
+subject_line = "ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE"
+subject = Subject.from_str(subject_line)
+
+print(f'Received a SINLI message: {subject.DOCTYPE} ({subject.get_doctype_desc()})')
+# Received a SINLI message: ENVIO (Albarán de envío de distribuidora)
+```
+
+Build a SINLI email subject
+```python
+from sinli.subject import Subject
+
+subject = Subject()
+
+subject.FROM = "L1234567"
+subject.TO = "LIB12345"
+subject.DOCTYPE = "ENVIO"
+subject.VERSION = 8
+
+print(f"Send email with subject '{subject}'")
+# Send email with subject 'ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE'
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.4/pyproject.toml` & `sinli-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.1.4"
+version = "1.1.5"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.1.4/src/sinli/common/encoded_values.py` & `sinli-1.1.5/src/sinli/common/encoded_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,7 +133,12 @@
         "O": "Otros"
     },
     ORDER_SOURCE = {
         "N": "Normal",
         "C": "Cliente",
     },
 
+    DEVOLUTION_CAUSE= {
+        "0": "Estropeados", 
+        "1": "Edición desfasada",
+        "2": "Incidencia en la entrega" 
+    }
```

### Comparing `sinli-1.1.4/src/sinli/doctype/__init__.py` & `sinli-1.1.5/src/sinli/doctype/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 from . import libros
 from . import pedido
 from . import envio
 from . import factul
 from . import mensaj
+from . import devolu
 
 class DocumentType(Enum):
     ABONO = ("Albarán o Factura de Abono", None)
     CAMPRE = ("Cambios de precio", None)
     ESTADO = ("Cambios de estado", None)  # noqa: F405
     LIBROS = ("Ficha del Libro", {
         "08": libros.v8.LibrosDoc,
@@ -26,7 +27,11 @@
         "01": factul.v1.FacturaDoc,
         "??": factul.v1.FacturaDoc,
     })
     MENSAJ = ("Mensaje", {
         "01": mensaj.v1.MensajeDoc,
         "??": mensaj.v1.MensajeDoc,
     })
+    DEVOLU = ("Devoluciones", {
+        "02": devolu.v2.DevolucionDoc,
+        "??": devolu.v2.DevolucionDoc,
+    })
```

### Comparing `sinli-1.1.4/src/sinli/doctype/envio/v8.py` & `sinli-1.1.5/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/doctype/factul/v1.py` & `sinli-1.1.5/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/doctype/libros/v8.py` & `sinli-1.1.5/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/doctype/libros/v9.py` & `sinli-1.1.5/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/doctype/mensaj/v1.py` & `sinli-1.1.5/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/doctype/pedido/v7.py` & `sinli-1.1.5/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/document.py` & `sinli-1.1.5/src/sinli/document.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli/line.py` & `sinli-1.1.5/src/sinli/line.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.4/src/sinli.egg-info/PKG-INFO` & `sinli-1.1.5/src/sinli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.4
+Version: 1.1.5
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,14 +666,16 @@
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions==4.3.0
+Requires-Dist: pycountry==22.3.5
 
 # SINLI
 
 ## Introduction and purpose
 
 This package is a libre-free implementation of the [SINLI standard](http://www.fande.es/normalizacion/sinli_indicedocumentos.html).
 It builds on top of email to allow applications to communicate all sort of operations of the book sector in Spain.
@@ -770,14 +772,40 @@
 # SINLI message string
 print(str(catalog))
 
 # Debugging string
 print(repr(catalog))
 ```
 
+Parse a SINLI email subject line
+```python
+from sinli.subject import Subject
+
+subject_line = "ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE"
+subject = Subject.from_str(subject_line)
+
+print(f'Received a SINLI message: {subject.DOCTYPE} ({subject.get_doctype_desc()})')
+# Received a SINLI message: ENVIO (Albarán de envío de distribuidora)
+```
+
+Build a SINLI email subject
+```python
+from sinli.subject import Subject
+
+subject = Subject()
+
+subject.FROM = "L1234567"
+subject.TO = "LIB12345"
+subject.DOCTYPE = "ENVIO"
+subject.VERSION = 8
+
+print(f"Send email with subject '{subject}'")
+# Send email with subject 'ESFANDEL1234567ESFANDELIB12345ENVIO 08FANDE'
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.4/src/sinli.egg-info/SOURCES.txt` & `sinli-1.1.5/src/sinli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 src/sinli/__init__.py
 src/sinli/document.py
 src/sinli/line.py
+src/sinli/subject.py
 src/sinli.egg-info/PKG-INFO
 src/sinli.egg-info/SOURCES.txt
 src/sinli.egg-info/dependency_links.txt
 src/sinli.egg-info/requires.txt
 src/sinli.egg-info/top_level.txt
 src/sinli/common/__init__.py
 src/sinli/common/encoded_values.py
 src/sinli/doctype/__init__.py
+src/sinli/doctype/devolu/__init__.py
+src/sinli/doctype/devolu/v2.py
 src/sinli/doctype/envio/__init__.py
 src/sinli/doctype/envio/v8.py
 src/sinli/doctype/factul/__init__.py
 src/sinli/doctype/factul/v1.py
 src/sinli/doctype/libros/__init__.py
 src/sinli/doctype/libros/v8.py
 src/sinli/doctype/libros/v9.py
```

