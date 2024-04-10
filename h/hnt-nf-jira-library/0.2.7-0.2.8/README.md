# Comparing `tmp/hnt_nf_jira_library-0.2.7.tar.gz` & `tmp/hnt_nf_jira_library-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.7.tar", last modified: Wed Apr 10 12:38:34 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.2.8.tar", last modified: Wed Apr 10 14:24:20 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.7.tar` & `hnt_nf_jira_library-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.159654 hnt_nf_jira_library-0.2.7/
--rw-rw-rw-   0        0        0      286 2024-04-10 12:38:34.155655 hnt_nf_jira_library-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.152655 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 12:38:33.000000 hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.099648 hnt_nf_jira_library-0.2.7/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.7/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:38:34.145654 hnt_nf_jira_library-0.2.7/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/chave_acesso.py
--rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.7/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    16509 2024-04-10 12:37:26.000000 hnt_nf_jira_library-0.2.7/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-10 12:38:34.160657 hnt_nf_jira_library-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-04-10 12:38:21.000000 hnt_nf_jira_library-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:24:20.248579 hnt_nf_jira_library-0.2.8/
+-rw-rw-rw-   0        0        0      286 2024-04-10 14:24:20.244577 hnt_nf_jira_library-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:24:20.242581 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-10 14:24:19.000000 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-04-10 14:24:20.000000 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:24:19.000000 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-10 14:24:19.000000 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 14:24:19.000000 hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:24:20.173572 hnt_nf_jira_library-0.2.8/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.8/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:24:20.221576 hnt_nf_jira_library-0.2.8/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:24:20.237578 hnt_nf_jira_library-0.2.8/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4750 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     1377 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     2941 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/dados_basicos.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.8/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    16509 2024-04-10 12:37:26.000000 hnt_nf_jira_library-0.2.8/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:24:20.249578 hnt_nf_jira_library-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-10 14:22:55.000000 hnt_nf_jira_library-0.2.8/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.7/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.2.8/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,8 +16,12 @@
 nf_jira/entities/item.py
 nf_jira/entities/jira_info.py
 nf_jira/entities/miro.py
 nf_jira/entities/nfe_sefaz.py
 nf_jira/entities/nota_pedido.py
 nf_jira/entities/referencia_pedido.py
 nf_jira/entities/sintese_itens.py
-nf_jira/entities/sintese_miro.py
+nf_jira/entities/sintese_miro.py
+nf_jira/entities/classes/form_jira.py
+nf_jira/entities/classes/helper.py
+nf_jira/entities/classes/issue_fields.py
+nf_jira/entities/classes/issue_jira.py
```

### Comparing `hnt_nf_jira_library-0.2.7/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.2.8/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.7/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.2.8/nf_jira/wrapper_nf_jira.py`

 * *Files identical despite different names*

