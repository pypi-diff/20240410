# Comparing `tmp/ai-enterprise-agent-0.0.3.tar.gz` & `tmp/ai-enterprise-agent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-enterprise-agent-0.0.3.tar", last modified: Wed Apr  3 17:46:17 2024, max compression
+gzip compressed data, was "ai-enterprise-agent-0.0.4.tar", last modified: Wed Apr 10 14:59:03 2024, max compression
```

## Comparing `ai-enterprise-agent-0.0.3.tar` & `ai-enterprise-agent-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/vector_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/open_api_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/orchestrator_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sequential_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/simple_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sql_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/vector_store_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/fetch_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.290716 ai-enterprise-agent-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-10 14:59:03.290716 ai-enterprise-agent-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.282716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.282716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.282716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.282716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/open_api_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/orchestrator_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/simple_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/sql_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/vector_store_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.286716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.286716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.286716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.286716 ai-enterprise-agent-0.0.4/ai_enterprise_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent/utils/fetch_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:59:03.286716 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-10 14:59:03.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-10 14:59:03.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:59:03.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-10 14:59:03.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 14:59:03.000000 ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:59:03.290716 ai-enterprise-agent-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-10 14:58:58.000000 ai-enterprise-agent-0.0.4/setup.py
```

### Comparing `ai-enterprise-agent-0.0.3/LICENSE` & `ai-enterprise-agent-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/PKG-INFO` & `ai-enterprise-agent-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: attrs==23.2.0
+Requires-Dist: azure-ai-documentintelligence==1.0.0b3
 Requires-Dist: azure-common==1.1.28
 Requires-Dist: azure-core==1.30.1
 Requires-Dist: azure-identity==1.15.0
 Requires-Dist: azure-search==1.0.0b2
 Requires-Dist: azure-search-documents==11.4.0
 Requires-Dist: boto3==1.34.70
 Requires-Dist: botocore==1.34.70
+Requires-Dist: build==1.2.1
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: cffi==1.16.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: dataclasses-json==0.6.4
@@ -75,14 +77,16 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pyasn1==0.5.1
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: PyJWT==2.8.0
+Requires-Dist: pypdf==4.2.0
+Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pywin32==306
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==2.0.0
@@ -94,14 +98,15 @@
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tiktoken==0.5.2
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==1.26.18
+Requires-Dist: wheel==0.43.0
 Requires-Dist: yarl==1.9.4
 
 
 [![Publish new version to NPM](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml/badge.svg)](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml)
 
 # AI Agent
```

### Comparing `ai-enterprise-agent-0.0.3/README.md` & `ai-enterprise-agent-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/agent.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,12 +95,14 @@
     return response
 
   async def _call(self, input: Dict[str, Any]):
     config = self.config
     self.memory = MemoryFactory.build(config.get('history'), input.get('chat_thread_id'))
     chain = self.build_chains()
     result = await chain._call(input)
-
     if config.get('processing_type') == PROCESSING_TYPE.sequential:
       result = self.refine_result(input, result[0])
 
+    self.memory.add_user_message(message=input.get('question'))
+    self.memory.add_ai_message(message=result)
+
     return result
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/chat_history.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/settings.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/interface/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     vector_store_chain = 'vector_store_chain'
 
 class PROCESSING_TYPE(Enum):
     single = 'single'
     sequential = 'sequential'
     orchestrated = 'orchestrated'
 
+class DOCUMENT_INTELLIGENCE_TYPE(Enum):
+    azure = 'azure'
+
 class IModel:
     type: LLM_TYPE
     model: str
     api_key: str
     temperature: Optional[float]
     endpoint: Optional[str]
     api_version: Optional[str]
@@ -101,16 +104,22 @@
     container: Optional[str]
     synchronize: bool = False
     limit: Optional[int]
 
 class ISystem:
     system_message: str
 
+class IDocumentIntelligence:
+    type: DOCUMENT_INTELLIGENCE_TYPE
+    endpoint: str
+    api_key: str
+
 class ISettings:
     model: IModel
     chains: List[CHAIN_TYPE]
     processing_type: PROCESSING_TYPE
     database: Optional[IDatabase]
     open_api: Optional[IOpenApi]
     vector_store: Optional[IVectorSearch]
     history: Optional[IChatHistory]
+    document_intelligence: Optional[DOCUMENT_INTELLIGENCE_TYPE]
     system: ISystem
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/open_api_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/open_api_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,40 +36,42 @@
     self.memory = memory
     self.open_api = config.get('open_api')
     self.config = config
 
   def get_fetch(self, question, custom_system_message) -> str:
     open_api = self.open_api
     schema = open_api.get('data')
-    prompt = ChatPromptTemplate.from_template(
-      """
-      You are an AI with expertise in OpenAPI and Swagger.\n
-      You should follow the following rules when generating an answer:\n
+    template = """
+      You are an AI with expertise in OpenAPI and Swagger.
+      You should follow the following rules when generating an answer:
       - Only execute the request on the service if the question is not in History, if the question has already been answered, use the same answer and do not make a request on the service.
-      - The response must be a JSON object containing an url, content type, method, and data, without triple quotes, json string on start and the end.\n\n
+      - The response must be a JSON object containing an url, content type, method, and data, without triple quotes, json string on start and the end.
       {custom_system_message}
       -------------------------------------------\n
       Schema: {schema}\n
       -------------------------------------------\n
       History: {history}\n
       -------------------------------------------\n
       Question: {question}\n
       ------------------------------------------\n
       API ANSWER:
-      """
-    )
+    """
+    prompt = ChatPromptTemplate.from_template(template)
     chain = prompt | self.model | StrOutputParser()
     return chain.invoke({"schema": schema, "question": question, "history": self.memory.get_messages(), "custom_system_message": custom_system_message})
 
   def chain(self, question, custom_system_message) -> RunnableSerializable[Any, Any]:
     fetch_sentence = self.get_fetch(question, custom_system_message)
     request = json.loads(fetch_sentence)
     response = fetch(url=request.get('url'), method=request.get('method'), data=request.get('data'), headers={})
     template = """
         Based on the context below, answer the question with natural language.
+        You should follow the following rules when generating and answer:
+        - Only attempt to answer if a question was posed.
+        - Always answer the question in the language in which the question was asked.
         Context: {context}
         Question: {question}
       """
     prompt = ChatPromptTemplate.from_template(template)
     chain = (RunnablePassthrough.assign(context=lambda _: response)) | prompt | self.model | StrOutputParser()
     return chain
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/orchestrator_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/orchestrator_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sequential_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/sequential_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/simple_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/simple_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,14 @@
     settings = self.config.get('system')
     prompt = ChatPromptTemplate.from_template(self.build_system_messages(settings.get('system_message')))
     return  RunnablePassthrough.assign(history=RunnableLambda(self.memory.get_messages()) | itemgetter("history")) | prompt | self.model | StrOutputParser()
 
   async def _call(self, input: Dict[str, Any]):
     chain = self.chain()
     response = chain.invoke(input)
-    self.memory.add_user_message(message=input.get('question'))
-    self.memory.add_ai_message(message=response)
     if self.config.get('processing_type') == PROCESSING_TYPE.sequential:
       return  { self.output_key: response }
     return response
 
   @property
   def _chain_type(self) -> str:
     return "simple_chain"
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sql_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/sql_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,18 @@
     try:
       return self.db.run(query)
     except Exception as e:
       print(f"Error executing query: {e}")
 
   def create_sql(self, _):
     template = """Based on the table schema below, write only a SQL query that would answer the user's question.
+    Your response must only be a valid SQL query, based on the schema provided.
     Remember to put double quotes around database table names. Remove triple quotes and sql word of the sentences.
+    Here are some important observations for generating the query:
+    - Only execute the request on the service if the question is not in History, if the question has already been answered, use the same answer and do not make a query on the database.
     If you don't find out what the table schema is, only response friendly can't be written a valid SQL query.
     Schema: {schema}
     History: {history}
     Question: {question}
     SQL Query:"""
     prompt = ChatPromptTemplate.from_template(template)
     return (
@@ -94,17 +97,17 @@
         or sqlL.startswith("insert")
     ):
       return sql
 
     if "```sql" in sqlL:
       regex = r"```(.*?)```"
       matches = re.findall(regex, sqlL, re.DOTALL)
-      codeBlocks = [match.replace("sql", "") for match in matches]
-      sqlBlock = codeBlocks[0]
-      return sqlBlock
+      code_blocks = [match.replace("sql", "") for match in matches]
+      sql_block = code_blocks[0]
+      return sql_block
     return None
 
   def chain(self, custom_system_message) -> RunnableSerializable[Any, Any]:
     template = """If you don't get a valid query to execute, only reply in a friendly manner that you didn't find the answer.\n
     Only execute the request on the service if the question is not in History, if the question has already been answered, use the same answer and do not make a query on the database.\n
     Based on the table schema below, question, sql query, and sql response, write a natural language response:\n\n
     {custom_system_message}
@@ -124,20 +127,17 @@
         | prompt | self.model | StrOutputParser()
       )
       return chain
     except Exception as e:
       print(f"Error: {e}")
 
   async def _call(self, input: Dict[str, Any] = None):
-    question = input.get('question')
     custom_system_message = input.get('custom_system_message', None)
     chain = self.chain(custom_system_message)
     response = chain.invoke(input)
-    self.memory.add_user_message(message=question)
-    self.memory.add_ai_message(message=response)
     if self.config.get('processing_type') == PROCESSING_TYPE.sequential:
       return { self.output_key: response }
     return response
 
   @property
   def _chain_type(self) -> str:
     return "sql_chain"
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/vector_store_chain.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chains/vector_store_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_history.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory_chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_redis.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/chat_history/memory_chat_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,14 @@
             "Please implement add_message or add_messages."
         )
 
   def add_messages(self, messages: Sequence[BaseMessage]) -> None:
     pass
 
   def load_memory_variables(self, inputs: Optional[Dict[str, Any]]) -> Dict[str, Any]:
-    return {self.memory_key: self.chat_history.messages}
+    return { self.memory_key: self.chat_history.messages }
 
   def get_messages(self):
     return self.load_memory_variables
 
   def clear(self):
     pass
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/azure.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/azure.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/google.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/google.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/model.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/llm/model.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/aws.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/aws.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/azure.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/pinecone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,39 @@
 from typing import Any, Iterable, List, Optional, Tuple, Type
 
-from azure.search.documents.indexes.models import (SearchableField,
-                                                   SearchField,
-                                                   SearchFieldDataType)
 from langchain.chains.retrieval_qa.base import RetrievalQA
-from langchain_community.vectorstores.azuresearch import AzureSearch
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.vectorstores import VectorStore
+from langchain_pinecone.vectorstores import PineconeVectorStore
 
 from ai_enterprise_agent.interface.settings import VECTOR_STORE_TYPE, ISettings
 from ai_enterprise_agent.interface.vector_search import ISearchType
 from ai_enterprise_agent.services.vector_store.embedding import \
     EmbeddingFactory
 
 
-class AzureVectorSearch(VectorStore):
+class PineconeVectorSearch(VectorStore):
 
   def __init__(self, config: ISettings, model: BaseChatModel) -> None:
     super().__init__()
     self.config = config
     self.model = model
     self.vector_store = self.build()
 
   def build(self):
-    config = self.config.get('vector_store')
-    embeddings = EmbeddingFactory.build(VECTOR_STORE_TYPE.azure_search, self.config)
+    config = self.config('vector_store')
+    embeddings = EmbeddingFactory.build(VECTOR_STORE_TYPE.pinecone, self.config)
+    return PineconeVectorStore(pinecone_api_key=config.get('api_key'), embedding=embeddings, index_name=config.get('index_name'))
 
-    fields = [
-      SearchableField(
-          name=config.get('fields_content'),
-          type=SearchFieldDataType.String,
-      ),
-      SearchField(
-          name=config.get('fields_content'),
-          type=SearchFieldDataType.Collection(SearchFieldDataType.Single),
-          searchable=True,
-          vector_search_dimensions=len(embeddings.embed_query("Text")),
-          vector_search_profile_name=config.get('vector_search_profile_name'),
-      ),
-    ]
-
-    return AzureSearch(
-      azure_search_endpoint=config.get('endpoint'),
-      azure_search_key=config.get('api_key'),
-      index_name=config.get('index_name'),
-      embedding_function=embeddings.embed_query,
-      fields=fields
-    )
-
-  def similarity_search(self, query: str, k: int = 4, search_type: ISearchType = ISearchType.similarity) -> List[Document]:
+  def similarity_search(self, query: str, k: int = 4) -> List[Document]:
     return self.vector_store.similarity_search(
       query=query,
       k=k,
-      search_type=search_type
     )
 
   def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int]) -> List[Tuple[Document, float]]:
     return self.vector_store.similarity_search_with_relevance_scores(
       query=query,
       k=k,
       score_threshold=score_threshold,
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/embedding.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/embedding.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/vector_store.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/services/vector_store/vector_store.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/fetch_helper.py` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent/utils/fetch_helper.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/PKG-INFO` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: attrs==23.2.0
+Requires-Dist: azure-ai-documentintelligence==1.0.0b3
 Requires-Dist: azure-common==1.1.28
 Requires-Dist: azure-core==1.30.1
 Requires-Dist: azure-identity==1.15.0
 Requires-Dist: azure-search==1.0.0b2
 Requires-Dist: azure-search-documents==11.4.0
 Requires-Dist: boto3==1.34.70
 Requires-Dist: botocore==1.34.70
+Requires-Dist: build==1.2.1
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: cffi==1.16.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: dataclasses-json==0.6.4
@@ -75,14 +77,16 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pyasn1==0.5.1
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: PyJWT==2.8.0
+Requires-Dist: pypdf==4.2.0
+Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pywin32==306
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==2.0.0
@@ -94,14 +98,15 @@
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tiktoken==0.5.2
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==1.26.18
+Requires-Dist: wheel==0.43.0
 Requires-Dist: yarl==1.9.4
 
 
 [![Publish new version to NPM](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml/badge.svg)](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml)
 
 # AI Agent
```

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/SOURCES.txt` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/requires.txt` & `ai-enterprise-agent-0.0.4/ai_enterprise_agent.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 aiohttp==3.9.3
 aiosignal==1.3.1
 annotated-types==0.6.0
 anyio==4.3.0
 attrs==23.2.0
+azure-ai-documentintelligence==1.0.0b3
 azure-common==1.1.28
 azure-core==1.30.1
 azure-identity==1.15.0
 azure-search==1.0.0b2
 azure-search-documents==11.4.0
 boto3==1.34.70
 botocore==1.34.70
+build==1.2.1
 cachetools==5.3.3
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 colorama==0.4.6
 cryptography==42.0.5
 dataclasses-json==0.6.4
@@ -64,14 +66,16 @@
 psycopg2-binary==2.9.9
 pyasn1==0.5.1
 pyasn1-modules==0.3.0
 pycparser==2.21
 pydantic==2.6.4
 pydantic_core==2.16.3
 PyJWT==2.8.0
+pypdf==4.2.0
+pyproject_hooks==1.0.0
 python-dateutil==2.9.0.post0
 pywin32==306
 PyYAML==6.0.1
 redis==5.0.3
 regex==2023.12.25
 requests==2.31.0
 requests-oauthlib==2.0.0
@@ -83,8 +87,9 @@
 SQLAlchemy==2.0.29
 tenacity==8.2.3
 tiktoken==0.5.2
 tqdm==4.66.2
 typing-inspect==0.9.0
 typing_extensions==4.10.0
 urllib3==1.26.18
+wheel==0.43.0
 yarl==1.9.4
```

### Comparing `ai-enterprise-agent-0.0.3/setup.py` & `ai-enterprise-agent-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='ai-enterprise-agent',
-    version='0.0.3',
+    version='0.0.4',
     license='Apache 2.0 License',
     author='Author',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='autor@autor.com.br',
     keywords='ai ai-agent agent assistant enterprise',
     description='AI Agent simplifies the implementation and use of generative AI with LangChain.',
@@ -17,21 +17,23 @@
     package_dir={'': '.', 'ai_enterprise_agent': './ai_enterprise_agent', 'ai_enterprise_agent.interface': './ai_enterprise_agent/interface', 'ai_enterprise_agent.services': './ai_enterprise_agent/services', 'ai_enterprise_agent.services.chains': './ai_enterprise_agent/services/chains', 'ai_enterprise_agent.services.chat_history': './ai_enterprise_agent/services/chat_history', 'ai_enterprise_agent.services.llm': './ai_enterprise_agent/services/llm', 'ai_enterprise_agent.services.vector_store': './ai_enterprise_agent/services/vector_store', 'ai_enterprise_agent.utils': './ai_enterprise_agent/utils'},
     install_requires=[
       'aiohttp==3.9.3',
       'aiosignal==1.3.1',
       'annotated-types==0.6.0',
       'anyio==4.3.0',
       'attrs==23.2.0',
+      'azure-ai-documentintelligence==1.0.0b3',
       'azure-common==1.1.28',
       'azure-core==1.30.1',
       'azure-identity==1.15.0',
       'azure-search==1.0.0b2',
       'azure-search-documents==11.4.0',
       'boto3==1.34.70',
       'botocore==1.34.70',
+      'build==1.2.1',
       'cachetools==5.3.3',
       'certifi==2024.2.2',
       'cffi==1.16.0',
       'charset-normalizer==3.3.2',
       'colorama==0.4.6',
       'cryptography==42.0.5',
       'dataclasses-json==0.6.4',
@@ -82,14 +84,16 @@
       'psycopg2-binary==2.9.9',
       'pyasn1==0.5.1',
       'pyasn1-modules==0.3.0',
       'pycparser==2.21',
       'pydantic==2.6.4',
       'pydantic_core==2.16.3',
       'PyJWT==2.8.0',
+      'pypdf==4.2.0',
+      'pyproject_hooks==1.0.0',
       'python-dateutil==2.9.0.post0',
       'pywin32==306',
       'PyYAML==6.0.1',
       'redis==5.0.3',
       'regex==2023.12.25',
       'requests==2.31.0',
       'requests-oauthlib==2.0.0',
@@ -101,10 +105,11 @@
       'SQLAlchemy==2.0.29',
       'tenacity==8.2.3',
       'tiktoken==0.5.2',
       'tqdm==4.66.2',
       'typing-inspect==0.9.0',
       'typing_extensions==4.10.0',
       'urllib3==1.26.18',
+      'wheel==0.43.0',
       'yarl==1.9.4',
     ]
 )
```

