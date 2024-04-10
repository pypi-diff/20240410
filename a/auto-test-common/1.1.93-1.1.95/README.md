# Comparing `tmp/auto-test-common-1.1.93.tar.gz` & `tmp/auto-test-common-1.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.93.tar", last modified: Wed Apr 10 01:35:42 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.95.tar", last modified: Wed Apr 10 05:37:15 2024, max compression
```

## Comparing `auto-test-common-1.1.93.tar` & `auto-test-common-1.1.95.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.579017 auto-test-common-1.1.93/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 01:35:42.579188 auto-test-common-1.1.93/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.535155 auto-test-common-1.1.93/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-10 01:35:42.000000 auto-test-common-1.1.93/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.535565 auto-test-common-1.1.93/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.93/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.538299 auto-test-common-1.1.93/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.93/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11452 2024-03-26 09:07:48.000000 auto-test-common-1.1.93/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.93/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.93/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.540799 auto-test-common-1.1.93/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.93/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7558 2024-04-10 01:35:33.000000 auto-test-common-1.1.93/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.93/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.541842 auto-test-common-1.1.93/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.93/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.93/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.545329 auto-test-common-1.1.93/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.93/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    24668 2024-03-26 09:07:48.000000 auto-test-common-1.1.93/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    11059 2024-03-26 08:31:29.000000 auto-test-common-1.1.93/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.93/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.551309 auto-test-common-1.1.93/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.93/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.93/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.93/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.93/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.553801 auto-test-common-1.1.93/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.93/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.93/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.93/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.559917 auto-test-common-1.1.93/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.93/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.93/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.93/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.93/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.93/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.93/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.561122 auto-test-common-1.1.93/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.93/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.93/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.565612 auto-test-common-1.1.93/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.93/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.93/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.93/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.93/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.93/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.93/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 01:35:42.577784 auto-test-common-1.1.93/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.93/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.93/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.93/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.93/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.93/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.93/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12350 2024-03-20 05:29:19.000000 auto-test-common-1.1.93/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.93/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.93/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.93/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.93/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.93/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.93/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-10 01:35:42.579990 auto-test-common-1.1.93/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.93/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.451922 auto-test-common-1.1.95/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 05:37:15.452152 auto-test-common-1.1.95/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.408733 auto-test-common-1.1.95/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.409041 auto-test-common-1.1.95/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.95/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.410372 auto-test-common-1.1.95/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.95/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11697 2024-04-10 05:37:08.000000 auto-test-common-1.1.95/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.95/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.95/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.412708 auto-test-common-1.1.95/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.95/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.95/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.95/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.413578 auto-test-common-1.1.95/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.95/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.415927 auto-test-common-1.1.95/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.95/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    24716 2024-04-10 05:26:16.000000 auto-test-common-1.1.95/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    11152 2024-04-10 05:26:16.000000 auto-test-common-1.1.95/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.95/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.421605 auto-test-common-1.1.95/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.95/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.95/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.95/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.423965 auto-test-common-1.1.95/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.95/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.95/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.95/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.431038 auto-test-common-1.1.95/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.95/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.95/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.95/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.95/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.95/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.95/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.432009 auto-test-common-1.1.95/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.436957 auto-test-common-1.1.95/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.95/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.95/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.95/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.95/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.95/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.95/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.450230 auto-test-common-1.1.95/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.95/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.95/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.95/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.95/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.95/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.95/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12914 2024-04-10 05:37:08.000000 auto-test-common-1.1.95/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.95/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.95/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.95/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.95/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.95/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.95/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-10 05:37:15.453516 auto-test-common-1.1.95/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.95/setup.py
```

### Comparing `auto-test-common-1.1.93/PKG-INFO` & `auto-test-common-1.1.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.93
+Version: 1.1.95
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.93/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.95/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.93
+Version: 1.1.95
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.93/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.95/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.95/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/autotest/base_requests.py` & `auto-test-common-1.1.95/common/autotest/base_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             DataProcess.save_response(case_number, res.json())
         try:
             return res.json(), expect, res
         except:
             return res.text, expect, res
 
     @classmethod
-    def api_exec(self, schemal_key, data=None, header=None, file=None, cookie=None, host: str = 'host', datatype: str='json', step:str='测试接口详情') -> object:
+    def api_exec(self, schemal_key, data=None, header=None, file=None, cookie=None, host: str = 'host', datatype: str='json', step:str='测试接口详情', _replace:int=0) -> object:
         """处理case数据，转换成可用数据发送请求
         :param case: 读取出来的每一行用例内容，可进行解包
         :param env: 环境名称 默认使用config.yaml server下的 dev 后面的基准地址
         return: 响应结果， 预期结果
         """
         DataBus.save_init_data()
         temp = data
@@ -103,39 +103,39 @@
                     schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                     content = schemal_body['body']
                     if isinstance(content,dict):
                         if 'file' in content:
                             from common.plugin.file_plugin import FilePlugin
                             content = FilePlugin.load_data(content['file'])
                     data = convert_json_bank(content, data)
-                data = DataProcess.handle_data(data)
+                data = DataProcess.handle_data(variable=data, _replace=_replace)
             else:
                 if 'body' in schemal_data:
                     schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                     content = schemal_body['body']
                     data = req_expr(content=content, data=data, _no_content=0)
             if 'format' in schemal_data:
                 if schemal_data['format'] == 'text':
-                    data = DataProcess.handle_data(data,False)
+                    data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
                 elif schemal_data['format'] == 'json':
-                    data = DataProcess.handle_data(data)
+                    data = DataProcess.handle_data(variable=data, _replace=_replace)
                 elif schemal_data['format'] == 'None':
                     data = data
                 else:
                     data = DataProcess.handle_data(data)
             else:
                 if schemal_data['datatype'] == 'xml':
-                    data = DataProcess.handle_data(data, False)
+                    data = DataProcess.handle_data(variable=data, jsonformat=False,_replace=_replace)
                 elif schemal_data['datatype'] == 'json':
-                    data = DataProcess.handle_data(data)
+                    data = DataProcess.handle_data(variable=data, _replace=_replace)
                 else:
-                    data = DataProcess.handle_data(data)
+                    data = DataProcess.handle_data(variable=data, _replace=_replace)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换dict异常' + repr(e))
-            data = DataProcess.handle_data(data, False)
+            data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
         if 'file' in schemal_data and file is None:
             file = schemal_body['file']
         file_obj = DataProcess.handler_files(file)
         if step == '测试接口详情' and DataProcess.isNotNull(schemal_data['desc']):
             step = '测试接口详情:'+schemal_data['desc']
         res = self.http_request(url=url, method=schemal_data['method'], parametric_key=schemal_data['datatype'],
                                header=DataProcess.setDictEncode(header), data=data, file=file_obj, cookie=cookie, desc=step)
```

### Comparing `auto-test-common-1.1.93/common/autotest/handle_allure.py` & `auto-test-common-1.1.95/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/autotest/handle_assert.py` & `auto-test-common-1.1.95/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/common/api_driver.py` & `auto-test-common-1.1.95/common/common/api_driver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import loguru
 import requests
-from common.autotest.handle_allure import allure_api_step
+from common.autotest.handle_allure import allure_api_step, allure_step
 from requests_toolbelt import MultipartEncoder
 from os import path
 import os
 from common.config.config import TEST_FILE_PATH
 
 
 class APIDriver(object):
@@ -127,14 +128,15 @@
                     _path = adjust_path(data[key])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         all_path = os.sep.join([TEST_FILE_PATH, _path])
                         from common.file.handle_system import adjust_path
                         all_path = adjust_path(all_path)
                         data[key] = (data[key], open(all_path, 'rb'))
                     else:
+                        loguru.Logger.warning('在file目录未找到上传文件【警告】')
                         allure_step('在file目录未找到上传文件【文件检查】', _path)
                 elif isinstance(data[key], tuple):
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key][1])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         if data[key].__len__() == 3:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
@@ -143,14 +145,15 @@
                             data[key] = (data[key][0], open(all_path, 'rb'), data[key][2])
                         elif data[key].__len__() == 2:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
                             all_path = adjust_path(all_path)
                             data[key] = (data[key][0], open(all_path, 'rb'))
                     else:
+                        loguru.Logger.warning('在file目录未找到上传文件【警告】')
                         allure_step('在file目录未找到上传文件【文件检查】',_path)
                 else:
                     data = data
         return data
```

### Comparing `auto-test-common-1.1.93/common/common/constant.py` & `auto-test-common-1.1.95/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/common/test.py` & `auto-test-common-1.1.95/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/config/config.py` & `auto-test-common-1.1.95/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/data/data_process.py` & `auto-test-common-1.1.95/common/data/data_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,26 +187,26 @@
                         if key.find('$') != 0:
                             _template[key] = cls.handle_data_fromat(_template[key], data, _no_content, _dataType)
                 return _template
 
 
 
     @classmethod
-    def handle_data(cls, variable: str, jsonformat:bool=True) -> dict:
+    def handle_data(cls, variable: str, jsonformat:bool=True, _replace:int=0) -> dict:
         """请求数据处理
         :param variable: 请求数据，传入的是可转换字典/json的字符串,其中可以包含变量表达式
         return 处理之后的json/dict类型的字典数据
         """
         if variable == '':
             return
         if isinstance(variable, str) and variable.find(".json",len(variable)-5) != -1:
             _path = path.join(TEST_DATA_PATH, variable, )
             with open(_path, "r") as json_file:
                 variable = json.load(json_file)
-        data = req_expr(variable, cls.response_dict)
+        data = req_expr(content=variable, data=cls.response_dict, _replace=_replace)
         if jsonformat:
             variable = convert_json(data)
         else:
             variable = data
         return variable
 
     @classmethod
```

### Comparing `auto-test-common-1.1.93/common/data/handle_common.py` & `auto-test-common-1.1.95/common/data/handle_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,28 @@
         result = jsonpath(obj, expr)
     except Exception as e:
         if error_flag:
             logger.warning(f'{expr} - 提取不到内容！{e}')
         result = expr
     return result
 
-def req_expr(content: str, data: dict = None, expr: str = '\\${(.*?)}', _no_content: int = 0, _dataType:bool=False) -> str:
+def req_expr(content: str, data: dict = None, expr: str = '\\${(.*?)}', _no_content: int = 0, _dataType:bool=False,_replace:int=0) -> str:
     """从请求参数的字符串中，使用正则的方法找出合适的字符串内容并进行替换
     :param content: 原始的字符串内容
     :param data: 在该项目中一般为响应字典，从字典取值出来
     :param expr: 查找用的正则表达式
     return content： 替换表达式后的字符串
     """
-    if isinstance(content, str):
-        content = content.replace('\\', '')
+    if _replace == 0:
+        if isinstance(content, str):
+            content = content.replace('\\', '')
+        else:
+            content = str(content).replace('\\', '')
     else:
-        content = str(content).replace('\\', '')
-
+        content = str(content)
     for i in re.findall(expr, content):
         if i.find(".") >= 0:
             from common.plugin.data_bus import DataBus
             _content = DataBus.get_key(i)
         elif i.find("|") >= 0:
             _arr = i.split('|')
             if get_system_key(f'{_arr[0]}') is None:
```

### Comparing `auto-test-common-1.1.93/common/data/template_data.py` & `auto-test-common-1.1.95/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_db.py` & `auto-test-common-1.1.95/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_db_batch.py` & `auto-test-common-1.1.95/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_mongo.py` & `auto-test-common-1.1.95/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_mysqldb.py` & `auto-test-common-1.1.95/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_oracle.py` & `auto-test-common-1.1.95/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/db/handle_sqlserver.py` & `auto-test-common-1.1.95/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/driver/ui_page.py` & `auto-test-common-1.1.95/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/ReadFile.py` & `auto-test-common-1.1.95/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/handle_excel.py` & `auto-test-common-1.1.95/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/handle_file.py` & `auto-test-common-1.1.95/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/handle_reques.py` & `auto-test-common-1.1.95/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/handle_system.py` & `auto-test-common-1.1.95/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/file/handle_yaml.py` & `auto-test-common-1.1.95/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/mq/handle_rabbit.py` & `auto-test-common-1.1.95/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plat/ATF_platform.py` & `auto-test-common-1.1.95/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plat/jenkin_platform.py` & `auto-test-common-1.1.95/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plat/jira_platform.py` & `auto-test-common-1.1.95/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plat/mysql_platform.py` & `auto-test-common-1.1.95/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plat/service_platform.py` & `auto-test-common-1.1.95/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/allure_plugin.py` & `auto-test-common-1.1.95/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/assert_plugin.py` & `auto-test-common-1.1.95/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/atf_plugin.py` & `auto-test-common-1.1.95/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/data_bus.py` & `auto-test-common-1.1.95/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/data_plugin.py` & `auto-test-common-1.1.95/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/file_plugin.py` & `auto-test-common-1.1.95/common/plugin/file_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,39 @@
 class FilePlugin(object):
 
     @classmethod
     def load_data(self, fileName, data=None):
         content = f'{fileName}文件内容不存在'
         try:
             if fileName.find(".json") >= 0:
-                content = self.load_json(fileName, _dict=data)
+                from common.file.handle_system import adjust_path
+                _path = adjust_path(fileName)
+                content = self.load_json(_path, _dict=data)
             elif fileName.find(".xml") >= 0:
-                content = self.load_xml(fileName, _dict=data)
+                from common.file.handle_system import adjust_path
+                _path = adjust_path(fileName)
+                content = self.load_xml(_path, _dict=data)
             elif fileName.find(".txt") >= 0:
-                content = self.load_xml(fileName, _dict=data)
+                from common.file.handle_system import adjust_path
+                _path = adjust_path(fileName)
+                content = self.load_xml(_path, _dict=data)
             elif fileName.find(".yaml") >= 0:
                 if fileName.find(".yaml|") >= 0:
                     from common.plugin.yaml_plugin import YamlPlugin
                     _arr = fileName.split('|')
-                    content = YamlPlugin.load_data(_arr[0], _arr[1])
+                    from common.file.handle_system import adjust_path
+                    _path = adjust_path(_arr[0])
+                    content = YamlPlugin.load_data(_path, _arr[1])
                 else:
+                    from common.file.handle_system import adjust_path
+                    _path = adjust_path(fileName)
                     from common.plugin.yaml_plugin import YamlPlugin
-                    content = YamlPlugin.load_data(fileName)
+                    content = YamlPlugin.load_data(_path)
         except Exception as e:
-            logger.info(f'{fileName}文件内容不存在')
+            logger.warning(f'{fileName}文件内容不存在')
         return content
 
 
     @classmethod
     def excel_to_dict(self, file_name, sheet: str='Sheet1', _filter: dict=None, _index:int=1, _replace: bool=True, file_path: str=TEST_DATA_PATH):
         """
            读取Excel中特定sheet的数据，按行将数据存入数组datalist[从第二行开始读数据】
```

### Comparing `auto-test-common-1.1.93/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.95/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.95/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.95/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/template_plugin.py` & `auto-test-common-1.1.95/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.95/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.93/setup.py` & `auto-test-common-1.1.95/setup.py`

 * *Files identical despite different names*

