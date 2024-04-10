# Comparing `tmp/pretix_fattura_elettronica-0.2.7.tar.gz` & `tmp/pretix_fattura_elettronica-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_fattura_elettronica-0.2.7.tar", last modified: Wed Mar 27 11:32:42 2024, max compression
+gzip compressed data, was "pretix_fattura_elettronica-0.2.8.tar", last modified: Wed Apr 10 14:33:28 2024, max compression
```

## Comparing `pretix_fattura_elettronica-0.2.7.tar` & `pretix_fattura_elettronica-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      576 2023-11-25 14:23:34.072549 pretix_fattura_elettronica-0.2.7/LICENSE
--rw-r--r--   0        0        0     1146 2023-11-30 16:55:25.351094 pretix_fattura_elettronica-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-11-30 21:33:20.634766 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/__init__.py
--rw-r--r--   0        0        0     2205 2023-11-30 22:27:26.840844 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/acubeapi.py
--rw-r--r--   0        0        0      813 2023-11-30 21:33:20.635133 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/apps.py
--rw-r--r--   0        0        0     1795 2023-11-30 21:33:20.616876 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/enums.py
--rw-r--r--   0        0        0     1887 2023-12-02 11:04:27.747492 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/forms.py
--rw-r--r--   0        0        0      334 2023-11-20 21:27:49.175625 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-11-20 21:27:49.175708 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      334 2023-11-20 21:27:49.175872 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1297 2023-11-30 21:33:20.618004 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-11-24 14:28:38.328431 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/migrations/__init__.py
--rw-r--r--   0        0        0      552 2023-11-30 21:33:20.618586 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/models.py
--rw-r--r--   0        0        0    16482 2024-03-27 11:27:58.417718 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/serializers.py
--rw-r--r--   0        0        0       61 2023-11-25 14:23:34.075229 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/signals/__init__.py
--rw-r--r--   0        0        0     1245 2023-12-02 12:14:10.851853 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/signals/forms.py
--rw-r--r--   0        0        0      638 2023-11-30 21:33:20.620108 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/signals/invoices.py
--rw-r--r--   0        0        0        0 2023-11-20 21:27:49.176106 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/static/pretix_fattura_elettronica/.gitkeep
--rw-r--r--   0        0        0        0 2023-11-20 21:27:49.176267 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/.gitkeep
--rw-r--r--   0        0        0     1676 2023-12-29 16:07:05.049234 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html
--rw-r--r--   0        0        0     3115 2023-12-30 11:23:41.500055 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html
--rw-r--r--   0        0        0     3806 2023-12-29 15:56:05.917674 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html
--rw-r--r--   0        0        0        0 2023-11-30 21:33:20.620556 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templatetags/__init__.py
--rw-r--r--   0        0        0      377 2023-11-30 21:33:20.620846 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templatetags/fatturaelt.py
--rw-r--r--   0        0        0     1215 2024-03-18 18:05:24.565729 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/urls.py
--rw-r--r--   0        0        0     3555 2023-12-30 15:48:33.493280 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/utils/__init__.py
--rw-r--r--   0        0        0      950 2024-03-27 11:14:01.431145 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/utils/tax.py
--rw-r--r--   0        0        0     8429 2024-03-27 10:06:00.942344 pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/views.py
--rw-r--r--   0        0        0     2382 2024-03-27 11:32:42.582987 pretix_fattura_elettronica-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-20 21:27:49.176698 pretix_fattura_elettronica-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     7847 2024-03-18 18:05:24.566974 pretix_fattura_elettronica-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-18 09:57:53.724318 pretix_fattura_elettronica-0.2.7/tests/serializers/__init__.py
--rw-r--r--   0        0        0    11192 2024-03-27 11:27:16.283426 pretix_fattura_elettronica-0.2.7/tests/serializers/test_private_order.py
--rw-r--r--   0        0        0     1800 2023-11-30 22:25:40.348379 pretix_fattura_elettronica-0.2.7/tests/test_acubeapi.py
--rw-r--r--   0        0        0    32394 2024-03-18 09:51:49.714355 pretix_fattura_elettronica-0.2.7/tests/test_serializers.py
--rw-r--r--   0        0        0      865 2023-11-30 21:33:20.624387 pretix_fattura_elettronica-0.2.7/tests/test_signals.py
--rw-r--r--   0        0        0     1752 2023-12-30 15:39:56.990658 pretix_fattura_elettronica-0.2.7/tests/test_validation.py
--rw-r--r--   0        0        0     3384 2024-03-18 18:05:24.567681 pretix_fattura_elettronica-0.2.7/tests/test_views.py
--rw-r--r--   0        0        0     3614 2023-11-30 21:33:20.625194 pretix_fattura_elettronica-0.2.7/tests/utils.py
--rw-r--r--   0        0        0     2335 1970-01-01 00:00:00.000000 pretix_fattura_elettronica-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      576 2024-04-08 11:41:35.013314 pretix_fattura_elettronica-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1146 2024-04-08 11:41:35.013687 pretix_fattura_elettronica-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.014674 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/__init__.py
+-rw-r--r--   0        0        0     2205 2024-04-08 11:41:35.015125 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/acubeapi.py
+-rw-r--r--   0        0        0      813 2024-04-08 11:41:35.015236 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/apps.py
+-rw-r--r--   0        0        0     1795 2024-04-08 11:41:35.015372 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/enums.py
+-rw-r--r--   0        0        0     1887 2024-04-08 11:41:35.015502 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/forms.py
+-rw-r--r--   0        0        0      334 2024-04-08 11:41:35.015828 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.015938 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      334 2024-04-08 11:41:35.016147 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1297 2024-04-08 11:41:35.016356 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.016402 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-08 11:41:35.016535 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/models.py
+-rw-r--r--   0        0        0    16374 2024-04-10 13:56:54.961562 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/serializers.py
+-rw-r--r--   0        0        0       61 2024-04-08 11:41:35.016904 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-08 11:41:35.017014 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/forms.py
+-rw-r--r--   0        0        0      638 2024-04-08 11:41:35.017125 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/invoices.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017309 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/static/pretix_fattura_elettronica/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017572 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/.gitkeep
+-rw-r--r--   0        0        0     1676 2024-04-08 11:41:35.017731 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html
+-rw-r--r--   0        0        0     3115 2024-04-08 11:41:35.017880 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html
+-rw-r--r--   0        0        0     3806 2024-04-08 11:41:35.018209 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.018344 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templatetags/__init__.py
+-rw-r--r--   0        0        0      377 2024-04-08 11:41:35.018520 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templatetags/fatturaelt.py
+-rw-r--r--   0        0        0     1215 2024-04-08 11:41:35.018658 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/urls.py
+-rw-r--r--   0        0        0     3555 2024-04-08 11:41:35.018914 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/__init__.py
+-rw-r--r--   0        0        0      950 2024-04-08 11:41:35.019062 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/tax.py
+-rw-r--r--   0        0        0     8429 2024-04-08 11:41:35.019273 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/views.py
+-rw-r--r--   0        0        0     2408 2024-04-10 14:33:28.576427 pretix_fattura_elettronica-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020103 pretix_fattura_elettronica-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     7847 2024-04-08 11:41:35.020401 pretix_fattura_elettronica-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020608 pretix_fattura_elettronica-0.2.8/tests/serializers/__init__.py
+-rw-r--r--   0        0        0    11282 2024-04-10 14:28:33.289351 pretix_fattura_elettronica-0.2.8/tests/serializers/test_private_order.py
+-rw-r--r--   0        0        0     1800 2024-04-08 11:41:35.020955 pretix_fattura_elettronica-0.2.8/tests/test_acubeapi.py
+-rw-r--r--   0        0        0    32411 2024-04-10 14:29:06.563216 pretix_fattura_elettronica-0.2.8/tests/test_serializers.py
+-rw-r--r--   0        0        0      865 2024-04-08 11:41:35.021298 pretix_fattura_elettronica-0.2.8/tests/test_signals.py
+-rw-r--r--   0        0        0     1752 2024-04-08 11:41:35.021442 pretix_fattura_elettronica-0.2.8/tests/test_validation.py
+-rw-r--r--   0        0        0     3384 2024-04-08 11:41:35.021557 pretix_fattura_elettronica-0.2.8/tests/test_views.py
+-rw-r--r--   0        0        0     3614 2024-04-08 11:41:35.021672 pretix_fattura_elettronica-0.2.8/tests/utils.py
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 pretix_fattura_elettronica-0.2.8/PKG-INFO
```

### Comparing `pretix_fattura_elettronica-0.2.7/LICENSE` & `pretix_fattura_elettronica-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/README.md` & `pretix_fattura_elettronica-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/acubeapi.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/acubeapi.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/apps.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/apps.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/enums.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/enums.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/forms.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/forms.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/migrations/0001_initial.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/models.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/models.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/serializers.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,18 +428,17 @@
 
     @property
     def codice_destinatario(self) -> str:
         invoice = self._invoice
 
         codice_destinatario = get_sdi(invoice.order)
 
-        # TODO: maybe validation needs to be in pydantic
         if self.is_italian_invoice:
             if self.is_business_invoice and not codice_destinatario:
-                raise ValueError("For a business invoice codice dest is required.")
+                return "0000000"
         else:
             return "XXXXXXX"
 
         return codice_destinatario or SETTINGS.CODICE_DESTINATARIO_DEFAULT
 
     @property
     def pec(self) -> str | None:
```

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/signals/forms.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/forms.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/signals/invoices.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/invoices.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/urls.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/urls.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/utils/__init__.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/utils/tax.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/tax.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pretix_fattura_elettronica/views.py` & `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/views.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/pyproject.toml` & `pretix_fattura_elettronica-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "pretix-fattura-elettronica"
 description = "Plugin for Italian Electronic Invoices"
 readme = "README.md"
 keywords = [
     "pretix",
 ]
-version = "0.2.7"
+version = "0.2.8"
 requires-python = ">=3.8"
 authors = [
     { name = "Python Italia", email = "info@pycon.it" },
 ]
 maintainers = [
     { name = "Python Italia", email = "info@pycon.it" },
 ]
@@ -32,14 +32,15 @@
     "django-rest-framework",
     "pretix",
     "django-countries>=7.5.1",
     "pytest-icdiff>=0.8",
     "pdbpp>=0.10.3",
     "time-machine>=2.14.0",
     "devtools>=0.12.2",
+    "setuptools>=69.2.0",
 ]
 
 [project.entry-points."pretix.plugin"]
 pretix_fattura_elettronica = "pretix_fattura_elettronica:PretixPluginMeta"
 
 [project.entry-points."distutils.commands"]
 build = "pretix_plugin_build.build:CustomBuild"
```

### Comparing `pretix_fattura_elettronica-0.2.7/tests/conftest.py` & `pretix_fattura_elettronica-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/tests/serializers/test_private_order.py` & `pretix_fattura_elettronica-0.2.8/tests/serializers/test_private_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         tax_rule_ticket,
         tax_rule_hotel=tax_rule_zero,
         tax_rule_membership=tax_rule_zero,
     )
 
 
 @pytest.fixture
+@time_machine.travel("2017-12-01T10:00:00Z")
 def private_invoice(private_order: Order):
     invoice = Invoice(
         order=private_order,
         event=private_order.event,
         organizer=private_order.event.organizer,
         date=datetime.datetime.now(private_order.event.timezone).date(),
     )
@@ -186,14 +187,15 @@
     if private_order.status == Order.STATUS_CANCELED:
         generate_cancellation(invoice, False)
 
     return invoice
 
 
 @pytest.fixture
+@time_machine.travel("2017-12-01T10:00:00Z")
 def private_invoice_legacy_tax_rules(private_order_legacy_tax_rules: Order):
     invoice = Invoice(
         order=private_order_legacy_tax_rules,
         event=private_order_legacy_tax_rules.event,
         organizer=private_order_legacy_tax_rules.event.organizer,
         date=datetime.datetime.now(
             private_order_legacy_tax_rules.event.timezone
@@ -288,15 +290,15 @@
 
     assert invoice["fattura_elettronica_body"] == [
         {
             "dati_generali": {
                 "dati_generali_documento": {
                     "tipo_documento": "TD01",
                     "divisa": "EUR",
-                    "data": "2024-03-27",
+                    "data": "2017-12-01",
                     "numero": "DUMMY-00001",
                 }
             },
             "dati_beni_servizi": {
                 "dettaglio_linee": [
                     {
                         "numero_linea": 1,
```

### Comparing `pretix_fattura_elettronica-0.2.7/tests/test_acubeapi.py` & `pretix_fattura_elettronica-0.2.8/tests/test_acubeapi.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/tests/test_serializers.py` & `pretix_fattura_elettronica-0.2.8/tests/test_serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,18 +384,20 @@
                 "pec": "pec_address",
                 "sdi": None,
                 "codice_fiscale": "RBTRST82T13F839G",
                 "confirm_messages": [],
             }
         )
         invoice3.save()
-        with pytest.raises(ValueError) as e:
-            OrderSerializer.serialize_invoices(business_order)
+        data = OrderSerializer.serialize_invoices(business_order)
 
-        assert str(e.value) == "For a business invoice codice dest is required."
+        assert (
+            data[0][1].fattura_elettronica_header.dati_trasmissione.codice_destinatario
+            == "0000000"
+        )
 
     def test_no_codice_destinatario_does_not_fail_if_not_it(
         self, business_order, invoice3
     ):
         invoice3.order.meta_info = json.dumps(
             {
                 "email": "pec_address",
```

### Comparing `pretix_fattura_elettronica-0.2.7/tests/test_signals.py` & `pretix_fattura_elettronica-0.2.8/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/tests/test_validation.py` & `pretix_fattura_elettronica-0.2.8/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/tests/test_views.py` & `pretix_fattura_elettronica-0.2.8/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/tests/utils.py` & `pretix_fattura_elettronica-0.2.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.7/PKG-INFO` & `pretix_fattura_elettronica-0.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-fattura-elettronica
-Version: 0.2.7
+Version: 0.2.8
 Summary: Plugin for Italian Electronic Invoices
 Keywords: pretix
 Home-page: https://github.com/pythonitalia/pretix-fattura-elettronica
 Author-Email: Python Italia <info@pycon.it>
 Maintainer-Email: Python Italia <info@pycon.it>
 License: Apache
 Project-URL: Homepage, https://github.com/pythonitalia/pretix-fattura-elettronica
@@ -21,14 +21,15 @@
 Requires-Dist: django-rest-framework; extra == "dev"
 Requires-Dist: pretix; extra == "dev"
 Requires-Dist: django-countries>=7.5.1; extra == "dev"
 Requires-Dist: pytest-icdiff>=0.8; extra == "dev"
 Requires-Dist: pdbpp>=0.10.3; extra == "dev"
 Requires-Dist: time-machine>=2.14.0; extra == "dev"
 Requires-Dist: devtools>=0.12.2; extra == "dev"
+Requires-Dist: setuptools>=69.2.0; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 Fattura Elettronica
 ==========================
 
 This is a plugin for `pretix`_.
```

