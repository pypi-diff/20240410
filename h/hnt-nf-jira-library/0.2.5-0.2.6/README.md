# Comparing `tmp/hnt_nf_jira_library-0.2.5.tar.gz` & `tmp/hnt_nf_jira_library-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.5.tar", last modified: Fri Apr  5 13:33:44 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.2.6.tar", last modified: Wed Apr 10 12:13:39 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.5.tar` & `hnt_nf_jira_library-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.176933 hnt_nf_jira_library-0.2.5/
--rw-rw-rw-   0        0        0      286 2024-04-05 13:33:44.175921 hnt_nf_jira_library-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.172921 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.124440 hnt_nf_jira_library-0.2.5/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.5/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.169769 hnt_nf_jira_library-0.2.5/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/chave_acesso.py
--rw-rw-rw-   0        0        0     1863 2024-04-05 13:32:32.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    23690 2024-04-05 13:33:00.000000 hnt_nf_jira_library-0.2.5/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-05 13:33:44.177919 hnt_nf_jira_library-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-04-05 13:33:25.000000 hnt_nf_jira_library-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.454932 hnt_nf_jira_library-0.2.6/
+-rw-rw-rw-   0        0        0      286 2024-04-10 12:13:39.450940 hnt_nf_jira_library-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.446929 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 12:13:39.000000 hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.402927 hnt_nf_jira_library-0.2.6/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.6/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:13:39.443931 hnt_nf_jira_library-0.2.6/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/chave_acesso.py
+-rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/dados_basicos.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.6/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    16472 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.6/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:13:39.455933 hnt_nf_jira_library-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-04-10 12:13:33.000000 hnt_nf_jira_library-0.2.6/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.2.6/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.5/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.2.6/nf_jira/wrapper_nf_jira.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,44 @@
 import json
 import requests
 import os
 from os import getcwd, path
 from datetime import datetime
-
 from pydantic import ValidationError
+
 from .entities.nota_pedido import NotaPedido
 from .entities.miro import Miro
 from .entities.constants import *
+from .entities.classes.form_jira import FormJira
+from .entities.classes.issue_jira import IssueJira
+from .entities.classes.issue_jira import AttachmentJira
+from .entities.classes.issue_fields import IssueFields
+from .entities.classes.helper import JiraFieldsHelper, JsonHelper
 
 from nf_consumo.consumo_service import ConsumoService
 
 
 class wrapper_jira:
 
     def __init__(self, debug=False):
-        self._auth = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
-        self._n8n_auth = (os.getenv("N8N_USERNAME"), os.getenv("N8N_PASSWORD"))
-        self._api_issue_url = os.getenv("ISSUE_URL")
-        self._api_form_url = os.getenv("FORM_URL")
-        self._cloud_id = os.getenv("CLOUD_ID")
-        self._api_domain_url = os.getenv("DOMAIN_URL")
         self._test_mode = debug
-        self._form_template_automacao = FORM_TEMPLATE_AUTOMACAO
-        self._form_template_complemento = FORM_TEMPLATE_COMPLEMENTO
         self._set_request()
+        self.FormJira         = FormJira()
+        self.IssueJira        = IssueJira()
+        self.AttachmentJira   = AttachmentJira()
+        self.JiraFieldsHelper = JiraFieldsHelper()
+        self.JsonHelper       = JsonHelper()
+        self.IssueFields      = IssueFields()
+        self.ConsumoService   = ConsumoService()
 
     def _set_request(self):
         self._api_headers = {
             "Accept": "application/json",
             "Content-Type": "application/json",
         }
-        self._api_attachment_headers = {
-            "Accept": "*/*",
-        }
-        self._api_atlassian_headers = {
-            "Accept": "application/json",
-            "X-ExperimentalApi": "opt-in",
-        }
-
-    def _remove_null_fields(self, fields):
-        fields_data_without_nulls = {}
-
-        for key, value in fields.items():
-            if value is not None:
-                fields_data_without_nulls[key] = value
-
-        return fields_data_without_nulls
-
-    def _rename_fields(self, fields):
-        fields = self._fields
-        new_fields_data = {}
-
-        for key, value in self._jira_fields.items():
-            if value in fields:
-                if "text" in fields[value]:
-                    new_value = fields[value].get("text")
-                elif "date" in fields[value]:
-                    new_value = fields[value].get("date")
-                elif "value" in fields[value]:
-                    new_value = fields[value].get("value")
-                else:
-                    new_value = fields[value]
-
-                new_fields_data[key] = new_value
-
-        self._fields = new_fields_data
 
     def _issue_factory(self, issue: dict):
 
         sintese_itens = []
         validTotalPercents = 0.0
 
         if not issue["allocation_data"]:
@@ -277,23 +246,21 @@
                 "jira_info": jira_info,
             }
 
             ##### PARSE JSON #####
             issue_model = self._issue_factory(issue)
 
             ##### CREATE MODEL #####
-            nota_pedido = NotaPedido(**issue_model)
+            nota_pedido = NotaPedido(**issue_model).model_dump()
 
             #### SAVE JSON ####
             if self._test_mode:
-                with open("issue_context_model.json", "w") as json_file:
-                    json.dump(nota_pedido.model_dump(), json_file, indent=4)
-
-            return NotaPedido(**issue_model).model_dump()
+                self.JsonHelper.save_json(f'Nota_Pedido_{issue_id}', nota_pedido)
 
+            return nota_pedido
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
     def get_nf_miro_context(self, issue_id: str, cod_sap: str):
@@ -318,224 +285,107 @@
             cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
             centro = self._get_nf_domain("centro", cnpj_centro)
 
             attachment["domain_data"] = {"fornecedor": fornecedor, "centro": centro}
 
             miro_model = self._miro_factory(attachment)
 
-            miro = Miro(**miro_model)
+            miro = Miro(**miro_model).model_dump()
 
             if self._test_mode:
-                with open("miro_context_model.json", "w") as json_file:
-                    json.dump(miro.model_dump(), json_file, indent=4)
+                self.JsonHelper.save_json(f'Miro_{issue_id}', miro)
 
-            return Miro(**miro_model).model_dump()
+            return miro
 
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
     def _get_nf_jira(self, issue_id: str):
         try:
-            #### REQUEST ####
-            issue_request = requests.get(
-                f"{self._api_issue_url}/issue/{issue_id}",
-                headers=self._api_headers,
-                auth=self._auth,
-            )
-            issue_request.raise_for_status()
-            issue_data = issue_request.json()
-
-            form_id_request = requests.get(
-                f"{self._api_form_url}/{self._cloud_id}/issue/{issue_id}/form",
-                headers=self._api_atlassian_headers,
-                auth=self._auth,
-            )
-            form_id_request.raise_for_status()
-            form_json = form_id_request.json()
-
-            for form in form_json:
-                if form.get("formTemplate")["id"] == self._form_template_complemento:
-                    form_id = form.get("id")
-                elif form.get("formTemplate")["id"] == self._form_template_automacao:
-                    automacao_form_id = form.get("id")
-
-            # Get the extra Issue Data From Issue ID and Form ID
-            form_request = requests.get(
-                f"{self._api_form_url}/{self._cloud_id}/issue/{issue_id}/form/{form_id}",
-                headers=self._api_atlassian_headers,
-                auth=self._auth,
-            )
-            form_request.raise_for_status()
-            form_data = form_request.json()
 
-            #### REMOVE NULL FIELDS ####
-            issue_data["fields"] = self._remove_null_fields(issue_data.get("fields"))
+            issue_data = self.IssueJira.get_issue(issue_id)
+            complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
 
-            ### GET ATTACHMENT ###
-            if issue_data.get("fields")["attachment"] is None:
-                raise Exception("Could not find attachment")
+            issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
+            attachment = self.AttachmentJira.get_attachment(issue_data)
 
-            for attachment in issue_data.get("fields")["attachment"]:
-                attachment_id = attachment["id"]
-                attachment = self._get_nf_issue_attachment(attachment_id)
+            nf_type_id = complement_form["tipo_conta"]
 
-                if attachment is not None:
-                    attachment_data = attachment
+            if nf_type_id == "ÁGUA":
+                nf_type = COMPLEMENTO_DE_ÁGUA
 
-            if "58" in form_data["state"]["answers"] is not None:
-                nf_type_id = form_data["state"]["answers"]["58"]["choices"][0]
+            elif nf_type_id == "ENERGIA":
+                nf_type = COMPLEMENTO_DE_ENERGIA
 
-                if nf_type_id == "1":
-                    nf_type = COMPLEMENTO_DE_ÁGUA
-
-                elif nf_type_id == "2":
-                    nf_type = COMPLEMENTO_DE_ENERGIA
-
-                elif nf_type_id == "3":
-                    nf_type = COMPLEMENTO_DE_GÁS
+            elif nf_type_id == "GÁS":
+                nf_type = COMPLEMENTO_DE_GÁS
 
             else:
                 if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
                     nf_type = COMPLEMENTO_DE_ÁGUA
                 elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
                     nf_type = COMPLEMENTO_DE_ENERGIA
                 elif attachment[COMPLEMENTO_DE_GÁS] is not None:
                     nf_type = COMPLEMENTO_DE_GÁS
 
-            attachment[CNPJ_DO_FORNECEDOR] = (
-                form_data["state"]["answers"]["33"]["text"]
-                if "33" in form_data["state"]["answers"]
-                else attachment.get(CNPJ_DO_FORNECEDOR)
-            )
-            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = (
-                form_data["state"]["answers"]["59"]["text"]
-                if "59" in form_data["state"]["answers"]
-                else attachment.get(RAZÃO_SOCIAL_DO_FORNECEDOR)
-            )
-            attachment[CNPJ_DO_CLIENTE] = (
-                form_data["state"]["answers"]["42"]["text"]
-                if "42" in form_data["state"]["answers"]
-                else attachment.get(CNPJ_DO_CLIENTE)
-            )
-            attachment[NÚMERO_DA_FATURA] = (
-                form_data["state"]["answers"]["44"]["text"]
-                if "44" in form_data["state"]["answers"]
-                else attachment.get(NÚMERO_DA_FATURA)
-            )
-            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = (
-                form_data["state"]["answers"]["45"]["text"]
-                if "45" in form_data["state"]["answers"]
-                else attachment.get(NÚMERO_DA_FATURA_DO_FORNECEDOR)
-            )
-            attachment[DATA_DE_EMISSÃO] = (
-                form_data["state"]["answers"]["46"]["date"]
-                if "46" in form_data["state"]["answers"]
-                else attachment.get(DATA_DE_EMISSÃO)
-            )
-            attachment[DATA_DE_VENCIMENTO] = (
-                form_data["state"]["answers"]["47"]["date"]
-                if "47" in form_data["state"]["answers"]
-                else attachment.get(DATA_DE_VENCIMENTO)
-            )
-            attachment[CHAVE_DE_ACESSO_DA_FATURA] = (
-                form_data["state"]["answers"]["49"]["text"]
-                if "49" in form_data["state"]["answers"]
-                else attachment.get(CHAVE_DE_ACESSO_DA_FATURA)
-            )
-            attachment[DATA_DE_REFERÊNCIA] = (
-                form_data["state"]["answers"]["50"]["text"]
-                if "50" in form_data["state"]["answers"]
-                else attachment.get(DATA_DE_REFERÊNCIA)
-            )
-            attachment["numero_log"] = (
-                form_data["state"]["answers"]["52"]["text"]
-                if "52" in form_data["state"]["answers"]
-                else attachment.get("numero_log")
-            )
-            attachment["data_procmto"] = (
-                form_data["state"]["answers"]["53"]["date"]
-                if "53" in form_data["state"]["answers"]
-                else attachment.get("data_procmto")
-            )
-            attachment["hora_procmto"] = (
-                form_data["state"]["answers"]["54"]["text"]
-                if "54" in form_data["state"]["answers"]
-                else attachment.get("hora_procmto")
-            )
-            attachment[nf_type]["DataLeituraAnterior"] = (
-                form_data["state"]["answers"]["55"]["date"]
-                if "55" in form_data["state"]["answers"]
-                else attachment[nf_type].get("DataLeituraAnterior")
-            )
-            attachment[nf_type]["DataLeituraAtual"] = (
-                form_data["state"]["answers"]["56"]["date"]
-                if "56" in form_data["state"]["answers"]
-                else attachment[nf_type].get("DataLeituraAtual")
-            )
+            attachment[CNPJ_DO_FORNECEDOR] = complement_form['cnpj_fornecedor']
+            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = complement_form['razao_social_fornecedor']
 
-            # Validação de Valor Liquido da Fatura
-            if "62" in form_data["state"]["answers"]:
-                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["62"][
-                    "text"
-                ]
-            elif "48" in form_data["state"]["answers"]:
-                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["48"][
-                    "text"
-                ]
+            attachment[CNPJ_DO_CLIENTE] = complement_form['cnpj_destinatario']
+            attachment[NÚMERO_DA_FATURA] = complement_form['nro_nota_fiscal']
+            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = complement_form['nro_fatura']
+            attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
+            attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
+            attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
+            attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
+            attachment["numero_log"] = complement_form['protocolo_autorizacao']
+            attachment["data_procmto"] = complement_form['data_autorizacao']
+            attachment["hora_procmto"] = complement_form['hora_autorizacao']
+            attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
+            attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
+            attachment["grupo_compradores"] = complement_form['grupo_compradores']
+            attachment["grupo_compradores"] = complement_form['grupo_compradores']
+
+            #Validação de Valor Liquido da Fatura
+            if complement_form['valor_liquido'] != None:
+                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
+            elif complement_form['valor_nota'] != None:
+                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
             else:
                 attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
                     VALOR_TOTAL_DA_FATURA
                 )
 
-            jira_info = {"issue_id": issue_id, "form_id": automacao_form_id}
+            automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
+
+            jira_info = {"issue_id": issue_id, "form_id": automation_form_id}
 
             nf_jira_json = {
                 "issue_data": issue_data,
-                "attachment": attachment_data,
+                "attachment": attachment,
                 "jira_info": jira_info,
             }
 
             return nf_jira_json
 
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
-    def _get_nf_issue_attachment(self, attachment_id: str):
-        try:
-            attachment_request = requests.get(
-                f"{self._api_issue_url}/attachment/content/{attachment_id}",
-                headers=self._api_attachment_headers,
-                auth=self._auth,
-            )
-            attachment_request.raise_for_status()
-            content_type = attachment_request.headers.get("Content-Type", "")
-            if "application/pdf" in content_type:
-                return None
-            attachment_data = attachment_request.json()
-
-            return attachment_data
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
-
     def _get_nf_domain(self, type: str, cnpj: str):
 
         try:
             domain_request = requests.get(
-                f"{self._api_domain_url}/{'fornecedores' if type == 'fornecedor' else 'centros'}?cnpj={cnpj}",
-                auth=self._n8n_auth,
+                f"{API_DOMAIN_N8N_URL}/{'fornecedores' if type == 'fornecedor' else 'centros'}?cnpj={cnpj}",
+                auth=N8N_AUTH,
             )
             domain_request.raise_for_status()
             domain_data = domain_request.json()
 
             if not domain_data:
                 raise Exception("Could not find domain")
 
@@ -546,94 +396,51 @@
 
     def _get_allocation(
         self, cnpj_fornecedor: str, cnpj_cliente: str, numero_contrato: str
     ):
 
         try:
             allocation_request = requests.get(
-                f"{self._api_domain_url}/rateio?cnpj_fornecedor={cnpj_fornecedor}&cnpj_hortifruti={cnpj_cliente}&numero_contrato={numero_contrato}",
-                auth=self._n8n_auth,
+                f"{API_DOMAIN_N8N_URL}/rateio?cnpj_fornecedor={cnpj_fornecedor}&cnpj_hortifruti={cnpj_cliente}&numero_contrato={numero_contrato}",
+                auth=N8N_AUTH,
             )
             allocation_request.raise_for_status()
             if allocation_request.text.strip() != "":
                 allocation_data = allocation_request.json()
             else:
                 allocation_data = None
         except Exception as e:
             raise Exception(f"Erro ao receber rateio:\n{e}")
 
         return allocation_data
 
     def _download_pdf(self, pdf_path):
-        path_dir = path.join(getcwd(), "output")
-        pdf_file = ConsumoService().download_pdf(pdf_path, path_dir)
+        path_dir = path.join(getcwd(), "output/pdf")
+        pdf_file = self.ConsumoService.download_pdf(pdf_path, path_dir)
 
         return pdf_file
 
-    def _save_form_answers(self, answers, issue_id, form_id):
 
-        try:
-            save_request = requests.put(
-                f"{self._api_form_url}/{self._cloud_id}/issue/{issue_id}/form/{form_id}",
-                headers=self._api_atlassian_headers,
-                auth=self._auth,
-                json=answers,
-            )
-
-            return save_request.raise_for_status()
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
-
-    def update_jira_form(self, issue, data):
-
-        answers = {
-            "answers": {
-                "4": {
-                    "text": (
-                        data["cod_fatura"] if "cod_fatura" in data else None
-                    )  ##Codigo SAP FV60
-                },
-                "5": {
-                    "text": (
-                        data["status_liberacao"] if "status_liberacao" in data else None
-                    )  ##Status de Aprovação
-                },
-                "7": {
-                    "text": (
-                        data["cod_miro"] if "cod_miro" in data else None
-                    )  ##Codigo SAP Miro
-                },
-                "6": {
-                    "text": (
-                        data["data_liberacao"] if "data_liberacao" in data else None
-                    )  ##Data de Aprovação
-                },
-                "1": {
-                    "text": (
-                        data["cod_nota_pedido"] if "cod_nota_pedido" in data else None
-                    )  ##Codigo SAP Nota de Pedido
-                },
-            }
-        }
-
-        self._save_form_answers(answers, issue["issue_id"], issue["form_id"])
-
-        return True
 
     def post_transition(self, transition_id, issue_id):
         payload = json.dumps(
             {
                 "transition": {"id": transition_id},
                 "update": {"comment": []},
             }
         )
         res = requests.post(
             f"{self._api_issue_url}/issue/{issue_id}/transitions",
-            auth=self._auth,
-            headers=self._api_headers,
+            auth=JIRA_AUTH,
+            headers=API_HEADERS,
             data=payload,
         )
         res.raise_for_status()
+
+    def _get_issue_fields_by_keys(self, issue_key, form_template):
+
+        form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
+        form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
+        jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
+        fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
+
+        return fields_by_jira_and_form
```

