# Comparing `tmp/adnexus-0.1.1.tar.gz` & `tmp/adnexus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnexus-0.1.1.tar", max compression
+gzip compressed data, was "adnexus-0.1.2.tar", max compression
```

## Comparing `adnexus-0.1.1.tar` & `adnexus-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2024-04-10 09:58:25.321921 adnexus-0.1.1/LICENCE
--rw-r--r--   0        0        0     1950 2024-04-10 09:58:25.321921 adnexus-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/__init__.py
--rw-r--r--   0        0        0      537 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/__init__.py
--rw-r--r--   0        0        0      527 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/base_loader.py
--rw-r--r--   0        0        0      696 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/builtin.py
--rw-r--r--   0        0        0      219 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/config/helpers.py
--rw-r--r--   0        0        0     3809 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/containers.py
--rw-r--r--   0        0        0      668 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/decorators.py
--rw-r--r--   0        0        0      518 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/integrations/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/integrations/starlette.py
--rw-r--r--   0        0        0      172 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/markers.py
--rw-r--r--   0        0        0     2123 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/providers.py
--rw-r--r--   0        0        0     2680 2024-04-10 09:58:25.321921 adnexus-0.1.1/adnexus/wrappers.py
--rw-r--r--   0        0        0      969 2024-04-10 09:58:25.321921 adnexus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 adnexus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-10 11:11:14.497185 adnexus-0.1.2/LICENCE
+-rw-r--r--   0        0        0     2050 2024-04-10 11:11:14.497185 adnexus-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/config/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/config/base_loader.py
+-rw-r--r--   0        0        0      696 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/config/builtin.py
+-rw-r--r--   0        0        0      219 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/config/helpers.py
+-rw-r--r--   0        0        0     3809 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/containers.py
+-rw-r--r--   0        0        0      668 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/decorators.py
+-rw-r--r--   0        0        0      518 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/integrations/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/integrations/starlette.py
+-rw-r--r--   0        0        0      172 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/markers.py
+-rw-r--r--   0        0        0     2123 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/providers.py
+-rw-r--r--   0        0        0     2680 2024-04-10 11:11:14.497185 adnexus-0.1.2/adnexus/wrappers.py
+-rw-r--r--   0        0        0     1074 2024-04-10 11:11:14.497185 adnexus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 adnexus-0.1.2/PKG-INFO
```

### Comparing `adnexus-0.1.1/LICENCE` & `adnexus-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/README.md` & `adnexus-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml)
+[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml) [![Docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml)
 # XDI Framework
 **XDI is a modern and declarative DI and IoC framework using pydantic for config and data.**
 
 ## Key features
 
 - **Fast:** Very high performance thanks to pydantic and preemptive wiring
 - **Developer friendly:** Declarative Container definition to take the "Magic" out of DI
 - **Good compatibility:** Can be used with almost every framework and supports async
 
-## Installation (via git for now)
+## Installation
 ```bash
-pip install git+https://github.com/Nictec/XDI
+pip install adnexus
 ```
 
 ## Basic Example
 
 ```python3
 from pathlib import Path
 from datetime import datetime
```

### Comparing `adnexus-0.1.1/adnexus/config/__init__.py` & `adnexus-0.1.2/adnexus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/config/base_loader.py` & `adnexus-0.1.2/adnexus/config/base_loader.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/config/builtin.py` & `adnexus-0.1.2/adnexus/config/builtin.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/containers.py` & `adnexus-0.1.2/adnexus/containers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/decorators.py` & `adnexus-0.1.2/adnexus/decorators.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/exceptions.py` & `adnexus-0.1.2/adnexus/exceptions.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/integrations/starlette.py` & `adnexus-0.1.2/adnexus/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/providers.py` & `adnexus-0.1.2/adnexus/providers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/adnexus/wrappers.py` & `adnexus-0.1.2/adnexus/wrappers.py`

 * *Files identical despite different names*

### Comparing `adnexus-0.1.1/pyproject.toml` & `adnexus-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "adnexus"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "Modern and fully typed declarative Di and IoC Framework"
 authors = [ "nl <nl@x-net.at>",]
 readme = "README.md"
+repository = "https://github.com/Nictec/adnexus/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.6.4"
 pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
```

### Comparing `adnexus-0.1.1/PKG-INFO` & `adnexus-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: adnexus
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Modern and fully typed declarative Di and IoC Framework
+Home-page: https://github.com/Nictec/adnexus/
 Author: nl
 Author-email: nl@x-net.at
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Project-URL: Repository, https://github.com/Nictec/adnexus/
 Description-Content-Type: text/markdown
 
-[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml)
+[![tests](https://github.com/Nictec/XDI/actions/workflows/main.yml/badge.svg)](https://github.com/Nictec/XDI/actions/workflows/main.yml) [![Docs](https://github.com/Nictec/adnexus/actions/workflows/docs.yml/badge.svg)](https://github.com/Nictec/adnexus/actions/workflows/docs.yml)
 # XDI Framework
 **XDI is a modern and declarative DI and IoC framework using pydantic for config and data.**
 
 ## Key features
 
 - **Fast:** Very high performance thanks to pydantic and preemptive wiring
 - **Developer friendly:** Declarative Container definition to take the "Magic" out of DI
 - **Good compatibility:** Can be used with almost every framework and supports async
 
-## Installation (via git for now)
+## Installation
 ```bash
-pip install git+https://github.com/Nictec/XDI
+pip install adnexus
 ```
 
 ## Basic Example
 
 ```python3
 from pathlib import Path
 from datetime import datetime
```

