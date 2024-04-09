# Comparing `tmp/promptlayer-0.5.4.tar.gz` & `tmp/promptlayer-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlayer-0.5.4.tar", max compression
+gzip compressed data, was "promptlayer-0.5.5.tar", max compression
```

## Comparing `promptlayer-0.5.4.tar` & `promptlayer-0.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-04-01 18:29:27.461644 promptlayer-0.5.4/LICENSE
--rw-r--r--   0        0        0     3839 2024-04-01 18:29:27.461644 promptlayer-0.5.4/README.md
--rw-r--r--   0        0        0     1110 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/__init__.py
--rw-r--r--   0        0        0       67 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/groups/__init__.py
--rw-r--r--   0        0        0      139 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/groups/groups.py
--rw-r--r--   0        0        0     3736 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/promptlayer.py
--rw-r--r--   0        0        0      205 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/__init__.py
--rw-r--r--   0        0        0     2348 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/chat.py
--rw-r--r--   0        0        0     3215 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/prompts.py
--rw-r--r--   0        0        0       63 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/__init__.py
--rw-r--r--   0        0        0      468 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/base.py
--rw-r--r--   0        0        0      220 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/prompt.py
--rw-r--r--   0        0        0      542 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/templates.py
--rw-r--r--   0        0        0      119 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/track/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/track/track.py
--rw-r--r--   0        0        0       61 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/types/__init__.py
--rw-r--r--   0        0        0     3752 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/types/prompt_template.py
--rw-r--r--   0        0        0    21160 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/utils.py
--rw-r--r--   0        0        0      487 2024-04-01 18:29:27.465644 promptlayer-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 promptlayer-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 23:09:15.850606 promptlayer-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3839 2024-04-09 23:09:15.850606 promptlayer-0.5.5/README.md
+-rw-r--r--   0        0        0     1110 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/groups/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/groups/groups.py
+-rw-r--r--   0        0        0     3736 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/promptlayer.py
+-rw-r--r--   0        0        0      205 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/prompts/__init__.py
+-rw-r--r--   0        0        0     2348 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/prompts/chat.py
+-rw-r--r--   0        0        0     3215 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/prompts/prompts.py
+-rw-r--r--   0        0        0       63 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/resources/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/resources/base.py
+-rw-r--r--   0        0        0      220 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/resources/prompt.py
+-rw-r--r--   0        0        0      542 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/templates.py
+-rw-r--r--   0        0        0      119 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/track/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/track/track.py
+-rw-r--r--   0        0        0       61 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/types/__init__.py
+-rw-r--r--   0        0        0     3806 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/types/prompt_template.py
+-rw-r--r--   0        0        0    21267 2024-04-09 23:09:15.854606 promptlayer-0.5.5/promptlayer/utils.py
+-rw-r--r--   0        0        0      487 2024-04-09 23:09:15.854606 promptlayer-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 promptlayer-0.5.5/PKG-INFO
```

### Comparing `promptlayer-0.5.4/LICENSE` & `promptlayer-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/README.md` & `promptlayer-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/__init__.py` & `promptlayer-0.5.5/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/promptlayer.py` & `promptlayer-0.5.5/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/prompts/chat.py` & `promptlayer-0.5.5/promptlayer/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/prompts/prompts.py` & `promptlayer-0.5.5/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/templates.py` & `promptlayer-0.5.5/promptlayer/templates.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/track/track.py` & `promptlayer-0.5.5/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.4/promptlayer/types/prompt_template.py` & `promptlayer-0.5.5/promptlayer/types/prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Literal, Sequence, TypedDict, Union
+from typing import Dict, List, Literal, Optional, Sequence, TypedDict, Union
 
 
 class GetPromptTemplate(TypedDict, total=False):
     version: int
     label: str
     provider: str
     input_variables: Dict[str, str]
@@ -146,16 +146,16 @@
 
 class PromptVersion(TypedDict, total=False):
     prompt_template: PromptTemplate
     commit_message: str
     metadata: Metadata
 
 
-class PublishPromptTemplate(BasePromptTemplate, PromptVersion):
-    pass
+class PublishPromptTemplate(BasePromptTemplate, PromptVersion, total=False):
+    release_label: Optional[str] = None
 
 
 class BasePromptTemplateResponse(TypedDict):
     id: int
     prompt_name: str
     tags: List[str]
     prompt_template: PromptTemplate
```

### Comparing `promptlayer-0.5.4/promptlayer/utils.py` & `promptlayer-0.5.5/promptlayer/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,19 @@
 def publish_prompt_template(
     body: PublishPromptTemplate,
 ) -> PublishPromptTemplateResponse:
     try:
         response = requests.post(
             f"{URL_API_PROMPTLAYER}/rest/prompt-templates",
             headers={"X-API-KEY": get_api_key()},
-            json={"prompt_template": {**body}, "prompt_version": {**body}},
+            json={
+                "prompt_template": {**body},
+                "prompt_version": {**body},
+                "release_label": body.get("release_label"),
+            },
         )
         if response.status_code == 400:
             raise Exception(
                 f"PromptLayer had the following error while publishing your prompt template: {response.text}"
             )
         return response.json()
     except requests.exceptions.RequestException as e:
```

### Comparing `promptlayer-0.5.4/PKG-INFO` & `promptlayer-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.5.4
+Version: 0.5.5
 Summary: PromptLayer is a platform for prompt engineering and tracks your LLM requests.
 License: Apache-2.0
 Author: Magniv
 Author-email: hello@magniv.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.5.4 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.5.5 Summary: PromptLayer is
 a platform for prompt engineering and tracks your LLM requests. License:
 Apache-2.0 Author: Magniv Author-email: hello@magniv.io Requires-Python:
 >=3.8.1,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

