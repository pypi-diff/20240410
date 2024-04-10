# Comparing `tmp/rag_doc_search-0.1.2.tar.gz` & `tmp/rag_doc_search-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_doc_search-0.1.2.tar", max compression
+gzip compressed data, was "rag_doc_search-0.1.4.tar", max compression
```

## Comparing `rag_doc_search-0.1.2.tar` & `rag_doc_search-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     3270 2024-03-13 11:04:32.283414 rag_doc_search-0.1.2/README.md
--rw-r--r--   0        0        0      646 2024-03-13 11:16:18.863280 rag_doc_search-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1533 2024-03-07 06:31:57.288198 rag_doc_search-0.1.2/rag_doc_search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.2/rag_doc_search/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.2/rag_doc_search/src/bot_models/__init__.py
--rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.2/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
--rw-r--r--   0        0        0     4687 2024-03-07 06:31:57.301574 rag_doc_search-0.1.2/rag_doc_search/src/bot_models/chatbot_model.py
--rw-r--r--   0        0        0     2477 2024-03-07 06:31:57.292242 rag_doc_search-0.1.2/rag_doc_search/src/bot_models/openai_chatbot_model.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.2/rag_doc_search/src/enums/__init__.py
--rw-r--r--   0        0        0      564 2024-03-05 06:19:39.071863 rag_doc_search-0.1.2/rag_doc_search/src/enums/provider.py
--rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.2/rag_doc_search/src/enums/search_type.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.2/rag_doc_search/src/models/__init__.py
--rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.2/rag_doc_search/src/models/chat_response.py
--rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.2/rag_doc_search/src/models/user_prompt.py
--rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.2/rag_doc_search/src/prompt_templates/default_prompt_templates.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.2/rag_doc_search/utils/__init__.py
--rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.2/rag_doc_search/utils/callback.py
--rw-r--r--   0        0        0    12712 2024-03-07 06:31:57.295507 rag_doc_search-0.1.2/rag_doc_search/utils/config.py
--rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.2/rag_doc_search/utils/miscellaneous.py
--rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 rag_doc_search-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3270 2024-03-13 11:04:32.283414 rag_doc_search-0.1.4/README.md
+-rw-r--r--   0        0        0      675 2024-04-10 15:18:09.919501 rag_doc_search-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.4/rag_doc_search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.4/rag_doc_search/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/__init__.py
+-rw-r--r--   0        0        0     2991 2024-04-10 15:17:55.474828 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/azure_chatbot_model.py
+-rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
+-rw-r--r--   0        0        0     4687 2024-03-07 06:31:57.301574 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/chatbot_model.py
+-rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.4/rag_doc_search/src/bot_models/openai_chatbot_model.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.4/rag_doc_search/src/enums/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.4/rag_doc_search/src/enums/provider.py
+-rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.4/rag_doc_search/src/enums/search_type.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.4/rag_doc_search/src/models/__init__.py
+-rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.4/rag_doc_search/src/models/chat_response.py
+-rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.4/rag_doc_search/src/models/user_prompt.py
+-rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.4/rag_doc_search/src/prompt_templates/default_prompt_templates.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.4/rag_doc_search/utils/__init__.py
+-rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.4/rag_doc_search/utils/callback.py
+-rw-r--r--   0        0        0    14038 2024-04-09 09:50:20.321385 rag_doc_search-0.1.4/rag_doc_search/utils/config.py
+-rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.4/rag_doc_search/utils/miscellaneous.py
+-rw-r--r--   0        0        0     4259 1970-01-01 00:00:00.000000 rag_doc_search-0.1.4/PKG-INFO
```

### Comparing `rag_doc_search-0.1.2/README.md` & `rag_doc_search-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/pyproject.toml` & `rag_doc_search-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "rag-doc-search"
-version = "0.1.2"
+version = "0.1.4"
 description = "This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs)."
 authors = ["Harshad Kadam <harshad.kadam@sourcefuse.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 boto3 = "^1.34.55"
 botocore = "^1.34.55"
-langchain = "0.1.1"
+langchain = "0.1.14"
 opensearch-py = "^2.4.2"
 faiss-cpu = "^1.8.0"
-openai = "0.28.0"
+openai = "1.16.1"
+langchain-openai = "^0.1.1"
 tiktoken = "^0.6.0"
 pgvector = "^0.2.5"
 psycopg2-binary = "^2.9.9"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `rag_doc_search-0.1.2/rag_doc_search/__init__.py` & `rag_doc_search-0.1.4/rag_doc_search/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,12 +37,15 @@
     match ai_provider:
         case AIProvider.BEDROCK:
             from rag_doc_search.src.bot_models.bedrock_chatbot_model import BedrockChatBot
             return BedrockChatBot()
         case AIProvider.OPENAI:
             from rag_doc_search.src.bot_models.openai_chatbot_model import OpenAIChatBot
             return OpenAIChatBot()
+        case AIProvider.AZURE_OPENAI:
+            from rag_doc_search.src.bot_models.azure_chatbot_model import AzureChatBot
+            return AzureChatBot()
         case _:
             raise ValueError("cannot initiate llm base model for given ai provider")
         
 # Export the init function
 __all__ = ["init"]
```

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/bot_models/bedrock_chatbot_model.py` & `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/bedrock_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/bot_models/chatbot_model.py` & `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/bot_models/openai_chatbot_model.py` & `rag_doc_search-0.1.4/rag_doc_search/src/bot_models/openai_chatbot_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from langchain_community.embeddings.openai import OpenAIEmbeddings
-from langchain.llms.openai import OpenAI
+from langchain_openai import OpenAIEmbeddings
+from langchain_openai import ChatOpenAI
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.chains import RetrievalQA
 from langchain.chains import ConversationalRetrievalChain
 
 from rag_doc_search.src.bot_models.chatbot_model import ChatBotModel
 from rag_doc_search import config
 
@@ -28,15 +28,15 @@
     def create_qa_instance(self) -> RetrievalQA:
         """
         Creates and returns an instance of RetrivalQA using OpenAI Language Model.
 
         Returns:
         An instance of RetrivalQA.
         """
-        cl_llm: BaseLanguageModel = OpenAI(
+        cl_llm: BaseLanguageModel = ChatOpenAI(
             model_name=self.config.llm,
             temperature=self.config.llm_temperature,
             max_tokens=self.config.llm_max_output_tokens,
         )
         qa = self.create_qa_chain(cl_llm)
         return qa
 
@@ -50,15 +50,15 @@
         - `stream_handler`: An instance of StreamingLLMCallbackHandler used for handling streaming callbacks.
         - `tracing`: A boolean indicating whether tracing is enabled. Default is False.
 
         Returns:
         An instance of ConversationalRetrievalChain for conversational question-answering.
         """
         stream_manager = self.create_stream_manager(stream_handler, tracing)
-        cl_llm: BaseLanguageModel = OpenAI(
+        cl_llm: BaseLanguageModel = ChatOpenAI(
             model_name=self.config.llm,
             temperature=self.config.llm_temperature,
             max_tokens=self.config.llm_max_output_tokens,
             streaming=True,
             callback_manager=stream_manager,
         )
         qa = self.create_conversational_qa_chain(cl_llm)
```

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/enums/provider.py` & `rag_doc_search-0.1.4/rag_doc_search/src/enums/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 
 class AIProvider(Enum):
     """
     Enum representing providers available for the AI model API.
 
     Attributes:
     - `OPENAI`: Refers to the OpenAI provider.
+    - `AZURE_OPENAI`: Refers to the Azure OpenAI provider.
     - `BEDROCK`: Refers to the Bedrock provider.
     """
     OPENAI = "OPENAI"
+    AZURE_OPENAI = "AZURE_OPENAI"
     BEDROCK = "BEDROCK"
```

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/enums/search_type.py` & `rag_doc_search-0.1.4/rag_doc_search/src/enums/search_type.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/models/chat_response.py` & `rag_doc_search-0.1.4/rag_doc_search/src/models/chat_response.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/src/prompt_templates/default_prompt_templates.py` & `rag_doc_search-0.1.4/rag_doc_search/src/prompt_templates/default_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/utils/callback.py` & `rag_doc_search-0.1.4/rag_doc_search/utils/callback.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/rag_doc_search/utils/config.py` & `rag_doc_search-0.1.4/rag_doc_search/utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class Config:
     """
     A class representing configuration settings for the System which can be used to initialize the llm model, vector stores and its retrivers argument
 
     ```
     Note: Ensure that the necessary environment variables are set before initializing the configuration.
     If AI Provider is OPENAI then ENV OPENAI_API_KEY is required.
+    If AI Provider is AZURE OPENAI then ENV AZURE_OPENAI_API_KEY, AZURE_OPENAI_ENDPOINT are required and AZURE_OPENAI_API_VERSION is optional, default is '2023-05-15'.
     If AI Provider is BEDROCK then ENV AWS_ACCESS_KEY,AWS_SECRET_ACCESS_KEY are required and AWS_REGION is optional, default is 'us-east-1'.
     If Vector Store Provider is PGVector then PGVECTOR_HOST, PGVECTOR_PORT,  PGVECTOR_DATABASE,  PGVECTOR_USER and PGVECTOR_PASSWORD are required
     """
 
     _instance = None
 
     def __new__(cls, config: dict = None):
@@ -55,14 +56,33 @@
 
         match self.ai_provider:
             case AIProvider.OPENAI:
                 if not os.environ.get("OPENAI_API_KEY"):
                     raise ValueError(
                         "OPENAI_API_KEY environment variable is required for OpenAI"
                     )
+            
+            case AIProvider.AZURE_OPENAI:
+                if not os.environ.get("AZURE_OPENAI_API_KEY"):
+                    raise ValueError(
+                        "AZURE_OPENAI_API_KEY environment variable is required for Azure OpenAI"
+                    )
+                if not os.environ.get("AZURE_OPENAI_ENDPOINT"):
+                    raise ValueError(
+                        "AZURE_OPENAI_ENDPOINT environment variable is required for Azure OpenAI"
+                    )
+                if not os.environ.get("AZURE_OPENAI_API_VERSION"):
+                    os.environ["AZURE_OPENAI_API_VERSION"] = "2023-05-15"
+                    print( os.environ.get("AZURE_OPENAI_API_VERSION") )
+                    self.logger.warning(
+                        'AZURE_OPENAI_API_VERSION key not found in enviroment variables, so "2023-05-15" will be used as default value.'
+                    )
+                    print(
+                        'AZURE_OPENAI_API_VERSION key not found in enviroment variables, so "2023-05-15" will be used as default value.'
+                    )
 
             case AIProvider.BEDROCK:
                 if not os.environ.get("AWS_ACCESS_KEY") or not os.environ.get(
                     "AWS_SECRET_ACCESS_KEY"
                 ):
                     raise ValueError(
                         "AWS_ACCESS_KEY and AWS_SECRET_ACCESS_KEY environment variables are required for Bedrock"
@@ -230,14 +250,15 @@
         if self.vector_store is None:
             match self.vector_store_provider:
                 case VectorStoreProvider.FAISS:
                     self.vector_store = FAISS.load_local(
                         folder_path=self.faiss_vector_embeddings_location,
                         embeddings=embeddings,
                         index_name=self.faiss_index_name,
+                        allow_dangerous_deserialization=True,
                     )
 
                 case VectorStoreProvider.PGVector:
                     CONNECTION_STRING = PGVector.connection_string_from_db_params(
                         driver="psycopg2",
                         host=os.environ.get("PGVECTOR_HOST", "localhost"),
                         port=int(os.environ.get("PGVECTOR_PORT", "5432")),
```

### Comparing `rag_doc_search-0.1.2/rag_doc_search/utils/miscellaneous.py` & `rag_doc_search-0.1.4/rag_doc_search/utils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.2/PKG-INFO` & `rag_doc_search-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rag-doc-search
-Version: 0.1.2
+Version: 0.1.4
 Summary: This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs).
 Author: Harshad Kadam
 Author-email: harshad.kadam@sourcefuse.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.55,<2.0.0)
 Requires-Dist: botocore (>=1.34.55,<2.0.0)
 Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
-Requires-Dist: langchain (==0.1.1)
-Requires-Dist: openai (==0.28.0)
+Requires-Dist: langchain (==0.1.14)
+Requires-Dist: langchain-openai (>=0.1.1,<0.2.0)
+Requires-Dist: openai (==1.16.1)
 Requires-Dist: opensearch-py (>=2.4.2,<3.0.0)
 Requires-Dist: pgvector (>=0.2.5,<0.3.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # RAG doc search
```

