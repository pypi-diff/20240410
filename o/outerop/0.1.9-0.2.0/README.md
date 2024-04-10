# Comparing `tmp/outerop-0.1.9.tar.gz` & `tmp/outerop-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outerop-0.1.9.tar", max compression
+gzip compressed data, was "outerop-0.2.0.tar", max compression
```

## Comparing `outerop-0.1.9.tar` & `outerop-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2498 2024-03-20 21:11:02.339695 outerop-0.1.9/README.md
--rw-r--r--   0        0        0    10998 2024-03-21 18:42:02.042098 outerop-0.1.9/outerop/__init__.py
--rw-r--r--   0        0        0      475 2024-03-21 18:42:16.536706 outerop-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 outerop-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3314 2024-04-10 07:01:40.307706 outerop-0.2.0/README.md
+-rw-r--r--   0        0        0    12518 2024-04-09 04:28:50.077741 outerop-0.2.0/outerop/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-10 07:09:01.769281 outerop-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 outerop-0.2.0/PKG-INFO
```

### Comparing `outerop-0.1.9/README.md` & `outerop-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -14,42 +14,59 @@
 
 To use the Outerop SDK, you need to create an instance of the `Outerop` class with your Outerop API key and optionally provide additional configuration options.
 
 ```python
 from outerop import Outerop
 
 outerop = Outerop(outerop_api_key="YOUR_OUTEROP_API_KEY", options={
-    "openaiApiKey": "YOUR_OPENAI_API_KEY",
-    "anthropicApiKey": "YOUR_ANTHROPIC_API_KEY",
-    "mistralApiKey": "YOUR_MISTRAL_API_KEY"
+   "openaiApiKey": "YOUR_OPENAI_API_KEY",
+   "anthropicApiKey": "YOUR_ANTHROPIC_API_KEY",
+   "mistralApiKey": "YOUR_MISTRAL_API_KEY"
 })
 ```
 
-### Retrieving a Prompt
+### Using the SDK
 
-To retrieve a prompt, use the `get_prompt` method:
+To call the AI API with a specific prompt and variables, you can use the `chat` method:
 
 ```python
-prompt = outerop.get_prompt(prompt_uuid="PROMPT_UUID", environment="development", version="latest")
+result = outerop.chat(
+   team_prompt_name"your-prompt-uuid",
+   version_name_or_environment="development",
+   variables={"name": "John", "age": "25"}
+)
 ```
 
-### Use 
+### Pinning a specific version in version control
 
-To use the prompt, use the `chat` method:
+You can replace the `environment` parameter with a specific version number to pin a specific version of the prompt.
 
 ```python
 result = outerop.chat(
-    prompt_uuid="PROMPT_UUID",
-    environment="development",
-    version="latest",
-    variables={"name": "John", "age": "25"}
+   team_prompt_name"your-prompt-uuid",
+   version_name_or_environment="o-1234567890",
+   variables={"name": "John", "age": "25"}
 )
 ```
 
-The `chat` method returns the AI's response based on the provided prompt and variables.
+We recommend keeping the instantiation of the `Outerop` class outside your main event loop to allow the caching to work.
+
+### Response format
+
+We standardise responses based on the OpenAI SDK for both python and JS. Other models outputs will be transformed to fit the schema. However if you need to, you can access the raw return from the API in the "raw" property of the response.
+
+However we **highly** recommend using the standardised format, as it will allow you to switch models without changing your code.
+
+### Other methods
+
+To retrieve a prompt, use the `get_prompt` method:
+
+```python
+prompt = outerop.get_prompt(team_prompt_name"your-prompt-uuid", environment="development", version="latest")
+```
 
 ## Configuration
 
 The `Outerop` class accepts an optional `options` parameter to configure additional settings:
 
 - `baseURL`: The base URL of the Outerop API (default: "https://app.outerop.com").
 - `loggingEnabled`: Enable or disable logging (default: True).
```

### Comparing `outerop-0.1.9/outerop/__init__.py` & `outerop-0.2.0/outerop/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,58 @@
+import re
 import json
 import time
+from enum import Enum
 from typing import List, Dict, Union
 import requests
 from openai import OpenAI
+import openai
 from anthropic import Anthropic
 from mistralai.client import MistralClient
 
+
+# CONSTANTS
+DEFAULT_TTL = 15 * 60  # 15 minutes
+
+
+class Environment(Enum):
+    PRODUCTION = "production"
+    DEVELOPMENT = "development"
+    STAGING = "staging"
+
+
 class LogCollector:
     def __init__(self, config: Dict):
         self.config = {**{"isEnabled": True, "baseURL": "https://app.outerop.com"}, **config}
         self.outerop_api_key = config["outeropApiKey"]
+        self.bypass_header = config.get("bypassHeader")
         self.pending_flush = False
         self.buffer = []
 
     @property
     def is_enabled(self):
         return self.config["isEnabled"]
 
     def record(self, event: Dict):
         prepared_event = self._prepare_event(event)
         self.buffer.append(prepared_event)
         self.flush()
 
     def flush(self):
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": self.outerop_api_key,
+        }
+        if self.bypass_header:
+            headers["x-vercel-protection-bypass"] = self.bypass_header
+
         try:
             response = requests.post(
                 f"{self.config['baseURL']}/api/v1/log",
-                headers={
-                    "Content-Type": "application/json",
-                    "Authorization": self.outerop_api_key,
-                },
+                headers=headers,
                 data=json.dumps(self.buffer),
             )
             response.raise_for_status()
         except requests.exceptions.RequestException:
             pass
         finally:
             self.pending_flush = False
@@ -44,29 +63,32 @@
 
 
 class Outerop:
     def __init__(self, outerop_api_key: str, options: Dict = None):
         self.outerop_api_key = outerop_api_key
         self.options = {**{"baseURL": "https://app.outerop.com", "loggingEnabled": True}, **(options or {})}
 
+
         self.log_collector = LogCollector(
             {
                 "isEnabled": True,
                 "baseURL": self.options.get("baseURL", "https://app.outerop.com"),
                 "outeropApiKey": self.outerop_api_key,
+                "bypassHeader": self.options.get("bypassHeader"),
             }
         )
 
         headers = {
             "Authorization": self.outerop_api_key,
             "Content-Type": "application/json",
         }
         if self.options.get("bypassHeader"):
             headers["x-vercel-protection-bypass"] = self.options["bypassHeader"]
 
+
         self.client = requests.Session()
         self.client.headers.update(headers)
         self.client.base_url = self.options["baseURL"]
 
         self.openai = None
         if self.options.get("openaiApiKey"):
             self.openai = OpenAI(api_key=self.options["openaiApiKey"])
@@ -76,58 +98,63 @@
             self.anthropic = Anthropic(api_key=self.options["anthropicApiKey"])
 
         self.mistral = None
         if self.options.get("mistralApiKey"):
             self.mistral = MistralClient(api_key=self.options["mistralApiKey"])
 
         self.prompt_cache: Dict[str, Dict] = {}
+        self.prompt_cache_ttl = options.get("promptCacheTTL", DEFAULT_TTL)  # Default TTL of 15 minutes
+        
+        
 
-    def get_prompt(self, prompt_uuid: str, environment: str, version: Union[int, str]):
-        cache_key = f"{prompt_uuid}-{environment}-{version}"
+    def get_prompt(self, team_prompt_name: str, version_name_or_environment: str):
+        cache_key = f"{team_prompt_name}-{version_name_or_environment}"
+        current_time = time.time()
         if cache_key in self.prompt_cache:
-            return self.prompt_cache[cache_key]
+            cached_prompt, timestamp = self.prompt_cache[cache_key]
+            if current_time - timestamp < self.prompt_cache_ttl:
+                return cached_prompt
 
         try:
-            print(f"promptUuid: {prompt_uuid}")
-            print(f"environment: {environment}")
-            print(f"version: {version}")
-            print(f"api key: {self.outerop_api_key}")
+            url = f"{self.options['baseURL']}/api/v1/prompt-by-version-name/{team_prompt_name}/{version_name_or_environment}"
+            if version_name_or_environment in list(Environment):
+                url = f"{self.options['baseURL']}/api/v1/prompt-by-environment/{team_prompt_name}/{version_name_or_environment}"
 
-            url = f"{self.options['baseURL']}/api/v1/prompt/{prompt_uuid}/{environment}/{version}"
             response = self.client.get(url)
             response.raise_for_status()
-            self.prompt_cache[cache_key] = response.json()["prompt"]
-            return response.json()["prompt"]
+            prompt_data = response.json()["prompt"]
+            self.prompt_cache[cache_key] = (prompt_data, current_time)  # Update cache with timestamp
+            return prompt_data
         except requests.exceptions.RequestException as e:
             status_code = e.response.status_code if e.response else "Unknown"
             response_text = e.response.text if e.response else "Unknown"
             raise Exception(f"Request failed with status code {status_code}: {response_text}")
         except Exception as e:
             print(f"error: {e}")
             raise Exception(f"Request failed: {e}")
+
         
 
     def chat(
         self,
-        prompt_uuid: str,
-        environment: str,
-        version: Union[int, str],
-        variables: Dict[str, str],
-        name: str = None,
+        team_prompt_name: str,
+        version_name_or_environment: str,
+        variables: Dict[str, str]
     ):
-        prompt = self.get_prompt(prompt_uuid, environment, version)
+        prompt = self.get_prompt(team_prompt_name, version_name_or_environment)
         messages = replace_variables_in_prompts(prompt["messages"], variables)
         messages_without_id = [
             {k: v for k, v in message.items() if k != "id"} for message in messages
         ]
 
         try:
             tools = prompt["tools"] if prompt["tools"] and len(prompt["tools"]) > 0 else None
 
-            print(prompt)
+            if prompt["model_config"]["provider"] == "groq":
+                raise Exception("Groq is not supported yet")
 
             if prompt["model_config"]["provider"] == "mistral":
                 if not self.mistral:
                     raise Exception("Mistral API key is not provided")
 
                 start_time = time.perf_counter()
                 result = self.mistral.chat(
@@ -137,16 +164,14 @@
                     temperature=prompt["temperature"],
                     tools=tools,
                     tool_choice=prompt.get("tool_choice", "auto"),
                 )
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
-                print(f"result: {result}")
-
                 self.log_collector.record(
                     {
                         "version": prompt["version"],
                         "team_prompt_id": prompt["team_prompt_id"],
                         "environment": prompt["environment"],
                         "prompt_environment_id": prompt["id"],
                         "input": messages_without_id,
@@ -218,33 +243,37 @@
                     messages=messages_without_system,
                     model=prompt["model_config"]["model_id"],
                     max_tokens=prompt["max_tokens"],
                     temperature=prompt["temperature"],
                     system=system_prompt,
                 )
 
+                print(result)
+
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
+                openai_result = convert_anthropic_output_to_openai(result)
+
                 self.log_collector.record(
                     {
                         "version": prompt["version"],
                         "team_prompt_id": prompt["team_prompt_id"],
                         "prompt_environment_id": prompt["id"],
                         "environment": prompt["environment"],
                         "input": messages_without_id,
-                        "output": result.completion,
+                        "output": openai_result["choices"][0]["message"]["content"],
                         "latency_ms": latency_ms,
-                        "output_tokens": result.usage_info.completion_tokens,
-                        "input_tokens": result.usage_info.prompt_tokens,
+                        "output_tokens": result.usage.output_tokens,
+                        "input_tokens": result.usage.input_tokens,
                         "model_config_id": prompt["model_config_id"],
                     }
                 )
 
-                return result
+                return openai_result
 
         except Exception as e:
             raise Exception(f"Request failed: {e}")
 
     def ping(self):
         try:
             url = f"{self.options['baseURL']}/ping"
@@ -255,24 +284,41 @@
             status_code = e.response.status_code if e.response else "Unknown"
             response_text = e.response.text if e.response else "Unknown"
             raise Exception(f"Request failed with status code {status_code}: {response_text}")
         except Exception as e:
             raise Exception(f"Request failed: {e}")
 
 def extract_variables(content: str) -> List[str]:
-    import re
-
-    return [v.replace("{{", "").replace("}}", "").strip() for v in re.findall(r"{{(.*?)}}", content)]
-
+    return [v.strip() for v in re.findall(r"{{(.*?)}}", content)]
 
 def replace_variables(content: str, variables: Dict[str, str]) -> str:
-    for variable_name, value in variables.items():
-        content = content.replace(f"{{{{{ variable_name }}}}}", value)
-    return content
+    def replace_func(match):
+        variable_name = match.group(1).strip()
+        return variables.get(variable_name, match.group(0))
 
+    return re.sub(r"{{(.*?)}}", replace_func, content)
 
 def replace_variables_in_prompts(
     prompts: List[Dict], variables: Dict[str, str]
 ) -> List[Dict]:
     return [
         {**prompt, "content": replace_variables(prompt["content"], variables)} for prompt in prompts
-    ]
+    ]
+
+def convert_anthropic_output_to_openai(anthropic_response):
+    choices = [
+        {
+            "message": {"content": choice.text, "role": "assistant"},
+            "index": index,
+            "finish_reason": "stop",
+        }
+        for index, choice in enumerate(anthropic_response.content)
+    ]
+
+    return {
+        "id": anthropic_response.id,
+        "created": int(time.time()),
+        "model": anthropic_response.model,
+        "choices": choices,
+        "object": "chat.completion",
+        "raw": anthropic_response,
+    }
```

### Comparing `outerop-0.1.9/PKG-INFO` & `outerop-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outerop
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: Stephen Byrne
 Author-email: 39441007+stephenbyrne99@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,42 +31,59 @@
 
 To use the Outerop SDK, you need to create an instance of the `Outerop` class with your Outerop API key and optionally provide additional configuration options.
 
 ```python
 from outerop import Outerop
 
 outerop = Outerop(outerop_api_key="YOUR_OUTEROP_API_KEY", options={
-    "openaiApiKey": "YOUR_OPENAI_API_KEY",
-    "anthropicApiKey": "YOUR_ANTHROPIC_API_KEY",
-    "mistralApiKey": "YOUR_MISTRAL_API_KEY"
+   "openaiApiKey": "YOUR_OPENAI_API_KEY",
+   "anthropicApiKey": "YOUR_ANTHROPIC_API_KEY",
+   "mistralApiKey": "YOUR_MISTRAL_API_KEY"
 })
 ```
 
-### Retrieving a Prompt
+### Using the SDK
 
-To retrieve a prompt, use the `get_prompt` method:
+To call the AI API with a specific prompt and variables, you can use the `chat` method:
 
 ```python
-prompt = outerop.get_prompt(prompt_uuid="PROMPT_UUID", environment="development", version="latest")
+result = outerop.chat(
+   team_prompt_name"your-prompt-uuid",
+   version_name_or_environment="development",
+   variables={"name": "John", "age": "25"}
+)
 ```
 
-### Use 
+### Pinning a specific version in version control
 
-To use the prompt, use the `chat` method:
+You can replace the `environment` parameter with a specific version number to pin a specific version of the prompt.
 
 ```python
 result = outerop.chat(
-    prompt_uuid="PROMPT_UUID",
-    environment="development",
-    version="latest",
-    variables={"name": "John", "age": "25"}
+   team_prompt_name"your-prompt-uuid",
+   version_name_or_environment="o-1234567890",
+   variables={"name": "John", "age": "25"}
 )
 ```
 
-The `chat` method returns the AI's response based on the provided prompt and variables.
+We recommend keeping the instantiation of the `Outerop` class outside your main event loop to allow the caching to work.
+
+### Response format
+
+We standardise responses based on the OpenAI SDK for both python and JS. Other models outputs will be transformed to fit the schema. However if you need to, you can access the raw return from the API in the "raw" property of the response.
+
+However we **highly** recommend using the standardised format, as it will allow you to switch models without changing your code.
+
+### Other methods
+
+To retrieve a prompt, use the `get_prompt` method:
+
+```python
+prompt = outerop.get_prompt(team_prompt_name"your-prompt-uuid", environment="development", version="latest")
+```
 
 ## Configuration
 
 The `Outerop` class accepts an optional `options` parameter to configure additional settings:
 
 - `baseURL`: The base URL of the Outerop API (default: "https://app.outerop.com").
 - `loggingEnabled`: Enable or disable logging (default: True).
```

