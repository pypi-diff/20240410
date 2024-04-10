# Comparing `tmp/pyWeclapp-0.0.3.tar.gz` & `tmp/pyWeclapp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyWeclapp-0.0.3.tar", last modified: Fri Feb  9 16:12:05 2024, max compression
+gzip compressed data, was "pyWeclapp-0.0.4.tar", last modified: Wed Apr 10 15:30:26 2024, max compression
```

## Comparing `pyWeclapp-0.0.3.tar` & `pyWeclapp-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.746086 pyWeclapp-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:12:05.746086 pyWeclapp-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.734086 pyWeclapp-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.738086 pyWeclapp-0.0.3/src/pyWeclapp/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.738086 pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/kitty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.738086 pyWeclapp-0.0.3/src/pyWeclapp/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/examples/article_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/examples/contract_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/examples/salesOrder_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/examples/shipment_Model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.738086 pyWeclapp-0.0.3/src/pyWeclapp/timeFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/timeFunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/timeFunctions/localizedTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.738086 pyWeclapp-0.0.3/src/pyWeclapp/weclapp/
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclapp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclapp/weclappError.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclapp/weclappResponseProcessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/article_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/contact_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/contract_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15996 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/customer_Model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/extraInfoForApp/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/extraInfoForApp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/party_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18462 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/quotation_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/salesInvoice_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/salesOrder_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/shipment_Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/ticket_Model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/
--rw-r--r--   0 runner    (1001) docker     (127)    29746 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCustomAttribute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/docDescription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-02-09 16:11:54.000000 pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:05.742086 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-09 16:12:05.000000 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-09 16:12:05.000000 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:12:05.000000 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-09 16:12:05.000000 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 16:12:05.000000 pyWeclapp-0.0.3/src/pyWeclapp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.012484 pyWeclapp-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:30:26.012484 pyWeclapp-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.000484 pyWeclapp-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.000484 pyWeclapp-0.0.4/src/pyWeclapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.004484 pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/kitty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.004484 pyWeclapp-0.0.4/src/pyWeclapp/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/examples/article_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/examples/contract_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/examples/salesOrder_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/examples/shipment_Model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.004484 pyWeclapp-0.0.4/src/pyWeclapp/timeFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/timeFunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/timeFunctions/localizedTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.004484 pyWeclapp-0.0.4/src/pyWeclapp/weclapp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclapp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclapp/weclappError.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclapp/weclappResponseProcessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/article_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/contact_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/contract_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15996 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/customer_Model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/extraInfoForApp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/extraInfoForApp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/incomingGoods_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/party_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/purchaseOrder_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18462 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/quotation_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/salesInvoice_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/salesOrder_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/shipment_Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/ticket_Model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/
+-rw-r--r--   0 runner    (1001) docker     (127)    29746 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCustomAttribute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/docDescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-10 15:30:11.000000 pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:30:26.008484 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-10 15:30:25.000000 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-10 15:30:25.000000 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:30:25.000000 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 15:30:25.000000 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 15:30:25.000000 pyWeclapp-0.0.4/src/pyWeclapp.egg-info/top_level.txt
```

### Comparing `pyWeclapp-0.0.3/LICENSE` & `pyWeclapp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/PKG-INFO` & `pyWeclapp-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyWeclapp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides methods, classes and classbuilders to integrate with the Weclapp API
 Home-page: https://github.com/AltruanGmbH/weclappFunctions
 Author: Altruan GmbH
 Author-email: jakob.goesswald@altruan.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyWeclapp-0.0.3/setup.py` & `pyWeclapp-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 "pydantic>=1.10.4",
                 "jsonschema>=4.17.3",
                 # "pymupdf>=1.21.1",
                 "pytz>=2022.7.1"]
 
 setup(
     name="pyWeclapp",
-    version="0.0.3",
+    version="0.0.4",
     description="Provides methods, classes and classbuilders to integrate with the Weclapp API",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AltruanGmbH/weclappFunctions",
     author="Altruan GmbH",
```

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/__init__.py` & `pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/config.py` & `pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/config.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/customAttributes/kitty.py` & `pyWeclapp-0.0.4/src/pyWeclapp/customAttributes/kitty.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/examples/article_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/examples/article_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/examples/contract_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/examples/contract_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/examples/salesOrder_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/examples/salesOrder_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/examples/shipment_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/examples/shipment_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/timeFunctions/localizedTime.py` & `pyWeclapp-0.0.4/src/pyWeclapp/timeFunctions/localizedTime.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/webhooks.py` & `pyWeclapp-0.0.4/src/pyWeclapp/webhooks.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclapp/__init__.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclapp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclapp/config.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclapp/config.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclapp/weclappError.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclapp/weclappError.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclapp/weclappResponseProcessing.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclapp/weclappResponseProcessing.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/article_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/article_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/contact_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/contact_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/contract_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/contract_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/customer_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/customer_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/extraInfoForApp/__init__.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/extraInfoForApp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/party_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/party_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/quotation_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/quotation_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/salesInvoice_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/salesInvoice_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/salesOrder_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/salesOrder_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/shipment_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/shipment_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/ticket_Model.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/ticket_Model.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/__init__.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/config.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/config.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCreator.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCreator.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCustomAttribute.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappClasses/weclappClassBlueprint/weclappClassCustomAttribute.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/__init__.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/docDescription.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/docDescription.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp/weclappDoc/document.py` & `pyWeclapp-0.0.4/src/pyWeclapp/weclappDoc/document.py`

 * *Files identical despite different names*

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp.egg-info/PKG-INFO` & `pyWeclapp-0.0.4/src/pyWeclapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyWeclapp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides methods, classes and classbuilders to integrate with the Weclapp API
 Home-page: https://github.com/AltruanGmbH/weclappFunctions
 Author: Altruan GmbH
 Author-email: jakob.goesswald@altruan.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyWeclapp-0.0.3/src/pyWeclapp.egg-info/SOURCES.txt` & `pyWeclapp-0.0.4/src/pyWeclapp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 src/pyWeclapp/weclapp/weclappError.py
 src/pyWeclapp/weclapp/weclappResponseProcessing.py
 src/pyWeclapp/weclappClasses/__init__.py
 src/pyWeclapp/weclappClasses/article_Model.py
 src/pyWeclapp/weclappClasses/contact_Model.py
 src/pyWeclapp/weclappClasses/contract_Model.py
 src/pyWeclapp/weclappClasses/customer_Model.py
+src/pyWeclapp/weclappClasses/incomingGoods_Model.py
 src/pyWeclapp/weclappClasses/party_Model.py
+src/pyWeclapp/weclappClasses/purchaseOrder_Model.py
 src/pyWeclapp/weclappClasses/quotation_Model.py
 src/pyWeclapp/weclappClasses/salesInvoice_Model.py
 src/pyWeclapp/weclappClasses/salesOrder_Model.py
 src/pyWeclapp/weclappClasses/shipment_Model.py
 src/pyWeclapp/weclappClasses/ticket_Model.py
 src/pyWeclapp/weclappClasses/extraInfoForApp/__init__.py
 src/pyWeclapp/weclappClasses/weclappClassBlueprint/__init__.py
```

