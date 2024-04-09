# Comparing `tmp/langchain_anthropic-0.1.6.tar.gz` & `tmp/langchain_anthropic-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_anthropic-0.1.6.tar", max compression
+gzip compressed data, was "langchain_anthropic-0.1.7.tar", max compression
```

## Comparing `langchain_anthropic-0.1.6.tar` & `langchain_anthropic-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/LICENSE
--rw-r--r--   0        0        0     1215 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/README.md
--rw-r--r--   0        0        0      225 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    17383 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0     4908 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    11687 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/llms.py
--rw-r--r--   0        0        0     2194 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/output_parsers.py
--rw-r--r--   0        0        0        0 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2677 2024-04-04 21:30:22.299585 langchain_anthropic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1215 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/README.md
+-rw-r--r--   0        0        0      225 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    25121 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    11687 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2194 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2677 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.7/PKG-INFO
```

### Comparing `langchain_anthropic-0.1.6/LICENSE` & `langchain_anthropic-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.6/README.md` & `langchain_anthropic-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.6/langchain_anthropic/experimental.py` & `langchain_anthropic-0.1.7/langchain_anthropic/experimental.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.6/langchain_anthropic/llms.py` & `langchain_anthropic-0.1.7/langchain_anthropic/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.6/langchain_anthropic/output_parsers.py` & `langchain_anthropic-0.1.7/langchain_anthropic/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.6/pyproject.toml` & `langchain_anthropic-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-anthropic"
-version = "0.1.6"
+version = "0.1.7"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.33"
+langchain-core = "^0.1.41"
 anthropic = ">=0.23.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_anthropic-0.1.6/PKG-INFO` & `langchain_anthropic-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-anthropic
-Version: 0.1.6
+Version: 0.1.7
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: langchain-core (>=0.1.33,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

