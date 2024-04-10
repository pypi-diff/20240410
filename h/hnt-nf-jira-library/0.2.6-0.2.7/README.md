# Comparing `tmp/hnt_nf_jira_library-0.2.6.tar.gz` & `tmp/hnt_nf_jira_library-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.6.tar", last modified: Wed Apr 10 12:13:39 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.2.7.tar", last modified: Wed Apr 10 12:38:34 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.6.tar` & `hnt_nf_jira_library-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.454932 hnt_nf_jira_library-0.2.6/
--rw-rw-rw-   0        0        0      286 2024-04-10 12:13:39.450940 hnt_nf_jira_library-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.446929 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.402927 hnt_nf_jira_library-0.2.6/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.6/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.443931 hnt_nf_jira_library-0.2.6/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/chave_acesso.py
--rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    16472 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-10 12:13:39.455933 hnt_nf_jira_library-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-04-10 12:13:33.000000 hnt_nf_jira_library-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.159654 hnt_nf_jira_library-0.2.7/
+-rw-rw-rw-   0        0        0      286 2024-04-10 12:38:34.155655 hnt_nf_jira_library-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.152655 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.099648 hnt_nf_jira_library-0.2.7/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.7/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.145654 hnt_nf_jira_library-0.2.7/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/chave_acesso.py
+-rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/dados_basicos.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    16509 2024-04-10 12:37:26.000000 hnt_nf_jira_library-0.2.7/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:38:34.160657 hnt_nf_jira_library-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-04-10 12:38:21.000000 hnt_nf_jira_library-0.2.7/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.6/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.2.7/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.6/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.2.7/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             "path": issue["pdf_data"]["path_dir"],
             "filename": issue["pdf_data"]["filename"],
         }
 
         nota_pedido = {
             "tipo": "ZCOR",
             "org_compras": issue["domain_data"]["centro"]["org_compras"],
-            "grp_compradores": "S01",
+            "grp_compradores": issue['json_data']['grupo_compradores'][0],
             "empresa": "HFNT",
             "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
             "sintese_itens": sintese_itens,
             "anexo": anexo,
             "jira_info": issue["jira_info"],
         }
```

