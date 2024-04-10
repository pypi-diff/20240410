# Comparing `tmp/django_esi-5.2.0.tar.gz` & `tmp/django_esi-5.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_esi-5.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_esi-5.3.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_esi-5.2.0.tar` & `django_esi-5.3.0b1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    35141 2024-03-16 03:42:03.524487 django_esi-5.2.0/LICENSE
--rw-r--r--   0        0        0     2591 2024-03-16 03:42:03.524487 django_esi-5.2.0/README.md
--rw-r--r--   0        0        0      155 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/__init__.py
--rw-r--r--   0        0        0     1100 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/admin.py
--rw-r--r--   0        0        0     3788 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/app_settings.py
--rw-r--r--   0        0        0      272 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/apps.py
--rw-r--r--   0        0        0     1154 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/checks.py
--rw-r--r--   0        0        0    21303 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/clients.py
--rw-r--r--   0        0        0     8081 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/decorators.py
--rw-r--r--   0        0        0      308 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/errors.py
--rw-r--r--   0        0        0      820 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1503 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1305 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      737 2024-03-16 03:42:03.526487 django_esi-5.2.0/esi/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1504 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      643 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1357 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      877 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1560 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      707 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1476 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      746 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1511 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      915 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1703 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      681 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1451 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-03-16 03:42:03.576486 django_esi-5.2.0/esi/management/commands/__init__.py
--rw-r--r--   0        0        0     6427 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/management/commands/migrate_to_ssov2.py
--rw-r--r--   0        0        0    11144 2024-03-16 03:42:03.527487 django_esi-5.2.0/esi/managers.py
--rw-r--r--   0        0        0     3396 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0001_initial.py
--rw-r--r--   0        0        0     2846 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0002_scopes_20161208.py
--rw-r--r--   0        0        0      734 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0003_hide_tokens_from_admin_site.py
--rw-r--r--   0        0        0      460 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0004_remove_unique_access_token.py
--rw-r--r--   0        0        0      676 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0005_remove_token_length_limit.py
--rw-r--r--   0        0        0      459 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0006_remove_url_length_limit.py
--rw-r--r--   0        0        0      460 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0007_fix_mysql_8_migration.py
--rw-r--r--   0        0        0      477 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0008_nullable_refresh_token.py
--rw-r--r--   0        0        0      417 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0009_set_old_tokens_to_sso_v1.py
--rw-r--r--   0        0        0      421 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0010_set_new_tokens_to_sso_v2.py
--rw-r--r--   0        0        0     1016 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0011_add_token_indices.py
--rw-r--r--   0        0        0      525 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/migrations/0012_fix_token_type_choices.py
--rw-r--r--   0        0        0        0 2024-03-16 03:42:03.576486 django_esi-5.2.0/esi/migrations/__init__.py
--rw-r--r--   0        0        0    11412 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/models.py
--rw-r--r--   0        0        0     2308 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_Black.png
--rw-r--r--   0        0        0     2248 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_White.png
--rw-r--r--   0        0        0     1622 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_Black.png
--rw-r--r--   0        0        0     1546 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_White.png
--rw-r--r--   0        0        0     1516 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/tasks.py
--rw-r--r--   0        0        0     6905 2024-03-16 03:42:03.528487 django_esi-5.2.0/esi/templates/esi/select_token.html
--rw-r--r--   0        0        0        0 2024-03-16 03:42:03.576486 django_esi-5.2.0/esi/templatetags/__init__.py
--rw-r--r--   0        0        0      167 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/templatetags/scope_tags.py
--rw-r--r--   0        0        0     3092 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/__init__.py
--rw-r--r--   0        0        0     1622 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/client_authed_pilot.py
--rw-r--r--   0        0        0     1252 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/client_public_pilot.py
--rw-r--r--   0        0        0     1368 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/factories.py
--rw-r--r--   0        0        0     1972 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/factories_2.py
--rw-r--r--   0        0        0     4944 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/jwt_factory.py
--rw-r--r--   0        0        0     1846 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_checks.py
--rw-r--r--   0        0        0    36037 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_clients.py
--rw-r--r--   0        0        0    15069 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_decorators.py
--rw-r--r--   0        0        0     9863 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_management_command.py
--rw-r--r--   0        0        0    24548 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_managers.py
--rw-r--r--   0        0        0    13748 2024-03-16 03:42:03.529487 django_esi-5.2.0/esi/tests/test_models.py
--rw-r--r--   0        0        0    17241 2024-03-16 03:42:03.530487 django_esi-5.2.0/esi/tests/test_swagger.json
--rw-r--r--   0        0        0  2548369 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/tests/test_swagger_full.json
--rw-r--r--   0        0        0     2104 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/tests/test_tasks.py
--rw-r--r--   0        0        0      517 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/tests/test_templatetags.py
--rw-r--r--   0        0        0    13073 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/tests/test_views.py
--rw-r--r--   0        0        0     1931 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/tests/threading_pilot.py
--rw-r--r--   0        0        0      161 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/urls.py
--rw-r--r--   0        0        0     3916 2024-03-16 03:42:03.538487 django_esi-5.2.0/esi/views.py
--rw-r--r--   0        0        0     1580 2024-03-16 03:42:03.538487 django_esi-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 django_esi-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-04-10 02:06:37.563369 django_esi-5.3.0b1/LICENSE
+-rw-r--r--   0        0        0     2591 2024-04-10 02:06:37.563369 django_esi-5.3.0b1/README.md
+-rw-r--r--   0        0        0      157 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/__init__.py
+-rw-r--r--   0        0        0     1100 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/admin.py
+-rw-r--r--   0        0        0     3783 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/app_settings.py
+-rw-r--r--   0        0        0      272 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/apps.py
+-rw-r--r--   0        0        0     1154 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/checks.py
+-rw-r--r--   0        0        0    21303 2024-04-10 02:06:37.564369 django_esi-5.3.0b1/esi/clients.py
+-rw-r--r--   0        0        0     8081 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/decorators.py
+-rw-r--r--   0        0        0      308 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/errors.py
+-rw-r--r--   0        0        0      820 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1503 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1305 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      737 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1504 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      643 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1357 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      877 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1560 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      707 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1476 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      746 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1511 2024-04-10 02:06:37.565369 django_esi-5.3.0b1/esi/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      915 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1703 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      681 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1451 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-10 02:06:37.613368 django_esi-5.3.0b1/esi/management/commands/__init__.py
+-rw-r--r--   0        0        0     6427 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/management/commands/migrate_to_ssov2.py
+-rw-r--r--   0        0        0    11455 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/managers.py
+-rw-r--r--   0        0        0     3396 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2846 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0002_scopes_20161208.py
+-rw-r--r--   0        0        0      734 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0003_hide_tokens_from_admin_site.py
+-rw-r--r--   0        0        0      460 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0004_remove_unique_access_token.py
+-rw-r--r--   0        0        0      676 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0005_remove_token_length_limit.py
+-rw-r--r--   0        0        0      459 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0006_remove_url_length_limit.py
+-rw-r--r--   0        0        0      460 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0007_fix_mysql_8_migration.py
+-rw-r--r--   0        0        0      477 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0008_nullable_refresh_token.py
+-rw-r--r--   0        0        0      417 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0009_set_old_tokens_to_sso_v1.py
+-rw-r--r--   0        0        0      421 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0010_set_new_tokens_to_sso_v2.py
+-rw-r--r--   0        0        0     1016 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0011_add_token_indices.py
+-rw-r--r--   0        0        0      525 2024-04-10 02:06:37.566369 django_esi-5.3.0b1/esi/migrations/0012_fix_token_type_choices.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:06:37.613368 django_esi-5.3.0b1/esi/migrations/__init__.py
+-rw-r--r--   0        0        0    11412 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/models.py
+-rw-r--r--   0        0        0     2308 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_Black.png
+-rw-r--r--   0        0        0     2248 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_White.png
+-rw-r--r--   0        0        0     1622 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_Black.png
+-rw-r--r--   0        0        0     1546 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_White.png
+-rw-r--r--   0        0        0     1516 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tasks.py
+-rw-r--r--   0        0        0     6905 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/templates/esi/select_token.html
+-rw-r--r--   0        0        0        0 2024-04-10 02:06:37.613368 django_esi-5.3.0b1/esi/templatetags/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/templatetags/scope_tags.py
+-rw-r--r--   0        0        0     3092 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/client_authed_pilot.py
+-rw-r--r--   0        0        0     1252 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/client_public_pilot.py
+-rw-r--r--   0        0        0     1368 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/factories.py
+-rw-r--r--   0        0        0     1972 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/factories_2.py
+-rw-r--r--   0        0        0     4944 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/jwt_factory.py
+-rw-r--r--   0        0        0     1846 2024-04-10 02:06:37.567369 django_esi-5.3.0b1/esi/tests/test_checks.py
+-rw-r--r--   0        0        0    36037 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_clients.py
+-rw-r--r--   0        0        0    15069 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_decorators.py
+-rw-r--r--   0        0        0     9863 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_management_command.py
+-rw-r--r--   0        0        0    24548 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_managers.py
+-rw-r--r--   0        0        0    13748 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_models.py
+-rw-r--r--   0        0        0    17241 2024-04-10 02:06:37.568369 django_esi-5.3.0b1/esi/tests/test_swagger.json
+-rw-r--r--   0        0        0  2548369 2024-04-10 02:06:37.576368 django_esi-5.3.0b1/esi/tests/test_swagger_full.json
+-rw-r--r--   0        0        0     2104 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/tests/test_tasks.py
+-rw-r--r--   0        0        0      517 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/tests/test_templatetags.py
+-rw-r--r--   0        0        0    13073 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/tests/test_views.py
+-rw-r--r--   0        0        0     1931 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/tests/threading_pilot.py
+-rw-r--r--   0        0        0      161 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/urls.py
+-rw-r--r--   0        0        0     3916 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/esi/views.py
+-rw-r--r--   0        0        0     1580 2024-04-10 02:06:37.577368 django_esi-5.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 django_esi-5.3.0b1/PKG-INFO
```

### Comparing `django_esi-5.2.0/LICENSE` & `django_esi-5.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/README.md` & `django_esi-5.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/admin.py` & `django_esi-5.3.0b1/esi/admin.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/app_settings.py` & `django_esi-5.3.0b1/esi/app_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ESI_INFO_LOGGING_ENABLED = getattr(settings, 'ESI_INFO_LOGGING_ENABLED', False)
 """Enable/disable verbose info logging."""
 
 ESI_LOG_LEVEL_LIBRARIES = str(getattr(settings, 'ESI_LOG_LEVEL_LIBRARIES', 'INFO'))
 """Set log level for libraries like bravado and urlib3."""
 
-ESI_DEBUG_RESPONSE_CONTENT_LOGGING = str(getattr(settings, 'ESI_DEBUG_RESPONSE_CONTENT_LOGGING', True))
+ESI_DEBUG_RESPONSE_CONTENT_LOGGING = getattr(settings, 'ESI_DEBUG_RESPONSE_CONTENT_LOGGING', True)
 """Enable/Disable logging of ESI response contents."""
 
 ESI_USER_CONTACT_EMAIL = getattr(settings, 'ESI_USER_CONTACT_EMAIL', None)
 """Contact email address of server owner.
 
 This will be included in the User-Agent header of every request.
 """
```

### Comparing `django_esi-5.2.0/esi/checks.py` & `django_esi-5.3.0b1/esi/checks.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/clients.py` & `django_esi-5.3.0b1/esi/clients.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/decorators.py` & `django_esi-5.3.0b1/esi/decorators.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/de/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/de/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/en/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/es/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/es/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/fr_FR/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/fr_FR/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/it_IT/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/it_IT/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ja/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ja/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ko_KR/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ko_KR/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ru/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/ru/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_esi-5.3.0b1/esi/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/locale/zh_Hans/LC_MESSAGES/django.po` & `django_esi-5.3.0b1/esi/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/management/commands/migrate_to_ssov2.py` & `django_esi-5.3.0b1/esi/management/commands/migrate_to_ssov2.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/managers.py` & `django_esi-5.3.0b1/esi/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,17 +72,33 @@
 
         Deletes those which fail to refresh or cannot be refreshed.
 
         Returns:
             All tokens which are still valid.
         """
         expired = self.get_expired()
-        valid = self.exclude(pk__in=expired)
-        valid_expired = expired.bulk_refresh()
-        return valid_expired | valid
+        valid = list(
+            self.exclude(
+                pk__in=expired
+            ).values_list(
+                "pk",
+                flat=True
+            )
+        )
+        valid_expired = list(
+            expired.bulk_refresh(
+            ).values_list(
+                "pk",
+                flat=True
+            )
+        )
+        _qs = self.filter(
+            pk__in=(valid + valid_expired)
+        )
+        return _qs
 
     def require_scopes(self, scope_string: Union[str, list]) -> models.QuerySet:
         """Filter tokens which have at least a subset of given scopes.
 
         Args:
             scope_string: The required scopes.
```

### Comparing `django_esi-5.2.0/esi/migrations/0001_initial.py` & `django_esi-5.3.0b1/esi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/migrations/0002_scopes_20161208.py` & `django_esi-5.3.0b1/esi/migrations/0002_scopes_20161208.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/migrations/0003_hide_tokens_from_admin_site.py` & `django_esi-5.3.0b1/esi/migrations/0003_hide_tokens_from_admin_site.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/migrations/0005_remove_token_length_limit.py` & `django_esi-5.3.0b1/esi/migrations/0005_remove_token_length_limit.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/migrations/0011_add_token_indices.py` & `django_esi-5.3.0b1/esi/migrations/0011_add_token_indices.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/migrations/0012_fix_token_type_choices.py` & `django_esi-5.3.0b1/esi/migrations/0012_fix_token_type_choices.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/models.py` & `django_esi-5.3.0b1/esi/models.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_Black.png` & `django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_Black.png`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_White.png` & `django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Large_White.png`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_Black.png` & `django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_Black.png`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_White.png` & `django_esi-5.3.0b1/esi/static/esi/img/EVE_SSO_Login_Buttons_Small_White.png`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tasks.py` & `django_esi-5.3.0b1/esi/tasks.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/templates/esi/select_token.html` & `django_esi-5.3.0b1/esi/templates/esi/select_token.html`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/__init__.py` & `django_esi-5.3.0b1/esi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/client_authed_pilot.py` & `django_esi-5.3.0b1/esi/tests/client_authed_pilot.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/client_public_pilot.py` & `django_esi-5.3.0b1/esi/tests/client_public_pilot.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/factories.py` & `django_esi-5.3.0b1/esi/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/factories_2.py` & `django_esi-5.3.0b1/esi/tests/factories_2.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/jwt_factory.py` & `django_esi-5.3.0b1/esi/tests/jwt_factory.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_checks.py` & `django_esi-5.3.0b1/esi/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_clients.py` & `django_esi-5.3.0b1/esi/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_decorators.py` & `django_esi-5.3.0b1/esi/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_management_command.py` & `django_esi-5.3.0b1/esi/tests/test_management_command.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_managers.py` & `django_esi-5.3.0b1/esi/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_models.py` & `django_esi-5.3.0b1/esi/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_swagger.json` & `django_esi-5.3.0b1/esi/tests/test_swagger.json`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_swagger_full.json` & `django_esi-5.3.0b1/esi/tests/test_swagger_full.json`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_tasks.py` & `django_esi-5.3.0b1/esi/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_templatetags.py` & `django_esi-5.3.0b1/esi/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/test_views.py` & `django_esi-5.3.0b1/esi/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/tests/threading_pilot.py` & `django_esi-5.3.0b1/esi/tests/threading_pilot.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/esi/views.py` & `django_esi-5.3.0b1/esi/views.py`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/pyproject.toml` & `django_esi-5.3.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_esi-5.2.0/PKG-INFO` & `django_esi-5.3.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-esi
-Version: 5.2.0
+Version: 5.3.0b1
 Summary: Django app for accessing the EVE Swagger Interface (ESI).
 Author-email: Alliance Auth <adarnof@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

