# Comparing `tmp/omni-api-0.5.0.tar.gz` & `tmp/omni-api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omni-api-0.5.0.tar", last modified: Thu Jan 19 11:37:26 2023, max compression
+gzip compressed data, was "dist/omni-api-0.5.1.tar", last modified: Wed Apr 10 10:29:14 2024, max compression
```

## Comparing `omni-api-0.5.0.tar` & `omni-api-0.5.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:37:26.000000 omni-api-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     2726 2023-01-19 11:37:20.000000 omni-api-0.5.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-01-19 11:37:26.000000 omni-api-0.5.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni/
--rw-r--r--   0 root         (0) root         (0)     3768 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/sale.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/media.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/errors.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/consignment_out.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/credit_note.py
--rw-r--r--   0 root         (0) root         (0)     1428 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/status.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/entity.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/return_.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/util.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/transfer.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/document.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/store.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/system_company.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni/models/
--rw-r--r--   0 root         (0) root         (0)     1435 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/sale.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/operation.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/line.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/entity.py
--rw-r--r--   0 root         (0) root         (0)     1354 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/merchandise.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/base.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/product.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/invoice.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/supplier.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/user.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/stock_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/sub_product.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/sale_order.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/consignment_slip.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/web.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/sale_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/signed_document.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/merchandise.py
--rw-r--r--   0 root         (0) root         (0)    10007 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/base.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/customer.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/receipt.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/identifiable.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/money_sale_slip.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/employee.py
--rw-r--r--   0 root         (0) root         (0)     4214 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/export.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-01-19 11:37:20.000000 omni-api-0.5.0/src/omni/inventory_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 11:37:22.000000 omni-api-0.5.0/src/omni_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     4960 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1200 2023-01-19 11:37:26.000000 omni-api-0.5.0/src/omni_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-19 11:37:26.000000 omni-api-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3434 2023-01-19 11:37:20.000000 omni-api-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:29:14.000000 omni-api-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-10 10:29:14.000000 omni-api-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3434 2024-04-10 10:29:08.000000 omni-api-0.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-10 10:29:08.000000 omni-api-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:29:10.000000 omni-api-0.5.1/src/omni_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     4960 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni_api.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni/
+-rw-r--r--   0 root         (0) root         (0)     3832 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/util.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/consignment_out.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/export.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/sub_product.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/return_.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/receipt.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/stock_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/consignment_slip.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/document.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/inventory_line.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/sale_order.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/signed_document.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/sale_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/store.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/customer.py
+-rw-r--r--   0 root         (0) root         (0)     9954 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/base.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/entity.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/saft_pt.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/media.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/product.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/web.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/user.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/identifiable.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/sale.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/supplier.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/merchandise.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/status.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/employee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:29:14.000000 omni-api-0.5.1/src/omni/models/
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/line.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/entity.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/operation.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/sale.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/models/merchandise.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/system_company.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/money_sale_slip.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-10 10:29:08.000000 omni-api-0.5.1/src/omni/credit_note.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2024-04-10 10:29:14.000000 omni-api-0.5.1/PKG-INFO
```

### Comparing `omni-api-0.5.0/setup.py` & `omni-api-0.5.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,65 +18,51 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "omni-api",
-    version = "0.5.0",
-    author = "Hive Solutions Lda.",
-    author_email = "development@hive.pt",
-    description = "Omni API Client",
-    license = "Apache License, Version 2.0",
-    keywords = "omni api",
-    url = "http://omni-api.hive.pt",
-    zip_safe = False,
-    packages = [
-        "omni",
-        "omni.models"
-    ],
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    install_requires = [
-        "appier"
-    ],
-    classifiers = [
+    name="omni-api",
+    version="0.5.1",
+    author="Hive Solutions Lda.",
+    author_email="development@hive.pt",
+    description="Omni API Client",
+    license="Apache License, Version 2.0",
+    keywords="omni api",
+    url="http://omni-api.hive.pt",
+    zip_safe=False,
+    packages=["omni", "omni.models"],
+    package_dir={"": os.path.normpath("src")},
+    install_requires=["appier"],
+    classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
-    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
-    long_description_content_type = "text/markdown"
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `omni-api-0.5.0/PKG-INFO` & `omni-api-0.5.1/src/omni_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Omni API Client
 Home-page: http://omni-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni API](http://omni-api.hive.pt)
```

### Comparing `omni-api-0.5.0/src/omni/sale.py` & `omni-api-0.5.1/src/omni/sale.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,99 +18,85 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class SaleAPI(object):
 
     def list_sales(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/sales.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def create_sale(self, payload):
         url = self.base_url + "omni/sales.json"
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
     def get_sale(self, object_id):
         url = self.base_url + "omni/sales/%d.json" % object_id
         contents = self.get(url)
         return contents
 
     def vat_sale(self, object_id):
         url = self.base_url + "omni/sales/%d/vat.json" % object_id
         contents = self.get(url)
         return contents
 
-    def issue_money_sale_slip_sale(self, object_id, metadata = {}):
+    def issue_money_sale_slip_sale(self, object_id, metadata={}):
         url = self.base_url + "omni/sales/%d/issue_money_sale_slip.json" % object_id
-        contents = self.post(url, data_j = dict(metadata = metadata))
+        contents = self.post(url, data_j=dict(metadata=metadata))
         return contents
 
-    def issue_invoice_sale(self, object_id, metadata = None):
+    def issue_invoice_sale(self, object_id, metadata=None):
         url = self.base_url + "omni/sales/%d/issue_invoice.json" % object_id
-        contents = self.post(url, data_j = dict(metadata = metadata))
+        contents = self.post(url, data_j=dict(metadata=metadata))
         return contents
 
-    def issue_receipt_sale(self, object_id, metadata = None):
+    def issue_receipt_sale(self, object_id, metadata=None):
         url = self.base_url + "omni/sales/%d/issue_receipt.json" % object_id
-        contents = self.post(url, data_j = dict(metadata = metadata))
+        contents = self.post(url, data_j=dict(metadata=metadata))
         return contents
 
-    def ensure_receipt_sale(self, object_id, metadata = None):
+    def ensure_receipt_sale(self, object_id, metadata=None):
         url = self.base_url + "omni/sales/%d/ensure_receipt.json" % object_id
-        contents = self.post(url, data_j = dict(metadata = metadata))
+        contents = self.post(url, data_j=dict(metadata=metadata))
         return contents
 
     def self_sales(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/sales/self.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def stats_sales(
         self,
-        date = None,
-        unit = "day",
-        span = 7,
-        store_id = None,
-        has_global = None,
-        output = "simple"
+        date=None,
+        unit="day",
+        span=7,
+        store_id=None,
+        has_global=None,
+        output="simple",
     ):
         url = self.base_url + "omni/sale_snapshots/stats.json"
         contents = self.get(
             url,
-            date = date,
-            unit = unit,
-            span = span,
-            store_id = store_id,
-            has_global = has_global,
-            output = output
+            date=date,
+            unit=unit,
+            span=span,
+            store_id=store_id,
+            has_global=has_global,
+            output=output,
         )
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/media.py` & `omni-api-0.5.1/src/omni/media.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,65 +18,55 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import base64
 
 import appier
 
 from . import util
 
+
 class MediaAPI(object):
 
     def list_media(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/media.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def info_media(self, object_id):
         url = self.base_url + "omni/media/%d/info.json" % object_id
         contents = self.get(url)
         return contents
 
     def update_media(self, object_id, payload):
         self._wrap_data(payload)
         url = self.base_url + "omni/media/%d/update.json" % object_id
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
     def delete_media(self, object_id):
         url = self.base_url + "omni/media/%d/delete.json" % object_id
         contents = self.post(url)
         return contents
 
-    def get_media_url(self, secret, size = "original"):
+    def get_media_url(self, secret, size="original"):
         return self.open_url + "omni/media/%s" % secret
 
     def _wrap_data(self, payload):
-        if not "data" in payload: return
+        if not "data" in payload:
+            return
         data = payload["data"]
         data_b64 = base64.b64encode(data)
         data_b64 = appier.legacy.str(data_b64)
         payload["data_b64"] = data_b64
         del payload["data"]
```

### Comparing `omni-api-0.5.0/src/omni/errors.py` & `omni-api-0.5.1/src/omni/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,34 +18,26 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import appier
 
+
 class OmniError(appier.APIError):
 
-    def __init__(self, error, exception = {}):
+    def __init__(self, error, exception={}):
         appier.APIError.__init__(self, "Omni internal error")
         self.error = error
         self.exception = exception
 
     def __str__(self):
         return self.full_message()
```

### Comparing `omni-api-0.5.0/src/omni/consignment_out.py` & `omni-api-0.5.1/src/omni/consignment_out.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,58 +18,47 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class ConsignmentOutAPI(object):
 
     def list_consignments_out(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/consignments_out.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def create_consignment_out(self, payload):
         url = self.base_url + "omni/consignments_out.json"
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
     def get_consignment_out(self, object_id):
         url = self.base_url + "omni/consignments_out/%d.json" % object_id
         contents = self.get(url)
         return contents
 
-    def issue_consignment_slip_consignment_out(self, object_id, metadata = {}):
-        url = self.base_url + "omni/consignments_out/%d/issue_consignment_slip.json" % object_id
-        contents = self.post(url, data_j = dict(metadata = metadata))
+    def issue_consignment_slip_consignment_out(self, object_id, metadata={}):
+        url = (
+            self.base_url
+            + "omni/consignments_out/%d/issue_consignment_slip.json" % object_id
+        )
+        contents = self.post(url, data_j=dict(metadata=metadata))
         return contents
 
     def self_consignments_out(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/consignments_out/self.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/credit_note.py` & `omni-api-0.5.1/src/omni/store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,43 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class CreditNoteAPI(object):
 
-    @classmethod
-    def normalize_credit_note(cls, credit_note):
-        cls.normalize_invoice(credit_note)
+class StoreAPI(object):
 
-    def list_credit_notes(self, *args, **kwargs):
+    def list_stores(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/credit_notes.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/stores.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_credit_note(self, object_id):
-        url = self.base_url + "omni/credit_notes/%d.json" % object_id
+    def get_store(self, object_id):
+        url = self.base_url + "omni/stores/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/status.py` & `omni-api-0.5.1/src/omni/models/customer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,28 +18,18 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-class StatusAPI(object):
+from . import base
+
 
-    def get_status(self):
-        url = self.base_url + "omni/status.json"
-        contents = self.get(url)
-        return contents
+class Customer(base.Base):
+    pass
```

### Comparing `omni-api-0.5.0/src/omni/entity.py` & `omni-api-0.5.1/src/omni/entity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,142 +18,103 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import base64
 
 import appier
 
 from . import util
 
+
 class EntityAPI(object):
 
     def list_entities(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/entities.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def get_entity(self, object_id):
         url = self.base_url + "omni/entities/%d.json" % object_id
         contents = self.get(url)
         return contents
 
     def update_entity(self, object_id, payload):
         url = self.base_url + "omni/entities/%d/update.json" % object_id
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
     def sequence_entity(self, object_id):
         url = self.base_url + "omni/entities/%d/sequence.json" % object_id
         contents = self.get(url)
         return contents
 
-    def media_entity(
-        self,
-        object_id,
-        position = None,
-        dimensions = None,
-        label = None
-    ):
+    def media_entity(self, object_id, position=None, dimensions=None, label=None):
         url = self.base_url + "omni/entities/%d/media.json" % object_id
-        contents = self.get(
-            url,
-            position = position,
-            dimensions = dimensions,
-            label = label
-        )
+        contents = self.get(url, position=position, dimensions=dimensions, label=label)
         return contents
 
     def public_media_entity(
-        self,
-        object_id,
-        position = None,
-        dimensions = None,
-        label = None
+        self, object_id, position=None, dimensions=None, label=None
     ):
         url = self.base_url + "omni/entities/%d/media/public.json" % object_id
-        contents = self.get(
-            url,
-            position = position,
-            dimensions = dimensions,
-            label = label
-        )
+        contents = self.get(url, position=position, dimensions=dimensions, label=label)
         return contents
 
-    def info_media_entity(
-        self,
-        object_id,
-        position = None,
-        dimensions = None,
-        label = None
-    ):
+    def info_media_entity(self, object_id, position=None, dimensions=None, label=None):
         url = self.base_url + "omni/entities/%d/media/info.json" % object_id
-        contents = self.get(
-            url,
-            position = position,
-            dimensions = dimensions,
-            label = label
-        )
+        contents = self.get(url, position=position, dimensions=dimensions, label=label)
         return contents
 
     def set_media_entity(
         self,
         object_id,
         data,
-        position = None,
-        label = None,
-        mime_type = None,
-        width = None,
-        height = None,
-        dimensions = None,
-        url = None,
-        visibility = None,
-        description = None,
-        engine = None,
-        thumbnails = None
+        position=None,
+        label=None,
+        mime_type=None,
+        width=None,
+        height=None,
+        dimensions=None,
+        url=None,
+        visibility=None,
+        description=None,
+        engine=None,
+        thumbnails=None,
     ):
         data_b64 = base64.b64encode(data)
         data_b64 = appier.legacy.str(data_b64)
         data_j = dict(
-            data_b64 = data_b64,
-            label = label,
-            mime_type = mime_type,
-            width = width,
-            height = height,
-            dimensions = dimensions,
-            url = url,
-            visibility = visibility,
-            description = description
+            data_b64=data_b64,
+            label=label,
+            mime_type=mime_type,
+            width=width,
+            height=height,
+            dimensions=dimensions,
+            url=url,
+            visibility=visibility,
+            description=description,
         )
-        if not position == None: data_j["position"] = position
-        if not engine == None: data_j["engine"] = engine
-        if not thumbnails == None: data_j["thumbnails"] = thumbnails
+        if not position == None:
+            data_j["position"] = position
+        if not engine == None:
+            data_j["engine"] = engine
+        if not thumbnails == None:
+            data_j["thumbnails"] = thumbnails
         url = self.base_url + "omni/entities/%d/media/set.json" % object_id
-        contents = self.post(url, data_j = data_j)
+        contents = self.post(url, data_j=data_j)
         return contents
 
     def clear_media_entity(self, object_id):
         url = self.base_url + "omni/entities/%d/media/clear.json" % object_id
         contents = self.post(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/return_.py` & `omni-api-0.5.1/src/omni/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,43 +18,20 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import util
 
-class ReturnAPI(object):
-
-    def list_returns(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/returns.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+class StatusAPI(object):
 
-    def self_returns(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/returns/self.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+    def get_status(self):
+        url = self.base_url + "omni/status.json"
+        contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/util.py` & `omni-api-0.5.1/src/omni/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,44 +18,44 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
+
 def format_places(number, places):
     format_s = "%%0.0%df" % places
     return format_s % number
 
+
 def filter_args(kwargs):
-    if not "object" in kwargs: return
+    if not "object" in kwargs:
+        return
     object = kwargs["object"]
 
     filter_def = object.get("find_d", None)
     filter_string = object.get("find_s", "")
     start_record = object.get("skip", 0)
     number_records = object.get("limit", 10)
 
     kwargs["start_record"] = start_record
     kwargs["number_records"] = number_records
-    if filter_def: kwargs["filters[]"] = [
-        "%s:%s" % (filter_part, filter_string) if filter_part.count(":") < 2 else\
-            filter_part for filter_part in filter_def
-    ]
-    else: kwargs["filter_string"] = filter_string
+    if filter_def:
+        kwargs["filters[]"] = [
+            (
+                "%s:%s" % (filter_part, filter_string)
+                if filter_part.count(":") < 2
+                else filter_part
+            )
+            for filter_part in filter_def
+        ]
+    else:
+        kwargs["filter_string"] = filter_string
 
     del kwargs["object"]
```

### Comparing `omni-api-0.5.0/src/omni/transfer.py` & `omni-api-0.5.1/src/omni/product.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,44 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class TransferAPI(object):
 
-    def list_transfers(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/transfers.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+class ProductAPI(object):
 
-    def create_transfer(self, payload):
-        url = self.base_url + "omni/transfers.json"
-        contents = self.post(url, data_j = payload)
+    def list_products(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/products.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_transfer(self, object_id):
-        url = self.base_url + "omni/transfers/%d.json" % object_id
+    def get_product(self, object_id):
+        url = self.base_url + "omni/products/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/document.py` & `omni-api-0.5.1/src/omni/document.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,48 +18,35 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class DocumentAPI(object):
 
     def list_documents(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/documents.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     @classmethod
     def default_customers(cls, documents):
         for document in documents:
             cls.default_customer(document)
 
     @classmethod
     def default_customer(cls, document):
         payload = document["payload"]
         operation = payload.get("operation", {})
         customer = operation.get("customer", None)
-        operation["customer"] = customer or dict(
-            short_name = "Anonymous"
-        )
+        operation["customer"] = customer or dict(short_name="Anonymous")
```

### Comparing `omni-api-0.5.0/src/omni/store.py` & `omni-api-0.5.1/src/omni/inventory_line.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,39 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class StoreAPI(object):
 
-    def list_stores(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/stores.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+class InventoryLineAPI(object):
 
-    def get_store(self, object_id):
-        url = self.base_url + "omni/stores/%d.json" % object_id
-        contents = self.get(url)
+    def list_inventory_lines(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/inventory_lines.json"
+        contents = self.get(url, **kwargs)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/system_company.py` & `omni-api-0.5.1/src/omni/system_company.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,67 +18,43 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
+
 class SystemCompanyAPI(object):
 
     def load_system_company(self):
         contents = self.self_system_company()
         self.company = contents
 
     def self_system_company(self):
         url = self.base_url + "omni/system_companies/self.json"
         contents = self.get(url)
         return contents
 
     def update_self_system_company(self, payload):
         url = self.base_url + "omni/system_companies/self/update.json"
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
-    def media_system_company(
-        self,
-        position = None,
-        dimensions = None,
-        label = None
-    ):
+    def media_system_company(self, position=None, dimensions=None, label=None):
         system_company = self.self_system_company()
         object_id = system_company["object_id"]
         return self.media_entity(
-            object_id,
-            position = position,
-            dimensions = dimensions,
-            label = label
+            object_id, position=position, dimensions=dimensions, label=label
         )
 
-    def public_media_system_company(
-        self,
-        position = None,
-        dimensions = None,
-        label = None
-    ):
+    def public_media_system_company(self, position=None, dimensions=None, label=None):
         system_company = self.self_system_company()
         object_id = system_company["object_id"]
         return self.public_media_entity(
-            object_id,
-            position = position,
-            dimensions = dimensions,
-            label = label
+            object_id, position=position, dimensions=dimensions, label=label
         )
```

### Comparing `omni-api-0.5.0/src/omni/models/sale.py` & `omni-api-0.5.1/src/omni/identifiable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,33 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import operation
+from . import util
 
-class Sale(operation.Operation):
 
-    discount = dict(
-        type = float
-    )
+class IdentifiableAPI(object):
 
-    discount_vat = dict(
-        type = float
-    )
+    def list_identifiables(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/identifiables.json"
+        contents = self.get(url, **kwargs)
+        return contents
```

### Comparing `omni-api-0.5.0/src/omni/models/operation.py` & `omni-api-0.5.1/src/omni/models/entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,29 +18,18 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
 
-class Operation(base.Base):
 
-    type = dict(
-        type = int
-    )
+class Entity(base.Base):
+    pass
```

### Comparing `omni-api-0.5.0/src/omni/models/line.py` & `omni-api-0.5.1/src/omni/models/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,41 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import base
+import appier
 
-class Line(base.Base):
 
-    price = dict(
-        type = float
-    )
+class Base(appier.Model):
 
-    price_vat = dict(
-        type = float
-    )
+    object_id = dict(type=int)
 
-    vat_rate = dict(
-        type = float
-    )
+    description = dict()
 
-    quantity = dict(
-        type = float
-    )
+    metadata = dict(type=dict)
```

### Comparing `omni-api-0.5.0/src/omni/models/entity.py` & `omni-api-0.5.1/src/omni/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,29 +15,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
-__author__ = "João Magalhães <joamag@hive.pt>"
-""" The author(s) of the module """
-
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
-
-class Entity(base.Base):
-    pass
+from . import customer
+from . import entity
+from . import line
+from . import merchandise
+from . import operation
+from . import sale
+
+from .base import Base
+from .customer import Customer
+from .entity import Entity
+from .line import Line
+from .merchandise import Merchandise
+from .operation import Operation
+from .sale import Sale
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `omni-api-0.5.0/src/omni/models/merchandise.py` & `omni-api-0.5.1/src/omni/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,27 +18,20 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import base
 
-class Merchandise(base.Base):
+class UserAPI(object):
 
-    company_product_code = dict()
+    def self_user(self):
+        url = self.base_url + "omni/users/self.json"
+        contents = self.get(url)
+        return contents
```

### Comparing `omni-api-0.5.0/src/omni/models/base.py` & `omni-api-0.5.1/src/omni/models/operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,35 +18,19 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-import appier
-
-class Base(appier.Model):
+from . import base
 
-    object_id = dict(
-        type = int
-    )
 
-    description = dict()
+class Operation(base.Base):
 
-    metadata = dict(
-        type = dict
-    )
+    type = dict(type=int)
```

### Comparing `omni-api-0.5.0/src/omni/models/customer.py` & `omni-api-0.5.1/src/omni/models/line.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,26 +18,25 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
 
-class Customer(base.Base):
-    pass
+
+class Line(base.Base):
+
+    price = dict(type=float)
+
+    price_vat = dict(type=float)
+
+    vat_rate = dict(type=float)
+
+    quantity = dict(type=float)
```

### Comparing `omni-api-0.5.0/src/omni/product.py` & `omni-api-0.5.1/src/omni/sub_product.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,39 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class ProductAPI(object):
 
-    def list_products(self, *args, **kwargs):
+class SubProductAPI(object):
+
+    def list_sub_products(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/products.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/sub_products.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_product(self, object_id):
-        url = self.base_url + "omni/products/%d.json" % object_id
+    def get_sub_product(self, object_id):
+        url = self.base_url + "omni/sub_products/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/invoice.py` & `omni-api-0.5.1/src/omni/receipt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,36 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class InvoiceAPI(object):
+
+class ReceiptAPI(object):
 
     @classmethod
-    def normalize_invoice(cls, invoice):
-        payload = invoice.get("payload", {})
+    def normalize_receipt(cls, receipt):
+        payload = receipt.get("payload", {})
         operation = payload.get("operation", {})
 
         type = operation.get("type", 1)
 
         if type == 1:
             operation["subtotal"] = operation["price_vat"] + operation["discount_vat"]
         elif type == 2:
@@ -56,15 +48,17 @@
         operation["vat_s"] = util.format_places(operation["vat"], 2)
         operation["subtotal_s"] = util.format_places(operation["subtotal"], 2)
 
         if "discount" in operation and not operation["discount"] == None:
             operation["discount_s"] = util.format_places(operation["discount"], 2)
 
         if "discount_vat" in operation and not operation["discount_vat"] == None:
-            operation["discount_vat_s"] = util.format_places(operation["discount_vat"], 2)
+            operation["discount_vat_s"] = util.format_places(
+                operation["discount_vat"], 2
+            )
 
         operation["price_vat_s"] = util.format_places(operation["price_vat"], 2)
 
         for item in operation["vat_list"]:
             item["vat_rate_s"] = util.format_places(item["vat_rate"], 2)
             item["vat_s"] = util.format_places(item["vat"], 2)
 
@@ -75,32 +69,31 @@
             merchandise = line["merchandise"]
             line["vat_rate_s"] = util.format_places(line["vat_rate"], 2)
             line["quantity_s"] = util.format_places(
                 line["quantity"],
                 merchandise.get("quantity_places", 0) or 0,
             )
             line["unit_discount_s"] = util.format_places(line["unit_discount"], 2)
-            line["unit_discount_vat_s"] = util.format_places(line["unit_discount_vat"], 2)
+            line["unit_discount_vat_s"] = util.format_places(
+                line["unit_discount_vat"], 2
+            )
             line["unit_price_s"] = util.format_places(line["unit_price"]["value"], 2)
             line["unit_price_vat_s"] = util.format_places(line["unit_price_vat"], 2)
             line["price_s"] = util.format_places(line["price"], 2)
             line["price_vat_s"] = util.format_places(line["price_vat"], 2)
             line["weight_s"] = util.format_places(
                 (merchandise["weight"] or 0.0) * line["quantity"], 3
             )
 
         if "sale_lines" in operation:
             operation["lines"] = operation["sale_lines"]
 
-    def list_invoices(self, *args, **kwargs):
+    def list_receipts(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/invoices.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/receipts.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_invoice(self, object_id):
-        url = self.base_url + "omni/invoices/%d.json" % object_id
+    def get_receipt(self, object_id):
+        url = self.base_url + "omni/receipts/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/supplier.py` & `omni-api-0.5.1/src/omni/money_sale_slip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,48 +18,32 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class SupplierAPI(object):
 
-    def list_suppliers(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/suppliers.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+class MoneySaleSlipAPI(object):
+
+    @classmethod
+    def normalize_money_sale_slip(cls, money_sale_slip):
+        cls.normalize_invoice(money_sale_slip)
 
-    def list_companies(self, *args, **kwargs):
+    def list_money_sale_slips(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/supplier_companies.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/money_sale_slips.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_company(self, object_id):
-        url = self.base_url + "omni/supplier_companies/%d.json" % object_id
+    def get_money_sale_slip(self, object_id):
+        url = self.base_url + "omni/money_sale_slips/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/user.py` & `omni-api-0.5.1/src/omni/sale_snapshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,28 +18,20 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-class UserAPI(object):
 
-    def self_user(self):
-        url = self.base_url + "omni/users/self.json"
-        contents = self.get(url)
+class SaleSnapshotAPI(object):
+
+    def entries_sales_snapshot(self, payload):
+        url = self.base_url + "omni/sale_snapshots/apply/entries.json"
+        contents = self.post(url, data_j=payload)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/stock_adjustment.py` & `omni-api-0.5.1/src/omni/stock_adjustment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,44 +18,33 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class StockAdjustmentAPI(object):
 
     def list_stock_adjustments(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/stock_adjustments.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def create_stock_adjustment(self, payload):
         url = self.base_url + "omni/stock_adjustments.json"
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
 
     def get_stock_adjustment(self, object_id):
         url = self.base_url + "omni/stock_adjustments/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/sub_product.py` & `omni-api-0.5.1/src/omni/sale_order.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,39 +18,23 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class SubProductAPI(object):
 
-    def list_sub_products(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/sub_products.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+class SaleOrderAPI(object):
 
-    def get_sub_product(self, object_id):
-        url = self.base_url + "omni/sub_products/%d.json" % object_id
-        contents = self.get(url)
+    def list_sale_orders(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/sale_orders.json"
+        contents = self.get(url, **kwargs)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/sale_order.py` & `omni-api-0.5.1/src/omni/web.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,34 +18,20 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import util
 
-class SaleOrderAPI(object):
+class WebAPI(object):
 
-    def list_sale_orders(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/sale_orders.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+    def subscribe_web(self, callback_url):
+        url = self.base_url + "omni/web/subscribe.json"
+        contents = self.post(url, params=dict(url=callback_url))
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/consignment_slip.py` & `omni-api-0.5.1/src/omni/consignment_slip.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,43 +18,32 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class ConsignmentSlipAPI(object):
 
     @classmethod
     def normalize_consignment_slip(cls, consignment_slip):
         cls.normalize_invoice(consignment_slip)
 
     def list_consignment_slips(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/consignment_slips.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def get_consignment_slip(self, object_id):
         url = self.base_url + "omni/consignment_slips/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/web.py` & `omni-api-0.5.1/src/omni/models/sale.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,33 +18,21 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-class WebAPI(object):
+from . import operation
+
+
+class Sale(operation.Operation):
+
+    discount = dict(type=float)
 
-    def subscribe_web(self, callback_url):
-        url = self.base_url + "omni/web/subscribe.json"
-        contents = self.post(
-            url,
-            params = dict(
-                url = callback_url
-            )
-        )
-        return contents
+    discount_vat = dict(type=float)
```

### Comparing `omni-api-0.5.0/src/omni/sale_snapshot.py` & `omni-api-0.5.1/src/omni/credit_note.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,28 +18,32 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-class SaleSnapshotAPI(object):
+from . import util
+
+
+class CreditNoteAPI(object):
+
+    @classmethod
+    def normalize_credit_note(cls, credit_note):
+        cls.normalize_invoice(credit_note)
+
+    def list_credit_notes(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/credit_notes.json"
+        contents = self.get(url, **kwargs)
+        return contents
 
-    def entries_sales_snapshot(self, payload):
-        url = self.base_url + "omni/sale_snapshots/apply/entries.json"
-        contents = self.post(url, data_j = payload)
+    def get_credit_note(self, object_id):
+        url = self.base_url + "omni/credit_notes/%d.json" % object_id
+        contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/signed_document.py` & `omni-api-0.5.1/src/omni/signed_document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,59 +18,57 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class SignedDocumentAPI(object):
 
     def list_signed_documents(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/signed_documents.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def qr_code_document(self, object_id):
         url = self.base_url + "omni/signed_documents/%d/qr_code" % object_id
         contents = self.get(url)
         return contents
 
     def digest_identifier_document(self, object_id):
-        url = self.base_url + "omni/signed_documents/%d/digest_identifier.json" % object_id
+        url = (
+            self.base_url
+            + "omni/signed_documents/%d/digest_identifier.json" % object_id
+        )
         contents = self.get(url)
         return contents["digest_identifier"]
 
     def verify_signed_document(self, object_id):
         url = self.base_url + "omni/signed_documents/%d/verify.json" % object_id
         contents = self.get(url)
         return contents
 
     def submit_invoice_at(self, object_id):
-        url = self.base_url + "omni/signed_documents/%d/submit_invoice_at.json" % object_id
+        url = (
+            self.base_url
+            + "omni/signed_documents/%d/submit_invoice_at.json" % object_id
+        )
         contents = self.get(url)
         return contents
 
     def submit_transport_at(self, object_id):
-        url = self.base_url + "omni/signed_documents/%d/submit_transport_at.json" % object_id
+        url = (
+            self.base_url
+            + "omni/signed_documents/%d/submit_transport_at.json" % object_id
+        )
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/merchandise.py` & `omni-api-0.5.1/src/omni/merchandise.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,57 +18,42 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class MerchandiseAPI(object):
 
     def list_merchandise(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/merchandise.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def update_merchandise(self, object_id, payload):
         url = self.base_url + "omni/merchandise/%d/update.json" % object_id
-        contents = self.post(url, data_m = payload)
+        contents = self.post(url, data_m=payload)
         return contents
 
-    def list_store_merchandise(self, store_id = None, *args, **kwargs):
+    def list_store_merchandise(self, store_id=None, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/merchandise/store.json"
-        contents = self.get(
-            url,
-            store_id = store_id,
-            **kwargs
-        )
+        contents = self.get(url, store_id=store_id, **kwargs)
         return contents
 
     def prices_merchandise(self, items):
         url = self.base_url + "omni/merchandise/prices.json"
-        self.put(url, data_j = items)
+        self.put(url, data_j=items)
 
     def costs_merchandise(self, items):
         url = self.base_url + "omni/merchandise/costs.json"
-        self.put(url, data_j = items)
+        self.put(url, data_j=items)
```

### Comparing `omni-api-0.5.0/src/omni/base.py` & `omni-api-0.5.1/src/omni/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,24 +18,15 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import appier
 
@@ -44,14 +35,15 @@
 from . import user
 from . import store
 from . import media
 from . import errors
 from . import entity
 from . import status
 from . import return_
+from . import saft_pt
 from . import invoice
 from . import product
 from . import receipt
 from . import customer
 from . import supplier
 from . import transfer
 from . import document
@@ -87,29 +79,31 @@
 in case none is provided to the API (client) """
 
 SCOPE = (
     "base",
     "base.user",
     "base.admin",
     "foundation.store.list",
-    "foundation.web.subscribe"
+    "foundation.web.subscribe",
 )
 """ The list of permissions to be used to create the
 scope string for the OAuth value """
 
+
 class API(
     appier.OAuth2API,
     web.WebAPI,
     sale.SaleAPI,
     user.UserAPI,
     store.StoreAPI,
     media.MediaAPI,
     entity.EntityAPI,
     status.StatusAPI,
     return_.ReturnAPI,
+    saft_pt.SaftPtAPI,
     invoice.InvoiceAPI,
     product.ProductAPI,
     receipt.ReceiptAPI,
     customer.CustomerAPI,
     supplier.SupplierAPI,
     transfer.TransferAPI,
     document.DocumentAPI,
@@ -122,15 +116,15 @@
     sale_snapshot.SaleSnapshotAPI,
     inventory_line.InventoryLineAPI,
     system_company.SystemCompanyAPI,
     money_sale_slip.MoneySaleSlipAPI,
     signed_document.SignedDocumentAPI,
     consignment_out.ConsignmentOutAPI,
     consignment_slip.ConsignmentSlipAPI,
-    stock_adjustment.StockAdjustmentAPI
+    stock_adjustment.StockAdjustmentAPI,
 ):
 
     def __init__(self, *args, **kwargs):
         appier.OAuth2API.__init__(self, *args, **kwargs)
         self.base_url = appier.conf("OMNI_BASE_URL", BASE_URL)
         self.open_url = appier.conf("OMNI_OPEN_URL", self.base_url)
         self.prefix = appier.conf("OMNI_PREFIX", "adm/")
@@ -158,131 +152,144 @@
         self.wrap_exception = kwargs.get("wrap_exception", True)
         self.mode = kwargs.get("mode", None) or self._get_mode()
 
     def build(
         self,
         method,
         url,
-        data = None,
-        data_j = None,
-        data_m = None,
-        headers = None,
-        params = None,
-        mime = None,
-        kwargs = None
+        data=None,
+        data_j=None,
+        data_m=None,
+        headers=None,
+        params=None,
+        mime=None,
+        kwargs=None,
     ):
         auth = kwargs.pop("auth", True)
         token = kwargs.pop("token", False)
-        if auth: kwargs["session_id"] = self.get_session_id()
-        if token: kwargs["access_token"] = self.get_access_token()
+        if auth:
+            kwargs["session_id"] = self.get_session_id()
+        if token:
+            kwargs["access_token"] = self.get_access_token()
 
     def handle_error(self, error):
         if not error.code in appier.http.AUTH_ERRORS:
             self._wrap_error(error)
         if self.is_direct():
             self._wrap_error(error)
         elif self.is_oauth():
             raise appier.OAuthAccessError(
-                message = "Problems using access token found must re-authorize"
+                message="Problems using access token found must re-authorize"
             )
         raise
 
     def get_session_id(self):
-        if self.session_id: return self.session_id
-        if self.is_direct(): return self.login()
-        elif self.is_oauth(): return self.oauth_session()
+        if self.session_id:
+            return self.session_id
+        if self.is_direct():
+            return self.login()
+        elif self.is_oauth():
+            return self.oauth_session()
 
     def get_access_token(self):
-        if self.access_token: return self.access_token
-        if self.is_direct(): return None
-        raise appier.OAuthAccessError(
-            message = "No access token found must re-authorize"
-        )
+        if self.access_token:
+            return self.access_token
+        if self.is_direct():
+            return None
+        raise appier.OAuthAccessError(message="No access token found must re-authorize")
 
     def auth_callback(self, params, headers):
-        if not self._has_mode(): raise appier.APIAccessError(
-            message = "Session expired or authentication issues"
-        )
+        if not self._has_mode():
+            raise appier.APIAccessError(
+                message="Session expired or authentication issues"
+            )
         self.session_id = None
         session_id = self.get_session_id()
         params["session_id"] = session_id
 
-    def login(self, username = None, password = None):
+    def login(self, username=None, password=None):
         username = username or self.username
         password = password or self.password
         url = self.base_url + "omni/login.json"
         contents = self.get(
             url,
-            callback = False,
-            auth = False,
-            token = False,
-            username = username,
-            password = password
+            callback=False,
+            auth=False,
+            token=False,
+            username=username,
+            password=password,
         )
         self.username = contents.get("username", None)
         self.object_id = contents.get("object_id", None)
         self.acl = contents.get("acl", None)
         self.session_id = contents.get("session_id", None)
         self.tokens = self.acl.keys()
         self.trigger("auth", contents)
         return self.session_id
 
-    def oauth_authorize(self, state = None):
+    def oauth_authorize(self, state=None):
         url = self.base_url + self.prefix + "oauth/authorize"
         values = dict(
-            client_id = self.client_id,
-            redirect_uri = self.redirect_url,
-            response_type = "code",
-            scope = " ".join(self.scope)
+            client_id=self.client_id,
+            redirect_uri=self.redirect_url,
+            response_type="code",
+            scope=" ".join(self.scope),
         )
-        if state: values["state"] = state
+        if state:
+            values["state"] = state
         data = appier.legacy.urlencode(values)
         url = url + "?" + data
         return url
 
     def oauth_access(self, code):
         url = self.base_url + "omni/oauth/access_token"
         contents = self.post(
             url,
-            auth = False,
-            token = False,
-            client_id = self.client_id,
-            client_secret = self.client_secret,
-            grant_type = "authorization_code",
-            redirect_uri = self.redirect_url,
-            code = code
+            auth=False,
+            token=False,
+            client_id=self.client_id,
+            client_secret=self.client_secret,
+            grant_type="authorization_code",
+            redirect_uri=self.redirect_url,
+            code=code,
         )
         self.access_token = contents["access_token"]
         self.trigger("access_token", self.access_token)
         return self.access_token
 
     def oauth_session(self):
         url = self.base_url + "omni/oauth/start_session"
-        contents = self.get(url, callback = False, auth = False, token = True)
+        contents = self.get(url, callback=False, auth=False, token=True)
         self.username = contents.get("username", None)
         self.object_id = contents.get("object_id", None)
         self.acl = contents.get("acl", None)
         self.session_id = contents.get("session_id", None)
         self.tokens = self.acl.keys()
         self.trigger("auth", contents)
         return self.session_id
 
     def ping(self):
         return self.self_user()
 
     def _wrap_error(self, error):
-        if not self.wrap_exception: raise
-        if not hasattr(error, "read_json"): raise
+        if not self.wrap_exception:
+            raise
+        if not hasattr(error, "read_json"):
+            raise
         data = error.read_json()
-        if not data: raise
-        if not isinstance(data, dict): raise
+        if not data:
+            raise
+        if not isinstance(data, dict):
+            raise
         exception = data.get("exception", {})
         error = errors.OmniError(error, exception)
         raise error
 
     def _has_mode(self):
         return self.is_direct() or self.is_oauth()
 
     def _get_mode(self):
-        if self.username and self.password: return appier.OAuthAPI.DIRECT_MODE
-        elif self.client_id and self.client_secret: return appier.OAuthAPI.OAUTH_MODE
+        if self.username and self.password:
+            return appier.OAuthAPI.DIRECT_MODE
+        elif self.client_id and self.client_secret:
+            return appier.OAuthAPI.OAUTH_MODE
         return appier.OAuthAPI.UNSET_MODE
```

### Comparing `omni-api-0.5.0/src/omni/customer.py` & `omni-api-0.5.1/src/omni/supplier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,53 +18,34 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class CustomerAPI(object):
 
-    def list_customers(self, *args, **kwargs):
+class SupplierAPI(object):
+
+    def list_suppliers(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/customers.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/suppliers.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def list_persons(self, *args, **kwargs):
+    def list_companies(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/customer_persons.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/supplier_companies.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_person(self, object_id):
-        url = self.base_url + "omni/customer_persons/%d.json" % object_id
+    def get_company(self, object_id):
+        url = self.base_url + "omni/supplier_companies/%d.json" % object_id
         contents = self.get(url)
         return contents
-
-    def update_person(self, object_id, payload):
-        url = self.base_url + "omni/customer_persons/%d/update.json" % object_id
-        contents = self.post(url, data_j = payload)
-        return contents
```

### Comparing `omni-api-0.5.0/src/omni/receipt.py` & `omni-api-0.5.1/src/omni/invoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,36 +18,28 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class ReceiptAPI(object):
+
+class InvoiceAPI(object):
 
     @classmethod
-    def normalize_receipt(cls, receipt):
-        payload = receipt.get("payload", {})
+    def normalize_invoice(cls, invoice):
+        payload = invoice.get("payload", {})
         operation = payload.get("operation", {})
 
         type = operation.get("type", 1)
 
         if type == 1:
             operation["subtotal"] = operation["price_vat"] + operation["discount_vat"]
         elif type == 2:
@@ -56,15 +48,17 @@
         operation["vat_s"] = util.format_places(operation["vat"], 2)
         operation["subtotal_s"] = util.format_places(operation["subtotal"], 2)
 
         if "discount" in operation and not operation["discount"] == None:
             operation["discount_s"] = util.format_places(operation["discount"], 2)
 
         if "discount_vat" in operation and not operation["discount_vat"] == None:
-            operation["discount_vat_s"] = util.format_places(operation["discount_vat"], 2)
+            operation["discount_vat_s"] = util.format_places(
+                operation["discount_vat"], 2
+            )
 
         operation["price_vat_s"] = util.format_places(operation["price_vat"], 2)
 
         for item in operation["vat_list"]:
             item["vat_rate_s"] = util.format_places(item["vat_rate"], 2)
             item["vat_s"] = util.format_places(item["vat"], 2)
 
@@ -75,32 +69,31 @@
             merchandise = line["merchandise"]
             line["vat_rate_s"] = util.format_places(line["vat_rate"], 2)
             line["quantity_s"] = util.format_places(
                 line["quantity"],
                 merchandise.get("quantity_places", 0) or 0,
             )
             line["unit_discount_s"] = util.format_places(line["unit_discount"], 2)
-            line["unit_discount_vat_s"] = util.format_places(line["unit_discount_vat"], 2)
+            line["unit_discount_vat_s"] = util.format_places(
+                line["unit_discount_vat"], 2
+            )
             line["unit_price_s"] = util.format_places(line["unit_price"]["value"], 2)
             line["unit_price_vat_s"] = util.format_places(line["unit_price_vat"], 2)
             line["price_s"] = util.format_places(line["price"], 2)
             line["price_vat_s"] = util.format_places(line["price_vat"], 2)
             line["weight_s"] = util.format_places(
                 (merchandise["weight"] or 0.0) * line["quantity"], 3
             )
 
         if "sale_lines" in operation:
             operation["lines"] = operation["sale_lines"]
 
-    def list_receipts(self, *args, **kwargs):
+    def list_invoices(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/receipts.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/invoices.json"
+        contents = self.get(url, **kwargs)
         return contents
 
-    def get_receipt(self, object_id):
-        url = self.base_url + "omni/receipts/%d.json" % object_id
+    def get_invoice(self, object_id):
+        url = self.base_url + "omni/invoices/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/identifiable.py` & `omni-api-0.5.1/src/omni/models/merchandise.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,34 +18,19 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import util
+from . import base
+
 
-class IdentifiableAPI(object):
+class Merchandise(base.Base):
 
-    def list_identifiables(self, *args, **kwargs):
-        util.filter_args(kwargs)
-        url = self.base_url + "omni/identifiables.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
-        return contents
+    company_product_code = dict()
```

### Comparing `omni-api-0.5.0/src/omni/__init__.py` & `omni-api-0.5.1/src/omni/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,24 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import models
 from . import base
@@ -50,14 +41,15 @@
 from . import invoice
 from . import media
 from . import merchandise
 from . import money_sale_slip
 from . import product
 from . import receipt
 from . import return_
+from . import saft_pt
 from . import sale_order
 from . import sale_snapshot
 from . import sale
 from . import signed_document
 from . import status
 from . import stock_adjustment
 from . import store
@@ -84,14 +76,15 @@
 from .invoice import InvoiceAPI
 from .media import MediaAPI
 from .merchandise import MerchandiseAPI
 from .money_sale_slip import MoneySaleSlipAPI
 from .product import ProductAPI
 from .receipt import ReceiptAPI
 from .return_ import ReturnAPI
+from .saft_pt import SaftPtAPI, SaftPtReport, SaftPtReportPayload
 from .sale_order import SaleOrderAPI
 from .sale_snapshot import SaleSnapshotAPI
 from .sale import SaleAPI
 from .signed_document import SignedDocumentAPI
 from .status import StatusAPI
 from .stock_adjustment import StockAdjustmentAPI
 from .store import StoreAPI
```

### Comparing `omni-api-0.5.0/src/omni/money_sale_slip.py` & `omni-api-0.5.1/src/omni/transfer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,43 +18,33 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class MoneySaleSlipAPI(object):
 
-    @classmethod
-    def normalize_money_sale_slip(cls, money_sale_slip):
-        cls.normalize_invoice(money_sale_slip)
+class TransferAPI(object):
 
-    def list_money_sale_slips(self, *args, **kwargs):
+    def list_transfers(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/money_sale_slips.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/transfers.json"
+        contents = self.get(url, **kwargs)
+        return contents
+
+    def create_transfer(self, payload):
+        url = self.base_url + "omni/transfers.json"
+        contents = self.post(url, data_j=payload)
         return contents
 
-    def get_money_sale_slip(self, object_id):
-        url = self.base_url + "omni/money_sale_slips/%d.json" % object_id
+    def get_transfer(self, object_id):
+        url = self.base_url + "omni/transfers/%d.json" % object_id
         contents = self.get(url)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/employee.py` & `omni-api-0.5.1/src/omni/employee.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,67 +18,56 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
+
 class EmployeeAPI(object):
 
     def list_employees(self, *args, **kwargs):
         util.filter_args(kwargs)
         url = self.base_url + "omni/employees.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        contents = self.get(url, **kwargs)
         return contents
 
     def get_employee(self, object_id):
         url = self.base_url + "omni/employees/%d.json" % object_id
         contents = self.get(url)
         return contents
 
     def self_employee(self):
         url = self.base_url + "omni/employees/self.json"
         contents = self.get(url)
         return contents
 
     def stats_employee(
         self,
-        date = None,
-        unit = "month",
-        span = 7,
-        store_id = None,
-        employee_id = None,
-        has_global = None,
-        output = "simple"
+        date=None,
+        unit="month",
+        span=7,
+        store_id=None,
+        employee_id=None,
+        has_global=None,
+        output="simple",
     ):
         url = self.base_url + "omni/employee_snapshots/stats.json"
         contents = self.get(
             url,
-            date = date,
-            unit = unit,
-            span = span,
-            store_id = store_id,
-            employee_id = employee_id,
-            has_global = has_global,
-            output = output
+            date=date,
+            unit=unit,
+            span=span,
+            store_id=store_id,
+            employee_id=employee_id,
+            has_global=has_global,
+            output=output,
         )
         return contents
```

### Comparing `omni-api-0.5.0/src/omni/export.py` & `omni-api-0.5.1/src/omni/export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,24 +18,15 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import csv
 import datetime
@@ -44,92 +35,90 @@
 
 STEP = 256
 """ The default step value to be used in the iteration
 around the values retrieved from the server side, a large
 value on this field may create some memory problems in the
 server and a large latency """
 
-def to_string(value, encoding = None):
+
+def to_string(value, encoding=None):
     if encoding and appier.legacy.is_unicode(value):
         value = value.encode(encoding, "ignore")
     return value
 
-def to_date(value, encoding = None):
-    try: value_d = datetime.datetime.utcfromtimestamp(value)
-    except Exception: return ""
+
+def to_date(value, encoding=None):
+    try:
+        value_d = datetime.datetime.utcfromtimestamp(value)
+    except Exception:
+        return ""
     return value_d.strftime("%Y-%m-%d")
 
-FUNCS = dict(
-    string = to_string,
-    date = to_date
-)
 
-def get_field(object, name, encoding = "latin-1", type_m = dict()):
-    if appier.legacy.PYTHON_3: encoding = None
+FUNCS = dict(string=to_string, date=to_date)
+
+
+def get_field(object, name, encoding="latin-1", type_m=dict()):
+    if appier.legacy.PYTHON_3:
+        encoding = None
     name_l = name.split(".")
 
     for key in name_l:
-        if not object: break
+        if not object:
+            break
         object = object[key]
 
     _type = type_m.get(name, "string")
     func = FUNCS.get(_type, None)
-    object = func(object, encoding = encoding) if func and not object == None else object
+    object = func(object, encoding=encoding) if func and not object == None else object
 
     return object
 
+
 def open_export(path):
-    if appier.legacy.PYTHON_3: return open(
-        path,
-        "w",
-        newline = "",
-        encoding = "latin-1",
-        errors = "ignore"
-    )
-    else: return open(path, "wb")
-
-def export(
-    file,
-    caller,
-    attributes,
-    names = None,
-    type_m = None,
-    step = STEP,
-    callback = None
-):
+    if appier.legacy.PYTHON_3:
+        return open(path, "w", newline="", encoding="latin-1", errors="ignore")
+    else:
+        return open(path, "wb")
+
+
+def export(file, caller, attributes, names=None, type_m=None, step=STEP, callback=None):
     names = names or attributes
     type_m = type_m or dict()
 
-    csv_f = csv.writer(file, delimiter = ";")
+    csv_f = csv.writer(file, delimiter=";")
     csv_f.writerow(names)
 
     index = 0
 
     while True:
         # runs a tick operation in the caller adjusting both the
         # skip and the limit values according to the current iteration
         # in case there are no object retrieves that indicates the
         # end of the loop and a break happens
-        object = dict(skip = index, limit = step)
-        objects = caller(object = object)
-        if not objects: break
+        object = dict(skip=index, limit=step)
+        objects = caller(object=object)
+        if not objects:
+            break
 
         # iterates over all the objects that have been retrieved
         # and obtains the target fields to write a new CSV row
         # per each of the retrieved object and according to the
         # requested set of attributes per object
         for object in objects:
-            values = [get_field(object, key, type_m = type_m) for key in attributes]
+            values = [get_field(object, key, type_m=type_m) for key in attributes]
             csv_f.writerow(values)
 
         # in case there's a valid callback function to be called
         # runs the call with the current index and objects
-        if callback: callback(index, objects)
+        if callback:
+            callback(index, objects)
 
         # increments the current base index by the length of the
         # received objects, this should be the next index
         index += len(objects)
 
         # verifies if the current retrieval is considered valid
         # meets expectations and if not breaks the current loop
         is_valid = len(objects) == step
-        if not is_valid: break
+        if not is_valid:
+            break
```

### Comparing `omni-api-0.5.0/src/omni/inventory_line.py` & `omni-api-0.5.1/src/omni/customer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Omni ERP
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Omni ERP.
 #
 # Hive Omni ERP is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,34 +18,39 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omni ERP. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import util
 
-class InventoryLineAPI(object):
 
-    def list_inventory_lines(self, *args, **kwargs):
+class CustomerAPI(object):
+
+    def list_customers(self, *args, **kwargs):
         util.filter_args(kwargs)
-        url = self.base_url + "omni/inventory_lines.json"
-        contents = self.get(
-            url,
-            **kwargs
-        )
+        url = self.base_url + "omni/customers.json"
+        contents = self.get(url, **kwargs)
+        return contents
+
+    def list_persons(self, *args, **kwargs):
+        util.filter_args(kwargs)
+        url = self.base_url + "omni/customer_persons.json"
+        contents = self.get(url, **kwargs)
+        return contents
+
+    def get_person(self, object_id):
+        url = self.base_url + "omni/customer_persons/%d.json" % object_id
+        contents = self.get(url)
+        return contents
+
+    def update_person(self, object_id, payload):
+        url = self.base_url + "omni/customer_persons/%d/update.json" % object_id
+        contents = self.post(url, data_j=payload)
         return contents
```

### Comparing `omni-api-0.5.0/src/omni_api.egg-info/PKG-INFO` & `omni-api-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Omni API Client
 Home-page: http://omni-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni API](http://omni-api.hive.pt)
```

### Comparing `omni-api-0.5.0/src/omni_api.egg-info/SOURCES.txt` & `omni-api-0.5.1/src/omni_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/omni/invoice.py
 src/omni/media.py
 src/omni/merchandise.py
 src/omni/money_sale_slip.py
 src/omni/product.py
 src/omni/receipt.py
 src/omni/return_.py
+src/omni/saft_pt.py
 src/omni/sale.py
 src/omni/sale_order.py
 src/omni/sale_snapshot.py
 src/omni/signed_document.py
 src/omni/status.py
 src/omni/stock_adjustment.py
 src/omni/store.py
```

### Comparing `omni-api-0.5.0/README.md` & `omni-api-0.5.1/README.md`

 * *Files identical despite different names*

