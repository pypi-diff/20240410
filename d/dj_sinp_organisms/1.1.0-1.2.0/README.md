# Comparing `tmp/dj_sinp_organisms-1.1.0.tar.gz` & `tmp/dj_sinp_organisms-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_organisms-1.1.0.tar", max compression
+gzip compressed data, was "dj_sinp_organisms-1.2.0.tar", max compression
```

## Comparing `dj_sinp_organisms-1.1.0.tar` & `dj_sinp_organisms-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0    34523 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/LICENSE
--rw-r--r--   0        0        0     1355 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/README.rst
--rw-r--r--   0        0        0     1709 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/sinp_organisms/__init__.py
--rw-r--r--   0        0        0      652 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/sinp_organisms/admin.py
--rw-r--r--   0        0        0      159 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/sinp_organisms/apps.py
--rw-r--r--   0        0        0        0 2024-03-23 23:30:02.473049 dj_sinp_organisms-1.1.0/sinp_organisms/fixtures/.gitkeep
--rw-r--r--   0        0        0 11416410 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/fixtures/inpn_organisms.xml
--rw-r--r--   0        0        0    10372 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0001_initial.py
--rw-r--r--   0        0        0     3898 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0002_auto_20210718_2027.py
--rw-r--r--   0        0        0      638 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0003_organism_parent.py
--rw-r--r--   0        0        0      661 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py
--rw-r--r--   0        0        0     1014 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py
--rw-r--r--   0        0        0     2235 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py
--rw-r--r--   0        0        0        0 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/migrations/__init__.py
--rw-r--r--   0        0        0     2241 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/mixins.py
--rw-r--r--   0        0        0     5303 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/models.py
--rw-r--r--   0        0        0     1695 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/serializers.py
--rw-r--r--   0        0        0      919 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/tests.py
--rw-r--r--   0        0        0      376 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/urls.py
--rw-r--r--   0        0        0      354 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/validators.py
--rw-r--r--   0        0        0     1386 2024-03-23 23:30:02.501049 dj_sinp_organisms-1.1.0/sinp_organisms/views.py
--rw-r--r--   0        0        0     2238 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-10 07:37:38.901162 dj_sinp_organisms-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1204 2024-04-10 07:37:38.901162 dj_sinp_organisms-1.2.0/README.md
+-rw-r--r--   0        0        0     1821 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/admin.py
+-rw-r--r--   0        0        0      159 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/apps.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:37:38.905162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/.gitkeep
+-rw-r--r--   0        0        0  4643951 2024-04-10 07:37:38.921162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/inpn_organisms.json
+-rw-r--r--   0        0        0    21517 2024-04-10 07:37:38.921162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/nomenclatures.json
+-rw-r--r--   0        0        0  7113254 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/fixtures/test_data.json
+-rw-r--r--   0        0        0      840 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/managers.py
+-rw-r--r--   0        0        0    10846 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4124 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0002_auto_20210718_2027.py
+-rw-r--r--   0        0        0      638 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0003_organism_parent.py
+-rw-r--r--   0        0        0      675 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py
+-rw-r--r--   0        0        0     1014 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py
+-rw-r--r--   0        0        0     4981 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0006_remove_organism_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/migrations/__init__.py
+-rw-r--r--   0        0        0     2241 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/mixins.py
+-rw-r--r--   0        0        0     5513 2024-04-10 07:37:38.941162 dj_sinp_organisms-1.2.0/sinp_organisms/models.py
+-rw-r--r--   0        0        0     1308 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/serializers.py
+-rw-r--r--   0        0        0     2570 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/tests.py
+-rw-r--r--   0        0        0      376 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/urls.py
+-rw-r--r--   0        0        0      330 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/validators.py
+-rw-r--r--   0        0        0     1386 2024-04-10 07:37:38.945162 dj_sinp_organisms-1.2.0/sinp_organisms/views.py
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 dj_sinp_organisms-1.2.0/PKG-INFO
```

### Comparing `dj_sinp_organisms-1.1.0/LICENSE` & `dj_sinp_organisms-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.1.0/README.rst` & `dj_sinp_organisms-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-=========================
-SINP Organisms for Django
-=========================
+# SINP Organisms for Django
 
-`DjangoSinpOrganisms <https://github.com/dbchiro/DjangoSinpOrganisms>`_ is a simple `Django <https://www.djangoproject.com/>`_ reusable app to manage `French SINP Organisms <http://standards-sinp.mnhn.fr/referentiel-des-organismes/>`_, respecting standard.
+[DjangoSinpOrganisms](https://github.com/dbchiro/DjangoSinpOrganisms) is a simple [Django](https://www.djangoproject.com/) reusable app to manage [French SINP Organisms](http://standards-sinp.mnhn.fr/referentiel-des-organismes/), respecting standard.
 
+See docs for more details : <https://dbchiro.github.io/DjangoSinpOrganisms/>
 
-Detailed documentation is in the "docs" directory.
-
-Quick start
------------
+## Quick start
 
 1. Install app
 
-.. code-block:: bash
-
-    $ pip install -U dj-sinp-organisms
-
-
-
-2. Configure ``INSTALLED_APPS``:
-
-.. code-block:: python
-
-    INSTALLED_APPS = (
-        'django.contrib.admin',
-        'django.contrib.auth',
-        (...),
-        'rest_framework',
-        'sinp_nomenclatures',
-        'sinp_organisms',
-        (...),
-    )
+```bash
+pip install -U dj-sinp-organisms
+```
+
+2. Configure `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = (
+    'django.contrib.admin',
+    'django.contrib.auth',
+    (...),
+    'rest_framework',
+    'sinp_nomenclatures',
+    'sinp_organisms',
+    (...),
+)
+```
+
+3. Configure `urls.py`:
+
+```python
+urlpatterns = [
+    path('admin/', admin.site.urls),
+    path('api-auth/', include('rest_framework.urls')),
+    (...),
+    path('api/v1/', include('sinp_nomenclatures.urls')),
+    path('api/v1/', include('sinp_organisms.urls')),
+    (...),
+]
+```
 
-
-3. Configure ``urls.py``:
-
-.. code-block:: python
-
-    urlpatterns = [
-        path('admin/', admin.site.urls),
-        path('api-auth/', include('rest_framework.urls')),
-        (...),
-        path('api/v1/', include('sinp_nomenclatures.urls')),
-        path('api/v1/', include('sinp_organisms.urls')),
-        (...),
-    ]
-
-4. Run ``python manage.py migrate`` to create the polls models.
-
-5. Start the development server and visit http://127.0.0.1:8000/admin/
+4. Run `python manage.py migrate` to create the polls models.
+5. Start the development server and visit <http://127.0.0.1:8000/admin/>
    to create an organism (you'll need the Admin app enabled).
-
-6. Visit http://127.0.0.1:8000/api/v1/organisms to view organisms API.
+6. Visit <http://127.0.0.1:8000/api/v1/organisms> to view organisms API.
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0001_initial.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0001_initial.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,87 +50,97 @@
                     "short_label",
                     models.CharField(
                         max_length=50, unique=True, verbose_name="Nom court"
                     ),
                 ),
                 (
                     "geographic_area_details",
-                    models.CharField(
+                    models.CharField(  # noqa: DJ01
                         blank=True,
-                        help_text="Information précisant la zone géographique d'action. Exemple : Basse-Terre",
+                        help_text="Information précisant la zone géographique d'action. Exemple : Basse-Terre",  # noqa: E501
                         max_length=500,
                         null=True,
                         verbose_name="Détails sur la zone géographique",
                     ),
                 ),
                 (
                     "address",
-                    models.CharField(
+                    models.CharField(  # noqa: DJ01
                         blank=True,
                         max_length=500,
                         null=True,
                         verbose_name="Adresse",
                     ),
                 ),
                 (
                     "postal_code",
-                    models.CharField(
+                    models.CharField(  # noqa: DJ01
                         blank=True,
                         max_length=20,
                         null=True,
                         verbose_name="Code postal",
                     ),
                 ),
                 (
                     "municipality",
-                    models.CharField(
+                    models.CharField(  # noqa: DJ01
                         blank=True,
                         max_length=250,
                         null=True,
                         verbose_name="Commune",
                     ),
                 ),
                 (
                     "email",
-                    models.EmailField(
+                    models.EmailField(  # noqa: DJ01
                         blank=True,
                         max_length=254,
                         null=True,
                         verbose_name="Adresse mail",
                     ),
                 ),
                 (
                     "phone_number",
-                    models.CharField(
+                    models.CharField(  # noqa: DJ01
                         blank=True,
                         max_length=17,
                         null=True,
                         validators=[
                             django.core.validators.RegexValidator(
-                                message="Les numéros de téléphones doivent être renseignés avec le format : '+999999999'. jusqu'à 15 chiffres sont autorisés",
+                                message=(
+                                    "Les numéros de téléphones doivent "
+                                    "être renseignés avec le format : "
+                                    "'+999999999'. jusqu'à 15 chiffres "
+                                    "sont autorisés"
+                                ),
                                 regex="^\\+?1?\\d{9,15}$",
                             )
                         ],
                         verbose_name="Numéro de téléphone",
                     ),
                 ),
                 (
                     "url",
-                    models.URLField(blank=True, null=True, verbose_name="URL"),
+                    models.URLField(  # noqa: DJ01
+                        blank=True, null=True, verbose_name="URL"
+                    ),
                 ),
                 (
                     "extra_data",
                     models.JSONField(
                         blank=True, null=True, verbose_name="Additional datas"
                     ),
                 ),
                 (
                     "action_scope",
                     models.ForeignKey(
-                        help_text="Périmètre d'action de l'organisme (Européen, national, Supra-régional, Régional, Inconnu)",
+                        help_text=(
+                            "Périmètre d'action de l'organisme (Européen, "
+                            "national, Supra-régional, Régional, Inconnu)"
+                        ),
                         limit_choices_to={"type": "action_scope"},
                         on_delete=django.db.models.deletion.DO_NOTHING,
                         related_name="organism_action_scope",
                         to="sinp_nomenclatures.nomenclature",
                         verbose_name="Périmètre d'action",
                     ),
                 ),
@@ -242,15 +252,17 @@
                 verbose_name="Membres",
             ),
         ),
         migrations.AddField(
             model_name="organism",
             name="status",
             field=models.ForeignKey(
-                help_text="Permet d'indiquer si l'organisme est public ou privé",
+                help_text=(
+                    "Permet d'indiquer si l'organisme est public ou privé"
+                ),
                 limit_choices_to={"type": "organism_status"},
                 on_delete=django.db.models.deletion.DO_NOTHING,
                 related_name="organism_status",
                 to="sinp_nomenclatures.nomenclature",
                 verbose_name="Statut",
             ),
         ),
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0002_auto_20210718_2027.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0002_auto_20210718_2027.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,43 +37,51 @@
                 to="sinp_nomenclatures.nomenclature",
                 verbose_name="Zone géographique",
             ),
         ),
         migrations.AlterField(
             model_name="organism",
             name="geographic_area_details",
-            field=models.CharField(
+            field=models.CharField(  # noqa: DJ01
                 blank=True,
-                help_text="Information précisant la zone géographique d'action.",
+                help_text=(
+                    "Information précisant la zone géographique d'action."
+                ),
                 max_length=500,
                 null=True,
                 verbose_name="Détails sur la zone géographique",
             ),
         ),
         migrations.AlterField(
             model_name="organism",
             name="phone_number",
-            field=models.CharField(
+            field=models.CharField(  # noqa: DJ01
                 blank=True,
                 max_length=17,
                 null=True,
                 validators=[
                     django.core.validators.RegexValidator(
-                        message="Les numéros de téléphones doivent être renseignés avec le format :'+999999999'. jusqu'à 15 chiffres sont autorisés",
+                        message=(
+                            "Les numéros de téléphones doivent être "
+                            "renseignés avec le format :'+999999999'. "
+                            "jusqu'à 15 chiffres sont autorisés"
+                        ),
                         regex="^\\+?1?\\d{9,15}$",
                     )
                 ],
                 verbose_name="Numéro de téléphone",
             ),
         ),
         migrations.AlterField(
             model_name="organism",
             name="status",
             field=models.ForeignKey(
-                help_text="Permet d'indiquer si l'organisme est public ou privé",
+                help_text=(
+                    "Permet d'indiquer si l'organisme est public ou privé"
+                ),
                 limit_choices_to={"type__mnemonic": "organism_status"},
                 on_delete=django.db.models.deletion.DO_NOTHING,
                 related_name="organism_status",
                 to="sinp_nomenclatures.nomenclature",
                 verbose_name="Statut",
             ),
         ),
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0003_organism_parent.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0003_organism_parent.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.2.5 on 2021-07-18 21:52
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("sinp_organisms", "0002_auto_20210718_2027"),
     ]
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0004_organism_administrative_reference_organism_enabled.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         ("sinp_organisms", "0003_organism_parent"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="organism",
             name="administrative_reference",
-            field=models.CharField(
+            field=models.CharField(  # noqa: DJ01
                 blank=True, max_length=100, null=True, verbose_name="SIRET"
             ),
         ),
         migrations.AddField(
             model_name="organism",
             name="enabled",
             field=models.BooleanField(default=True, verbose_name="Actif"),
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/migrations/0005_remove_organism_geographic_area_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/mixins.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/mixins.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/models.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,41 @@
-from uuid import uuid4
+from typing import Tuple
+from uuid import UUID, uuid4
 
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext as _
 from sinp_nomenclatures.models import Nomenclature
 
+from .managers import OrganismManager, OrganismMemberManager
 from .validators import phone_regex
 
-# class BaseModel(models.Model):
-#     """Generic base model with standard metadatas"""
 
-#     timestamp_create = models.DateTimeField(auto_now_add=True, editable=False)
-#     timestamp_update = models.DateTimeField(auto_now=True, editable=False)
-#     created_by = models.ForeignKey(
-#         settings.AUTH_USER_MODEL,
-#         null=True,
-#         blank=True,
-#         db_index=True,
-#         editable=False,
-#         related_name="+",
-#         on_delete=models.SET_NULL,
-#     )
-#     updated_by = models.ForeignKey(
-#         settings.AUTH_USER_MODEL,
-#         null=True,
-#         blank=True,
-#         db_index=True,
-#         editable=False,
-#         related_name="+",
-#         on_delete=models.SET_NULL,
-#     )
+class BaseModel(models.Model):
+    """Generic base model with standard metadatas"""
 
-#     class Meta:
-#         abstract = True
+    timestamp_create = models.DateTimeField(auto_now_add=True, editable=False)
+    timestamp_update = models.DateTimeField(auto_now=True, editable=False)
+
+    class Meta:
+        abstract = True
 
 
 # Create your models here.
-class Organism(models.Model):
+class Organism(BaseModel):
     """Organism model"""
 
     uuid = models.UUIDField(
         default=uuid4,
         unique=True,
         editable=False,
         verbose_name=_("Identifiant unique"),
     )
     administrative_reference = models.CharField(
-        max_length=100, blank=True, null=True, verbose_name=_("SIRET")
+        max_length=100, blank=True, verbose_name=_("SIRET")
     )
     parent = models.ForeignKey(
         "Organism",
         verbose_name=_("Organisme parent"),
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
@@ -75,15 +60,14 @@
         limit_choices_to={"type__mnemonic": "geographic_area"},
         related_name="organism_geographic_area",
         verbose_name=_("Zone géographique"),
         help_text=_("Zone d'action géographique de l'organisme"),
     )
     geographic_area_details = models.CharField(
         max_length=500,
-        null=True,
         blank=True,
         verbose_name=_("Détails sur la zone géographique"),
         help_text=_("Information précisant la zone géographique d'action."),
     )
     status = models.ForeignKey(
         Nomenclature,
         on_delete=models.DO_NOTHING,
@@ -96,74 +80,98 @@
         Nomenclature,
         on_delete=models.DO_NOTHING,
         limit_choices_to={"type__mnemonic": "organism_type"},
         related_name="organism_type",
         verbose_name=_("Type d'organisme"),
     )
     address = models.CharField(
-        max_length=500, blank=True, null=True, verbose_name=_("Adresse")
+        max_length=500, blank=True, verbose_name=_("Adresse")
     )
     postal_code = models.CharField(
-        max_length=20, blank=True, null=True, verbose_name=_("Code postal")
+        max_length=20, blank=True, verbose_name=_("Code postal")
     )
     municipality = models.CharField(
-        max_length=250, blank=True, null=True, verbose_name=_("Commune")
-    )
-    email = models.EmailField(
-        blank=True, null=True, verbose_name=_("Adresse mail")
+        max_length=250, blank=True, verbose_name=_("Commune")
     )
+    email = models.EmailField(blank=True, verbose_name=_("Adresse mail"))
     phone_number = models.CharField(
         validators=[phone_regex],
         max_length=17,
         blank=True,
-        null=True,
         verbose_name=_("Numéro de téléphone"),
     )
-    url = models.URLField(
-        max_length=200, blank=True, null=True, verbose_name=_("URL")
-    )
+    url = models.URLField(max_length=200, blank=True, verbose_name=_("URL"))
     members = models.ManyToManyField(
         settings.AUTH_USER_MODEL,
         through="OrganismMember",
         through_fields=("organism", "member"),
         blank=True,
         related_name="organism_member",
         verbose_name=_("Membres"),
     )
     enabled = models.BooleanField(default=True, verbose_name=_("Actif"))
     extra_data = models.JSONField(
         blank=True, null=True, verbose_name=_("Additional datas")
     )
+    objects = OrganismManager()
 
     class Meta:
         verbose_name_plural = _("organismes")
 
+        constraints = [
+            models.UniqueConstraint(
+                fields=["uuid"],
+                name="unique_uuid",
+            ),
+        ]
+
+    def natural_key(self):
+        return (self.uuid,)
+
     def __str__(self):
-        return self.short_label
+        return str(self.short_label)
 
 
-class OrganismMember(models.Model):
+class OrganismMember(BaseModel):
     """Organism members model"""
 
     member = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         verbose_name=_("Utilisateur"),
-        related_name="members",
+        # related_name="organisms",
     )
     organism = models.ForeignKey(
-        "Organism", on_delete=models.CASCADE, verbose_name=_("Organisme")
+        "Organism",
+        on_delete=models.CASCADE,
+        verbose_name=_("Organisme"),
+        # related_name="members_set",
     )
     member_level = models.ForeignKey(
         Nomenclature,
         on_delete=models.CASCADE,
         limit_choices_to={"type__mnemonic": "member_level"},
         related_name="member_level",
         verbose_name=_("Niveau du membre"),
     )
+    objects = OrganismMemberManager()
 
     class Meta:
         verbose_name_plural = _("Membre des organismes")
         unique_together = ("member", "organism", "member_level")
 
     def __str__(self):
-        return f"{self.member.username} [{self.member_level}]"
+        return f"{self.member} [{self.member_level}]"
+
+    def natural_key(self) -> Tuple[UUID, UUID, str, str]:
+        """_summary_
+
+        Returns:
+            Tuple[UUID,UUID, UUID,str,str]: A tuple with respectively
+            member UUID, organism UUID, member_level code
+        """
+        return (
+            self.member.username,
+            self.organism.uuid,
+            self.member_level.code,
+            self.member_level.type.mnemonic,
+        )
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/serializers.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,14 @@
     class Meta:
         model = OrganismMember
         fields = [
             "id",
             "member",
             "member_level",
         ]
-        read_only_fields = [
-            "created_by",
-            "updated_by",
-            "timestamp_create",
-            "timestamp_update",
-        ]
 
 
 class OrganismSerializer(ModelSerializer):
     class Meta:
         model = Organism
         fields = [
             "id",
@@ -37,24 +31,16 @@
             "type",
             "address",
             "postal_code",
             "municipality",
             "email",
             "phone_number",
             "url",
-            "created_by",
-            "updated_by",
-            "timestamp_create",
-            "timestamp_update",
         ]
         read_only_fields = [
-            "created_by",
-            "updated_by",
-            "timestamp_create",
-            "timestamp_update",
             "uuid",
         ]
 
 
 class OrganismDetailledSerializer(OrganismSerializer):
     action_scope = NomenclatureSerializer(read_only=True)
     geographic_area = NomenclatureSerializer(read_only=True, many=True)
```

### Comparing `dj_sinp_organisms-1.1.0/sinp_organisms/views.py` & `dj_sinp_organisms-1.2.0/sinp_organisms/views.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_organisms-1.1.0/PKG-INFO` & `dj_sinp_organisms-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 Metadata-Version: 2.1
 Name: dj_sinp_organisms
-Version: 1.1.0
+Version: 1.2.0
 Summary: Django app to manage french SINP organisms standard
-Home-page: https://github.com/dbchiro/DjangoSinpNomenclature
+Home-page: https://github.com/dbchiro/DjangoSinpOrganisms
 License: AGPLv3
 Keywords: SINP,Nomenclatures,Django,France,dbChiroWeb
 Author: dbChiro project
-Author-email: project@dbchiro.org
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
-Requires-Dist: dj-sinp-nomenclatures (>=0.2.4,<0.3.0)
+Requires-Dist: dj-sinp-nomenclatures (>=1.0.0,<2.0.0)
 Requires-Dist: djangorestframework (>=3,<4)
-Project-URL: Repository, https://github.com/dbchiro/DjangoSinpNomenclature
-Description-Content-Type: text/x-rst
+Project-URL: Documentation, https://dbchiro.github.io/DjangoSinpOrganisms/
+Project-URL: Repository, https://github.com/dbchiro/DjangoSinpOrganisms
+Description-Content-Type: text/markdown
 
-=========================
-SINP Organisms for Django
-=========================
+# SINP Organisms for Django
 
-`DjangoSinpOrganisms <https://github.com/dbchiro/DjangoSinpOrganisms>`_ is a simple `Django <https://www.djangoproject.com/>`_ reusable app to manage `French SINP Organisms <http://standards-sinp.mnhn.fr/referentiel-des-organismes/>`_, respecting standard.
+[DjangoSinpOrganisms](https://github.com/dbchiro/DjangoSinpOrganisms) is a simple [Django](https://www.djangoproject.com/) reusable app to manage [French SINP Organisms](http://standards-sinp.mnhn.fr/referentiel-des-organismes/), respecting standard.
 
+See docs for more details : <https://dbchiro.github.io/DjangoSinpOrganisms/>
 
-Detailed documentation is in the "docs" directory.
-
-Quick start
------------
+## Quick start
 
 1. Install app
 
-.. code-block:: bash
-
-    $ pip install -U dj-sinp-organisms
-
-
-
-2. Configure ``INSTALLED_APPS``:
-
-.. code-block:: python
-
-    INSTALLED_APPS = (
-        'django.contrib.admin',
-        'django.contrib.auth',
-        (...),
-        'rest_framework',
-        'sinp_nomenclatures',
-        'sinp_organisms',
-        (...),
-    )
+```bash
+pip install -U dj-sinp-organisms
+```
+
+2. Configure `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = (
+    'django.contrib.admin',
+    'django.contrib.auth',
+    (...),
+    'rest_framework',
+    'sinp_nomenclatures',
+    'sinp_organisms',
+    (...),
+)
+```
+
+3. Configure `urls.py`:
+
+```python
+urlpatterns = [
+    path('admin/', admin.site.urls),
+    path('api-auth/', include('rest_framework.urls')),
+    (...),
+    path('api/v1/', include('sinp_nomenclatures.urls')),
+    path('api/v1/', include('sinp_organisms.urls')),
+    (...),
+]
+```
 
-
-3. Configure ``urls.py``:
-
-.. code-block:: python
-
-    urlpatterns = [
-        path('admin/', admin.site.urls),
-        path('api-auth/', include('rest_framework.urls')),
-        (...),
-        path('api/v1/', include('sinp_nomenclatures.urls')),
-        path('api/v1/', include('sinp_organisms.urls')),
-        (...),
-    ]
-
-4. Run ``python manage.py migrate`` to create the polls models.
-
-5. Start the development server and visit http://127.0.0.1:8000/admin/
+4. Run `python manage.py migrate` to create the polls models.
+5. Start the development server and visit <http://127.0.0.1:8000/admin/>
    to create an organism (you'll need the Admin app enabled).
-
-6. Visit http://127.0.0.1:8000/api/v1/organisms to view organisms API.
+6. Visit <http://127.0.0.1:8000/api/v1/organisms> to view organisms API.
```

