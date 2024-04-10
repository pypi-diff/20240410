# Comparing `tmp/spid_cie_oidc-1.4.3.tar.gz` & `tmp/spid_cie_oidc-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spid_cie_oidc-1.4.3.tar", last modified: Fri Mar 22 08:42:59 2024, max compression
+gzip compressed data, was "spid_cie_oidc-1.4.4.tar", last modified: Wed Apr 10 09:09:45 2024, max compression
```

## Comparing `spid_cie_oidc-1.4.3.tar` & `spid_cie_oidc-1.4.4.tar`

### file list

```diff
@@ -1,384 +1,384 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.271850 spid_cie_oidc-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 08:42:59.271850 spid_cie_oidc-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.211850 spid_cie_oidc-1.4.3/spid_cie_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.215850 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/admin_inlines.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.215850 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.215850 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/templatetags/has_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.215850 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.219850 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0006_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0012_remove_federationdescendant_issue_x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0013_alter_federationdescendant_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.219850 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.219850 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13732 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_05_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_08_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-22 08:42:52.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/authority/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.223850 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/abstract_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/jwtse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.231850 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0019_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0023_alter_federationhistoricalkey_jwk.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0024_alter_federationhistoricalkey_kid.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0025_alter_federationhistoricalkey_jwk.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0026_alter_federationhistoricalkey_jwk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0030_remove_federationentityconfiguration_issue_x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0031_alter_federationentityconfiguration_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0032_alter_fetchedentitystatement_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15432 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.231850 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/resolve_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.235850 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/fa_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/jwks_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/op_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/rp_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_01_op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_03_jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_05_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_06_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_07_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_08_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_09_trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_10_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/trust_chain_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/entity/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.235850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.239850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0010_alter_onboardingregistration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.207850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.239850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/images/logo-it.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.239850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_entities.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_landing.html
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.239850 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_02_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_11_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/tools_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.243850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.243850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.243850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.243850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0008_alter_oidcsession_authz_request.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/authn_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/authn_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/client_assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/token_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.207850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/css/provider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)   196297 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/images/logo-cie.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/logo-cie.svg
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/no_image_available.svg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg-LTS.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_consent.html
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_history.html
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.247850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templatetags/spid_cie_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.255850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/authn_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/authn_responses_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/introspection_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/introspection_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/revocation_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/revocation_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_03_authn_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_03_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_04_authn_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_05_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_06_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_06_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_07_introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_08_introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_09_revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_10_no_consent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_10_revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_11_user_access_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_12_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/token_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/token_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.255850 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/authz_request_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/consent_page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/userinfo_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.255850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.255850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.211850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/css/access-button.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/js/spid_button.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb-LTS.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.259850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/echo_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_base.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_introspection.html
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_landing.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.263850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/mocked_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.263850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_extend_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_landing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.211850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/static/images/oops.webp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-22 08:42:53.000000 spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:42:59.267850 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-22 08:42:59.000000 spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.412739 spid_cie_oidc-1.4.4/spid_cie_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.412739 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/admin_inlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.416739 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.416739 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/templatetags/has_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.416739 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.420739 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0006_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0012_remove_federationdescendant_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0013_alter_federationdescendant_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.420739 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.420739 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_05_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_08_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/authority/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.424739 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/abstract_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/jwtse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.432739 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0019_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0023_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0024_alter_federationhistoricalkey_kid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0025_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0026_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0030_remove_federationentityconfiguration_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0031_alter_federationentityconfiguration_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0032_alter_fetchedentitystatement_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15432 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.432739 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/resolve_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.436740 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/fa_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/jwks_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/op_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/rp_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_01_op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_03_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_05_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_06_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_07_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_08_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_09_trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_10_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/trust_chain_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/entity/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.436740 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.440739 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0010_alter_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.408739 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.440739 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/images/logo-it.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.444739 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_entities.html
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_landing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.444739 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_02_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_11_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/tools_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.444739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.444739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.444739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.448739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0008_alter_oidcsession_authz_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.448739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/authn_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/client_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/token_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.408739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.448739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/css/provider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.448739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   196297 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/images/logo-cie.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.452740 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/logo-cie.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/no_image_available.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg-LTS.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.452740 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_consent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_history.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.452740 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templatetags/spid_cie_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.456740 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/authn_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/authn_responses_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/introspection_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/introspection_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/revocation_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/revocation_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_03_authn_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_03_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_04_authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_05_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_06_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_06_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_07_introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_08_introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_09_revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_10_no_consent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_10_revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_11_user_access_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_12_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/token_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/token_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/authz_request_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/consent_page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/userinfo_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.460739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.464740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.412739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.464740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/css/access-button.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.464740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/js/spid_button.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.464740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb-LTS.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.464740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/echo_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_introspection.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_landing.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/mocked_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_extend_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_landing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.412739 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.468740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/static/images/oops.webp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-10 09:09:36.000000 spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:09:45.472740 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 09:09:45.000000 spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/top_level.txt
```

### Comparing `spid_cie_oidc-1.4.3/LICENSE` & `spid_cie_oidc-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/PKG-INFO` & `spid_cie_oidc-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spid_cie_oidc
-Version: 1.4.3
+Version: 1.4.4
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `spid_cie_oidc-1.4.3/README.md` & `spid_cie_oidc-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/setup.py` & `spid_cie_oidc-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/accounts/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/accounts/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0006_stafftoken.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0006_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/migrations/0013_alter_federationdescendant_type_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/migrations/0013_alter_federationdescendant_type_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/mocked_responses.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/mocked_responses.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,18 @@
         tc_ser = trust_chain.serialize()
         _p0 = unpad_jwt_payload(tc_ser[0])
         _p1 = unpad_jwt_payload(tc_ser[1])
         _p2 = unpad_jwt_payload(tc_ser[2])
         _p3 = unpad_jwt_payload(tc_ser[3])
 
         self.assertEqual(_p0['iss'], _p0['sub'])
+        self.assertEqual(_p0['iss'], _p1['sub'])
         self.assertNotEqual(_p2['iss'], _p1['sub'])
         self.assertNotEqual(_p2['iss'], _p2['sub'])
+        self.assertEqual(_p3['sub'], _p2['iss'])
         self.assertEqual(_p3['iss'], _p3['sub'])
         
         dumps = dumps_statements_from_trust_chain_to_db(trust_chain)
 
         self.assertTrue(isinstance(dumps, list) and len(dumps) == 5)
 
         self.assertTrue("sub" in dumps[0].get_entity_configuration_as_obj().payload)
```

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_05_validators.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_05_validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/tests/test_08_schemas.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/tests/test_08_schemas.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/urls.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/validators.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/authority/views.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/authority/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/abstract_models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/abstract_models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/exceptions.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/exceptions.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/http_client.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/http_client.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/jwks.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/jwtse.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/jwtse.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0019_stafftoken.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0019_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/migrations/0031_alter_federationentityconfiguration_entity_type.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/migrations/0031_alter_federationentityconfiguration_entity_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/policy.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/policy.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/jwks.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/op_metadata.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/op_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/resolve_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/resolve_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/schemas/rp_metadata.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/schemas/rp_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/statements.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/statements.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/jwks_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/jwks_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/op_metadata_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/op_metadata_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/rp_metadata_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/rp_metadata_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_01_entity_configuration.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_01_entity_configuration.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_01_op_metadata.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_01_op_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_02_rp_metadata.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_02_rp_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_03_jwks.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_03_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_05_policy.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_05_policy.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_07_validators.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_07_validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_08_statements.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_08_statements.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/tests/test_09_trust_chain.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/tests/test_09_trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/trust_chain.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/trust_chain_operations.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/trust_chain_operations.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/urls.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/utils.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/utils.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/validators.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/views.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/entity/x509.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/entity/x509.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/forms.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/migrations/0010_alter_onboardingregistration_type.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/migrations/0010_alter_onboardingregistration_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/static/images/logo-it.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/static/images/logo-it.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/base.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_entities.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_entities.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_jwk.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_landing.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_landing.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_registration.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_registration.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_schemas.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_schemas.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_01_onboarding.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_01_onboarding.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_02_tools.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_02_tools.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/test_11_admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/test_11_admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/tests/tools_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/tests/tools_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/urls.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/onboarding/views.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/onboarding/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/forms.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/authn_requests.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/authn_requests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/authn_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/client_assertion.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/client_assertion.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/introspection_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/jwt.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/jwt.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/token_requests.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/token_requests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/schemas/token_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/schemas/token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/css/provider.css` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/css/provider.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/images/logo-cie.png` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/images/logo-cie.png`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/logo-cie.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/logo-cie.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg-LTS.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg-LTS.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_base.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_consent.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_consent.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_history.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_history.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templates/op_user_login.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templates/op_user_login.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/templatetags/spid_cie_op.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/templatetags/spid_cie_op.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/authn_request_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/authn_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/authn_responses_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/authn_responses_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/introspection_request_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/introspection_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/introspection_response_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/introspection_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/revocation_request_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/revocation_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/revocation_response_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/revocation_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_03_authn_request.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_03_authn_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_03_refresh_token.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_03_refresh_token.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_04_authn_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_04_authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_05_token_request.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_05_token_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_06_token_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_06_token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_07_introspection_request.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_07_introspection_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_08_introspection_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_08_introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_08_token_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_08_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_09_revocation_request.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_09_revocation_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_10_no_consent.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_10_no_consent.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_10_revocation_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_10_revocation_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_11_user_access_history.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_11_user_access_history.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/test_12_init.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/test_12_init.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/token_request_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/token_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/tests/token_response_settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/tests/token_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/urls.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/__init__.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/authz_request_view.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/authz_request_view.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/connect.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/connect.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/consent_page_view.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/consent_page_view.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/introspection_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/introspection_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/revocation_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/token_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/provider/views/userinfo_endpoint.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/provider/views/userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oauth2/__init__.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/oidc/__init__.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/settings.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/css/access-button.css` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/css/access-button.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/js/spid_button.js` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/js/spid_button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb-LTS.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb-LTS.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/favicon.ico` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/favicon.ico`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/echo_attributes.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_base.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_error.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_error.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_introspection.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_introspection.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/templates/rp_landing.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/templates/rp_landing.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/mocked_response.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/mocked_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/tests/test_09_rp_model.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/tests/test_09_rp_model.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/urls.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/urls.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/utils.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/utils.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/__init__.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                 "iss": authz.client_id,
                 "sub": authz.client_id,
                 "aud": [audience],
                 "iat": iat_now(),
                 "exp": exp_from_now(),
                 "jti": str(uuid.uuid4())
             },
-            jwk_dict=get_key(rp_conf)
+            jwk_dict = get_key(rp_conf.jwks_core)
         )
         token_request_data["client_assertion"] = client_assertion
 
         try:
             token_request = requests.post(
                 audience,
                 data=token_request_data,
```

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_begin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_begin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_callback.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_callback.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_extend_session.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_extend_session.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_initiated_logout.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_introspection.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_introspection.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party/views/rp_landing.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party/views/rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/admin.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/forms.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/0001_initial.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/models.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/README.md` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/README.md`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/crawler.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/crawler.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/static/images/oops.webp` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/static/images/oops.webp`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc/relying_party_test/views.py` & `spid_cie_oidc-1.4.4/spid_cie_oidc/relying_party_test/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/PKG-INFO` & `spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spid_cie_oidc
-Version: 1.4.3
+Version: 1.4.4
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `spid_cie_oidc-1.4.3/spid_cie_oidc.egg-info/SOURCES.txt` & `spid_cie_oidc-1.4.4/spid_cie_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

