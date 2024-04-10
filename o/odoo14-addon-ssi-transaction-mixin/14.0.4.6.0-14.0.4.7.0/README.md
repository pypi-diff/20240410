# Comparing `tmp/odoo14_addon_ssi_transaction_mixin-14.0.4.6.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_mixin-14.0.4.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 57170 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1216 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/__init__.py
--rw-r--r--  2.0 unx      617 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_mixin/__manifest__.py
--rw-r--r--  2.0 unx      341 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/menu.xml
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/models/__init__.py
--rw-r--r--  2.0 unx    12605 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/models/mixin_transaction.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     7474 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml
--rw-r--r--  2.0 unx     1887 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1300 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/RECORD
-12 files, 74243 bytes uncompressed, 54882 bytes compressed:  26.1%
+Zip file size: 57184 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1216 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/__init__.py
+-rw-r--r--  2.0 unx      617 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      341 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/menu.xml
+-rw-r--r--  2.0 unx      192 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/models/__init__.py
+-rw-r--r--  2.0 unx    12607 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/models/mixin_transaction.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     7494 b- defN 24-Apr-09 02:44 odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml
+-rw-r--r--  2.0 unx     1887 b- defN 24-Apr-09 02:44 odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 02:44 odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-09 02:44 odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1300 b- defN 24-Apr-09 02:44 odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/RECORD
+12 files, 74265 bytes uncompressed, 54896 bytes compressed:  26.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: odoo/addons/ssi_transaction_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin",
-    "version": "14.0.4.6.0",
+    "version": "14.0.4.7.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "mail",
         "ssi_policy_mixin",
```

## odoo/addons/ssi_transaction_mixin/models/mixin_transaction.py

```diff
@@ -100,15 +100,15 @@
     )
     manual_number_ok = fields.Boolean(
         string="Can Input Manual Document Number",
         compute="_compute_policy",
         compute_sudo=True,
     )
     display_name = fields.Char(
-        string="# Document", compute="_compute_display_name", store=True, index=True
+        string="Display Name", compute="_compute_display_name", store=True, index=True
     )
 
     @api.depends(lambda self: [self._document_number_field])
     def _compute_display_name(self):
         names = dict(self.name_get())
         for rec in self:
             rec.display_name = names.get(rec.id)
```

## odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml

### odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml

```diff
@@ -38,15 +38,15 @@
     <field name="arch" type="xml">
       <tree decoration-bf="message_unread==True">
         <header>
           <button name="action_restart" type="object" string="Restart" confirm="Restart data. Are you sure?"/>
         </header>
         <field name="message_unread" invisible="1"/>
         <field name="id" optional="hide"/>
-        <field name="display_name"/>
+        <field name="display_name" string="# Document"/>
         <field name="company_id" groups="base.group_multi_company" optional="hide"/>
         <field name="user_id" optional="show" widget="many2one_avatar"/>
         <field name="activity_ids" widget="list_activity" optional="show"/>
         <field name="state" widget="badge" decoration-info="state == 'draft'"/>
       </tree>
     </field>
   </record>
```

## Comparing `odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-mixin
-Version: 14.0.4.6.0
+Version: 14.0.4.7.0
 Summary: Transaction Mixin
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 odoo/addons/ssi_transaction_mixin/README.rst,sha256=dlTwm2a66EGatr4WmLUEqK-hwneNoxhoENilO278tik,1216
 odoo/addons/ssi_transaction_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_mixin/__manifest__.py,sha256=gAT96L9Yjqgw1Kv8AjM167iHexjiMYfLvyVXJSObTGQ,617
+odoo/addons/ssi_transaction_mixin/__manifest__.py,sha256=EiajVamsNJ1g35ySCkAlFkvJQXLfA_HMKS0Cgf8QE8Q,617
 odoo/addons/ssi_transaction_mixin/menu.xml,sha256=vJc-x2cLR4LYWh0jAgFPLUVuIRGIzgDHy0LNiAZP5dk,341
 odoo/addons/ssi_transaction_mixin/models/__init__.py,sha256=FUu5JrrfMjy2GyiS-GJHAcImvmU9bru2e4DBCTwj2XY,192
-odoo/addons/ssi_transaction_mixin/models/mixin_transaction.py,sha256=n2crAVdmT_W6eilpfFn3Md8r1ufa5FzbDS4ttSvvFE0,12605
+odoo/addons/ssi_transaction_mixin/models/mixin_transaction.py,sha256=x1W8fnOOh519xkYJZBH-6NUaRItGQc6gMKm6NGslTMU,12607
 odoo/addons/ssi_transaction_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml,sha256=7Ny6rfWyHvLHndDUEqomxQszYdijYv9qxN-rtoz_3MM,7474
-odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/METADATA,sha256=8nHwr6V2aSp9JgYPACqMS0qqy3y8Y94NenLoc_F9SWU,1887
-odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_mixin-14.0.4.6.0.dist-info/RECORD,,
+odoo/addons/ssi_transaction_mixin/views/mixin_transaction_views.xml,sha256=GGpEv3Q7qDULxLOEFafK1w0JaY4r5l_EAEBoTdYO0dE,7494
+odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/METADATA,sha256=CcUAkVGQjpXf00TnDh8XREU--Y4_lA6GiHuFOKRw3sA,1887
+odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_mixin-14.0.4.7.0.dist-info/RECORD,,
```

