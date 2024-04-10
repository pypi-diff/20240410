# Comparing `tmp/neo_sapiens-0.0.2.tar.gz` & `tmp/neo_sapiens-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_sapiens-0.0.2.tar", max compression
+gzip compressed data, was "neo_sapiens-0.0.4.tar", max compression
```

## Comparing `neo_sapiens-0.0.2.tar` & `neo_sapiens-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-04-07 22:57:58.790247 neo_sapiens-0.0.2/LICENSE
--rw-r--r--   0        0        0      162 2024-04-08 23:22:44.874098 neo_sapiens-0.0.2/README.md
--rw-r--r--   0        0        0      332 2024-04-08 23:09:17.415055 neo_sapiens-0.0.2/neo_sapiens/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-08 21:24:39.357613 neo_sapiens-0.0.2/neo_sapiens/few_shot_prompts.py
--rw-r--r--   0        0        0     5404 2024-04-08 23:19:48.269885 neo_sapiens-0.0.2/neo_sapiens/hass_schema.py
--rw-r--r--   0        0        0     1342 2024-04-08 23:23:11.870591 neo_sapiens-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 neo_sapiens-0.0.2/setup.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 neo_sapiens-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 22:57:58.790247 neo_sapiens-0.0.4/LICENSE
+-rw-r--r--   0        0        0      315 2024-04-10 14:58:18.826324 neo_sapiens-0.0.4/README.md
+-rw-r--r--   0        0        0      455 2024-04-10 14:50:26.476068 neo_sapiens-0.0.4/neo_sapiens/__init__.py
+-rw-r--r--   0        0        0     6423 2024-04-10 14:52:15.126745 neo_sapiens-0.0.4/neo_sapiens/few_shot_prompts.py
+-rw-r--r--   0        0        0     6732 2024-04-10 14:49:59.540629 neo_sapiens-0.0.4/neo_sapiens/hass_schema.py
+-rw-r--r--   0        0        0     1342 2024-04-10 14:58:27.026683 neo_sapiens-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 neo_sapiens-0.0.4/setup.py
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 neo_sapiens-0.0.4/PKG-INFO
```

### Comparing `neo_sapiens-0.0.2/LICENSE` & `neo_sapiens-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_sapiens-0.0.2/neo_sapiens/hass_schema.py` & `neo_sapiens-0.0.4/neo_sapiens/hass_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,52 @@
+import json
+import os
+import re
 from typing import List
 
+from dotenv import load_dotenv
 from pydantic import BaseModel, Field
-from swarms import Agent, OpenAIChat
-from swarms.utils.json_utils import base_model_to_json
-from neo_sapiens.hass_schema import (
+from swarms import Agent, Anthropic, SwarmNetwork
+
+from neo_sapiens.few_shot_prompts import (
     data,
     data1,
     data2,
     data3,
-    data5,
+    orchestrator_prompt_agent,
 )
-from neo_sapiens.main import browser, terminal
-from swarms import SwarmNetwork
-from swarms.utils.parse_code import extract_code_from_markdown
+
+# Load environment variables
+load_dotenv()
 
 # Swarmnetowr
 network = SwarmNetwork(api_enabled=True, logging_enabled=True)
 
 
-def tool_router(tool: str, *args, **kwargs):
-    if "terminal" in tool:
-        return terminal(*args, **kwargs)
-    elif "browser" in tool:
-        return browser(*args, **kwargs)
+# def tool_router(tool: str, *args, **kwargs):
+#     if "terminal" in tool:
+#         return terminal(*args, **kwargs)
+#     elif "browser" in tool:
+#         return browser(*args, **kwargs)
+
+
+def find_agent_id_by_name(name: str):
+    """
+    Find an agent's ID by its name.
+
+    Args:
+        name (str): The name of the agent.
+
+    Returns:
+        str: The ID of the agent.
+    """
+    agents = network.list_agents()
+    for agent in agents:
+        if agent.name == name:
+            return agent.id
 
 
 class ToolSchema(BaseModel):
     tool: str = Field(
         ...,
         title="Tool name",
         description="Either `browser` or `terminal`",
@@ -77,41 +97,47 @@
     # rules: str = Field(
     #     ...,
     #     title="Rules for the agents",
     #     description="Rules for the agents",
     # )
 
 
-def transform_schema_to_json(schema: BaseModel):
-    json = schema.model_json_schema()
-    json = base_model_to_json(HassSchema)
-    print(f"JSON Schema: {json}")
-
-
-def parse_hass_schema(data: str) -> tuple:
-    """
-    Parses the Home Assistant schema data and returns a tuple containing the plan,
-    number of agents, and the agents themselves.
-
-    Args:
-        data (str): The Home Assistant schema data to be parsed.
+# import json
+def parse_json_from_input(input_str):
+    # Validate input is not None or empty
+    if not input_str:
+        print("Error: Input string is None or empty.")
+        return None, None, None
+
+    # Attempt to extract JSON from markdown using regular expression
+    json_pattern = re.compile(r"```json\n(.*?)\n```", re.DOTALL)
+    match = json_pattern.search(input_str)
+    json_str = match.group(1).strip() if match else input_str.strip()
+    # print(json_str)
+
+    # Attempt to parse the JSON string
+    try:
+        data = json.loads(json_str)
+        # print(str(data))
+    except json.JSONDecodeError as e:
+        print(f"Error: JSON decoding failed with message '{e}'")
+        return None, None, None
 
-    Returns:
-        tuple: A tuple containing the plan, number of agents, and the agents themselves.
-    """
-    parsed_data = eval(data)
-    hass_schema = HassSchema(**parsed_data)
+    hass_schema = HassSchema(**data)
     return (
         hass_schema.plan,
         hass_schema.number_of_agents,
         hass_schema.agents,
         # hass_schema.rules,
     )
 
 
+# You can test the function with a markdown string similar to the one provided.
+
+
 def merge_plans_into_str(
     plan: List[str] = [data, data1, data2, data3]
 ) -> str:
     """
     Merge a list of plans into a single string.
 
     Args:
@@ -119,16 +145,16 @@
 
     Returns:
         str: The merged plans as a single string.
     """
     return "\n".join(plan)
 
 
-parsed_schema = parse_hass_schema(data5)
-plan, number_of_agents, agents = parsed_schema
+# parsed_schema = parse_hass_schema(data5)
+# plan, number_of_agents, agents = parsed_schema
 
 
 def merge_rules_into_str(prompts: List[str]):
     """
     Merge a list of prompts into a single string.
 
     Args:
@@ -160,59 +186,91 @@
         print(agent.name)
         print(agent.system_prompt)
         print("\n")
 
         out = Agent(
             agent_name=name,
             system_prompt=system_prompt,
-            llm=OpenAIChat(
-                openai_api_key="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",
+            llm=Anthropic(
+                anthropic_api_key=os.getenv("ANTHROPIC_API_KEY")
             ),
-            max_loops="auto",
+            max_loops=1,
             autosave=True,
             dashboard=False,
             verbose=True,
             stopping_token="<DONE>",
             interactive=True,
         )
 
         network.add_agent(out)
 
     return out
 
 
-out = create_agents(agents)
-# print(out)
+# out = create_agents(agents)
+# # print(out)
 
-# Use network
-list_agents = network.list_agents()
-print(list_agents)
+# # # Use network
+# # list_agents = network.list_agents()
+# # print(list_agents)
 
 # # Run the workflow on a task
 # run = network.run_single_agent(
 #     agent2.id, "What's your name?"
 # )
 # print(out)
 
 
-def run_task(task: str = None):
+def run_swarm(task: str = None):
+    """
+    Run a task using the Swarm Orchestrator agent.
+
+    Args:
+        task (str): The task to be executed.
+
+    Returns:
+        None
+    """
+    system_prompt_daddy = orchestrator_prompt_agent(task)
+    # print(system_prompt_daddy)
     agent = Agent(
         agent_name="Swarm Orchestrator",
-        system_prompt=None,
-        llm=OpenAIChat(
-            openai_api_key=None,
+        system_prompt=system_prompt_daddy,
+        llm=Anthropic(
+            anthropic_api_key=os.getenv("ANTHROPIC_API_KEY"),
+            max_tokens=4000,
         ),
-        max_loops="auto",
+        max_loops=1,
         autosave=True,
         dashboard=False,
         verbose=True,
         stopping_token="<DONE>",
         # interactive=True,
     )
-    out = agent(task)
-    json = extract_code_from_markdown(out)
-    parsed_schema = parse_hass_schema(json)
-    plan, number_of_agents, agents = parsed_schema
+    out = agent.run(task)
+    # print(out)
+    out = str(out)
+    print(f"Output: {out}")
+    out = parse_json_from_input(out)
+    print(str(out))
+    plan, number_of_agents, agents = out
+    print(agents)
     agents = create_agents(agents)
-    # Run the agents
-    
-    
+    print(agents)
+    # return agents
+    # print(out)
+    # json_template = extract_code_from_markdown(str(out))
+    # print(json_template)
+    # parsed_schema = parse_json_from_markdown(json_template)
+    # plan, number_of_agents, agents = parsed_schema
+    # print(f"Plan: {agents}")
+    # # agents = create_agents(agents)
+    # print(agents)
+    # return agents
+    return out
+
+
+# out = run_task(
+#     "Create a team of AI engineers to create an AI for a"
+#     " self-driving car"
+# )
+# # print(out)
```

### Comparing `neo_sapiens-0.0.2/pyproject.toml` & `neo_sapiens-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "neo-sapiens"
-version = "0.0.2"
+version = "0.0.4"
 description = "Neo Sapiens - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/NeoSapiens"
 documentation = "https://github.com/kyegomez/NeoSapiens"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/NeoSapiens"
```

### Comparing `neo_sapiens-0.0.2/setup.py` & `neo_sapiens-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic', 'swarms']
 
 setup_kwargs = {
     'name': 'neo-sapiens',
-    'version': '0.0.2',
+    'version': '0.0.4',
     'description': 'Neo Sapiens - Pytorch',
-    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Neo Sapiens\n\n\n## install\n`$ pip install -U swarms neo-sapiens`\n\n\n## usage\n\n\n\n# License\nMIT\n',
+    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Neo Sapiens\n\n\n## install\n`$ pip install -U swarms neo-sapiens`\n\n\n## usage\n```python\nfrom neo_sapiens import run_swarm\n\n# Run the swarm\nout = run_swarm("Create a self-driving car system using a team of AI agents")\nprint(out)\n```\n\n\n# License\nMIT\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/NeoSapiens',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `neo_sapiens-0.0.2/PKG-INFO` & `neo_sapiens-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-sapiens
-Version: 0.0.2
+Version: 0.0.4
 Summary: Neo Sapiens - Pytorch
 Home-page: https://github.com/kyegomez/NeoSapiens
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -29,13 +29,19 @@
 
 
 ## install
 `$ pip install -U swarms neo-sapiens`
 
 
 ## usage
+```python
+from neo_sapiens import run_swarm
 
+# Run the swarm
+out = run_swarm("Create a self-driving car system using a team of AI agents")
+print(out)
+```
 
 
 # License
 MIT
```

