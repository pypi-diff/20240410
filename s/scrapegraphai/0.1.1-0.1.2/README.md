# Comparing `tmp/scrapegraphai-0.1.1.tar.gz` & `tmp/scrapegraphai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.1.1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.1.2.tar", max compression
```

## Comparing `scrapegraphai-0.1.1.tar` & `scrapegraphai-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.1/LICENSE
--rw-r--r--   0        0        0     6321 2024-04-09 09:44:17.063929 scrapegraphai-0.1.1/README.md
--rw-r--r--   0        0        0     1621 2024-04-09 09:44:31.922633 scrapegraphai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3010 2024-04-09 09:44:17.065498 scrapegraphai-0.1.1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     3041 2024-04-08 20:24:28.569893 scrapegraphai-0.1.1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2160 2024-04-09 09:44:17.065954 scrapegraphai-0.1.1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2264 2024-04-09 08:20:31.578158 scrapegraphai-0.1.1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3000 2024-04-09 09:44:17.066614 scrapegraphai-0.1.1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      700 2024-04-09 09:44:17.066995 scrapegraphai-0.1.1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3793 2024-04-09 09:44:17.067324 scrapegraphai-0.1.1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.1.1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      600 2024-04-09 09:44:17.067663 scrapegraphai-0.1.1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.1.1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.1.1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.1.1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.1.1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.1.1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.1.1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3209 2024-04-09 09:44:17.067983 scrapegraphai-0.1.1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-08 20:26:19.442517 scrapegraphai-0.1.1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4701 2024-04-09 09:44:17.068360 scrapegraphai-0.1.1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4521 2024-04-09 08:22:49.561048 scrapegraphai-0.1.1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-08 20:27:04.824493 scrapegraphai-0.1.1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 scrapegraphai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6831 2024-04-09 11:20:43.619492 scrapegraphai-0.1.2/README.md
+-rw-r--r--   0        0        0     1621 2024-04-09 11:47:21.583850 scrapegraphai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3010 2024-04-09 09:44:17.065498 scrapegraphai-0.1.2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     3041 2024-04-08 20:24:28.569893 scrapegraphai-0.1.2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2161 2024-04-09 11:20:43.625882 scrapegraphai-0.1.2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2264 2024-04-09 08:20:31.578158 scrapegraphai-0.1.2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3000 2024-04-09 09:44:17.066614 scrapegraphai-0.1.2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.1.2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.1.2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.1.2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.1.2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.1.2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.1.2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.1.2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.1.2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.1.2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.1.2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3209 2024-04-09 09:44:17.067983 scrapegraphai-0.1.2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-08 20:26:19.442517 scrapegraphai-0.1.2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4701 2024-04-09 09:44:17.068360 scrapegraphai-0.1.2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4521 2024-04-09 08:22:49.561048 scrapegraphai-0.1.2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-08 20:27:04.824493 scrapegraphai-0.1.2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     8418 1970-01-01 00:00:00.000000 scrapegraphai-0.1.2/PKG-INFO
```

### Comparing `scrapegraphai-0.1.1/LICENSE` & `scrapegraphai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/README.md` & `scrapegraphai-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,33 @@
 ### Case 1: Extracting informations using a local LLM 
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
+from scrapegraphai.graphs import SmartScraperGraph
+
+graph_config = {
+    "llm": {
+        "model": "ollama/mistral",
+        "temperature": 0,
+        "format": "json",  # Ollama needs the format to be specified explicitly
+    },
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the news with their description.",
+    # also accepts a string with the already downloaded HTML code
+    source="https://www.wired.com",
+    config=graph_config
+)
 
+result = smart_scraper_graph.run()
+print(result)
 ```
 
 
 ### Case 2: Extracting informations using Openai model
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
```

### Comparing `scrapegraphai-0.1.1/pyproject.toml` & `scrapegraphai-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.1.1"
+version = "0.1.2"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.1.1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.1.2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.1.2/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.1.2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.1.2/scrapegraphai/graphs/search_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
+
 class SearchGraph(AbstractGraph):
     """ 
     Module for searching info on the internet
     """
 
     def _create_graph(self):
         """
```

### Comparing `scrapegraphai-0.1.1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.1.2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.1.2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.1.2/scrapegraphai/helpers/models_tokens.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 
     "ollama": {
         "llama2": 4096,
         "mistral": 8192,
         "codellama": 16000,
         "dolphin-mixtral": 32000,
         "mistral-openorca": 32000,
+        "stablelm-zephyr": 8192
     }
 }
```

### Comparing `scrapegraphai-0.1.1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.1.2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Nodes metadata for the scrapegraphai package.
 """
 
 nodes_metadata = {
     "SearchInternetNode": {
-        "description": "Refactors the user's query into a search query and fetches the search result URLs.",
+        "description": """Refactors the user's query into a search
+          query and fetches the search result URLs.""",
         "type": "node",
         "args": {
             "user_input": "User's query or question."
         },
         "returns": "Updated state with the URL of the search result under 'url' key."
     },
     "FetchNode": {
```

### Comparing `scrapegraphai-0.1.1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.1.2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.1.2/scrapegraphai/models/azure_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ 
 Azure Openai configuration wrapper
 """
 from langchain_openai import AzureChatOpenAI
 
+
 class AzureOpenAI(AzureChatOpenAI):
     """Class for wrapping openai module"""
 
     def __init__(self, llm_config: dict):
         """
         A wrapper for the ChatOpenAI class that provides default configuration
         and could be extended with additional methods if needed.
```

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/gemini.py` & `scrapegraphai-0.1.2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/ollama.py` & `scrapegraphai-0.1.2/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/openai.py` & `scrapegraphai-0.1.2/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.1.2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.1.2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.1.2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.1.2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.1/PKG-INFO` & `scrapegraphai-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.1.1
+Version: 0.1.2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
@@ -80,15 +80,33 @@
 ### Case 1: Extracting informations using a local LLM 
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
+from scrapegraphai.graphs import SmartScraperGraph
+
+graph_config = {
+    "llm": {
+        "model": "ollama/mistral",
+        "temperature": 0,
+        "format": "json",  # Ollama needs the format to be specified explicitly
+    },
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the news with their description.",
+    # also accepts a string with the already downloaded HTML code
+    source="https://www.wired.com",
+    config=graph_config
+)
 
+result = smart_scraper_graph.run()
+print(result)
 ```
 
 
 ### Case 2: Extracting informations using Openai model
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
```

