# Comparing `tmp/pih-ds-0.12.tar.gz` & `tmp/pih-ds-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ds-0.12.tar", last modified: Wed Mar 13 14:14:15 2024, max compression
+gzip compressed data, was "pih-ds-0.13.tar", last modified: Wed Apr 10 01:29:49 2024, max compression
```

## Comparing `pih-ds-0.12.tar` & `pih-ds-0.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:14:15.804580 pih-ds-0.12/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:14:15.413964 pih-ds-0.12/DataSourceService/
--rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.12/DataSourceService/__init__.py
--rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.12/DataSourceService/__main__.py
--rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.12/DataSourceService/anecdotica.py
--rw-rw-rw-   0        0        0    38013 2024-02-19 04:03:42.000000 pih-ds-0.12/DataSourceService/api.py
--rw-rw-rw-   0        0        0     3309 2024-03-13 14:14:06.000000 pih-ds-0.12/DataSourceService/const.py
--rw-rw-rw-   0        0        0     9780 2024-03-13 07:33:29.000000 pih-ds-0.12/DataSourceService/service.py
--rw-rw-rw-   0        0        0      100 2024-02-13 00:15:00.000000 pih-ds-0.12/DataSourceService/test.py
--rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.12/DataSourceService/tools.py
--rw-rw-rw-   0        0        0      394 2024-03-13 14:14:15.757703 pih-ds-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 14:14:15.726453 pih-ds-0.12/pih_ds.egg-info/
--rw-rw-rw-   0        0        0      394 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-13 14:14:14.000000 pih-ds-0.12/pih_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 14:14:15.820201 pih-ds-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:29:49.203405 pih-ds-0.13/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:29:48.412367 pih-ds-0.13/DataSourceService/
+-rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.13/DataSourceService/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.13/DataSourceService/__main__.py
+-rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.13/DataSourceService/anecdotica.py
+-rw-rw-rw-   0        0        0    38013 2024-02-19 04:03:42.000000 pih-ds-0.13/DataSourceService/api.py
+-rw-rw-rw-   0        0        0     3309 2024-04-09 23:56:15.000000 pih-ds-0.13/DataSourceService/const.py
+-rw-rw-rw-   0        0        0     9780 2024-03-13 07:33:29.000000 pih-ds-0.13/DataSourceService/service.py
+-rw-rw-rw-   0        0        0      100 2024-02-13 00:15:00.000000 pih-ds-0.13/DataSourceService/test.py
+-rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.13/DataSourceService/tools.py
+-rw-rw-rw-   0        0        0      394 2024-04-10 01:29:49.187781 pih-ds-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:29:49.140907 pih-ds-0.13/pih_ds.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:29:49.219033 pih-ds-0.13/setup.cfg
```

### Comparing `pih-ds-0.12/DataSourceService/anecdotica.py` & `pih-ds-0.13/DataSourceService/anecdotica.py`

 * *Files identical despite different names*

### Comparing `pih-ds-0.12/DataSourceService/api.py` & `pih-ds-0.13/DataSourceService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ds-0.12/DataSourceService/const.py` & `pih-ds-0.13/DataSourceService/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DATABASE_NAME: str = "pih_db"
 DATABASE_PORT: int = 3306
 DATABASE_POOL_SIZE: int = 5
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.12"
+VERSION: str = "0.13"
 
 MODULES: tuple[str, ...] = ("mysql-connector-python", "lmdb==1.4.0", "lmdbm", "dadata")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Data storage and source service",
     host=HOST.NAME,
```

### Comparing `pih-ds-0.12/DataSourceService/service.py` & `pih-ds-0.13/DataSourceService/service.py`

 * *Files identical despite different names*

