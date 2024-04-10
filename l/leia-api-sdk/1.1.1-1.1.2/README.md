# Comparing `tmp/leia_api_sdk-1.1.1.tar.gz` & `tmp/leia_api_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leia_api_sdk-1.1.1.tar", last modified: Mon Mar 13 15:27:49 2023, max compression
+gzip compressed data, was "leia_api_sdk-1.1.2.tar", last modified: Wed Apr 10 13:43:03 2024, max compression
```

## Comparing `leia_api_sdk-1.1.1.tar` & `leia_api_sdk-1.1.2.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/
--rw-r--r--   0 hatok     (1000) hatok     (1000)     1073 2021-04-29 08:24:03.000000 leia_api_sdk-1.1.1/LICENSE
--rw-r--r--   0 hatok     (1000) hatok     (1000)      322 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/PKG-INFO
--rw-r--r--   0 hatok     (1000) hatok     (1000)    15605 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/README.md
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.534189 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/
--rw-r--r--   0 hatok     (1000) hatok     (1000)      322 2023-03-13 15:27:49.000000 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2047 2023-03-13 15:27:49.000000 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 hatok     (1000) hatok     (1000)        1 2023-03-13 15:27:49.000000 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 hatok     (1000) hatok     (1000)       70 2023-03-13 15:27:49.000000 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/requires.txt
--rw-r--r--   0 hatok     (1000) hatok     (1000)        8 2023-03-13 15:27:49.000000 leia_api_sdk-1.1.1/leia_api_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.534189 leia_api_sdk-1.1.1/leiaapi/
--rw-r--r--   0 hatok     (1000) hatok     (1000)        0 2021-10-08 09:05:32.000000 leia_api_sdk-1.1.1/leiaapi/__init__.py
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.534189 leia_api_sdk-1.1.1/leiaapi/generated/
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2989 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/__init__.py
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/leiaapi/generated/api/
--rw-r--r--   0 hatok     (1000) hatok     (1000)      822 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/__init__.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    58237 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/annotation_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    74937 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/application_admin_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    19355 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/application_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)   122246 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/document_admin_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)   115195 2023-03-09 15:05:45.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/document_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     6107 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/health_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    64579 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/job_admin_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    60013 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/job_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)   123718 2023-03-09 15:09:12.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/model_admin_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    76490 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/model_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     7241 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/worker_admin_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    13692 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/api/worker_api.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    29872 2023-03-09 15:37:19.000000 leia_api_sdk-1.1.1/leiaapi/generated/api_client.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    14176 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/configuration.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     5051 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/exceptions.py
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/leiaapi/generated/models/
--rw-r--r--   0 hatok     (1000) hatok     (1000)     1739 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/__init__.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2685 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/annotation.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      616 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/annotation_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     3468 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/application.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      593 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/application_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2791 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/apply_body.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2096 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/classification.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2317 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/conditional_body.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     3603 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/document.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      578 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/format_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     3714 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/job.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     5748 2023-03-09 15:59:47.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/job_result.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      649 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/job_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     1837 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/login_body.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2250 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/login_token.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     4794 2023-03-08 17:35:53.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/model.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      787 2023-03-08 17:41:04.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/model_input_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      669 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/model_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      797 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/result_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      622 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/speed.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      773 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/statuses.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2628 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/train_body.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2791 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/transform_body.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)      725 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/transform_types.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     2026 2023-03-08 17:00:55.000000 leia_api_sdk-1.1.1/leiaapi/generated/models/worker.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)    12614 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/leiaapi/generated/rest.py
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/leiaapi/helpers/
--rw-r--r--   0 hatok     (1000) hatok     (1000)        0 2021-10-08 09:05:59.000000 leia_api_sdk-1.1.1/leiaapi/helpers/__init__.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     8440 2023-03-08 17:35:50.000000 leia_api_sdk-1.1.1/leiaapi/helpers/download.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     1279 2021-10-08 09:05:59.000000 leia_api_sdk-1.1.1/leiaapi/helpers/scheduler.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     3953 2023-03-08 17:26:25.000000 leia_api_sdk-1.1.1/leiaapi/helpers/session.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)       69 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/setup.cfg
--rw-r--r--   0 hatok     (1000) hatok     (1000)     1078 2023-03-13 15:27:29.000000 leia_api_sdk-1.1.1/setup.py
-drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2023-03-13 15:27:49.544189 leia_api_sdk-1.1.1/test/
--rw-r--r--   0 hatok     (1000) hatok     (1000)        0 2023-03-08 17:00:56.000000 leia_api_sdk-1.1.1/test/__init__.py
--rw-r--r--   0 hatok     (1000) hatok     (1000)     8201 2023-03-09 16:18:39.000000 leia_api_sdk-1.1.1/test/test_application_api.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     1073 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/LICENSE
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      452 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/PKG-INFO
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    15605 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/README.md
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      452 2024-04-10 13:43:03.000000 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2030 2024-04-10 13:43:03.000000 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 hatok     (1000) hatok     (1000)        1 2024-04-10 13:43:03.000000 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 hatok     (1000) hatok     (1000)       70 2024-04-10 13:43:03.000000 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 hatok     (1000) hatok     (1000)        8 2024-04-10 13:43:03.000000 leia_api_sdk-1.1.2/leia_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leiaapi/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)        0 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/__init__.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leiaapi/generated/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2989 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/__init__.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leiaapi/generated/api/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      822 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/__init__.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    58237 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/annotation_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    74937 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/application_admin_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    19355 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/application_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)   122246 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/document_admin_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)   115195 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/document_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     6107 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/health_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    64579 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/job_admin_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    60013 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/job_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)   123718 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/model_admin_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    76490 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/model_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     7241 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/worker_admin_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    13692 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api/worker_api.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    29872 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/api_client.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    14176 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/configuration.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     5051 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/exceptions.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leiaapi/generated/models/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     1739 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/__init__.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2685 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/annotation.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      616 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/annotation_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     3468 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/application.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      593 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/application_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2791 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/apply_body.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2096 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/classification.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2317 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/conditional_body.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     3603 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/document.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      578 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/format_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     3714 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/job.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     5748 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/job_result.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      649 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/job_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     1837 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/login_body.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2250 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/login_token.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     4794 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/model.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      787 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/model_input_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      669 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/model_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      797 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/result_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      622 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/speed.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      773 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/statuses.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2628 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/train_body.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2791 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/transform_body.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)      725 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/transform_types.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     2026 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/models/worker.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)    12614 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/generated/rest.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/leiaapi/helpers/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)        0 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/helpers/__init__.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     8440 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/helpers/download.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     1279 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/leiaapi/helpers/scheduler.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     3953 2024-04-10 12:28:32.000000 leia_api_sdk-1.1.2/leiaapi/helpers/session.py
+-rw-r--r--   0 hatok     (1000) hatok     (1000)       69 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/setup.cfg
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     1078 2024-04-10 13:41:55.000000 leia_api_sdk-1.1.2/setup.py
+drwxr-xr-x   0 hatok     (1000) hatok     (1000)        0 2024-04-10 13:43:03.599279 leia_api_sdk-1.1.2/test/
+-rw-r--r--   0 hatok     (1000) hatok     (1000)     8201 2024-04-10 12:26:56.000000 leia_api_sdk-1.1.2/test/test_application_api.py
```

### Comparing `leia_api_sdk-1.1.1/LICENSE` & `leia_api_sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/README.md` & `leia_api_sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leia_api_sdk.egg-info/SOURCES.txt` & `leia_api_sdk-1.1.2/leia_api_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,8 @@
 leiaapi/generated/models/transform_body.py
 leiaapi/generated/models/transform_types.py
 leiaapi/generated/models/worker.py
 leiaapi/helpers/__init__.py
 leiaapi/helpers/download.py
 leiaapi/helpers/scheduler.py
 leiaapi/helpers/session.py
-test/__init__.py
 test/test_application_api.py
```

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/__init__.py` & `leia_api_sdk-1.1.2/leiaapi/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/__init__.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/__init__.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/annotation_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/annotation_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/application_admin_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/application_admin_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/application_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/application_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/document_admin_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/document_admin_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/document_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/document_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/health_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/health_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/job_admin_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/job_admin_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/job_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/job_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/model_admin_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/model_admin_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/model_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/model_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/worker_admin_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/worker_admin_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api/worker_api.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api/worker_api.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/api_client.py` & `leia_api_sdk-1.1.2/leiaapi/generated/api_client.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/configuration.py` & `leia_api_sdk-1.1.2/leiaapi/generated/configuration.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/exceptions.py` & `leia_api_sdk-1.1.2/leiaapi/generated/exceptions.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/__init__.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/annotation.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/annotation.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/annotation_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/annotation_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/application.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/application.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/application_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/application_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/apply_body.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/apply_body.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/classification.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/classification.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/conditional_body.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/conditional_body.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/document.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/document.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/format_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/format_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/job.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/job.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/job_result.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/job_result.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/job_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/job_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/login_body.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/login_body.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/login_token.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/login_token.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/model.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/model.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/model_input_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/model_input_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/model_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/model_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/result_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/result_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/speed.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/speed.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/statuses.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/statuses.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/train_body.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/train_body.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/transform_body.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/transform_body.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/transform_types.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/transform_types.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/models/worker.py` & `leia_api_sdk-1.1.2/leiaapi/generated/models/worker.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/generated/rest.py` & `leia_api_sdk-1.1.2/leiaapi/generated/rest.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/helpers/download.py` & `leia_api_sdk-1.1.2/leiaapi/helpers/download.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/helpers/scheduler.py` & `leia_api_sdk-1.1.2/leiaapi/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `leia_api_sdk-1.1.1/leiaapi/helpers/session.py` & `leia_api_sdk-1.1.2/leiaapi/helpers/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         if resource_path == '/login':
             raise
         if e.status != 401 or 'token' not in header_params:
             # It's not a login error, we do not care for it
             # Or there is no token to send in the request, and we do not care either
             raise
         logger.info("Leia Token is invalid or non existent, trying to refresh it")
-        SessionManager.DEFAULT_SESSION.login()
+        self.session.login()
 
-        header_params['token'] = SessionManager.DEFAULT_SESSION.token
+        header_params['token'] = self.session.token
         return old__call_api(self, resource_path, method, path_params, query_params, header_params, *args, **kwargs)
 
 # We override the initial __call_api method to be able to automatically login if the token is not valid
 leiaapi.generated.api_client.ApiClient._ApiClient__call_api = __call_api_with_auto_login
 
 
 class SessionManager:
@@ -46,14 +46,15 @@
         :param api_key: The API Key to connect to api.leia.io
         :param client: A ApiClient object configure with the information of the server
         :param auto_update_token: Set to False to not update the token validity automatically
         """
         super().__init__()
         self._api_key: str = api_key
         self._client: Optional[ApiClient] = client
+        self._client.session = self
         self._token: Optional[str] = None
         self._application_api: ApplicationApi = ApplicationApi(api_client=self.client)
         self._application: Optional[Application] = None
         self._scheduler: Optional[Scheduler] = None
         self._auto_update_token = auto_update_token
 
     @property
```

### Comparing `leia_api_sdk-1.1.1/setup.py` & `leia_api_sdk-1.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "leia_api_sdk"
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil >= 2.5.3",
     "pydantic >= 1.10.2",
     "aenum >= 3.1.11"
 ]
```

### Comparing `leia_api_sdk-1.1.1/test/test_application_api.py` & `leia_api_sdk-1.1.2/test/test_application_api.py`

 * *Files identical despite different names*

