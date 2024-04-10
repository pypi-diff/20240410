# Comparing `tmp/pretix_fattura_elettronica-0.2.8.tar.gz` & `tmp/pretix_fattura_elettronica-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_fattura_elettronica-0.2.8.tar", last modified: Wed Apr 10 14:33:28 2024, max compression
+gzip compressed data, was "pretix_fattura_elettronica-0.2.9.tar", last modified: Wed Apr 10 14:55:47 2024, max compression
```

## Comparing `pretix_fattura_elettronica-0.2.8.tar` & `pretix_fattura_elettronica-0.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      576 2024-04-08 11:41:35.013314 pretix_fattura_elettronica-0.2.8/LICENSE
--rw-r--r--   0        0        0     1146 2024-04-08 11:41:35.013687 pretix_fattura_elettronica-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.014674 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/__init__.py
--rw-r--r--   0        0        0     2205 2024-04-08 11:41:35.015125 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/acubeapi.py
--rw-r--r--   0        0        0      813 2024-04-08 11:41:35.015236 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/apps.py
--rw-r--r--   0        0        0     1795 2024-04-08 11:41:35.015372 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/enums.py
--rw-r--r--   0        0        0     1887 2024-04-08 11:41:35.015502 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/forms.py
--rw-r--r--   0        0        0      334 2024-04-08 11:41:35.015828 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.015938 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      334 2024-04-08 11:41:35.016147 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1297 2024-04-08 11:41:35.016356 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.016402 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/__init__.py
--rw-r--r--   0        0        0      552 2024-04-08 11:41:35.016535 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/models.py
--rw-r--r--   0        0        0    16374 2024-04-10 13:56:54.961562 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/serializers.py
--rw-r--r--   0        0        0       61 2024-04-08 11:41:35.016904 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/__init__.py
--rw-r--r--   0        0        0     1245 2024-04-08 11:41:35.017014 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/forms.py
--rw-r--r--   0        0        0      638 2024-04-08 11:41:35.017125 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/invoices.py
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017309 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/static/pretix_fattura_elettronica/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017572 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/.gitkeep
--rw-r--r--   0        0        0     1676 2024-04-08 11:41:35.017731 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html
--rw-r--r--   0        0        0     3115 2024-04-08 11:41:35.017880 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html
--rw-r--r--   0        0        0     3806 2024-04-08 11:41:35.018209 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.018344 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templatetags/__init__.py
--rw-r--r--   0        0        0      377 2024-04-08 11:41:35.018520 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templatetags/fatturaelt.py
--rw-r--r--   0        0        0     1215 2024-04-08 11:41:35.018658 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/urls.py
--rw-r--r--   0        0        0     3555 2024-04-08 11:41:35.018914 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/__init__.py
--rw-r--r--   0        0        0      950 2024-04-08 11:41:35.019062 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/tax.py
--rw-r--r--   0        0        0     8429 2024-04-08 11:41:35.019273 pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/views.py
--rw-r--r--   0        0        0     2408 2024-04-10 14:33:28.576427 pretix_fattura_elettronica-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020103 pretix_fattura_elettronica-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     7847 2024-04-08 11:41:35.020401 pretix_fattura_elettronica-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020608 pretix_fattura_elettronica-0.2.8/tests/serializers/__init__.py
--rw-r--r--   0        0        0    11282 2024-04-10 14:28:33.289351 pretix_fattura_elettronica-0.2.8/tests/serializers/test_private_order.py
--rw-r--r--   0        0        0     1800 2024-04-08 11:41:35.020955 pretix_fattura_elettronica-0.2.8/tests/test_acubeapi.py
--rw-r--r--   0        0        0    32411 2024-04-10 14:29:06.563216 pretix_fattura_elettronica-0.2.8/tests/test_serializers.py
--rw-r--r--   0        0        0      865 2024-04-08 11:41:35.021298 pretix_fattura_elettronica-0.2.8/tests/test_signals.py
--rw-r--r--   0        0        0     1752 2024-04-08 11:41:35.021442 pretix_fattura_elettronica-0.2.8/tests/test_validation.py
--rw-r--r--   0        0        0     3384 2024-04-08 11:41:35.021557 pretix_fattura_elettronica-0.2.8/tests/test_views.py
--rw-r--r--   0        0        0     3614 2024-04-08 11:41:35.021672 pretix_fattura_elettronica-0.2.8/tests/utils.py
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 pretix_fattura_elettronica-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      576 2024-04-08 11:41:35.013314 pretix_fattura_elettronica-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1146 2024-04-08 11:41:35.013687 pretix_fattura_elettronica-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.014674 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/__init__.py
+-rw-r--r--   0        0        0     2205 2024-04-08 11:41:35.015125 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/acubeapi.py
+-rw-r--r--   0        0        0      813 2024-04-08 11:41:35.015236 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/apps.py
+-rw-r--r--   0        0        0     1795 2024-04-08 11:41:35.015372 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/enums.py
+-rw-r--r--   0        0        0     1887 2024-04-08 11:41:35.015502 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/forms.py
+-rw-r--r--   0        0        0      334 2024-04-08 11:41:35.015828 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.015938 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      334 2024-04-08 11:41:35.016147 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1297 2024-04-08 11:41:35.016356 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.016402 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/migrations/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-08 11:41:35.016535 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/models.py
+-rw-r--r--   0        0        0    16312 2024-04-10 14:53:40.184838 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/serializers.py
+-rw-r--r--   0        0        0       61 2024-04-08 11:41:35.016904 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/signals/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-08 11:41:35.017014 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/signals/forms.py
+-rw-r--r--   0        0        0      638 2024-04-08 11:41:35.017125 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/signals/invoices.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017309 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/static/pretix_fattura_elettronica/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.017572 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/.gitkeep
+-rw-r--r--   0        0        0     1676 2024-04-08 11:41:35.017731 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html
+-rw-r--r--   0        0        0     3115 2024-04-08 11:41:35.017880 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html
+-rw-r--r--   0        0        0     3806 2024-04-08 11:41:35.018209 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.018344 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templatetags/__init__.py
+-rw-r--r--   0        0        0      377 2024-04-08 11:41:35.018520 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templatetags/fatturaelt.py
+-rw-r--r--   0        0        0     1215 2024-04-08 11:41:35.018658 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/urls.py
+-rw-r--r--   0        0        0     3555 2024-04-08 11:41:35.018914 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/utils/__init__.py
+-rw-r--r--   0        0        0      950 2024-04-08 11:41:35.019062 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/utils/tax.py
+-rw-r--r--   0        0        0     8429 2024-04-08 11:41:35.019273 pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/views.py
+-rw-r--r--   0        0        0     2408 2024-04-10 14:55:47.387263 pretix_fattura_elettronica-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020103 pretix_fattura_elettronica-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     7847 2024-04-08 11:41:35.020401 pretix_fattura_elettronica-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:41:35.020608 pretix_fattura_elettronica-0.2.9/tests/serializers/__init__.py
+-rw-r--r--   0        0        0    11282 2024-04-10 14:28:33.289351 pretix_fattura_elettronica-0.2.9/tests/serializers/test_private_order.py
+-rw-r--r--   0        0        0     1800 2024-04-08 11:41:35.020955 pretix_fattura_elettronica-0.2.9/tests/test_acubeapi.py
+-rw-r--r--   0        0        0    32063 2024-04-10 14:52:13.636936 pretix_fattura_elettronica-0.2.9/tests/test_serializers.py
+-rw-r--r--   0        0        0      865 2024-04-08 11:41:35.021298 pretix_fattura_elettronica-0.2.9/tests/test_signals.py
+-rw-r--r--   0        0        0     1765 2024-04-10 14:54:26.999140 pretix_fattura_elettronica-0.2.9/tests/test_validation.py
+-rw-r--r--   0        0        0     3384 2024-04-08 11:41:35.021557 pretix_fattura_elettronica-0.2.9/tests/test_views.py
+-rw-r--r--   0        0        0     3614 2024-04-08 11:41:35.021672 pretix_fattura_elettronica-0.2.9/tests/utils.py
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 pretix_fattura_elettronica-0.2.9/PKG-INFO
```

### Comparing `pretix_fattura_elettronica-0.2.8/LICENSE` & `pretix_fattura_elettronica-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/README.md` & `pretix_fattura_elettronica-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/acubeapi.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/acubeapi.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/apps.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/apps.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/enums.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/enums.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/forms.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/forms.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/migrations/0001_initial.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/models.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/models.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/serializers.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,17 @@
     aliquota_iva: Annotated[str, Field(serialization_alias="AliquotaIVA")]
     ritenuta: Annotated[str | None, Field(serialization_alias="Ritenuta")] = None
     natura: Annotated[str | None, Field(serialization_alias="Natura")] = None
 
     # validate natura based on aliquota_iva
     @validator("natura", always=True)
     def check_natura(cls, v: str | None, values: dict[str, str | None]) -> str | None:
+        description = values.get("descrizione")
         if values.get("aliquota_iva") == "0.00" and not v:
-            raise ValueError("Natura non valida per aliquota IVA 0.00")
+            raise ValueError(f"Natura non valida per aliquota IVA 0.00: {v} - {description}")
 
         return v
 
 
 class DatiRiepilogo(BaseModel):
     aliquota_iva: Annotated[str, Field(serialization_alias="AliquotaIVA")]
     natura: Annotated[str | None, Field(serialization_alias="Natura")] = None
@@ -443,17 +444,14 @@
     @property
     def pec(self) -> str | None:
         return get_pec(self._invoice.order)
 
     @property
     def vat_id(self) -> str | None:
         if self.is_business_invoice:
-            if not self._invoice.invoice_to_vat_id:
-                raise ValueError("For a business invoice VAT ID is required.")
-
             return self._invoice.invoice_to_vat_id
 
         return None
 
     @property
     def codice_fiscale(self) -> str | None:
         codice_fiscale = get_codice_fiscale(self._invoice.order)
```

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/forms.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/signals/forms.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/signals/invoices.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/signals/invoices.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/change_info.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretix_fattura_elettronica/einvoices.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/templates/pretixcontrol/order/index.html`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/urls.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/urls.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/__init__.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/utils/tax.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/utils/tax.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pretix_fattura_elettronica/views.py` & `pretix_fattura_elettronica-0.2.9/pretix_fattura_elettronica/views.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/pyproject.toml` & `pretix_fattura_elettronica-0.2.9/pyproject.toml`

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
-version = "0.2.8"
+version = "0.2.9"
 requires-python = ">=3.8"
 authors = [
     { name = "Python Italia", email = "info@pycon.it" },
 ]
 maintainers = [
     { name = "Python Italia", email = "info@pycon.it" },
 ]
```

### Comparing `pretix_fattura_elettronica-0.2.8/tests/conftest.py` & `pretix_fattura_elettronica-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/tests/serializers/test_private_order.py` & `pretix_fattura_elettronica-0.2.9/tests/serializers/test_private_order.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/tests/test_acubeapi.py` & `pretix_fattura_elettronica-0.2.9/tests/test_acubeapi.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/tests/test_serializers.py` & `pretix_fattura_elettronica-0.2.9/tests/test_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,22 +363,14 @@
         invoice = data[0][1]
 
         assert (
             invoice.fattura_elettronica_header.cessionario_committente.dati_anagrafici.codice_fiscale
             is None
         )
 
-    def test_wrong_business_customer_vat_id(self, business_order, invoice3):
-        invoice3.invoice_to_vat_id = None  # DELETING vat id
-        invoice3.save()
-        with pytest.raises(ValueError) as e:
-            OrderSerializer.serialize_invoices(business_order)
-
-        assert str(e.value) == "For a business invoice VAT ID is required."
-
     def test_wrong_business_customer_recipient_codice_dest(
         self, business_order, invoice3
     ):
         invoice3.order.meta_info = json.dumps(
             {
                 "email": "pec_address",
                 "pec": "pec_address",
```

### Comparing `pretix_fattura_elettronica-0.2.8/tests/test_signals.py` & `pretix_fattura_elettronica-0.2.9/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/tests/test_validation.py` & `pretix_fattura_elettronica-0.2.9/tests/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             prezzo_totale="1.00",
             aliquota_iva="0.00",
         )
 
     assert e.value.errors() == [
         {
             "loc": ("natura",),
-            "msg": "Value error, Natura non valida per aliquota IVA 0.00",
+            "msg": "Value error, Natura non valida per aliquota IVA 0.00: None - Test",
             "type": "value_error",
             "url": ANY,
             "ctx": ANY,
             "input": None,
         }
     ]
```

### Comparing `pretix_fattura_elettronica-0.2.8/tests/test_views.py` & `pretix_fattura_elettronica-0.2.9/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/tests/utils.py` & `pretix_fattura_elettronica-0.2.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pretix_fattura_elettronica-0.2.8/PKG-INFO` & `pretix_fattura_elettronica-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-fattura-elettronica
-Version: 0.2.8
+Version: 0.2.9
 Summary: Plugin for Italian Electronic Invoices
 Keywords: pretix
 Home-page: https://github.com/pythonitalia/pretix-fattura-elettronica
 Author-Email: Python Italia <info@pycon.it>
 Maintainer-Email: Python Italia <info@pycon.it>
 License: Apache
 Project-URL: Homepage, https://github.com/pythonitalia/pretix-fattura-elettronica
```

