# Comparing `tmp/datasette-enrichments-gpt-0.3.tar.gz` & `tmp/datasette-enrichments-gpt-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-enrichments-gpt-0.3.tar", last modified: Fri Dec  1 22:55:15 2023, max compression
+gzip compressed data, was "datasette-enrichments-gpt-0.4.tar", last modified: Wed Apr 10 03:28:44 2024, max compression
```

## Comparing `datasette-enrichments-gpt-0.3.tar` & `datasette-enrichments-gpt-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:55:15.902710 datasette-enrichments-gpt-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-12-01 22:55:15.902710 datasette-enrichments-gpt-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:55:15.898710 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:55:15.898710 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/templates/enrichment-gpt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:55:15.898710 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-01 22:55:15.000000 datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 22:55:15.902710 datasette-enrichments-gpt-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:55:15.898710 datasette-enrichments-gpt-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-01 22:55:02.000000 datasette-enrichments-gpt-0.3/tests/test_enrichments_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/enrichment-gpt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/tests/test_enrichments_gpt.py
```

### Comparing `datasette-enrichments-gpt-0.3/LICENSE` & `datasette-enrichments-gpt-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-gpt-0.3/PKG-INFO` & `datasette-enrichments-gpt-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-gpt
-Version: 0.3
+Version: 0.4
 Summary: Datasette enrichment for analyzing row data using OpenAI's GPT models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-gpt
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-gpt/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-gpt/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-gpt/actions
@@ -48,15 +48,17 @@
   datasette-enrichments-gpt:
     api_key:
       $env: OPENAI_API_KEY
 ```
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+
+The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.3/README.md` & `datasette-enrichments-gpt-0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
   datasette-enrichments-gpt:
     api_key:
       $env: OPENAI_API_KEY
 ```
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+
+The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/__init__.py` & `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
         class ConfigForm(Form):
             # Select box to pick model from gpt-3.5-turbo or gpt-4-turbo
             model = SelectField(
                 "Model",
                 choices=[
                     ("gpt-3.5-turbo", "gpt-3.5-turbo"),
-                    ("gpt-4-1106-preview", "gpt-4-turbo"),
-                    ("gpt-4-vision-preview", "gpt-4-vision"),
+                    ("gpt-4-turbo", "gpt-4-turbo"),
+                    ("gpt-4-vision", "gpt-4-turbo vision"),
                 ],
                 default="gpt-3.5-turbo",
             )
             prompt = TextAreaField(
                 "Prompt",
                 description="A template to run against each row to generate a prompt. Use {{ COL }} for columns.",
                 default=default,
@@ -128,17 +128,15 @@
 
     async def _chat_completion(
         self, api_key, model, messages, json_format=False
     ) -> str:
         body = {"model": model, "messages": messages}
         if json_format:
             body["response_format"] = {"type": "json_object"}
-        # Bump up max tokens on gpt-4-vision-preview
-        if model == "gpt-4-vision-preview":
-            body["max_tokens"] = 1000
+        body["max_tokens"] = 1000
         async with httpx.AsyncClient() as client:
             response = await client.post(
                 "https://api.openai.com/v1/chat/completions",
                 headers={
                     "Content-Type": "application/json",
                     "Authorization": "Bearer {}".format(api_key),
                 },
@@ -162,26 +160,25 @@
         return await self._chat_completion(
             api_key, model, messages, json_format=json_format
         )
 
     async def gpt4_vision(self, api_key, prompt, image_url, system=None) -> str:
         messages = []
         if system:
-            # TODO: Check that gpt-4-vision-preview supports system prompts
             messages.append({"role": "system", "content": system})
         messages.append(
             {
                 "role": "user",
                 "content": [
                     {"type": "text", "text": prompt},
                     {"type": "image_url", "image_url": {"url": image_url}},
                 ],
             }
         )
-        return await self._chat_completion(api_key, "gpt-4-vision-preview", messages)
+        return await self._chat_completion(api_key, "gpt-4-turbo", messages)
 
     async def enrich_batch(
         self,
         datasette: "Datasette",
         db: Database,
         table: str,
         rows: List[dict],
@@ -205,15 +202,15 @@
                 "{{%s}}" % key, str(value or "")
             )
             if image_url:
                 image_url = image_url.replace(
                     "{{ %s }}" % key, str(value or "")
                 ).replace("{{%s}}" % key, str(value or ""))
         model = config["model"]
-        if model == "gpt-4-vision-preview":
+        if model == "gpt-4-vision":
             output = await self.gpt4_vision(api_key, prompt, image_url, system)
         else:
             output = await self.turbo_completion(
                 api_key, model, prompt, system, json_format
             )
         await db.execute_write(
             "update [{table}] set [{output_column}] = ? where {wheres}".format(
```

### Comparing `datasette-enrichments-gpt-0.3/datasette_enrichments_gpt/templates/enrichment-gpt.html` & `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/enrichment-gpt.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 const modelSelect = document.querySelector('#model');
 const divForImageUrlLabel = document.querySelector('label[for="image_url"]').parentNode;
 const divForImageUrlInput = document.querySelector('#image_url').parentNode;
 const divForJsonFormatLabel = document.querySelector('label[for="json_format"]').parentNode;
 const divForJsonFormatInput = document.querySelector('#json_format').parentNode;
 function handleModelChange() {
     // If gpt-4-vision-preview, hide JSON, show image URL
-    if (modelSelect.value === 'gpt-4-vision-preview') {
+    if (modelSelect.value === 'gpt-4-vision') {
         divForImageUrlLabel.style.display = '';
         divForImageUrlInput.style.display = '';
         divForJsonFormatLabel.style.display = 'none';
         divForJsonFormatInput.style.display = 'none';
     } else {
         divForImageUrlLabel.style.display = 'none';
         divForImageUrlInput.style.display = 'none';
```

### Comparing `datasette-enrichments-gpt-0.3/datasette_enrichments_gpt.egg-info/PKG-INFO` & `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-gpt
-Version: 0.3
+Version: 0.4
 Summary: Datasette enrichment for analyzing row data using OpenAI's GPT models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-gpt
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-gpt/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-gpt/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-gpt/actions
@@ -48,15 +48,17 @@
   datasette-enrichments-gpt:
     api_key:
       $env: OPENAI_API_KEY
 ```
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+
+The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.3/pyproject.toml` & `datasette-enrichments-gpt-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-enrichments-gpt"
-version = "0.3"
+version = "0.4"
 description = "Datasette enrichment for analyzing row data using OpenAI's GPT models"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

