# Comparing `tmp/odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 55135 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1288 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/__init__.py
--rw-r--r--  2.0 unx      588 b- defN 24-Apr-08 04:44 odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py
--rw-r--r--  2.0 unx      200 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py
--rw-r--r--  2.0 unx    10895 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     2242 b- defN 24-Apr-08 04:43 odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
--rw-r--r--  2.0 unx     1924 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1314 b- defN 24-Apr-08 04:44 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/RECORD
-11 files, 67062 bytes uncompressed, 52783 bytes compressed:  21.3%
+Zip file size: 55230 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1288 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/__init__.py
+-rw-r--r--  2.0 unx      588 b- defN 24-Apr-10 00:00 odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      200 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py
+-rw-r--r--  2.0 unx    11842 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     2839 b- defN 24-Apr-09 23:59 odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
+-rw-r--r--  2.0 unx     1924 b- defN 24-Apr-10 00:00 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 00:00 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-10 00:00 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1314 b- defN 24-Apr-10 00:00 odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/RECORD
+11 files, 68606 bytes uncompressed, 52878 bytes compressed:  22.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Transaction Mixin - Waiting for Approval State",
-    "version": "14.0.2.6.0",
+    "version": "14.0.2.7.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_transaction_mixin",
         "ssi_multiple_approval_mixin",
```

## odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py

```diff
@@ -22,14 +22,15 @@
     _confirm_state = "confirm"
 
     # Attributes related to automatic form view
     _automatically_insert_confirm_policy_fields = True
     _automatically_insert_confirm_button = True
     _automatically_insert_approve_button = True
     _automatically_insert_reject_button = True
+    _automatically_insert_restart_approval_button = True
 
     # Attributes related to add element on search view automatically
     _automatically_insert_confirm_filter = True
     _automatically_insert_reject_filter = True
 
     # Attributes related to add element on tree view automatically
     _automatically_insert_confirm_state_badge_decorator = True
@@ -118,15 +119,15 @@
             record.write(record._prepare_confirm_data())
             record._run_post_confirm_check()
             record._run_post_confirm_action()
             record.action_request_approval()
 
     def _check_confirm_policy(self):
         self.ensure_one()
-        if self.env.context.get("bypass_confirm_policy", False):
+        if self.env.context.get("bypass_policy_check", False):
             return True
 
         if not self.confirm_ok:
             error_message = """
                 Context: Confirm %s
                 Database ID: %s
                 Problem: Document is not allowed to confirm
@@ -154,14 +155,15 @@
 
         view_arch = etree.XML(result["arch"])
         if view_type == "form" and self._automatically_insert_view_element:
             view_arch = self._view_add_policy_field(view_arch)
             view_arch = self._view_add_confirm_button(view_arch)
             view_arch = self._view_add_approve_button(view_arch)
             view_arch = self._view_add_reject_button(view_arch)
+            view_arch = self._view_add_restart_approval_button(view_arch)
             view_arch = self._reorder_header_button(view_arch)
             view_arch = self._reorder_policy_field(view_arch)
         elif view_type == "tree" and self._automatically_insert_view_element:
             view_arch = self._add_confirm_state_badge_decorator(view_arch)
             view_arch = self._add_reject_state_badge_decorator(view_arch)
         elif view_type == "search" and self._automatically_insert_view_element:
             view_arch = self._add_confirm_filter_on_search_view(view_arch)
@@ -256,14 +258,25 @@
                 "ssi_transaction_confirm_mixin.button_approve",
                 "/form/header/field[@name='state']",
                 "before",
             )
         return view_arch
 
     @api.model
+    def _view_add_restart_approval_button(self, view_arch):
+        if self._automatically_insert_restart_approval_button:
+            view_arch = self._add_view_element(
+                view_arch,
+                "ssi_transaction_confirm_mixin.button_restart_approval",
+                "/form/header/field[@name='state']",
+                "before",
+            )
+        return view_arch
+
+    @api.model
     def _view_add_reject_button(self, view_arch):
         if self._automatically_insert_reject_button:
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_confirm_mixin.button_reject",
                 "/form/header/field[@name='state']",
                 "before",
@@ -278,27 +291,38 @@
                 "ssi_transaction_confirm_mixin.tree_button_confirm",
                 "/tree/header",
                 "inside",
             )
         return view_arch
 
     @ssi_decorator.insert_on_tree_view()
-    def _02_view_add_tree_approve_button(self, view_arch):
+    def _03_view_add_tree_approve_button(self, view_arch):
         if self._automatically_insert_approve_button:
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_confirm_mixin.tree_button_approve",
                 "/tree/header",
                 "inside",
             )
         return view_arch
 
     @ssi_decorator.insert_on_tree_view()
-    def _01_view_add_tree_reject_button(self, view_arch):
+    def _02_view_add_tree_reject_button(self, view_arch):
         if self._automatically_insert_reject_button:
             view_arch = self._add_view_element(
                 view_arch,
                 "ssi_transaction_confirm_mixin.tree_button_reject",
                 "/tree/header",
                 "inside",
             )
         return view_arch
+
+    @ssi_decorator.insert_on_tree_view()
+    def _01_view_add_tree_reject_button(self, view_arch):
+        if self._automatically_insert_restart_approval_button:
+            view_arch = self._add_view_element(
+                view_arch,
+                "ssi_transaction_confirm_mixin.tree_button_restart_approval",
+                "/tree/header",
+                "inside",
+            )
+        return view_arch
```

## odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml

### odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml

```diff
@@ -23,17 +23,23 @@
   </template>
   <template id="button_approve">
     <button name="action_approve_approval" string="Approve" type="object" class="oe_highlight" confirm="Approve data. Are you sure?" attrs="{'invisible':[('approve_ok','!=',True)]}"/>
   </template>
   <template id="button_reject">
     <button name="action_reject_approval" string="Reject" type="object" confirm="Reject data. Are you sure?" attrs="{'invisible':[('reject_ok','!=',True)]}"/>
   </template>
+  <template id="button_restart_approval">
+    <button name="action_reload_approval_template" string="Restart Approval Process" type="object" confirm="Restart approval process. Are you sure?" attrs="{'invisible':[('restart_approval_ok','!=',True)]}"/>
+  </template>
   <template id="tree_button_confirm">
     <button name="action_confirm" string="Confirm" type="object" confirm="Confirm data. Are you sure?"/>
   </template>
   <template id="tree_button_approve">
     <button name="action_approve_approval" string="Approve" type="object" confirm="Approve data. Are you sure?"/>
   </template>
   <template id="tree_button_reject">
     <button name="action_reject_approval" string="Reject" type="object" confirm="Reject data. Are you sure?"/>
   </template>
+  <template id="tree_button_restart_approval">
+    <button name="action_reload_approval_template" string="Restart Approval Process" type="object" confirm="Restart approval process. Are you sure?"/>
+  </template>
 </odoo>
```

## Comparing `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/METADATA` & `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-transaction-confirm-mixin
-Version: 14.0.2.6.0
+Version: 14.0.2.7.0
 Summary: Transaction Mixin - Waiting for Approval State
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/RECORD` & `odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_transaction_confirm_mixin/README.rst,sha256=LnAs5oFV6kOiX1rOHkZtPpEUaAQUJlcQk1BLL_Dgbg4,1288
 odoo/addons/ssi_transaction_confirm_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py,sha256=wdG8UKF3iQuwejdjoYpfgTzO5QDteS_A7qXdwq-8BLo,588
+odoo/addons/ssi_transaction_confirm_mixin/__manifest__.py,sha256=ahcn_swBqceMKUkglTmU5TLiF1cZLNpGyfypSGJumnQ,588
 odoo/addons/ssi_transaction_confirm_mixin/models/__init__.py,sha256=kJTOEh8MVP031XPCjCUhq32C99VJfwAreZ3lnX7HFxQ,200
-odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py,sha256=bcBlhaLHw60eIM9bsBoBLpC2xd9VRDn_0s1J4W5_x8k,10895
+odoo/addons/ssi_transaction_confirm_mixin/models/mixin_transaction_confirm.py,sha256=UiaO7v37l07MpGhu0F_ybsri8y9pPJjJmYyIBlOkFqE,11842
 odoo/addons/ssi_transaction_confirm_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml,sha256=So7MKK57tqBrqP0YcxDsWD_g6W4BIxoKW_D11IGtL2c,2242
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/METADATA,sha256=OSbdCGKA7JqwlxFcM62hGN4tM6d3u-cZsUxx_biHT9c,1924
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.6.0.dist-info/RECORD,,
+odoo/addons/ssi_transaction_confirm_mixin/templates/mixin_transaction_confirm_templates.xml,sha256=gOWK1MYp7R7bQv2WUTXzsug81vEDhMFi80lSgJaMMnM,2839
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/METADATA,sha256=b2_hU7uD6lUUq_xyzBSgxWIdgsT3in9_dai14K4AiI0,1924
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_transaction_confirm_mixin-14.0.2.7.0.dist-info/RECORD,,
```

