# Comparing `tmp/mllibprodest-1.8.4.tar.gz` & `tmp/mllibprodest-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllibprodest-1.8.4.tar", last modified: Thu Mar 14 13:50:19 2024, max compression
+gzip compressed data, was "mllibprodest-1.8.5.tar", last modified: Wed Apr 10 21:34:02 2024, max compression
```

## Comparing `mllibprodest-1.8.4.tar` & `mllibprodest-1.8.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/
--rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/LICENSE
--rw-r--r--   0 messias   (1000) messias   (1000)    27189 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)    26069 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/README.md
--rw-rw-r--   0 messias   (1000) messias   (1000)     1025 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/pyproject.toml
--rw-rw-r--   0 messias   (1000) messias   (1000)      190 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/setup.cfg
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.501966 mllibprodest-1.8.4/src/
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.501966 mllibprodest-1.8.4/src/mllibprodest/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/__init__.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/src/mllibprodest/initiators/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/initiators/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     5671 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/initiators/model_initiator.py
--rw-rw-r--   0 messias   (1000) messias   (1000)    11202 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/interfaces.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     5416 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/provider.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/src/mllibprodest/providers_types/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/providers_types/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2126 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/providers_types/local_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2392 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/providers_types/minio_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     8142 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/providers_types/mlflow_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     8667 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/shared_classes.py
--rw-rw-r--   0 messias   (1000) messias   (1000)    11509 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/utils.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/src/mllibprodest/validators/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/validators/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)    22004 2024-03-14 13:40:10.000000 mllibprodest-1.8.4/src/mllibprodest/validators/test.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-03-14 13:50:19.505966 mllibprodest-1.8.4/src/mllibprodest.egg-info/
--rw-r--r--   0 messias   (1000) messias   (1000)    27189 2024-03-14 13:50:19.000000 mllibprodest-1.8.4/src/mllibprodest.egg-info/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)      753 2024-03-14 13:50:19.000000 mllibprodest-1.8.4/src/mllibprodest.egg-info/SOURCES.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)        1 2024-03-14 13:50:19.000000 mllibprodest-1.8.4/src/mllibprodest.egg-info/dependency_links.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       64 2024-03-14 13:50:19.000000 mllibprodest-1.8.4/src/mllibprodest.egg-info/requires.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       13 2024-03-14 13:50:19.000000 mllibprodest-1.8.4/src/mllibprodest.egg-info/top_level.txt
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/
+-rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/LICENSE
+-rw-r--r--   0 messias   (1000) messias   (1000)    27162 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)    26042 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/README.md
+-rw-rw-r--   0 messias   (1000) messias   (1000)     1025 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/pyproject.toml
+-rw-rw-r--   0 messias   (1000) messias   (1000)      190 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/setup.cfg
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.521781 mllibprodest-1.8.5/src/
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.521781 mllibprodest-1.8.5/src/mllibprodest/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/__init__.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/src/mllibprodest/initiators/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/initiators/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     5633 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/initiators/model_initiator.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    11202 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/interfaces.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     6342 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/provider.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/src/mllibprodest/providers_types/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/providers_types/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2087 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/providers_types/local_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2373 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/providers_types/minio_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    10388 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/providers_types/mlflow_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     1573 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/providers_types/utils.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     8505 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/shared_classes.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    11299 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/utils.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/src/mllibprodest/validators/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/validators/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    22004 2024-04-10 21:26:00.000000 mllibprodest-1.8.5/src/mllibprodest/validators/test.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2024-04-10 21:34:02.525781 mllibprodest-1.8.5/src/mllibprodest.egg-info/
+-rw-r--r--   0 messias   (1000) messias   (1000)    27162 2024-04-10 21:34:02.000000 mllibprodest-1.8.5/src/mllibprodest.egg-info/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)      795 2024-04-10 21:34:02.000000 mllibprodest-1.8.5/src/mllibprodest.egg-info/SOURCES.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)        1 2024-04-10 21:34:02.000000 mllibprodest-1.8.5/src/mllibprodest.egg-info/dependency_links.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       64 2024-04-10 21:34:02.000000 mllibprodest-1.8.5/src/mllibprodest.egg-info/requires.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       13 2024-04-10 21:34:02.000000 mllibprodest-1.8.5/src/mllibprodest.egg-info/top_level.txt
```

### Comparing `mllibprodest-1.8.4/LICENSE` & `mllibprodest-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.8.4/PKG-INFO` & `mllibprodest-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.8.4
+Version: 1.8.5
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
@@ -216,16 +216,16 @@
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
 - Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
-- Desative a opção **'New model registry UI'**;
-- Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
+- Na opção **'Aliases'**, clique em **'Add'**;
+- Digite ***production*** e clique em **'Save aliases'**.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
 Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de
```

### Comparing `mllibprodest-1.8.4/README.md` & `mllibprodest-1.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,16 @@
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
 - Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
-- Desative a opção **'New model registry UI'**;
-- Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
+- Na opção **'Aliases'**, clique em **'Add'**;
+- Digite ***production*** e clique em **'Save aliases'**.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
 Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de
```

### Comparing `mllibprodest-1.8.4/pyproject.toml` & `mllibprodest-1.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=69.1.1']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mllibprodest"
-version = "1.8.4"
+version = "1.8.5"
 license = {text = "GPLv3"}
 authors = [
   { name="Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)", email="prodest@prodest.es.gov.br" },
 ]
 description = "Biblioteca de Machine Learning (ML) do Prodest."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/initiators/model_initiator.py` & `mllibprodest-1.8.5/src/mllibprodest/initiators/model_initiator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 modulo = importlib.import_module(caminho_import, package=None)
             except ModuleNotFoundError as e:
                 msg_erro = str(e)
 
                 if caminho_import in msg_erro:
                     msg = f"Modelo: {model_name}. O módulo '{caminho_import}' não foi encontrado. Verifique no " \
                           f"arquivo 'params.conf' se o parâmetro 'source_file' foi informado corretamente e/ou se " \
-                          f"este módulo está dentro da pasta 'models'. Programa abortado!"
+                          f"este módulo está dentro da pasta 'models'."
                     LOGGER.error(msg)
                     raise ModuleNotFoundError(msg) from None
                 else:
                     msg = f"Modelo: {model_name}. Erro ao importar os módulos necessários para o módulo " \
                           f"'{caminho_import}'. Mensagem do Import: {msg_erro}"
                     LOGGER.error(msg)
                     # Não utilizei o 'from None' para preservar o traceback
@@ -87,12 +87,12 @@
                           f"'ModelPublicationInterfaceRETRAIN' e possua as implementações para os métodos " \
                           f"abstratos dela."
                     LOGGER.error(msg)
                     raise TypeError(msg)
             else:
                 msg = f"Modelo: {model_name}. O valor do parâmetro 'model_class' está incorreto. Foi informado " \
                       f"'{models_params[model_name]['model_class']}' no arquivo 'params.conf', porém deve ser " \
-                      f"'ModeloCLF' ou 'ModeloRETRAIN'. Programa abortado!"
+                      f"'ModeloCLF' ou 'ModeloRETRAIN'."
                 LOGGER.error(msg)
                 raise ValueError(msg)
 
         return modelos
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/interfaces.py` & `mllibprodest-1.8.5/src/mllibprodest/interfaces.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.8.4/src/mllibprodest/provider.py` & `mllibprodest-1.8.5/src/mllibprodest/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ----------------------------------------------------------------------------------------------------
 # Funções para prover o acesso aos modelos persistidos e aos datasets
 # ----------------------------------------------------------------------------------------------------
 from .utils import make_log
 from .providers_types.minio_provider import load_datasets_minio
 from .providers_types.local_provider import load_datasets_local
 from .providers_types.mlflow_provider import load_production_params_mlflow, load_production_datasets_names_mlflow, \
-    load_production_baseline_mlflow, load_model_mlflow
+    load_production_baseline_mlflow, load_model_mlflow, get_models_versions_mlflow
 
 # Para facilitar, define um logger único para todas as funções
 LOGGER = make_log("LOG_MLLIB.log")
 
 
 class Provider:
     """
@@ -25,52 +25,51 @@
             :return: Dicionário com os datasets carregados.
         """
         if provider == "minio":
             return load_datasets_minio(datasets_filenames)
         elif provider == "local":
             return load_datasets_local(datasets_filenames)
         else:
-            msg = f"Não foi possível carregar os datasets. O provider '{provider}' não foi encontrado. Programa " \
-                  f"abortado!"
+            msg = f"Não foi possível carregar os datasets. O provider '{provider}' não foi encontrado."
             LOGGER.error(msg)
-            raise RuntimeError(msg)
+            raise ValueError(msg)
 
     @staticmethod
     def load_production_params(model_name: str, provider: str = 'mlflow') -> dict:
         """
         Carrega os parâmetros utilizados para treinar o modelo que está em produção.
             :param model_name: Nome do modelo que está em produção.
             :param provider: Nome do provedor que fornecerá os parâmetros do modelo em produção. Tipos de provider:
                              'mlflow'.
             :return: Dicionário contendo os parâmetros carregados.
         """
         if provider == "mlflow":
             return load_production_params_mlflow(model_name)
         else:
             msg = f"Não foi possível carregar os parâmetros do modelo '{model_name}'. O provider '{provider}' não " \
-                  f"foi encontrado. Programa abortado!"
+                  f"foi encontrado."
             LOGGER.error(msg)
-            raise RuntimeError(msg)
+            raise ValueError(msg)
 
     @staticmethod
     def load_production_datasets_names(model_name: str, provider: str = 'mlflow') -> dict:
         """
         Carrega os nomes dos datasets que foram utilizados para treinar o modelo que está em produção.
             :param model_name: Nome do modelo que está em produção.
             :param provider: Nome do provedor que fornecerá os nomes dos datasets do modelo em produção. Tipos de
                              provider: 'mlflow'.
             :return: Dicionário contendo os nomes dos datasets carregados.
         """
         if provider == "mlflow":
             return load_production_datasets_names_mlflow(model_name)
         else:
             msg = f"Não foi possível carregar os nomes dos datasets do modelo '{model_name}'. O provider " \
-                  f"'{provider}' não foi encontrado. Programa abortado!"
+                  f"'{provider}' não foi encontrado."
             LOGGER.error(msg)
-            raise RuntimeError(msg)
+            raise ValueError(msg)
 
     @staticmethod
     def load_production_baseline(model_name: str, provider: str = 'mlflow') -> dict:
         """
         Carrega as métricas do modelo que está em produção que serão utilizadas como baseline para avaliação
         automatizada do modelo.
             :param model_name: Nome do modelo que está em produção.
@@ -78,27 +77,47 @@
                              'mlflow'.
             :return: Dicionário contendo as métricas de baseline.
         """
         if provider == "mlflow":
             return load_production_baseline_mlflow(model_name)
         else:
             msg = f"Não foi possível carregar o baseline do modelo '{model_name}'. O provider '{provider}' não " \
-                  f"foi encontrado. Programa abortado!"
+                  f"foi encontrado."
             LOGGER.error(msg)
-            raise RuntimeError(msg)
+            raise ValueError(msg)
 
     @staticmethod
     def load_model(model_name: str, provider: str = 'mlflow', artifacts_destination_path: str = 'temp_area'):
         """
         Carrega o modelo que está em produção e baixa os artefatos necessários.
             :param model_name: Nome do modelo que será carregado.
             :param provider: Nome do provedor que fornecerá o modelo. Tipos de provider: 'mlflow'.
             :param artifacts_destination_path: Caminho para onde os artefatos serão baixados.
             :return: Modelo carregado.
         """
         if provider == "mlflow":
             return load_model_mlflow(model_name, artifacts_destination_path)
         else:
-            msg = f"Não foi possível carregar o modelo '{model_name}'. O provider '{provider}' não foi encontrado. " \
-                  f"Programa abortado!"
+            msg = f"Não foi possível carregar o modelo '{model_name}'. O provider '{provider}' não foi encontrado."
             LOGGER.error(msg)
-            raise RuntimeError(msg)
+            raise ValueError(msg)
+
+    @staticmethod
+    def get_models_versions(models_names: list, provider: str = 'mlflow') -> dict:
+        """
+        Obtém as versões de alguns modelos que estão sendo providos pelo provider.
+            :param models_names: Lista com os nomes dos modelos para obtenção das versões.
+            :param provider: Provedor para obtenção das versões dos modelos.
+            :return: Dicionário com o nome de cada modelo como chave e a respectiva versão como valor.
+        """
+        if type(models_names) is not list:
+            msg = f"Não foi possível obter as versões para os modelos. '{models_names}' não é uma lista de modelos."
+            LOGGER.error(msg)
+            raise TypeError(msg)
+
+        if provider == "mlflow":
+            return get_models_versions_mlflow(models_names)
+        else:
+            msg = f"Não foi possível obter as versões para os modelos: {models_names}. O provider '{provider}' não " \
+                  f"foi encontrado."
+            LOGGER.error(msg)
+            raise ValueError(msg)
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/providers_types/local_provider.py` & `mllibprodest-1.8.5/src/mllibprodest/providers_types/local_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     # Obtém as informações necessárias para carregar os arquivos
     load_env_variables()
     local_path = os.environ.get("LOCAL_PATH")
 
     if local_path is None:
         msg = f"Não foram encontradas todas as variáveis de ambiente necessárias. Certifique-se que um arquivo " \
               f"chamado '.env' exista; esteja localizado na pasta da aplicação e que possua valor para a variável: " \
-              f"'LOCAL_PATH'. Ou se preferir, configure essa variável de ambiente e seu respectivo valor. " \
-              f"Programa abortado!"
+              f"'LOCAL_PATH'. Ou se preferir, configure essa variável de ambiente e seu respectivo valor."
         LOGGER.error(msg)
         raise RuntimeError(msg)
 
     datasets = {}
 
     for tipo, nome_arquivo in datasets_filenames.items():
         datasets[tipo] = BytesIO(get_file_local(str(Path(local_path) / nome_arquivo)))
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/providers_types/minio_provider.py` & `mllibprodest-1.8.5/src/mllibprodest/providers_types/minio_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     secret_key = os.environ.get("SECRET_KEY")
     bucket = os.environ.get("BUCKET")
 
     if s3_server is None or access_key is None or secret_key is None or bucket is None:
         msg = f"Não foram encontradas todas as variáveis de ambiente necessárias. Certifique-se que um arquivo " \
               f"chamado '.env' exista; esteja localizado na pasta da aplicação e que possua valores para as " \
               f"variáveis: 'MINIO', 'ACCESS_KEY', 'SECRET_KEY' e 'BUCKET'. Ou se preferir, configure essas variáveis " \
-              f"de ambiente e seus respectivos valores. Programa abortado!"
+              f"de ambiente e seus respectivos valores."
         LOGGER.error(msg)
         raise RuntimeError(msg)
 
     datasets = {}
 
     for tipo, nome_arquivo in datasets_filenames.items():
         datasets[tipo] = BytesIO(get_file_s3(nome_arquivo, s3_server, access_key, secret_key, bucket))
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/shared_classes.py` & `mllibprodest-1.8.5/src/mllibprodest/shared_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,28 +105,27 @@
         """
         caminho_artefato = str(Path(path) / model_name / file_name)
 
         try:
             arq = open(caminho_artefato, 'wb')
         except FileNotFoundError:
             msg = f"Não foi possível gerar o artefato '{file_name}' convertido. O caminho '{caminho_artefato}' está " \
-                  f"incorreto. Programa abortado!"
+                  f"incorreto."
             LOGGER.error(msg)
             raise FileNotFoundError(msg) from None
         except PermissionError:
             msg = f"Não foi possível gerar o artefato '{file_name}' convertido no caminho '{caminho_artefato}'. " \
-                  f"Permissão de escrita negada. Programa abortado!"
+                  f"Permissão de escrita negada."
             LOGGER.error(msg)
             raise PermissionError(msg) from None
 
         try:
             pickle.dump(artifact, arq)
         except TypeError as e:
-            msg = f"Não foi possível gerar o artefato '{file_name}' com o Pickle (mensagem Pickle: {e}). Programa " \
-                  f"abortado!"
+            msg = f"Não foi possível gerar o artefato '{file_name}' com o Pickle (mensagem Pickle: {e})."
             LOGGER.error(msg)
             raise TypeError(msg) from None
 
         arq.close()
 
     @staticmethod
     def convert_artifact_to_object(model_name: str, file_name: str, path: str = "temp_area") -> \
@@ -140,27 +139,26 @@
         """
         caminho_artefato = str(Path(path) / model_name / file_name)
 
         try:
             arq = open(caminho_artefato, 'rb')
         except FileNotFoundError:
             msg = f"Não foi possível converter o artefato '{file_name}'. O caminho '{caminho_artefato}' não foi " \
-                  f"encontrado. Programa abortado!"
+                  f"encontrado."
             LOGGER.error(msg)
             raise FileNotFoundError(msg) from None
         except PermissionError:
             msg = f"Não foi possível converter o artefato '{file_name}' usando o caminho '{caminho_artefato}'. " \
-                  f"Permissão de leitura negada. Programa abortado!"
+                  f"Permissão de leitura negada."
             LOGGER.error(msg)
             raise PermissionError(msg) from None
 
         try:
             objeto = pickle.load(arq)
         except pickle.UnpicklingError as e:
-            msg = f"Não foi possível converter o artefato '{file_name}' com o Pickle (mensagem Pickle: {e}). " \
-                  f"Programa abortado!"
+            msg = f"Não foi possível converter o artefato '{file_name}' com o Pickle (mensagem Pickle: {e})."
             LOGGER.error(msg)
             raise RuntimeError(msg)
 
         arq.close()
 
         return objeto
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/utils.py` & `mllibprodest-1.8.5/src/mllibprodest/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,19 @@
         # Configuração de parâmetros para gravação de logs
         try:
             rotatehandler = RotatingFileHandler(log_file_path, mode='a', maxBytes=10485760, backupCount=5)
             rotatehandler.setLevel(logging.INFO)
             rotatehandler.setFormatter(formatter)
             logger.addHandler(rotatehandler)
         except FileNotFoundError:
-            msg = f"Não foi possível encontrar/criar o arquivo de log no caminho '{log_file_path}'. Programa abortado!"
+            msg = f"Não foi possível encontrar/criar o arquivo de log no caminho '{log_file_path}'."
             raise FileNotFoundError(msg) from None
         except PermissionError:
             msg = f"Não foi possível criar/acessar o arquivo de log no caminho '{log_file_path}'. Permissão de " \
-                f"escrita/leitura negada. Programa abortado!"
+                f"escrita/leitura negada."
             raise PermissionError(msg) from None
     else:
         raise ValueError(f"A variável de ambiente 'STACK_LOG_OUTPUT' contém um tipo de saída do log incorreto "
                          f"('{stack_log_output}'). Os possíveis valores são: 'console' ou 'file'.")
 
     return logger
 
@@ -118,20 +118,19 @@
         :param file_path: Caminho do arquivo a ser carregado.
         :return: Objeto contendo o arquivo carregado.
     """
     try:
         with open(file_path, 'rb') as arq:
             bytes_arq = arq.read()
     except FileNotFoundError:
-        msg = f"Não foi possível encontrar o arquivo no caminho '{file_path}'. Programa abortado!"
+        msg = f"Não foi possível encontrar o arquivo no caminho '{file_path}'."
         LOGGER.error(msg)
         raise FileNotFoundError(msg) from None
     except PermissionError:
-        msg = f"Não foi possível ler o arquivo no caminho '{file_path}'. Permissão de leitura negada. Programa " \
-              f"abortado!"
+        msg = f"Não foi possível ler o arquivo no caminho '{file_path}'. Permissão de leitura negada."
         LOGGER.error(msg)
         raise PermissionError(msg) from None
 
     return bytes_arq
 
 
 def validate_params(received_params: list, expected_params: dict) -> tuple:
@@ -203,37 +202,37 @@
     conf = configparser.ConfigParser()
     param_file_path = str(Path(path) / "params.conf")
 
     # Carrega os parâmetros
     try:
         nome_arq_params = conf.read(param_file_path)
     except configparser.MissingSectionHeaderError as e:
-        msg = f"O arquivo com os parâmetros dos modelos ('params.conf') possui seções inválidas. Programa abortado! " \
-              f"Mensagem configParser: '{e}'."
+        msg = f"O arquivo com os parâmetros dos modelos ('params.conf') possui seções inválidas. Mensagem " \
+              f"configParser: '{e}'."
         LOGGER.error(msg)
         raise ValueError(msg) from None
     except configparser.DuplicateSectionError as e:
-        msg = f"Existem seções duplicadas. Programa abortado! Mensagem configParser: '{e}'."
+        msg = f"Existem seções duplicadas. Mensagem configParser: '{e}'."
         LOGGER.error(msg)
         raise ValueError(msg) from None
     except configparser.DuplicateOptionError as e:
-        msg = f"Existem parâmetros duplicados. Programa abortado! Mensagem configParser: '{e}'."
+        msg = f"Existem parâmetros duplicados. Mensagem configParser: '{e}'."
         LOGGER.error(msg)
         raise ValueError(msg) from None
 
     if "params.conf" not in nome_arq_params:
         msg = "Não foi possível encontrar o arquivo com os parâmetros dos modelos ('params.conf') ou não possui " \
-              "permissão para leitura. Programa abortado!"
+              "permissão para leitura."
         LOGGER.error(msg)
         raise RuntimeError(msg)
 
     secoes = conf.sections()
 
     if not secoes:
-        msg = "O arquivo com os parâmetros dos modelos ('params.conf') está vazio. Programa abortado!"
+        msg = "O arquivo com os parâmetros dos modelos ('params.conf') está vazio."
         LOGGER.error(msg)
         raise ValueError(msg)
 
     # Verifica se tem parâmetros padrões faltantes
     for s in secoes:
         parametros_faltantes = []
 
@@ -243,15 +242,15 @@
 
         if parametros_faltantes:
             faltou_parametro = True
             parametros_faltantes_por_secao[s] = parametros_faltantes
 
     if faltou_parametro:
         msg = f"Um ou mais parâmetros não foram encontrados no arquivo 'params.conf'. Parâmetros faltantes por " \
-              f"modelo: {parametros_faltantes_por_secao}. Programa abortado!"
+              f"modelo: {parametros_faltantes_por_secao}."
         LOGGER.error(msg)
         raise ValueError(msg)
 
     parametros_por_modelo = {}
 
     # Obtém os parâmetros e gera o dicionário com os modelos e parâmetros
     for s in secoes:
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest/validators/test.py` & `mllibprodest-1.8.5/src/mllibprodest/validators/test.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.8.4/src/mllibprodest.egg-info/PKG-INFO` & `mllibprodest-1.8.5/src/mllibprodest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.8.4
+Version: 1.8.5
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
@@ -216,16 +216,16 @@
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
 - Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
-- Desative a opção **'New model registry UI'**;
-- Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
+- Na opção **'Aliases'**, clique em **'Add'**;
+- Digite ***production*** e clique em **'Save aliases'**.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
 Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de
```

### Comparing `mllibprodest-1.8.4/src/mllibprodest.egg-info/SOURCES.txt` & `mllibprodest-1.8.5/src/mllibprodest.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 src/mllibprodest.egg-info/top_level.txt
 src/mllibprodest/initiators/__init__.py
 src/mllibprodest/initiators/model_initiator.py
 src/mllibprodest/providers_types/__init__.py
 src/mllibprodest/providers_types/local_provider.py
 src/mllibprodest/providers_types/minio_provider.py
 src/mllibprodest/providers_types/mlflow_provider.py
+src/mllibprodest/providers_types/utils.py
 src/mllibprodest/validators/__init__.py
 src/mllibprodest/validators/test.py
```

