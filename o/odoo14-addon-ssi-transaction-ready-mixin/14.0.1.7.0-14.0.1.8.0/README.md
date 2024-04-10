# Comparing `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54694 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/__init__.py
--rw-r--r--  2.0 unx      543 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
--rw-r--r--  2.0 unx     7310 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
--rw-r--r--  2.0 unx      804 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
--rw-r--r--  2.0 unx     1846 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD
-11 files, 61870 bytes uncompressed, 52394 bytes compressed:  15.3%
+Zip file size: 54696 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/__init__.py
+-rw-r--r--  2.0 unx      543 b- defN 24-Apr-10 00:00 odoo/addons/ssi_transaction_ready_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      198 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7310 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx      804 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
+-rw-r--r--  2.0 unx     1846 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-10 00:01 odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD
+11 files, 61870 bytes uncompressed, 52396 bytes compressed:  15.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_ready_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Ready to Process State",
-    "version": "14.0.1.7.0",
+    "version": "14.0.1.8.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
     ],
```

## odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py

```diff
@@ -104,15 +104,15 @@
             record._run_pre_ready_action()
             record.write(record._prepare_ready_data())
             record._run_post_ready_check()
             record._run_post_ready_action()
 
     def _check_ready_policy(self):
         self.ensure_one()
-        if self.env.context.get("bypass_ready_policy", False):
+        if self.env.context.get("bypass_policy_check", False):
             return True
 
         if not self.ready_ok:
             error_message = """
             Context: Stage %s
             Database ID: %s
             Problem: Document is not allowed to stage
```

## Comparing `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-ready-mixin
-Version: 14.0.1.7.0
+Version: 14.0.1.8.0
 Summary: Transaction Mixin - Ready to Process State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_ready_mixin/README.rst,sha256=Q5zmi0IIuueW7CbBTomlXKXWbnM66bVGAqh-Lg6Ma1s,1272
 odoo/addons/ssi_transaction_ready_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_ready_mixin/__manifest__.py,sha256=0nUgRu5qo_catDf6BiMSwSbG2r8_sqd6NrGpxqWNoAQ,543
+odoo/addons/ssi_transaction_ready_mixin/__manifest__.py,sha256=Hro8quKGZBsnX9_O-E-hGEtN3M-8YHIpl-EQfGT3xdw,543
 odoo/addons/ssi_transaction_ready_mixin/models/__init__.py,sha256=lOfO70jrUznLOmoFqDgf3m1pEV4Qij3s_sNFeGQulLA,198
-odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py,sha256=k1DocbpZWUF_DgYmF-BeefM7I3I6mXoEoOXM4V3RibU,7310
+odoo/addons/ssi_transaction_ready_mixin/models/mixin_transaction_ready.py,sha256=YslNAxxxomqRgqIpUreuj8uKNXdaEjw03MXQNJAZDxk,7310
 odoo/addons/ssi_transaction_ready_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
 odoo/addons/ssi_transaction_ready_mixin/templates/mixin_transaction_ready_templates.xml,sha256=Ojf_LdJpD45bIRgd4bUf7J55hNNbtrCWGYrF8aEnyGY,804
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/METADATA,sha256=UyC2O2FS56PEFgBk4Y8mDGK6bfj_uXEwY3LlKz3S2Io,1846
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_ready_mixin-14.0.1.7.0.dist-info/RECORD,,
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/METADATA,sha256=f4D80kmYx2SjCpI74qtI6kWuCdGyYjne2AT8JBgyzIw,1846
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_ready_mixin-14.0.1.8.0.dist-info/RECORD,,
```

