# Comparing `tmp/hdn-research-environment-3.0.5.tar.gz` & `tmp/hdn-research-environment-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdn-research-environment-3.0.5.tar", last modified: Thu Apr  4 13:19:56 2024, max compression
+gzip compressed data, was "hdn-research-environment-3.0.6.tar", last modified: Tue Apr  9 13:29:59 2024, max compression
```

## Comparing `hdn-research-environment-3.0.5.tar` & `hdn-research-environment-3.0.6.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.742180 hdn-research-environment-3.0.5/
--rw-r--r--   0 rafal      (501) staff       (20)     1551 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/LICENSE
--rw-r--r--   0 rafal      (501) staff       (20)      115 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/MANIFEST.in
--rw-r--r--   0 rafal      (501) staff       (20)      978 2024-04-04 13:19:56.742282 hdn-research-environment-3.0.5/PKG-INFO
--rw-r--r--   0 rafal      (501) staff       (20)      229 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/README.md
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.720022 hdn-research-environment-3.0.5/environment/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/__init__.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.724019 hdn-research-environment-3.0.5/environment/api/
--rw-r--r--   0 rafal      (501) staff       (20)     8203 2024-03-26 11:53:16.000000 hdn-research-environment-3.0.5/environment/api/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)      939 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/api/decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)      154 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/apps.py
--rw-r--r--   0 rafal      (501) staff       (20)     3074 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/constants.py
--rw-r--r--   0 rafal      (501) staff       (20)     1546 2024-02-16 14:02:50.000000 hdn-research-environment-3.0.5/environment/decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)     5362 2024-02-29 13:11:14.000000 hdn-research-environment-3.0.5/environment/deserializers.py
--rw-r--r--   0 rafal      (501) staff       (20)     4404 2024-04-04 13:19:22.000000 hdn-research-environment-3.0.5/environment/entities.py
--rw-r--r--   0 rafal      (501) staff       (20)     1421 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.5/environment/exceptions.py
--rw-r--r--   0 rafal      (501) staff       (20)     7674 2024-04-04 13:19:22.000000 hdn-research-environment-3.0.5/environment/forms.py
--rw-r--r--   0 rafal      (501) staff       (20)     2518 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/mailers.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.727265 hdn-research-environment-3.0.5/environment/migrations/
--rw-r--r--   0 rafal      (501) staff       (20)     2174 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/migrations/00012_bucketsharinginvite.py
--rw-r--r--   0 rafal      (501) staff       (20)     1443 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0001_initial.py
--rw-r--r--   0 rafal      (501) staff       (20)     1579 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 rafal      (501) staff       (20)      403 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.5/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.5/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 rafal      (501) staff       (20)     2220 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0005_workflow.py
--rw-r--r--   0 rafal      (501) staff       (20)      394 2023-05-26 09:35:04.000000 hdn-research-environment-3.0.5/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 rafal      (501) staff       (20)     2348 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 rafal      (501) staff       (20)      476 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.5/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.5/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 rafal      (501) staff       (20)     1364 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 rafal      (501) staff       (20)      858 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/migrations/0011_refactor_workflow.py
--rw-r--r--   0 rafal      (501) staff       (20)     1042 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.5/environment/migrations/0013_bucketsharinginvite_type_and_more.py
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/migrations/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)     2423 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.5/environment/models.py
--rw-r--r--   0 rafal      (501) staff       (20)    25434 2024-03-11 11:52:51.000000 hdn-research-environment-3.0.5/environment/services.py
--rw-r--r--   0 rafal      (501) staff       (20)     4519 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/signals.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.710978 hdn-research-environment-3.0.5/environment/static/
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.727353 hdn-research-environment-3.0.5/environment/static/environment/
--rw-r--r--   0 rafal      (501) staff       (20)     6148 2023-02-02 14:12:52.000000 hdn-research-environment-3.0.5/environment/static/environment/.DS_Store
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.728742 hdn-research-environment-3.0.5/environment/static/environment/css/
--rw-r--r--   0 rafal      (501) staff       (20)    11789 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/static/environment/css/bucket_files_dropzone.css
--rw-r--r--   0 rafal      (501) staff       (20)      342 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/static/environment/css/creation_form.css
--rw-r--r--   0 rafal      (501) staff       (20)     6583 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/static/environment/css/environment-base.css
--rw-r--r--   0 rafal      (501) staff       (20)      117 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.5/environment/static/environment/css/management_views.css
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.730559 hdn-research-environment-3.0.5/environment/static/environment/js/
--rw-r--r--   0 rafal      (501) staff       (20)   114702 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/static/environment/js/bucket_files_dropzone.min.js
--rw-r--r--   0 rafal      (501) staff       (20)      564 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/static/environment/js/cookie.js
--rw-r--r--   0 rafal      (501) staff       (20)      199 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/static/environment/js/destroy_shared_bucket.js
--rw-r--r--   0 rafal      (501) staff       (20)      291 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.5/environment/static/environment/js/forms.js
--rw-r--r--   0 rafal      (501) staff       (20)     2835 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 rafal      (501) staff       (20)     3308 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tasks.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.711294 hdn-research-environment-3.0.5/environment/templates/
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.734458 hdn-research-environment-3.0.5/environment/templates/environment/
--rw-r--r--   0 rafal      (501) staff       (20)     7510 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.5/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     3268 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.5/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     2766 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/_environment_tabs.html
--rw-r--r--   0 rafal      (501) staff       (20)     5553 2024-03-01 11:52:17.000000 hdn-research-environment-3.0.5/environment/templates/environment/_shared_buckets_list.html
--rw-r--r--   0 rafal      (501) staff       (20)     1073 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.5/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 rafal      (501) staff       (20)     3847 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/bucket_files_form.html
--rw-r--r--   0 rafal      (501) staff       (20)     3628 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 rafal      (501) staff       (20)     1208 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/create_shared_bucket.html
--rw-r--r--   0 rafal      (501) staff       (20)     1154 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/create_shared_workspace.html
--rw-r--r--   0 rafal      (501) staff       (20)     1630 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.735337 hdn-research-environment-3.0.5/environment/templates/environment/email/
--rw-r--r--   0 rafal      (501) staff       (20)      272 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.5/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 rafal      (501) staff       (20)      263 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/email/bucket_sharing_confirmation.html
--rw-r--r--   0 rafal      (501) staff       (20)      351 2023-06-05 07:22:20.000000 hdn-research-environment-3.0.5/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 rafal      (501) staff       (20)     1163 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 rafal      (501) staff       (20)     5936 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.5/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 rafal      (501) staff       (20)     1010 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 rafal      (501) staff       (20)     6113 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket.html
--rw-r--r--   0 rafal      (501) staff       (20)     1075 2024-03-01 10:51:33.000000 hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket_files.html
--rw-r--r--   0 rafal      (501) staff       (20)     1007 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket_invitation.html
--rw-r--r--   0 rafal      (501) staff       (20)     1719 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/templates/environment/research_environments.html
--rw-r--r--   0 rafal      (501) staff       (20)     5970 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/environment/shared_bucket_files.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.739704 hdn-research-environment-3.0.5/environment/templates/tag/
--rw-r--r--   0 rafal      (501) staff       (20)     1287 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/tag/bucket_modal_button.html
--rw-r--r--   0 rafal      (501) staff       (20)      241 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 rafal      (501) staff       (20)     1486 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/templates/tag/environment_modal_button.html
--rw-r--r--   0 rafal      (501) staff       (20)     1955 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templates/tag/workspace_destroy_modal_button.html
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.740154 hdn-research-environment-3.0.5/environment/templatetags/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/templatetags/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)     5724 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/templatetags/action_buttons.py
--rw-r--r--   0 rafal      (501) staff       (20)      136 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/templatetags/environment_templatetags.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.741538 hdn-research-environment-3.0.5/environment/tests/
--rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/environment/tests/__init__.py
--rw-r--r--   0 rafal      (501) staff       (20)      645 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/helpers.py
--rw-r--r--   0 rafal      (501) staff       (20)    12158 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.5/environment/tests/mocks.py
--rw-r--r--   0 rafal      (501) staff       (20)     3007 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_decorators.py
--rw-r--r--   0 rafal      (501) staff       (20)    10682 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_services.py
--rw-r--r--   0 rafal      (501) staff       (20)     5327 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_signals.py
--rw-r--r--   0 rafal      (501) staff       (20)     2909 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_utilities.py
--rw-r--r--   0 rafal      (501) staff       (20)      640 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_validators.py
--rw-r--r--   0 rafal      (501) staff       (20)     3380 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/tests/test_views.py
--rw-r--r--   0 rafal      (501) staff       (20)     3175 2024-03-01 10:23:41.000000 hdn-research-environment-3.0.5/environment/urls.py
--rw-r--r--   0 rafal      (501) staff       (20)     1243 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.5/environment/utilities.py
--rw-r--r--   0 rafal      (501) staff       (20)      235 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.5/environment/validators.py
--rw-r--r--   0 rafal      (501) staff       (20)    23431 2024-03-11 09:11:16.000000 hdn-research-environment-3.0.5/environment/views.py
-drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-04 13:19:56.742081 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/
--rw-r--r--   0 rafal      (501) staff       (20)      978 2024-04-04 13:19:56.000000 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 rafal      (501) staff       (20)     4041 2024-04-04 13:19:56.000000 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 rafal      (501) staff       (20)        1 2024-04-04 13:19:56.000000 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 rafal      (501) staff       (20)       84 2024-04-04 13:19:56.000000 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 rafal      (501) staff       (20)       12 2024-04-04 13:19:56.000000 hdn-research-environment-3.0.5/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 rafal      (501) staff       (20)      109 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/pyproject.toml
--rw-r--r--   0 rafal      (501) staff       (20)     1056 2024-04-04 13:19:56.742671 hdn-research-environment-3.0.5/setup.cfg
--rw-r--r--   0 rafal      (501) staff       (20)       38 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.5/setup.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.900683 hdn-research-environment-3.0.6/
+-rw-r--r--   0 rafal      (501) staff       (20)     1551 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/LICENSE
+-rw-r--r--   0 rafal      (501) staff       (20)      115 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/MANIFEST.in
+-rw-r--r--   0 rafal      (501) staff       (20)      978 2024-04-09 13:29:59.900869 hdn-research-environment-3.0.6/PKG-INFO
+-rw-r--r--   0 rafal      (501) staff       (20)      229 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/README.md
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.883596 hdn-research-environment-3.0.6/environment/
+-rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/__init__.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.884149 hdn-research-environment-3.0.6/environment/api/
+-rw-r--r--   0 rafal      (501) staff       (20)     8203 2024-03-26 11:53:16.000000 hdn-research-environment-3.0.6/environment/api/__init__.py
+-rw-r--r--   0 rafal      (501) staff       (20)      939 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/api/decorators.py
+-rw-r--r--   0 rafal      (501) staff       (20)      154 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/apps.py
+-rw-r--r--   0 rafal      (501) staff       (20)     3074 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/constants.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1546 2024-02-16 14:02:50.000000 hdn-research-environment-3.0.6/environment/decorators.py
+-rw-r--r--   0 rafal      (501) staff       (20)     5362 2024-02-29 13:11:14.000000 hdn-research-environment-3.0.6/environment/deserializers.py
+-rw-r--r--   0 rafal      (501) staff       (20)     4404 2024-04-04 13:19:22.000000 hdn-research-environment-3.0.6/environment/entities.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1421 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6/environment/exceptions.py
+-rw-r--r--   0 rafal      (501) staff       (20)     7674 2024-04-04 13:19:22.000000 hdn-research-environment-3.0.6/environment/forms.py
+-rw-r--r--   0 rafal      (501) staff       (20)     2518 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/mailers.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.887399 hdn-research-environment-3.0.6/environment/migrations/
+-rw-r--r--   0 rafal      (501) staff       (20)     2174 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/migrations/00012_bucketsharinginvite.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1443 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0001_initial.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1579 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 rafal      (501) staff       (20)      403 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.6/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-16 11:52:08.000000 hdn-research-environment-3.0.6/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 rafal      (501) staff       (20)     2220 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0005_workflow.py
+-rw-r--r--   0 rafal      (501) staff       (20)      394 2023-05-26 09:35:04.000000 hdn-research-environment-3.0.6/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 rafal      (501) staff       (20)     2348 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 rafal      (501) staff       (20)      476 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 rafal      (501) staff       (20)      420 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1364 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 rafal      (501) staff       (20)      858 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/migrations/0011_refactor_workflow.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1042 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.6/environment/migrations/0013_bucketsharinginvite_type_and_more.py
+-rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/migrations/__init__.py
+-rw-r--r--   0 rafal      (501) staff       (20)     2423 2024-03-05 12:56:41.000000 hdn-research-environment-3.0.6/environment/models.py
+-rw-r--r--   0 rafal      (501) staff       (20)    25434 2024-03-11 11:52:51.000000 hdn-research-environment-3.0.6/environment/services.py
+-rw-r--r--   0 rafal      (501) staff       (20)     4519 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/signals.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.876276 hdn-research-environment-3.0.6/environment/static/
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.887488 hdn-research-environment-3.0.6/environment/static/environment/
+-rw-r--r--   0 rafal      (501) staff       (20)     6148 2023-02-02 14:12:52.000000 hdn-research-environment-3.0.6/environment/static/environment/.DS_Store
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.888566 hdn-research-environment-3.0.6/environment/static/environment/css/
+-rw-r--r--   0 rafal      (501) staff       (20)    11789 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/static/environment/css/bucket_files_dropzone.css
+-rw-r--r--   0 rafal      (501) staff       (20)      342 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/static/environment/css/creation_form.css
+-rw-r--r--   0 rafal      (501) staff       (20)     6583 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 rafal      (501) staff       (20)      117 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6/environment/static/environment/css/management_views.css
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.889975 hdn-research-environment-3.0.6/environment/static/environment/js/
+-rw-r--r--   0 rafal      (501) staff       (20)   114702 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/static/environment/js/bucket_files_dropzone.min.js
+-rw-r--r--   0 rafal      (501) staff       (20)      564 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/static/environment/js/cookie.js
+-rw-r--r--   0 rafal      (501) staff       (20)      199 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/static/environment/js/destroy_shared_bucket.js
+-rw-r--r--   0 rafal      (501) staff       (20)      291 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6/environment/static/environment/js/forms.js
+-rw-r--r--   0 rafal      (501) staff       (20)     2835 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 rafal      (501) staff       (20)     3308 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tasks.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.876579 hdn-research-environment-3.0.6/environment/templates/
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.896293 hdn-research-environment-3.0.6/environment/templates/environment/
+-rw-r--r--   0 rafal      (501) staff       (20)     7510 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.6/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 rafal      (501) staff       (20)     3268 2023-09-08 13:35:54.000000 hdn-research-environment-3.0.6/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 rafal      (501) staff       (20)     2964 2024-04-09 13:28:41.000000 hdn-research-environment-3.0.6/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 rafal      (501) staff       (20)     5553 2024-03-01 11:52:17.000000 hdn-research-environment-3.0.6/environment/templates/environment/_shared_buckets_list.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1073 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 rafal      (501) staff       (20)     3847 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/bucket_files_form.html
+-rw-r--r--   0 rafal      (501) staff       (20)     3628 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1208 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/create_shared_bucket.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1154 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/create_shared_workspace.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1630 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.896928 hdn-research-environment-3.0.6/environment/templates/environment/email/
+-rw-r--r--   0 rafal      (501) staff       (20)      272 2023-06-12 13:30:54.000000 hdn-research-environment-3.0.6/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 rafal      (501) staff       (20)      263 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/email/bucket_sharing_confirmation.html
+-rw-r--r--   0 rafal      (501) staff       (20)      351 2023-06-05 07:22:20.000000 hdn-research-environment-3.0.6/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1163 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 rafal      (501) staff       (20)     5936 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.6/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1010 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 rafal      (501) staff       (20)     6113 2024-03-01 10:40:36.000000 hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1075 2024-03-01 10:51:33.000000 hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket_files.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1007 2024-01-29 13:36:38.000000 hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket_invitation.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1719 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/templates/environment/research_environments.html
+-rw-r--r--   0 rafal      (501) staff       (20)     5970 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/environment/shared_bucket_files.html
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.897911 hdn-research-environment-3.0.6/environment/templates/tag/
+-rw-r--r--   0 rafal      (501) staff       (20)     1287 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/tag/bucket_modal_button.html
+-rw-r--r--   0 rafal      (501) staff       (20)      241 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1486 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/templates/tag/environment_modal_button.html
+-rw-r--r--   0 rafal      (501) staff       (20)     1955 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templates/tag/workspace_destroy_modal_button.html
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.898274 hdn-research-environment-3.0.6/environment/templatetags/
+-rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/templatetags/__init__.py
+-rw-r--r--   0 rafal      (501) staff       (20)     5724 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/templatetags/action_buttons.py
+-rw-r--r--   0 rafal      (501) staff       (20)      136 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/templatetags/environment_templatetags.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.900033 hdn-research-environment-3.0.6/environment/tests/
+-rw-r--r--   0 rafal      (501) staff       (20)        0 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/environment/tests/__init__.py
+-rw-r--r--   0 rafal      (501) staff       (20)      645 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/helpers.py
+-rw-r--r--   0 rafal      (501) staff       (20)    12158 2023-05-29 14:50:53.000000 hdn-research-environment-3.0.6/environment/tests/mocks.py
+-rw-r--r--   0 rafal      (501) staff       (20)     3007 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_decorators.py
+-rw-r--r--   0 rafal      (501) staff       (20)    10682 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_services.py
+-rw-r--r--   0 rafal      (501) staff       (20)     5327 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_signals.py
+-rw-r--r--   0 rafal      (501) staff       (20)     2909 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_utilities.py
+-rw-r--r--   0 rafal      (501) staff       (20)      640 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_validators.py
+-rw-r--r--   0 rafal      (501) staff       (20)     3380 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/tests/test_views.py
+-rw-r--r--   0 rafal      (501) staff       (20)     3175 2024-03-01 10:23:41.000000 hdn-research-environment-3.0.6/environment/urls.py
+-rw-r--r--   0 rafal      (501) staff       (20)     1243 2024-01-29 08:25:22.000000 hdn-research-environment-3.0.6/environment/utilities.py
+-rw-r--r--   0 rafal      (501) staff       (20)      235 2023-09-08 13:07:53.000000 hdn-research-environment-3.0.6/environment/validators.py
+-rw-r--r--   0 rafal      (501) staff       (20)    23604 2024-04-09 13:28:41.000000 hdn-research-environment-3.0.6/environment/views.py
+drwxr-xr-x   0 rafal      (501) staff       (20)        0 2024-04-09 13:29:59.900585 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/
+-rw-r--r--   0 rafal      (501) staff       (20)      978 2024-04-09 13:29:59.000000 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 rafal      (501) staff       (20)     4041 2024-04-09 13:29:59.000000 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 rafal      (501) staff       (20)        1 2024-04-09 13:29:59.000000 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 rafal      (501) staff       (20)       84 2024-04-09 13:29:59.000000 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 rafal      (501) staff       (20)       12 2024-04-09 13:29:59.000000 hdn-research-environment-3.0.6/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 rafal      (501) staff       (20)      109 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/pyproject.toml
+-rw-r--r--   0 rafal      (501) staff       (20)     1056 2024-04-09 13:29:59.901233 hdn-research-environment-3.0.6/setup.cfg
+-rw-r--r--   0 rafal      (501) staff       (20)       38 2023-01-30 07:27:57.000000 hdn-research-environment-3.0.6/setup.py
```

### Comparing `hdn-research-environment-3.0.5/LICENSE` & `hdn-research-environment-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/PKG-INFO` & `hdn-research-environment-3.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.5
+Version: 3.0.6
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.5/environment/api/__init__.py` & `hdn-research-environment-3.0.6/environment/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/api/decorators.py` & `hdn-research-environment-3.0.6/environment/api/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/constants.py` & `hdn-research-environment-3.0.6/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/decorators.py` & `hdn-research-environment-3.0.6/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/deserializers.py` & `hdn-research-environment-3.0.6/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/entities.py` & `hdn-research-environment-3.0.6/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/exceptions.py` & `hdn-research-environment-3.0.6/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/forms.py` & `hdn-research-environment-3.0.6/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/mailers.py` & `hdn-research-environment-3.0.6/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/00012_bucketsharinginvite.py` & `hdn-research-environment-3.0.6/environment/migrations/00012_bucketsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0001_initial.py` & `hdn-research-environment-3.0.6/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-3.0.6/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0005_workflow.py` & `hdn-research-environment-3.0.6/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-3.0.6/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-3.0.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0011_refactor_workflow.py` & `hdn-research-environment-3.0.6/environment/migrations/0011_refactor_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/migrations/0013_bucketsharinginvite_type_and_more.py` & `hdn-research-environment-3.0.6/environment/migrations/0013_bucketsharinginvite_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/models.py` & `hdn-research-environment-3.0.6/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/services.py` & `hdn-research-environment-3.0.6/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/signals.py` & `hdn-research-environment-3.0.6/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/.DS_Store` & `hdn-research-environment-3.0.6/environment/static/environment/.DS_Store`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/css/bucket_files_dropzone.css` & `hdn-research-environment-3.0.6/environment/static/environment/css/bucket_files_dropzone.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/css/environment-base.css` & `hdn-research-environment-3.0.6/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/js/bucket_files_dropzone.min.js` & `hdn-research-environment-3.0.6/environment/static/environment/js/bucket_files_dropzone.min.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/js/cookie.js` & `hdn-research-environment-3.0.6/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-3.0.6/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tasks.py` & `hdn-research-environment-3.0.6/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-3.0.6/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-3.0.6/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/_environment_tabs.html` & `hdn-research-environment-3.0.6/environment/templates/environment/_environment_tabs.html`

 * *Files 16% similar despite different names*

```diff
@@ -68,35 +68,36 @@
       >
         {% include "environment/_billing_accounts_list.html" %}
       </div>
     </div>
   </div>
 </div>
 
+<script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.7.5/socket.io.js" integrity="sha512-luMnTJZ7oEchNDZAtQhgjomP1eZefnl82ruTH/3Oj/Yu5qYtwL7+dVRccACS/Snp1lFXq188XFipHKYE75IaQQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script>
     function refreshCards(executionId) {
         fetchNewCards(executionId)
         .then(html => $("#environment-tabs").html(html));
     }
 
     function pollExecutionStatus(executionId) {
         const pollUrl = `{% url "check_execution_status" %}?execution_resource_name=${executionId}`;
         fetch(pollUrl)
         .then(response => response.json())
         .then(({ finished }) => {
             if (finished) {
                 refreshCards(executionId);
-            } else {
-                scheduleExecutionPolling(executionId);
             }
         });
     }
 
-    function scheduleExecutionPolling(executionId, immediate=false) {
-        const timeout = immediate ? 0 : 30000;
-        setTimeout(() => pollExecutionStatus(executionId), timeout);
-    }
+    var socket = io("{{ websocket_url }}");
+
+    socket.on('workflow_update', function(data) {
+        refreshCards(data.workbench_activity_id);
+    });
 
     {% for workflow in workflows %}
-        scheduleExecutionPolling("{{ workflow.execution_resource_name }}", true);
+        socket.emit("join", "{{ workflow.execution_resource_name }}");
+        pollExecutionStatus("{{ workflow.execution_resource_name }}");
     {% endfor %}
 </script>
```

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/_shared_buckets_list.html` & `hdn-research-environment-3.0.6/environment/templates/environment/_shared_buckets_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-3.0.6/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/bucket_files_form.html` & `hdn-research-environment-3.0.6/environment/templates/environment/bucket_files_form.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-3.0.6/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/create_shared_bucket.html` & `hdn-research-environment-3.0.6/environment/templates/environment/create_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/create_shared_workspace.html` & `hdn-research-environment-3.0.6/environment/templates/environment/create_shared_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/create_workspace.html` & `hdn-research-environment-3.0.6/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-3.0.6/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-3.0.6/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket.html` & `hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket_files.html` & `hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/manage_shared_bucket_invitation.html` & `hdn-research-environment-3.0.6/environment/templates/environment/manage_shared_bucket_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/research_environments.html` & `hdn-research-environment-3.0.6/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/environment/shared_bucket_files.html` & `hdn-research-environment-3.0.6/environment/templates/environment/shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/tag/bucket_modal_button.html` & `hdn-research-environment-3.0.6/environment/templates/tag/bucket_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-3.0.6/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templates/tag/workspace_destroy_modal_button.html` & `hdn-research-environment-3.0.6/environment/templates/tag/workspace_destroy_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/templatetags/action_buttons.py` & `hdn-research-environment-3.0.6/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/helpers.py` & `hdn-research-environment-3.0.6/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/mocks.py` & `hdn-research-environment-3.0.6/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_decorators.py` & `hdn-research-environment-3.0.6/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_services.py` & `hdn-research-environment-3.0.6/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_signals.py` & `hdn-research-environment-3.0.6/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_utilities.py` & `hdn-research-environment-3.0.6/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_validators.py` & `hdn-research-environment-3.0.6/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/tests/test_views.py` & `hdn-research-environment-3.0.6/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/urls.py` & `hdn-research-environment-3.0.6/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/utilities.py` & `hdn-research-environment-3.0.6/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/environment/views.py` & `hdn-research-environment-3.0.6/environment/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import concurrent
 import json
 import re
 
+from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.db import transaction
 from django.http import Http404, JsonResponse
 from django.shortcuts import redirect, render
 from django.views.decorators.http import require_GET, require_http_methods
 
@@ -80,14 +81,15 @@
     running_workflows = services.get_running_workflows(request.user)
 
     context = {
         "shared_workspaces": shared_workspaces,
         "workspaces_with_workbenches": workspaces,
         "billing_accounts_list": billing_accounts_list,
         "workflows": running_workflows,
+        "websocket_url": settings.CLOUD_RESEARCH_ENVIRONMENTS_API_URL
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
     )
@@ -114,14 +116,15 @@
     running_workflows = services.get_running_workflows(request.user)
 
     context = {
         "shared_workspaces": shared_workspaces,
         "workspaces_with_workbenches": workspaces,
         "billing_accounts_list": billing_accounts_list,
         "workflows": running_workflows,
+        "websocket_url": settings.CLOUD_RESEARCH_ENVIRONMENTS_API_URL
     }
 
     execution_resource_name = request.GET.get("execution_resource_name")
     if execution_resource_name:
         workflow = services.get_execution(execution_resource_name)
         workflow_state_context = {
             "recent_workflow": workflow,
```

### Comparing `hdn-research-environment-3.0.5/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-3.0.6/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.5
+Version: 3.0.6
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.5/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-3.0.6/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.5/setup.cfg` & `hdn-research-environment-3.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 3.0.5
+version = 3.0.6
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

