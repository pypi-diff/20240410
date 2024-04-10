# Comparing `tmp/tikit-1.6.8.240306.tar.gz` & `tmp/tikit-1.7.1.240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikit-1.6.8.240306.tar", last modified: Wed Mar  6 06:51:36 2024, max compression
+gzip compressed data, was "tikit-1.7.1.240409.tar", last modified: Wed Apr 10 11:49:09 2024, max compression
```

## Comparing `tikit-1.6.8.240306.tar` & `tikit-1.7.1.240409.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.559244 tikit-1.6.8.240306/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)       71 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/MANIFEST.in
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1503 2024-03-06 06:51:36.558925 tikit-1.6.8.240306/PKG-INFO
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      499 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/README.md
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      413 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/requirements.txt
--rw-r--r--   0 zoeyjiali   (501) staff       (20)       38 2024-03-06 06:51:36.559320 tikit-1.6.8.240306/setup.cfg
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      858 2024-03-06 06:47:04.000000 tikit-1.6.8.240306/setup.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.542562 tikit-1.6.8.240306/tikit/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      185 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     7896 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/cli.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)   217718 2024-03-06 06:47:04.000000 tikit-1.6.8.240306/tikit/client.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     3976 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/default_client.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.545397 tikit-1.6.8.240306/tikit/display_optimize/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      133 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/display_optimize/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     3820 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/display_optimize/dataset.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     2242 2024-02-23 06:48:46.000000 tikit-1.6.8.240306/tikit/display_optimize/resource_group.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     4933 2023-08-31 11:08:06.000000 tikit-1.6.8.240306/tikit/display_optimize/training_model.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    12302 2023-08-31 11:08:06.000000 tikit-1.6.8.240306/tikit/display_optimize/training_task.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1779 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/hdfs.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    35625 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/hive.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    20234 2024-02-29 06:21:02.000000 tikit-1.6.8.240306/tikit/models.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.545846 tikit-1.6.8.240306/tikit/templates/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     7622 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/templates/service_config.yaml
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.546093 tikit-1.6.8.240306/tikit/tencentcloud/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      630 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.547772 tikit-1.6.8.240306/tikit/tencentcloud/common/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    16473 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     2337 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     2002 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    12338 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.548281 tikit-1.6.8.240306/tikit/tencentcloud/common/exception/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      741 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      760 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.548756 tikit-1.6.8.240306/tikit/tencentcloud/common/http/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     5071 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.549680 tikit-1.6.8.240306/tikit/tencentcloud/common/profile/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1657 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1857 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1574 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.549971 tikit-1.6.8.240306/tikit/tencentcloud/emr/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.550986 tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     6015 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     3465 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    33848 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.551372 tikit-1.6.8.240306/tikit/tencentcloud/tione/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.554090 tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    12419 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)   768274 2024-02-23 06:48:46.000000 tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)   262984 2024-02-23 06:48:46.000000 tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.556630 tikit-1.6.8.240306/tikit/tencentcloud/wedata/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.558082 tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        0 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      819 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)    19834 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     4802 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      893 2023-08-28 11:15:01.000000 tikit-1.6.8.240306/tikit/util.py
-drwxr-xr-x   0 zoeyjiali   (501) staff       (20)        0 2024-03-06 06:51:36.558441 tikit-1.6.8.240306/tikit.egg-info/
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1503 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/PKG-INFO
--rw-r--r--   0 zoeyjiali   (501) staff       (20)     1883 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        1 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 zoeyjiali   (501) staff       (20)       40 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/entry_points.txt
--rw-r--r--   0 zoeyjiali   (501) staff       (20)      413 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/requires.txt
--rw-r--r--   0 zoeyjiali   (501) staff       (20)        6 2024-03-06 06:51:36.000000 tikit-1.6.8.240306/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      700 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/README.md
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      858 2024-04-09 13:14:07.000000 tikit-1.7.1.240409/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/
+-rw-r--r--   0 root         (0) root         (0)      185 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7896 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/cli.py
+-rw-r--r--   0 root         (0) root         (0)   218778 2024-04-10 11:48:19.000000 tikit-1.7.1.240409/tikit/client.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/default_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/display_optimize/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/resource_group.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/training_model.py
+-rw-r--r--   0 root         (0) root         (0)    12329 2024-04-09 13:08:11.000000 tikit-1.7.1.240409/tikit/display_optimize/training_task.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    35625 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/hive.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/templates/
+-rw-r--r--   0 root         (0) root         (0)     7622 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/templates/service_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16473 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/common_client.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5071 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/http/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6015 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    33848 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12419 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   769939 2024-04-10 11:48:19.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)   263659 2024-04-09 13:08:11.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      819 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19834 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      700 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/top_level.txt
```

### Comparing `tikit-1.6.8.240306/setup.py` & `tikit-1.7.1.240409/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.6.8.240306',
+    version='1.7.1.240409',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.6.8.240306/tikit/cli.py` & `tikit-1.7.1.240409/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/client.py` & `tikit-1.7.1.240409/tikit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import re
 import time
 import os
 import json
 import types
 import datetime
+import base64
 from typing import List
 
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from qcloud_cos.cos_threadpool import SimpleThreadPool
 
 from tikit.tencentcloud.common import credential
@@ -923,17 +924,21 @@
                     rdma_config.Enable = enable_rdma
                     ps_info.RDMAConfig = rdma_config
                 req.ResourceConfigInfos.append(ps_info)
 
             req.Output = self.parse_cos_info(cos_output) if cos_output else None
             req.Tags = tags
             req.CodePackagePath = self.parse_cos_info(code_package_path) if code_package_path else None
-            req.StartCmdInfo = models.StartCmdInfo()
-            req.StartCmdInfo.WorkerStartCmd = worker_start_cmd
-            req.StartCmdInfo.PsStartCmd = ps_start_cmd
+
+            start_cmd_info = models.StartCmdInfo()
+            start_cmd_info.WorkerStartCmd = worker_start_cmd
+            start_cmd_info.PsStartCmd = ps_start_cmd
+            req.EncodedStartCmdInfo = models.EncodedStartCmdInfo()
+            req.EncodedStartCmdInfo.StartCmdInfo = base64.b64encode(
+                start_cmd_info.to_json_string().encode('utf-8')).decode('ascii')
 
             if input_data_config is not None:
                 req.DataConfigs, req.DataSource = self._parse_training_task_input_data(input_data_config)
 
             req.TuningParameters = json.dumps(tuning_parameters_dict)
             req.Remark = remark
             req.LogEnable = log_enable
@@ -2554,14 +2559,16 @@
                         worker_info.InstanceTypeAlias = v.SpecAlias
                         break
                 if worker_info.InstanceType is None:
                     raise Exception("please enter the correct InstanceType: %s" % resource_config_info.InstanceType)
             req.ResourceConfigInfo = worker_info
 
             req.StartCmd = start_cmd
+            if start_cmd is not None:
+                req.StartCmdBase64 = base64.b64encode(start_cmd.encode()).decode("utf-8")
 
             if log_enable:
                 req.LogConfig = models.LogConfig()
                 req.LogConfig.LogsetId = log_logset_id
                 req.LogConfig.TopicId = log_topic_id
             req.LogEnable = log_enable
 
@@ -2699,15 +2706,16 @@
                                      log_enable=False,
                                      log_logset_id=None,
                                      log_topic_id=None,
                                      authorization_enable=False,
                                      tags=None,
                                      cron_scale_jobs=None,
                                      scale_strategy=None,
-                                     hybrid_billing_prepaid_replicas=None):
+                                     hybrid_billing_prepaid_replicas=None,
+                                     command=None):
 
         """创建模型服务版本
 
         :param worker_resource:        worker节点的配置
         :type worker_resource:         :class:`tikit.models.ModelServiceResourceConfigInfo`
         :param framework:              运行的框架环境
         :type framework:               :class:`tikit.models.FrameworkInfo`
@@ -2751,24 +2759,26 @@
         :type cron_scale_jobs:         list of :class:`tikit.tencentcloud.tione.v20211111.models.CronScaleJob`
         :param scale_strategy:         自动伸缩策略配置 HPA
         :type scale_strategy:          str
         :param hybrid_billing_prepaid_replicas: 混合计费模式下预付费实例数
         :type hybrid_billing_prepaid_replicas:  int
         :param model_hot_update_enable: 是否开启模型的热更新。默认不开启
         :type model_hot_update_enable: bool
+        :param command:                启动命令
+        :type command:                 str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateModelServiceResponse`
         """
 
         return self._create_model_service_do("", worker_resource, framework, service_group_id,
                                             service_description, resource_group_id, model_config_info, model_cos_path,
                                             volume_mount, service_limit, scheduled_action, model_hot_update_enable,
                                             env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
                                             log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
-                                            scale_strategy, hybrid_billing_prepaid_replicas, True, model_hot_update_enable)
+                                            scale_strategy, hybrid_billing_prepaid_replicas,command,True)
 
     def create_model_service(self,
                             service_group_name,
                             worker_resource,
                             framework=None,
                             service_description=None,
                             resource_group_id=None,
@@ -2785,15 +2795,16 @@
                             log_enable=False,
                             log_logset_id=None,
                             log_topic_id=None,
                             authorization_enable=False,
                             tags=None,
                             cron_scale_jobs=None,
                             scale_strategy=None,
-                            hybrid_billing_prepaid_replicas=None):
+                            hybrid_billing_prepaid_replicas=None,
+                            command=None):
 
         """创建模型服务
 
         :param service_group_name:     服务名称
         :type service_group_name:      str
         :param worker_resource:        worker节点的配置
         :type worker_resource:         :class:`tikit.models.ModelServiceResourceConfigInfo`
@@ -2835,24 +2846,26 @@
         :type tags:                    list of :class:`tikit.tencentcloud.tione.v20211111.models.Tag`
         :param cron_scale_jobs:        定时任务配置
         :type cron_scale_jobs:         list of :class:`tikit.tencentcloud.tione.v20211111.models.CronScaleJob`
         :param scale_strategy:         自动伸缩策略配置 HPA
         :type scale_strategy:          str
         :param hybrid_billing_prepaid_replicas: 混合计费模式下预付费实例数
         :type hybrid_billing_prepaid_replicas:  int
+        :param command:                启动命令
+        :type command:                 str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateModelServiceResponse`
         """
 
         return self._create_model_service_do(service_group_name, worker_resource, framework, "",
                                             service_description, resource_group_id, model_config_info, model_cos_path,
                                             volume_mount, service_limit, scheduled_action, model_hot_update_enable,
                                             env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
                                             log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
-                                            scale_strategy, hybrid_billing_prepaid_replicas, False)
+                                            scale_strategy, hybrid_billing_prepaid_replicas, command,False)
 
     def create_taiji_model_service(self,
                                      service_name,
                                      service_description,
                                      model_version_id,
                                      instance_type,
                                      replicas=1,
@@ -3177,14 +3190,15 @@
                                 log_logset_id=None,
                                 log_topic_id=None,
                                 authorization_enable=False,
                                 tags=None,
                                 cron_scale_jobs=None,
                                 scale_strategy=None,
                                 hybrid_billing_prepaid_replicas=None,
+                                command=None,
                                 new_version=False):
         """创建模型服务
 
         :param service_group_name:     服务名称
         :type service_group_name:      str
         :param worker_resource:        worker节点的配置
         :type worker_resource:         :class:`tikit.models.ModelServiceResourceConfigInfo`
@@ -3241,14 +3255,15 @@
         """
 
         try:
             req = models.CreateModelServiceRequest()
             req.ServiceGroupName = service_group_name
             charge_type = worker_resource.ChargeType
             req.ChargeType = charge_type
+            req.Command = command
 
             if not framework:
                 if not model_config_info or not model_config_info.ModelVersionId:
                     raise ValueError("framework should not be empty when no models chosen")
                 modelInfo = self.describe_training_model_version(model_config_info.ModelVersionId)
                 framework = TiModels.FrameworkInfo.new_custom_image(
                                                                     "PRESET",
@@ -3307,14 +3322,17 @@
                 req.LogConfig.TopicId = log_topic_id
             req.AuthorizationEnable = authorization_enable
             req.Tags = tags
             req.CronScaleJobs = cron_scale_jobs
             req.ScaleStrategy = scale_strategy
             req.HybridBillingPrepaidReplicas = hybrid_billing_prepaid_replicas
             req.NewVersion = new_version
+            #
+            if req.Command is not None:
+                req.CommandBase64 = base64.b64encode(req.Command.encode()).decode("utf-8")
 
             print(req._serialize())
             return self._tione_client.CreateModelService(req)
         except TencentCloudSDKException as err:
             raise
 
     def _modify_model_service_from_file(self, filename: str):
@@ -3476,14 +3494,15 @@
                              log_logset_id=None,
                              log_topic_id=None,
                              service_action=None,
                              service_description=None,
                              scale_strategy=None,
                              cron_scale_jobs=None,
                              hybrid_billing_prepaid_replicas=None,
+                             command=None,
                              )->models.ModifyModelServiceResponse:
         """更新模型服务版本
 
         :param service_id:                 服务版本id
         :type service_id:                  str
         :param model_config_info:          模型信息
         :type model_config_info:           :class:`tikit.models.ModelConfigInfo`
@@ -3528,14 +3547,15 @@
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.ModifyModelServiceResponse`
         """
 
         try:            
             req = models.ModifyModelServiceRequest()
             req.ServiceId = service_id
+            req.Command = command
 
             if model_config_info is not None:
                 req.ModelInfo = models.ModelInfo()
                 req.ModelInfo.ModelId = model_config_info.ModelId
                 req.ModelInfo.ModelName = model_config_info.ModelName
                 req.ModelInfo.ModelVersionId = model_config_info.ModelVersionId
                 req.ModelInfo.ModelVersion = model_config_info.ModelVersion
@@ -3583,14 +3603,16 @@
                 req.LogConfig.TopicId = log_topic_id
 
             req.ServiceAction = service_action
             req.ServiceDescription = service_description
             req.ScaleStrategy = scale_strategy
             req.CronScaleJobs = cron_scale_jobs
             req.HybridBillingPrepaidReplicas = hybrid_billing_prepaid_replicas
+            if req.Command is not None:
+                req.CommandBase64 = base64.b64encode(req.Command.encode()).decode("utf-8")
 
             print(req._serialize())
             return self._tione_client.ModifyModelService(req)
         except TencentCloudSDKException as err:
             raise
         
     def patch_model_service(self,
```

### Comparing `tikit-1.6.8.240306/tikit/default_client.py` & `tikit-1.7.1.240409/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/display_optimize/dataset.py` & `tikit-1.7.1.240409/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/display_optimize/resource_group.py` & `tikit-1.7.1.240409/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/display_optimize/training_model.py` & `tikit-1.7.1.240409/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/display_optimize/training_task.py` & `tikit-1.7.1.240409/tikit/display_optimize/training_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     :param taiji_hy_template_list_response: the response
     :type DescribeTAIJITemplateListResponse:   :class:`tikit.tencentcloud.tione.v20211111.models.DescribeTAIJITemplateListResponse`
     :return: pretty table
     :rtype: PrettyTable
     """
     table = PrettyTable()
     template_list = taiji_hy_template_list_response.TemplateList
-    if len(template_list) < 0:
+    if  template_list is None or len(template_list) <= 0:
         return table
     table.field_names = [ 
         "模版名称",
         "模版描述",
         "模型ID",
         "训练模式",
         "配置方式",
```

### Comparing `tikit-1.6.8.240306/tikit/hdfs.py` & `tikit-1.7.1.240409/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/hive.py` & `tikit-1.7.1.240409/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/models.py` & `tikit-1.7.1.240409/tikit/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/templates/service_config.yaml` & `tikit-1.7.1.240409/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/__init__.py` & `tikit-1.7.1.240409/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/common_client.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/credential.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/http/request.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/common/sign.py` & `tikit-1.7.1.240409/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1759,14 +1759,16 @@
         :type ModelInfo: :class:`tencentcloud.tione.v20211111.models.ModelInfo`
         :param ImageInfo: 自定义镜像信息
         :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
         :param CodePackage: 代码包
         :type CodePackage: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         :param StartCmd: 启动命令
         :type StartCmd: str
+        :param StartCmdBase64: 按照Base64编码的启动命令
+        :type StartCmdBase64: str
         :param DataConfigs: 数据配置
         :type DataConfigs: list of DataConfig
         :param LogConfig: 日志配置
         :type LogConfig: :class:`tencentcloud.tione.v20211111.models.LogConfig`
         :param VpcId: VPC Id
         :type VpcId: str
         :param SubnetId: 子网Id
@@ -1783,14 +1785,15 @@
         self.CronInfo = None
         self.ResourceGroupId = None
         self.Tags = None
         self.ModelInfo = None
         self.ImageInfo = None
         self.CodePackage = None
         self.StartCmd = None
+        self.StartCmdBase64 = None
         self.DataConfigs = None
         self.LogConfig = None
         self.VpcId = None
         self.SubnetId = None
         self.Remark = None
 
 
@@ -1824,14 +1827,15 @@
         if params.get("ImageInfo") is not None:
             self.ImageInfo = ImageInfo()
             self.ImageInfo._deserialize(params.get("ImageInfo"))
         if params.get("CodePackage") is not None:
             self.CodePackage = CosPathInfo()
             self.CodePackage._deserialize(params.get("CodePackage"))
         self.StartCmd = params.get("StartCmd")
+        self.StartCmdBase64 = params.get("StartCmdBase64")
         if params.get("DataConfigs") is not None:
             self.DataConfigs = []
             for item in params.get("DataConfigs"):
                 obj = DataConfig()
                 obj._deserialize(item)
                 self.DataConfigs.append(obj)
         if params.get("LogConfig") is not None:
@@ -2719,14 +2723,16 @@
         self.HybridBillingPrepaidReplicas = None
         self.CreateSource = None
         self.ModelHotUpdateEnable = None
         self.ScheduledAction = None
         self.VolumeMount = None
         self.ServiceLimit = None
         self.ServiceCategory = None
+        self.Command = None
+        self.CommandBase64= None
 
 
     def _deserialize(self, params):
         if params.get("ImageInfo") is not None:
             self.ImageInfo = ImageInfo()
             self.ImageInfo._deserialize(params.get("ImageInfo"))
         self.ServiceGroupId = params.get("ServiceGroupId")
@@ -3387,14 +3393,16 @@
         :type TaskId: str
         :param DataSource: 数据来源，eg：DATASET、COS、CFS、HDFS
         :type DataSource: str
         :param TAIJITemplateId: 太极训练模版ID，eg：DATASET、COS、CFS、HDFS
         :type TAIJITemplateId: str
         :param PreTrainModel: 预训练模型信息
         :type PreTrainModel: class:`tencentcloud.tione.v20211111.models.PreTrainModel`
+        :param EncodedStartCmdInfo: 编码后的启动命令信息
+        :type EncodedStartCmdInfo: :class:`tencentcloud.tione.v20211111.models.EncodedStartCmdInfo`
         """
         self.Name = None
         self.ChargeType = None
         self.ResourceConfigInfos = None
         self.CodePackagePath = None
         self.TrainingMode = None
         self.Output = None
@@ -3413,14 +3421,15 @@
         self.TuningParameters = None
         self.Remark = None
         self.TaskType = None
         self.TaskId = None
         self.DataSource = None
         self.TAIJITemplateId = None
         self.PreTrainModel = None
+        self.EncodedStartCmdInfo = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.ChargeType = params.get("ChargeType")
         if params.get("ResourceConfigInfos") is not None:
             self.ResourceConfigInfos = []
@@ -3469,14 +3478,17 @@
         self.TaskId = params.get("TaskId")
         self.DataSource = params.get("DataSource")
         if params.get("TAIJITemplateId") is not None:
             self.TAIJITemplateId = params.get("TAIJITemplateId")
         if params.get("PreTrainModel") is not None:
             self.PreTrainModel = PreTrainModel()
             self.PreTrainModel._deserialize(params.get("PreTrainModel"))
+        if params.get("EncodedStartCmdInfo") is not None:
+            self.EncodedStartCmdInfo = EncodedStartCmdInfo()
+            self.EncodedStartCmdInfo._deserialize(params.get("EncodedStartCmdInfo"))
 
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3840,14 +3852,37 @@
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
+class EncodedStartCmdInfo(AbstractModel):
+    """编码后的启动命令信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartCmdInfo: JSON 序列化 StartCmdInfo 结构体后再使用 Base64 编码的启动命令
+        :type StartCmdInfo: str
+        """
+        self.StartCmdInfo = None
+
+
+    def _deserialize(self, params):
+        self.StartCmdInfo = params.get("StartCmdInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
 
 class DatasetConfigs(AbstractModel):
     """自动学习数据集配置信息
 
     """
 
     def __init__(self):
@@ -15497,14 +15532,16 @@
         self.CronScaleJobs = None
         self.HybridBillingPrepaidReplicas = None
         self.ModelHotUpdateEnable = None
         self.ScheduledAction = None
         self.ServiceLimit = None
         self.VolumeMount = None
         self.AuthorizationEnable = None
+        self.Command = None
+        self.CommandBase64 = None
 
 
     def _deserialize(self, params):
         self.ServiceId = params.get("ServiceId")
         if params.get("ModelInfo") is not None:
             self.ModelInfo = ModelInfo()
             self.ModelInfo._deserialize(params.get("ModelInfo"))
@@ -18741,14 +18778,17 @@
         :type HybridBillingPrepaidReplicas: int
         :param OldHybridBillingPrepaidReplicas: 历史 HYBRID_PAID 时的实例数，用户恢复服务
 注意：此字段可能返回 null，表示取不到有效值。
         :type OldHybridBillingPrepaidReplicas: int
         :param ModelHotUpdateEnable: 是否开启模型的热更新。默认不开启
 注意：此字段可能返回 null，表示取不到有效值。
         :type ModelHotUpdateEnable: bool
+        :param Command: 启动命令
+        :type Command: str
+注意：此字段可能返回 null，表示取不到有效值。
         """
         self.Replicas = None
         self.ImageInfo = None
         self.Env = None
         self.Resources = None
         self.InstanceType = None
         self.ModelInfo = None
@@ -18760,14 +18800,15 @@
         self.Weight = None
         self.PodList = None
         self.ResourceTotal = None
         self.OldReplicas = None
         self.HybridBillingPrepaidReplicas = None
         self.OldHybridBillingPrepaidReplicas = None
         self.ModelHotUpdateEnable = None
+        self.Command = None
 
 
     def _deserialize(self, params):
         self.Replicas = params.get("Replicas")
         if params.get("ImageInfo") is not None:
             self.ImageInfo = ImageInfo()
             self.ImageInfo._deserialize(params.get("ImageInfo"))
@@ -18800,14 +18841,15 @@
         if params.get("ResourceTotal") is not None:
             self.ResourceTotal = ResourceInfo()
             self.ResourceTotal._deserialize(params.get("ResourceTotal"))
         self.OldReplicas = params.get("OldReplicas")
         self.HybridBillingPrepaidReplicas = params.get("HybridBillingPrepaidReplicas")
         self.OldHybridBillingPrepaidReplicas = params.get("OldHybridBillingPrepaidReplicas")
         self.ModelHotUpdateEnable = params.get("ModelHotUpdateEnable")
+        self.Command = params.get("Command")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6025,18 +6025,24 @@
         :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeTAIJITemplateResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTAIJITemplate", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeTAIJITemplateResponse()
-            model._deserialize(response["Response"])
-            return model
+            response = json.loads(body) 
+            if "Error" not in response["Response"]:
+                model = models.DescribeTAIJITemplateResponse()
+                model._deserialize(response["Response"])
+                return model
+            else:
+                code = response["Response"]["Error"]["Code"]
+                message = response["Response"]["Error"]["Message"]
+                reqid = response["Response"]["RequestId"]
+                raise TencentCloudSDKException(code, message, reqid)
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
@@ -6049,15 +6055,21 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTAIJITemplateList", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeTAIJITemplateListResponse()
-            model._deserialize(response["Response"])
-            return model
+            if "Error" not in response["Response"]:
+                model = models.DescribeTAIJITemplateListResponse()
+                model._deserialize(response["Response"])
+                return model
+            else:
+                code = response["Response"]["Error"]["Code"]
+                message = response["Response"]["Error"]["Message"]
+                reqid = response["Response"]["RequestId"]
+                raise TencentCloudSDKException(code, message, reqid)
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit/util.py` & `tikit-1.7.1.240409/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.6.8.240306/tikit.egg-info/SOURCES.txt` & `tikit-1.7.1.240409/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

