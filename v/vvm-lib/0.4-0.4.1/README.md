# Comparing `tmp/vvm_lib-0.4.tar.gz` & `tmp/vvm_lib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-0.4.tar", last modified: Fri Apr  5 12:47:38 2024, max compression
+gzip compressed data, was "vvm_lib-0.4.1.tar", last modified: Wed Apr 10 05:49:26 2024, max compression
```

## Comparing `vvm_lib-0.4.tar` & `vvm_lib-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.690784 vvm_lib-0.4/
--rw-rw-rw-   0        0        0      428 2024-04-05 12:47:38.689779 vvm_lib-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-04-05 12:46:01.000000 vvm_lib-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 12:47:38.699807 vvm_lib-0.4/setup.cfg
--rw-rw-rw-   0        0        0      574 2024-04-05 12:43:44.000000 vvm_lib-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.666685 vvm_lib-0.4/vvm_lib/
--rw-rw-rw-   0        0        0      229 2024-04-04 10:13:09.000000 vvm_lib-0.4/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-04-05 12:41:47.000000 vvm_lib-0.4/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     3545 2024-04-05 12:43:44.000000 vvm_lib-0.4/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      654 2024-04-05 12:43:44.000000 vvm_lib-0.4/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      807 2024-04-05 12:29:39.000000 vvm_lib-0.4/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.689779 vvm_lib-0.4/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      428 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 09:46:15.000000 vvm_lib-0.4/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 05:49:26.163828 vvm_lib-0.4.1/
+-rw-rw-rw-   0        0        0      454 2024-04-10 05:49:26.163828 vvm_lib-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-09 13:19:33.000000 vvm_lib-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 05:49:26.167827 vvm_lib-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      624 2024-04-10 05:47:46.000000 vvm_lib-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 05:49:26.142470 vvm_lib-0.4.1/vvm_lib/
+-rw-rw-rw-   0        0        0      229 2024-04-09 13:19:33.000000 vvm_lib-0.4.1/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-04-09 13:19:33.000000 vvm_lib-0.4.1/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     3545 2024-04-09 13:19:33.000000 vvm_lib-0.4.1/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      654 2024-04-09 13:19:33.000000 vvm_lib-0.4.1/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      855 2024-04-10 05:47:46.000000 vvm_lib-0.4.1/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-10 05:49:26.162830 vvm_lib-0.4.1/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 05:49:26.000000 vvm_lib-0.4.1/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-0.4/vvm_lib/google_book.py` & `vvm_lib-0.4.1/vvm_lib/google_book.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4/vvm_lib/greenplum.py` & `vvm_lib-0.4.1/vvm_lib/greenplum.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4/vvm_lib/mssql.py` & `vvm_lib-0.4.1/vvm_lib/mssql.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4/vvm_lib/vault.py` & `vvm_lib-0.4.1/vvm_lib/vault.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import hvac
+import urllib3
 
 
 def read_secret_data(secret_path: str, vault_token_env: str = "DATA_VAULT_TOKEN",
                      url: str='https://secure-vault.srv.goods.local'):
     """
     Функция для получения доступов из vault
     :param secret_path: Название секрета в DAS_team
     :param vault_token_env: токент доступа
     :param url: url vault
     :return: Словарь с секретами
 
     пример:
         secret_data = read_secret_data('ИМЯ', token_vault)
     """
+    urllib3.disable_warnings()
     client = hvac.Client(url, token=vault_token_env, verify=False)
     assert client.is_authenticated()
     secret = client.secrets.kv.v1.read_secret(path=f'goods/merchants/DAS_team/{secret_path}', mount_point='secrets')
     return secret.get('data')
```

