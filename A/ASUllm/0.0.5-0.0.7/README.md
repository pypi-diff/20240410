# Comparing `tmp/ASUllm-0.0.5.tar.gz` & `tmp/ASUllm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASUllm-0.0.5.tar", last modified: Wed Apr 10 15:57:48 2024, max compression
+gzip compressed data, was "ASUllm-0.0.7.tar", last modified: Wed Apr 10 16:25:47 2024, max compression
```

## Comparing `ASUllm-0.0.5.tar` & `ASUllm-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.048793 ASUllm-0.0.5/
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.046617 ASUllm-0.0.5/ASUllm/
--rw-r--r--   0 wenxing1   (503) staff       (20)      138 2024-04-09 23:58:07.000000 ASUllm-0.0.5/ASUllm/__init__.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1463 2024-04-09 20:54:31.000000 ASUllm-0.0.5/ASUllm/api.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.5/ASUllm/model_config.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1258 2024-04-09 23:58:05.000000 ASUllm-0.0.5/ASUllm/models.py
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.048173 ASUllm-0.0.5/ASUllm.egg-info/
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)      225 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/SOURCES.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/dependency_links.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        7 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/top_level.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.5/LICENSE
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 15:57:48.048499 ASUllm-0.0.5/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.5/README.md
--rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-10 15:57:13.000000 ASUllm-0.0.5/pyproject.toml
--rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-10 15:57:48.048889 ASUllm-0.0.5/setup.cfg
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 16:25:47.481807 ASUllm-0.0.7/
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 16:25:47.479802 ASUllm-0.0.7/ASUllm/
+-rw-r--r--   0 wenxing1   (503) staff       (20)      122 2024-04-10 16:25:15.000000 ASUllm-0.0.7/ASUllm/__init__.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     2216 2024-04-10 16:19:20.000000 ASUllm-0.0.7/ASUllm/api.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.7/ASUllm/model_config.py
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 16:25:47.481285 ASUllm-0.0.7/ASUllm.egg-info/
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 16:25:47.000000 ASUllm-0.0.7/ASUllm.egg-info/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)      208 2024-04-10 16:25:47.000000 ASUllm-0.0.7/ASUllm.egg-info/SOURCES.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-10 16:25:47.000000 ASUllm-0.0.7/ASUllm.egg-info/dependency_links.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        7 2024-04-10 16:25:47.000000 ASUllm-0.0.7/ASUllm.egg-info/top_level.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.7/LICENSE
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 16:25:47.481566 ASUllm-0.0.7/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.7/README.md
+-rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-10 16:25:18.000000 ASUllm-0.0.7/pyproject.toml
+-rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-10 16:25:47.482036 ASUllm-0.0.7/setup.cfg
```

### Comparing `ASUllm-0.0.5/ASUllm/api.py` & `ASUllm-0.0.7/ASUllm/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,63 @@
 import traceback
 from time import sleep
 from model_config import ModelConfig
 
 __author__ = 'swliu'
 
 
+def query_llm(model: ModelConfig, query, num_retry: int = 3) -> str:
+    for i in range(num_retry):
+        try:
+            payload = _compute_payload(model=model, query=query)
+            headers = _compute_headers(model.access_token)
+            response = requests.post(model.api_url, json=payload, headers=headers)
+            response_text = response.json()['response']
+            return response_text
+        except Exception as e:
+            print(traceback.format_exc())
+            sleep(1)
+            continue
+    return ""
+
+
+def query_model_info_api(access_token, url, num_retry: int = 3) -> list:
+    """
+    :param access_token: API access token.
+    :param url: API endpoint
+    :param num_retry: int
+    :return: a list of large language models that are hosted by ASU
+    """
+    for i in range(num_retry):
+        try:
+            headers = _compute_headers(access_token=access_token)
+            response = requests.get(url=url, headers=headers)
+            models_dict = json.loads(response.content)
+            models = models_dict["models"]
+            return models
+        except Exception as e:
+            print(traceback.format_exc())
+            sleep(1)
+            continue
+    return []
+
+
+def model_provider_mapper(models: list) -> dict:
+    mapper = {
+        model["name"]: model["provider"]
+        for model in models
+    }
+    return mapper
+
+
+def model_list(models: list) -> set:
+    models = {model["name"] for model in models}
+    return models
+
+
 def _compute_headers(access_token):
     headers = {
         "Accept": "application/json",
         "Authorization": f'Bearer {access_token}'
     }
     return headers
 
@@ -26,28 +75,7 @@
         "prompt": query,
         # optional
         "enable_search": model.enable_search,
         # optional
         "search_params": model.search_params
     }
     return payload
-
-
-def query_llm(model: ModelConfig, query, num_retry: int = 3) -> str:
-    for i in range(num_retry):
-        try:
-            payload = _compute_payload(model=model, query=query)
-            headers = _compute_headers(model.access_token)
-            response = requests.post(model.api_url, json=payload, headers=headers)
-            response_text = response.json()['response']
-            return response_text
-        except Exception as e:
-            print(traceback.format_exc())
-            sleep(1)
-            continue
-    return ""
-
-
-if __name__ == '__main__':
-    model = ModelConfig(name="claudeinstant", provider="aws", enable_search=True)
-    res = query_llm(model=model, query="Where is phoenix arizona?")
-    print(res)
```

### Comparing `ASUllm-0.0.5/ASUllm/model_config.py` & `ASUllm-0.0.7/ASUllm/model_config.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.5/ASUllm.egg-info/PKG-INFO` & `ASUllm-0.0.7/ASUllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.5
+Version: 0.0.7
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ASUllm-0.0.5/LICENSE` & `ASUllm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.5/PKG-INFO` & `ASUllm-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.5
+Version: 0.0.7
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ASUllm-0.0.5/README.md` & `ASUllm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.5/pyproject.toml` & `ASUllm-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ASUllm"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
 ]
 description = "A simple python package to facilitate connection to ASU LLM API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

