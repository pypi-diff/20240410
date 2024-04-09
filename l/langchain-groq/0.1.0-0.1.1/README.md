# Comparing `tmp/langchain_groq-0.1.0.tar.gz` & `tmp/langchain_groq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_groq-0.1.0.tar", max compression
+gzip compressed data, was "langchain_groq-0.1.1.tar", max compression
```

## Comparing `langchain_groq-0.1.0.tar` & `langchain_groq-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/LICENSE
--rw-r--r--   0        0        0     1986 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/README.md
--rw-r--r--   0        0        0       72 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/__init__.py
--rw-r--r--   0        0        0    38440 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/chat_models.py
--rw-r--r--   0        0        0        0 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/py.typed
--rw-r--r--   0        0        0     2544 2024-04-03 22:23:27.639171 langchain_groq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1986 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/README.md
+-rw-r--r--   0        0        0       72 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/__init__.py
+-rw-r--r--   0        0        0    38440 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/chat_models.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/py.typed
+-rw-r--r--   0        0        0     2544 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.1/PKG-INFO
```

### Comparing `langchain_groq-0.1.0/LICENSE` & `langchain_groq-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.0/README.md` & `langchain_groq-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.0/langchain_groq/chat_models.py` & `langchain_groq-0.1.1/langchain_groq/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.0/pyproject.toml` & `langchain_groq-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-groq"
-version = "0.1.0"
+version = "0.1.1"
 description = "An integration package connecting Groq and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.40"
+langchain-core = "^0.1.41"
 groq = ">=0.4.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_groq-0.1.0/PKG-INFO` & `langchain_groq-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-groq
-Version: 0.1.0
+Version: 0.1.1
 Summary: An integration package connecting Groq and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: groq (>=0.4.1,<1)
-Requires-Dist: langchain-core (>=0.1.40,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq
 Description-Content-Type: text/markdown
 
 # langchain-groq
 
 ## Welcome to Groq! 🚀
```

