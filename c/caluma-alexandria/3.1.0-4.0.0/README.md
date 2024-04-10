# Comparing `tmp/caluma_alexandria-3.1.0.tar.gz` & `tmp/caluma_alexandria-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-3.1.0.tar", max compression
+gzip compressed data, was "caluma_alexandria-4.0.0.tar", max compression
```

## Comparing `caluma_alexandria-3.1.0.tar` & `caluma_alexandria-4.0.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0    23293 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/LICENSE
--rw-r--r--   0        0        0     8416 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/alexandria/core/__init__.py
--rw-r--r--   0        0        0     2149 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/alexandria/core/api.py
--rw-r--r--   0        0        0      127 2024-03-20 17:06:47.132151 caluma_alexandria-3.1.0/alexandria/core/apps.py
--rw-r--r--   0        0        0    13501 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/factories.py
--rw-r--r--   0        0        0     6937 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/filters.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2394 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/management/commands/encrypt_files.py
--rw-r--r--   0        0        0      586 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/management/commands/generate_missing_thumbnails.py
--rw-r--r--   0        0        0     1084 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/management/commands/set_mime_type_and_size.py
--rw-r--r--   0        0        0    12553 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2840 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0      652 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0007_category_parent.py
--rw-r--r--   0        0        0      397 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0008_document_date.py
--rw-r--r--   0        0        0      466 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0009_file_checksum.py
--rw-r--r--   0        0        0     2973 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0010_mark.py
--rw-r--r--   0        0        0     1205 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0011_tag_uuid.py
--rw-r--r--   0        0        0     1655 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0012_tag_uuid_schema.py
--rw-r--r--   0        0        0     2086 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0013_file_content.py
--rw-r--r--   0        0        0      975 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0014_file_mime_type_size.py
--rw-r--r--   0        0        0     3304 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0015_fix_modified_by_description.py
--rw-r--r--   0        0        0      672 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/0016_category_allowed_mime_types.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0    10691 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/models.py
--rw-r--r--   0        0        0     1823 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/presign_urls.py
--rw-r--r--   0        0        0    11065 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/serializers.py
--rw-r--r--   0        0        0      409 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/urls.py
--rw-r--r--   0        0        0     9113 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/views.py
--rw-r--r--   0        0        0     1363 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/core/visibilities.py
--rw-r--r--   0        0        0     1703 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/dav.py
--rw-r--r--   0        0        0     4530 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/dav_provider.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     7390 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     5154 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/settings/django.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/storages/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/storages/backends/__init__.py
--rw-r--r--   0        0        0     1493 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/storages/backends/s3.py
--rw-r--r--   0        0        0     2595 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/storages/fields.py
--rw-r--r--   0        0        0      162 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/urls.py
--rw-r--r--   0        0        0     1048 2024-03-20 17:06:47.136151 caluma_alexandria-3.1.0/alexandria/wsgi.py
--rw-r--r--   0        0        0     3265 2024-03-20 17:06:47.140151 caluma_alexandria-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    10120 1970-01-01 00:00:00.000000 caluma_alexandria-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    23937 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/LICENSE
+-rw-r--r--   0        0        0     8517 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/__init__.py
+-rw-r--r--   0        0        0     2199 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/api.py
+-rw-r--r--   0        0        0      127 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/apps.py
+-rw-r--r--   0        0        0    13501 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/factories.py
+-rw-r--r--   0        0        0     6937 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/filters.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2394 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/encrypt_files.py
+-rw-r--r--   0        0        0      586 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/generate_missing_thumbnails.py
+-rw-r--r--   0        0        0     1084 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/management/commands/set_mime_type_and_size.py
+-rw-r--r--   0        0        0    12553 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2840 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0      652 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0007_category_parent.py
+-rw-r--r--   0        0        0      397 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0008_document_date.py
+-rw-r--r--   0        0        0      466 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0009_file_checksum.py
+-rw-r--r--   0        0        0     2973 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0010_mark.py
+-rw-r--r--   0        0        0     1205 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0011_tag_uuid.py
+-rw-r--r--   0        0        0     1655 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0012_tag_uuid_schema.py
+-rw-r--r--   0        0        0     2086 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0013_file_content.py
+-rw-r--r--   0        0        0      975 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0014_file_mime_type_size.py
+-rw-r--r--   0        0        0     3304 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0015_fix_modified_by_description.py
+-rw-r--r--   0        0        0      672 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/0016_category_allowed_mime_types.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0    10789 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/models.py
+-rw-r--r--   0        0        0     1823 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/presign_urls.py
+-rw-r--r--   0        0        0    11317 2024-04-10 09:27:07.580954 caluma_alexandria-4.0.0/alexandria/core/serializers.py
+-rw-r--r--   0        0        0      409 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1463 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/validations.py
+-rw-r--r--   0        0        0     9113 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/views.py
+-rw-r--r--   0        0        0     1363 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0     1703 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/dav.py
+-rw-r--r--   0        0        0     4530 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/dav_provider.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     7450 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     5154 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/settings/django.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/backends/__init__.py
+-rw-r--r--   0        0        0     1493 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/backends/s3.py
+-rw-r--r--   0        0        0     2595 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/storages/fields.py
+-rw-r--r--   0        0        0      162 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/urls.py
+-rw-r--r--   0        0        0     1048 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/alexandria/wsgi.py
+-rw-r--r--   0        0        0     3265 2024-04-10 09:27:07.584954 caluma_alexandria-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10221 1970-01-01 00:00:00.000000 caluma_alexandria-4.0.0/PKG-INFO
```

### Comparing `caluma_alexandria-3.1.0/CHANGELOG.md` & `caluma_alexandria-4.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# 4.0.0
+### Feature
+* **document:** Create document and file in one request! ([`444912d`](https://github.com/projectcaluma/alexandria/commit/444912d4cb584c05096ca8a78dd455b8471e9441))
+
+### Breaking
+* The document post endpoint now requires the file data to be provided as well. The reason for this change is allowing the frontend to create documents and files in one request, preventing documents with no associated files. Which fixes the problem if the file got rejected for any reason, the application would create an empty document. ([`444912d`](https://github.com/projectcaluma/alexandria/commit/444912d4cb584c05096ca8a78dd455b8471e9441))
+
 # 3.1.0
 ### Feature
 * **category:** Define allowed mime types ([`d4fd84e`](https://github.com/projectcaluma/alexandria/commit/d4fd84e6edb0502818f885082217aa48f0e56c5b))
 
 ### Fix
 * **mimetypes:** Cleanup, simplify error handling ([`3bde9c4`](https://github.com/projectcaluma/alexandria/commit/3bde9c490f5ba67d4859767fa37afeabba3f1326))
 * **translation:** Use string replacement instead of f string ([`74dd485`](https://github.com/projectcaluma/alexandria/commit/74dd485587e30765bea4a784beead595a33df405))
```

### Comparing `caluma_alexandria-3.1.0/LICENSE` & `caluma_alexandria-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/README.md` & `caluma_alexandria-4.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
   - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
   - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
   - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
 - Authorization configurations
   - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#visibilities) classes that define visibility for all models
   - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#permissions) classes that define permissions for all models
 - Data validation configuration
-  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations
+  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations. A default base class is used for file validation. Extend `AlexandriaValidator` for own validations.
 - Thumbnail configuration (optional)
 
   - `ALEXANDRIA_ENABLE_THUMBNAIL_GENERATION`: Set to `false` to disable thumbnail generation
     - Check the docker-compose file for an example on how to set up generation with s3 hooks
   - `ALEXANDRIA_THUMBNAIL_WIDTH`: Width of generated thumbnails
   - `ALEXANDRIA_THUMBNAIL_HEIGHT`: Height of generated thumbnails
   - `ALEXANDRIA_ENABLE_CHECKSUM`: Set to `false` to disable file checksums. Checksums are calculated after upload to allow later verification (not implemented in Alexandria)
```

### Comparing `caluma_alexandria-3.1.0/alexandria/core/api.py` & `caluma_alexandria-4.0.0/alexandria/core/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 from django.conf import settings
 from django.core.files import File
 
 from alexandria.core import models
+from alexandria.core.validations import validate_file
 
 log = logging.getLogger(__name__)
 
 
 def create_document_file(
     user: str,
     group: str,
@@ -61,15 +62,15 @@
 ):
     """
     Create a file with defaults and generate a thumbnail.
 
     Use this instead of the normal File.objects.create to ensure that all important fields are set.
     As well as generating a thumbnail for the file.
     """
-    file = models.File.objects.create(
+    file = models.File(
         name=name,
         content=content,
         mime_type=mime_type,
         size=size,
         document=document,
         encryption_status=(
             settings.ALEXANDRIA_ENCRYPTION_METHOD
@@ -78,11 +79,11 @@
         ),
         created_by_user=user,
         created_by_group=group,
         modified_by_user=user,
         modified_by_group=group,
         **additional_attributes,
     )
-
-    file.create_thumbnail()
+    validate_file(file)
+    file.save()
 
     return file
```

### Comparing `caluma_alexandria-3.1.0/alexandria/core/factories.py` & `caluma_alexandria-4.0.0/alexandria/core/factories.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/filters.py` & `caluma_alexandria-4.0.0/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/management/commands/encrypt_files.py` & `caluma_alexandria-4.0.0/alexandria/core/management/commands/encrypt_files.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/management/commands/generate_missing_thumbnails.py` & `caluma_alexandria-4.0.0/alexandria/core/management/commands/generate_missing_thumbnails.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/management/commands/set_mime_type_and_size.py` & `caluma_alexandria-4.0.0/alexandria/core/management/commands/set_mime_type_and_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0007_category_parent.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0007_category_parent.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0010_mark.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0010_mark.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0011_tag_uuid.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0011_tag_uuid.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0012_tag_uuid_schema.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0012_tag_uuid_schema.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0013_file_content.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0013_file_content.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0014_file_mime_type_size.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0014_file_mime_type_size.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0015_fix_modified_by_description.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0015_fix_modified_by_description.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/migrations/0016_category_allowed_mime_types.py` & `caluma_alexandria-4.0.0/alexandria/core/migrations/0016_category_allowed_mime_types.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/models.py` & `caluma_alexandria-4.0.0/alexandria/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,16 +177,14 @@
                 file.write(latest_original.content.file.file.read())
 
                 latest_original.content = DjangoFile(file)
                 latest_original.pk = None
                 latest_original.document = self
                 latest_original.save()
 
-        latest_original.create_thumbnail()
-
         return self
 
 
 class File(UUIDModel):
     class EncryptionStatus(models.TextChoices):
         NOT_ENCRYPTED = "none", "No at-rest enryption"
         SSEC_GLOBAL_KEY = "ssec-global", "SSE-C global key encryption (AES256)"
@@ -237,15 +235,21 @@
         self.checksum = self.make_checksum(self.content.file.file.read())
 
     def save(
         self, force_insert=False, force_update=False, using=None, update_fields=None
     ):
         if settings.ALEXANDRIA_ENABLE_CHECKSUM:
             self.set_checksum()
-        return super().save(force_insert, force_update, using, update_fields)
+
+        file = super().save(force_insert, force_update, using, update_fields)
+
+        if self.variant == File.Variant.ORIGINAL and self.renderings.count() == 0:
+            self.create_thumbnail()
+
+        return file
 
     def get_webdav_url(self, username, group, host="localhost:8000"):
         # The path doesn't need to match the actual file path, because we're accessing
         # the file via the `File.pk`. So we can use just the name, that will then be
         # the last part of the URL
         path = Path(self.name)
         key = Key.from_dictionary({"manabi": {"key": settings.MANABI_SHARED_KEY}})
```

### Comparing `caluma_alexandria-3.1.0/alexandria/core/presign_urls.py` & `caluma_alexandria-4.0.0/alexandria/core/presign_urls.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/serializers.py` & `caluma_alexandria-4.0.0/alexandria/core/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+import json
 import logging
-from mimetypes import guess_type
 
 from django.conf import settings
 from django.template.defaultfilters import slugify
 from django.utils import translation
-from django.utils.translation import gettext as _
-from django_clamd.validators import validate_file_infection
 from generic_permissions.validation import ValidatorMixin
 from generic_permissions.visibilities import (
     VisibilityResourceRelatedField,
     VisibilitySerializerMixin,
 )
-from rest_framework.exceptions import ValidationError
 from rest_framework_json_api import serializers
 
 from . import models
 
 log = logging.getLogger(__name__)
 
 
@@ -214,45 +211,18 @@
 
         # TODO: When next working on file / storage stuff, consider extracting
         # the storage code into it's own project, so we can reuse it outside
         # of Alexandria: https://github.com/projectcaluma/alexandria/issues/480
         if settings.ALEXANDRIA_ENABLE_AT_REST_ENCRYPTION:
             validated_data["encryption_status"] = settings.ALEXANDRIA_ENCRYPTION_METHOD
 
-        mime_type = validated_data["content"].content_type
-        if mime_type == "application/octet-stream":
-            guess, encoding = guess_type(validated_data["name"])
-            if guess is not None:
-                mime_type = guess
-
-        category = models.Document.objects.get(
-            pk=self.initial_data.get("document")["id"]
-        ).category
-        if (
-            category.allowed_mime_types is not None
-            and len(category.allowed_mime_types)
-            and mime_type not in category.allowed_mime_types
-        ):
-            raise ValidationError(
-                _(
-                    "File type %(mime_type)s is not allowed in category %(category)s."
-                    % {"mime_type": mime_type, "category": category.pk}
-                )
-            )
-
-        validated_data["mime_type"] = mime_type
         validated_data["size"] = validated_data["content"].size
 
         return validated_data
 
-    def create(self, validated_data):
-        file = super().create(validated_data)
-        file.create_thumbnail()
-        return file
-
     def _prepare_multipart(self):
         """Massage multipart data into jsonapi-compatible form."""
 
         # Depending on incoming data, the parser converts the request into
         # a dict or an immutable QueryDict. In the latter case, we cannot
         # modify the dict anymore to accomodate the multipart -> jsonapi
         # conversion as needed, thus we need to unlock it.
@@ -272,18 +242,14 @@
         # the storage code into it's own project, so we can reuse it outside
         # of Alexandria: https://github.com/projectcaluma/alexandria/issues/480
 
         if self.context["request"].content_type.startswith("multipart/"):
             self._prepare_multipart()
         return super().is_valid(*args, raise_exception=raise_exception, **kwargs)
 
-    def validate_content(self, value):
-        validate_file_infection(value)
-        return value
-
     class Meta:
         model = models.File
         fields = BaseSerializer.Meta.fields + (
             "variant",
             "name",
             "original",
             "renderings",
@@ -301,28 +267,69 @@
             "mime_type",
             "size",
         )
         extra_kwargs = {"content": {"write_only": True}}
 
 
 class DocumentSerializer(BaseSerializer):
+    category = serializers.ResourceRelatedField(queryset=models.Category.objects)
     files = serializers.ResourceRelatedField(
         queryset=models.File.objects.all(), required=False, many=True
     )
+    content = serializers.FileField(write_only=True, required=True)
+
     included_serializers = {
         "category": CategorySerializer,
         "tags": TagSerializer,
         "marks": MarkSerializer,
         "files": FileSerializer,
     }
 
+    def create(self, validated_data):
+        content = validated_data.pop("content")
+        document = super().create(validated_data)
+
+        file_data = {
+            "name": content.name,
+            "document": {
+                "type": "documents",
+                "id": document.pk,
+            },
+            "content": content,
+        }
+        file_serializer = FileSerializer(data=file_data, context=self.context)
+        file_serializer.is_valid(raise_exception=True)
+        file_serializer.save()
+
+        return document
+
+    def _prepare_multipart(self):
+        """Massage multipart data into jsonapi-compatible form."""
+        self.initial_data = self.initial_data.dict()
+
+        self.initial_data.update(
+            json.loads(self.initial_data["data"].read().decode("utf-8"))
+        )
+        if not isinstance(self.initial_data.get("category"), dict):
+            self.initial_data["category"] = {
+                "type": "categories",
+                "id": self.initial_data["category"],
+            }
+
+    def is_valid(self, *args, raise_exception=False, **kwargs):
+        if self.context["request"].content_type.startswith("multipart/"):
+            self._prepare_multipart()
+        return super().is_valid(*args, raise_exception=raise_exception, **kwargs)
+
     class Meta:
         model = models.Document
         fields = BaseSerializer.Meta.fields + (
             "files",
             "title",
             "description",
             "date",
             "category",
             "tags",
             "marks",
+            "content",
         )
+        extra_kwargs = {"content": {"write_only": True}}
```

### Comparing `caluma_alexandria-3.1.0/alexandria/core/views.py` & `caluma_alexandria-4.0.0/alexandria/core/views.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/core/visibilities.py` & `caluma_alexandria-4.0.0/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/dav.py` & `caluma_alexandria-4.0.0/alexandria/dav.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/dav_provider.py` & `caluma_alexandria-4.0.0/alexandria/dav_provider.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-4.0.0/alexandria/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/oidc_auth/models.py` & `caluma_alexandria-4.0.0/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/settings/alexandria.py` & `caluma_alexandria-4.0.0/alexandria/settings/alexandria.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,18 @@
     "ALEXANDRIA_VISIBILITY_CLASSES",
     default=default(["generic_permissions.visibilities.Any"], []),
 )
 ALEXANDRIA_PERMISSION_CLASSES = env.list(
     "ALEXANDRIA_PERMISSION_CLASSES",
     default=default(["generic_permissions.permissions.AllowAny"], []),
 )
-ALEXANDRIA_VALIDATION_CLASSES = env.list("ALEXANDRIA_VALIDATION_CLASSES", default=[])
+ALEXANDRIA_VALIDATION_CLASSES = env.list(
+    "ALEXANDRIA_VALIDATION_CLASSES",
+    default=["alexandria.core.validations.AlexandriaValidator"],
+)
 
 # We use DGAP as a permission/visibility/validation handler. Copy
 # the configuration over so DGAP knows
 GENERIC_PERMISSIONS_VISIBILITY_CLASSES = ALEXANDRIA_VISIBILITY_CLASSES
 GENERIC_PERMISSIONS_PERMISSION_CLASSES = ALEXANDRIA_PERMISSION_CLASSES
 GENERIC_PERMISSIONS_VALIDATION_CLASSES = ALEXANDRIA_VALIDATION_CLASSES
```

### Comparing `caluma_alexandria-3.1.0/alexandria/settings/django.py` & `caluma_alexandria-4.0.0/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/storages/backends/s3.py` & `caluma_alexandria-4.0.0/alexandria/storages/backends/s3.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/storages/fields.py` & `caluma_alexandria-4.0.0/alexandria/storages/fields.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/alexandria/wsgi.py` & `caluma_alexandria-4.0.0/alexandria/wsgi.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-3.1.0/pyproject.toml` & `caluma_alexandria-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "3.1.0"
+version = "4.0.0"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -52,25 +52,25 @@
 flake8-tuple = "0.4.1"
 gitlint = "0.19.1"
 isort = "5.13.2"
 pdbpp = "0.10.3"
 pillow = "^10.1.0"
 pre-commit = "3.5.0"
 pytest = "8.1.1"
-pytest-cov = "4.1.0"
+pytest-cov = "5.0.0"
 pytest-django = "4.8.0"
 pytest-env = "1.1.3"
 pytest-factoryboy = "2.7.0"
 pytest-freezegun = "0.4.2"
-pytest-mock = "3.12.0"
+pytest-mock = "3.14.0"
 pytest-randomly = "3.15.0"
 python-semantic-release = "7.33.3"
-requests-mock = "1.11.0"
+requests-mock = "1.12.1"
 syrupy = "4.6.1"
-werkzeug = "3.0.1"
+werkzeug = "3.0.2"
 moto = {extras = ["s3"], version = "^5.0.2"}
 webtest = "^3.0.0"
 
 [tool.isort]
 skip = ["migrations"]
 known_first_party = ["alexandria"]
 multi_line_output = 3
```

### Comparing `caluma_alexandria-3.1.0/PKG-INFO` & `caluma_alexandria-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 3.1.0
+Version: 4.0.0
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -113,15 +113,15 @@
   - `ALEXANDRIA_OIDC_USER_FACTORY`: Overwrite the default user with your own
   - `ALEXANDRIA_CREATED_BY_USER_PROPERTY`: Overwrite the default user property which is used for `..._by_user` (default: username)
   - `ALEXANDRIA_CREATED_BY_GROUP_PROPERTY`: Overwrite the default group property which is used for `..._by_group` (default: group)
 - Authorization configurations
   - `ALEXANDRIA_VISIBILITY_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#visibilities) classes that define visibility for all models
   - `ALEXANDRIA_PERMISSION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#permissions) classes that define permissions for all models
 - Data validation configuration
-  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations
+  - `ALEXANDRIA_VALIDATION_CLASSES`: Comma-separated list of [DGAP](https://github.com/adfinis/django-generic-api-permissions/?tab=readme-ov-file#data-validation) classes that define custom validations. A default base class is used for file validation. Extend `AlexandriaValidator` for own validations.
 - Thumbnail configuration (optional)
 
   - `ALEXANDRIA_ENABLE_THUMBNAIL_GENERATION`: Set to `false` to disable thumbnail generation
     - Check the docker-compose file for an example on how to set up generation with s3 hooks
   - `ALEXANDRIA_THUMBNAIL_WIDTH`: Width of generated thumbnails
   - `ALEXANDRIA_THUMBNAIL_HEIGHT`: Height of generated thumbnails
   - `ALEXANDRIA_ENABLE_CHECKSUM`: Set to `false` to disable file checksums. Checksums are calculated after upload to allow later verification (not implemented in Alexandria)
```

