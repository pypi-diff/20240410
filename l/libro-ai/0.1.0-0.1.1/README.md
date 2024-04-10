# Comparing `tmp/libro_ai-0.1.0.tar.gz` & `tmp/libro_ai-0.1.1.tar.gz`

## Comparing `libro_ai-0.1.0.tar` & `libro_ai-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libro_ai-0.1.0/.python-version
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/_version.py
--rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/__init__.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/executor.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/item.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/langchain_variable.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/langchain_variable_executor.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/openai.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/openai_chat_executor.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/provider.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/chat/source.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/flow/__init__.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/flow/libro_client.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/flow/nb_args.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/magics/__init__.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/magics/exception.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/magics/prompt_magic.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/utils/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/utils/base.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/utils/inspector.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 libro_ai-0.1.0/src/libro_ai/utils/langchain.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 libro_ai-0.1.0/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 libro_ai-0.1.0/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 libro_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libro_ai-0.1.1/.python-version
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/_version.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/extensions.py
+-rwxr-xr-x   0        0        0      852 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/chat_message.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/chat_record.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/executor.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/item.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/langchain_variable.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/langchain_variable_executor.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/object.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/object_manager.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/openai.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/openai_chat_executor.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/provider.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/source.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/__init__.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/libro_client.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/nb_args.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/__init__.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/exception.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/prompt_magic.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/base.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/inspector.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/langchain.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 libro_ai-0.1.1/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro_ai-0.1.1/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 libro_ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 libro_ai-0.1.1/PKG-INFO
```

### Comparing `libro_ai-0.1.0/src/libro_ai/chat/executor.py` & `libro_ai-0.1.1/src/libro_ai/chat/executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 from abc import ABC, abstractmethod
 import requests
 from pydantic import BaseModel
-from IPython.display import display
-from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
+from typing import Any, Dict
+
+from ..utils import is_ipython
+
 
 class ChatExecutor(BaseModel, ABC):
     name: str = "custom"
     order: int = 0
 
     @abstractmethod
     def run(
-        self,value,**kwargs,
-    ) -> str:
+        self,
+        value,
+        **kwargs,
+    ) -> Any:
         """Chat and get result."""
-    
+
     def display(
-        self,value,**kwargs,
-    ) -> str:
-        data = {
-            "application/vnd.libro.prompt+json": value
-        }
-        display(data, raw=True)
+        self,
+        value,
+        **kwargs,
+    ):
+        data = {"application/vnd.libro.prompt+json": value}
+        if is_ipython():
+            from IPython.display import display
+
+            display(data, raw=True)
+
 
 class LLMChat(ChatExecutor):
     name: str = "custom"
 
     @abstractmethod
-    def load(
-        self,config: dict
-    ) -> bool:
+    def load(self, config: dict) -> bool:
         """Load LLM from Config Dict."""
 
-    @abstractmethod
-    def run(
-        self,value,**kwargs,
-    ) -> str:
-        """Chat and get result."""
 
 class APIChat(ChatExecutor):
     name: str = "api"
     url: str
     headers: Dict[str, str]
     data: Dict[str, Any]
-    
+
     def get_request_config(self):
-        return {
-            "url":self.url,
-            "headers":self.headers,
-            "json":self.data
-        }
-    
+        return {"url": self.url, "headers": self.headers, "json": self.data}
 
-    def handle_request(self,value,**kwargs):
+    def handle_request(self, value, **kwargs):
         handled_request_config = {
             **self.get_request_config(),
             **kwargs,
         }
         return handled_request_config
 
-    def handle_response(self,response):
+    def handle_response(self, response):
         return response
 
-    def run(self,value,**kwargs):
-        config = self.handle_request(value,**kwargs)
+    def run(self, value, **kwargs):
+        config = self.handle_request(value, **kwargs)
         result = requests.post(**config)
         handled_result = self.handle_response(result.json())
         return handled_result
-
-
```

### Comparing `libro_ai-0.1.0/src/libro_ai/chat/item.py` & `libro_ai-0.1.1/src/libro_ai/chat/object.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import ABC, abstractmethod
 from pydantic import BaseModel
 from typing import Callable
 
 from .source import CHAT_SOURCE
 from .executor import ChatExecutor
 
-class ChatItem(BaseModel):
+class ChatObject(BaseModel):
     name: str = None
     type: str = CHAT_SOURCE["CUSTOM"]
     order: int = 0
     to_executor: Callable[[], ChatExecutor] = None
 
     @property
     def key(self):
@@ -19,13 +19,13 @@
     def model_dump(self):
         '''Dump to dict'''
         return {
             **super().model_dump(exclude="to_executor"),
             "key":self.key
         }
 
-class ChatItemProvider(BaseModel, ABC):
+class ChatObjectProvider(BaseModel, ABC):
     name: str = "custom"
 
     @abstractmethod
-    def list(self) -> List[ChatItem]:
+    def list(self) -> List[ChatObject]:
         """List chat executors."""
```

### Comparing `libro_ai-0.1.0/src/libro_ai/chat/openai.py` & `libro_ai-0.1.1/src/libro_ai/chat/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,78 @@
-from typing import Any, Dict, List, Optional
-from pydantic import Field
-from IPython.display import display
+from typing import Dict, List
 
 from .source import CHAT_SOURCE
 
-from .executor import LLMChat,ChatExecutor
-from .item import ChatItem, ChatItemProvider
+from .executor import ChatExecutor
+from .object import ChatObject, ChatObjectProvider
 from ..utils import is_langchain_installed
 
 MODEL_NAME_ALIASES = {
     "text-davinci-003": "gpt3",
-    "gpt-3.5-turbo":"chatgpt",
+    "gpt-3.5-turbo": "chatgpt",
     "gpt-4": "gpt4",
     "dall-e-3": "dalle-3",
     "dall-e-2": "dalle-2",
-
 }
 
 ALIASE_NAME_MODEL = {
-    "gpt3":"text-davinci-003",
+    "gpt3": "text-davinci-003",
     "chatgpt": "gpt-3.5-turbo",
     "gpt4": "gpt-4",
     "dalle-3": "dall-e-3",
     "dalle-2": "dall-e-2",
 }
 
-class OpenAIChatItemProvider(ChatItemProvider):
+
+class OpenAIChatObjectProvider(ChatObjectProvider):
     name: str = "openai"
     cache: Dict[str, ChatExecutor] = {}
-    models: List[str] = ["gpt-3.5-turbo","gpt-4"]
+    LLMs: List[str] = ["gpt-3.5-turbo", "gpt-4"]
+    LMMs: List[str] = ["dall-e-3"]
 
     def get_or_create_executor(self, name: str) -> ChatExecutor:
         model = ALIASE_NAME_MODEL.get(name, name)
         if model in self.cache:
             return self.cache[model]
         from .openai_chat_executor import OpenAIChat
+
         executor = OpenAIChat(model=model, name=name)
         if executor.load():
             self.cache[model] = executor
         return executor
 
-    def list(self) -> List[ChatItem]:
-        if not is_langchain_installed():
-            return []
-        return map(lambda n: ChatItem(name=MODEL_NAME_ALIASES.get(n, n), to_executor=lambda:self.get_or_create_executor(n), type=CHAT_SOURCE["LLM"]), self.models)
-
-class DALLEChatItemProvider(ChatItemProvider):
-    name: str = "dalle"
-    cache: Dict[str, ChatExecutor] = {}
-    models: List[str] = ["dall-e-3","dall-e-2"]
-
-    def get_or_create_executor(self, name: str) -> ChatExecutor:
+    def get_or_create_lmm_executor(self, name: str) -> ChatExecutor:
         model = ALIASE_NAME_MODEL.get(name, name)
         if model in self.cache:
             return self.cache[model]
         from .openai_chat_executor import DalleChat
+
         executor = DalleChat(model=model, name=name)
         if executor.load():
             self.cache[model] = executor
         return executor
 
-    def list(self) -> List[ChatItem]:
+    def list(self) -> List[ChatObject]:
         if not is_langchain_installed():
             return []
-        return map(lambda n: ChatItem(name=MODEL_NAME_ALIASES.get(n, n), to_executor=lambda:self.get_or_create_executor(n), type=CHAT_SOURCE["LLM"]), self.models)
+        return [
+            *list(
+                map(
+                    lambda n: ChatObject(
+                        name=MODEL_NAME_ALIASES.get(n, n),
+                        to_executor=lambda: self.get_or_create_executor(n),
+                        type=CHAT_SOURCE["LLM"],
+                    ),
+                    self.LLMs,
+                )
+            ),
+            *list(
+                map(
+                    lambda n: ChatObject(
+                        name=MODEL_NAME_ALIASES.get(n, n),
+                        to_executor=lambda: self.get_or_create_lmm_executor(n),
+                        type=CHAT_SOURCE["LMM"],
+                    ),
+                    self.LMMs,
+                )
+            ),
+        ]
```

### Comparing `libro_ai-0.1.0/src/libro_ai/chat/openai_chat_executor.py` & `libro_ai-0.1.1/src/libro_ai/chat/openai_chat_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,77 @@
-from typing import Any, Dict, List, Optional
-from numpy import isin
 from pydantic import Field
 
-from .source import CHAT_SOURCE
-
 from .executor import LLMChat
 from ..utils import is_langchain_installed
 from langchain_openai import ChatOpenAI
 from langchain_core.messages import AIMessage
 from langchain.callbacks import get_openai_callback
 from langchain_community.utilities.dalle_image_generator import DallEAPIWrapper
 from IPython.display import display
-from IPython.display import HTML
+
 
 class OpenAIChat(LLMChat):
     name: str = "chatgpt"
     model: str = Field(default="gpt-3.5-turbo")
     chat: ChatOpenAI = None
 
     def load(self):
         if is_langchain_installed():
             self.chat = ChatOpenAI(model_name=self.model)
             return True
         return False
-    def run(self,value,**kwargs):
+
+    def run(self, value, **kwargs):
         if not self.chat:
             self.load()
         try:
             if not self.chat:
                 raise Exception("Chat model not loaded")
             chat = self.chat
             with get_openai_callback() as cb:
-                result = chat.invoke(value,**kwargs)
+                result = chat.invoke(value, **kwargs)
                 # print(f"Total Tokens: {cb.total_tokens}")
                 # print(f"Prompt Tokens: {cb.prompt_tokens}")
                 # print(f"Completion Tokens: {cb.completion_tokens}")
                 return result
             # result = chat.invoke(value,**kwargs)
             # return result
         except Exception as e:
             return ""
-    def display(self,value,**kwargs):
+
+    def display(self, value, **kwargs):
         if isinstance(value, str):
-            data = {
-                "application/vnd.libro.prompt+json": value
-            }
+            data = {"application/vnd.libro.prompt+json": value}
             display(data, raw=True)
         if isinstance(value, AIMessage):
-            data = {
-                "application/vnd.libro.prompt+json": value.content
-            }
+            data = {"application/vnd.libro.prompt+json": value.content}
             display(data, raw=True)
-        return self.run(value,**kwargs)
+
 
 class DalleChat(LLMChat):
     name: str = "dalle-3"
     model: str = Field(default="dall-e-3")
     dalle: DallEAPIWrapper = None
+
     def load(self):
         if is_langchain_installed():
             self.dalle = DallEAPIWrapper()
             self.dalle.model_name = self.model
             return True
         return False
-    def run(self,value,**kwargs):
+
+    def run(self, value, **kwargs):
         if not self.dalle:
             self.load()
         try:
             if not self.dalle:
                 raise Exception("Chat model not loaded")
             dalle = self.dalle
             result = dalle.run(value.text)
             return result
         except Exception as e:
             return ""
-    def display(self,value,**kwargs):
-        data = {
-            "text/html": f'<img src = {value}>'
-        }
+
+    def display(self, value, **kwargs):
+        data = {"text/html": f"<img src = {value}>"}
         display(data, raw=True)
         # HTML(f'<img src = {value}>',raw=True)
```

### Comparing `libro_ai-0.1.0/src/libro_ai/chat/provider.py` & `libro_ai-0.1.1/src/libro_ai/chat/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-from abc import ABC, abstractmethod
 import json
 from typing import List, Dict
 from pydantic import BaseModel
-from .item import ChatItem,ChatItemProvider
+from .object import ChatObject, ChatObjectProvider
 from .executor import ChatExecutor
 
 
-class ChatProvider(BaseModel):
-    providers: List[ChatItemProvider] = []
+class ChatObjectManager(BaseModel):
+    providers: List[ChatObject] = []
     executors: Dict[str, ChatExecutor] = {}
     
 
-    def register_provider(self, provider:ChatItemProvider):
+    def register_provider(self, provider:ChatObjectProvider):
         if provider.name in self.providers:
             print(f"Provider {provider.name} already exists")
             return
-        if isinstance(provider, ChatItemProvider) == False:
-            raise TypeError('provider must be ChatItemProvider')
+        if isinstance(provider, ChatObjectProvider) == False:
+            raise TypeError('provider must be ChatObjectProvider')
         if provider.name in map(lambda x: x.name, self.providers):
             print(f"Provider {provider.name} already exists")
             return
         self.providers.append(provider)
     
-    def get_provider_dict(self) -> Dict[str, ChatItem]:
-        chat_items: Dict[str, ChatItem] = {}
+    def get_object_dict(self) -> Dict[str, ChatObject]:
+        chat_objects: Dict[str, ChatObject] = {}
         for provider in self.providers:
             for item in provider.list():
                 key = item.key
-                exists = chat_items.get(key)
+                exists = chat_objects.get(key)
                 if exists:
                     if exists.order > item.order:
                         continue
-                chat_items[key] = item
-        return chat_items
+                chat_objects[key] = item
+        return chat_objects
 
-    def get_provider_list(self) -> List[ChatItem]:
+    def get_object_list(self) -> List[ChatObject]:
         """List chat items."""
-        list = sorted(self.get_provider_dict().values(), key=lambda x: x.order)
+        list = sorted(self.get_object_dict().values(), key=lambda x: x.order)
         return list
     
     def dump_list_json(self) -> str:
         """List chat items."""
-        list = self.get_provider_list()
+        list = self.get_object_list()
         return json.dumps([item.model_dump() for item in list])
```

### Comparing `libro_ai-0.1.0/src/libro_ai/flow/libro_client.py` & `libro_ai-0.1.1/src/libro_ai/flow/libro_client.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.0/src/libro_ai/flow/nb_args.py` & `libro_ai-0.1.1/src/libro_ai/flow/nb_args.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.0/src/libro_ai/magics/exception.py` & `libro_ai-0.1.1/src/libro_ai/magics/exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import traceback
+from IPython.core.interactiveshell import InteractiveShell
 
-from IPython.core.getipython import get_ipython
-from IPython.core.magic import register_line_magic
-from IPython.core.ultratb import ListTB
 
-
-def store_exception(shell, etype, evalue, tb, tb_offset=None):
+def store_exception(shell: InteractiveShell, etype: type, evalue, tb, tb_offset=None):
     # A structured traceback (a list of strings) or None
 
     if issubclass(etype, SyntaxError):
         # Disable ANSI color strings
         shell.SyntaxTB.color_toggle()
         # Don't display a stacktrace because a syntax error has no stacktrace
         stb = shell.SyntaxTB.structured_traceback(etype, evalue, [])
```

### Comparing `libro_ai-0.1.0/src/libro_ai/magics/prompt_magic.py` & `libro_ai-0.1.1/src/libro_ai/magics/prompt_magic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,133 @@
 # -*- coding: utf-8 -*-
 
-from ast import arg
 from IPython.core.magic import Magics, magics_class, line_cell_magic
 
-from notebook.base.handlers import log
-from ..chat import chat_provider
+from ..chat import chat_object_manager, chat_record_provider
 from langchain.prompts import PromptTemplate
-
-logger = log()
+from langchain_core.messages import BaseMessage, AIMessage
 
 
 def preprocessing_line_prompt(line, local_ns):
     import base64
+
     try:
         user_input = str(base64.decodebytes(line.encode()), "utf-8")
         import json
+
         # 将JSON字符串解析成Python对象
         json_obj = json.loads(user_input)
         prompt = json_obj.get("prompt")
         # 替换prompt content变量
-        if(prompt):
+        if prompt:
             for key, value in local_ns.items():
-                if not key.startswith("_"):
+                if key and not key.startswith("_"):
                     prompt = prompt.replace("{{" + key + "}}", str(value))
             json_obj["prompt"] = prompt
         return json_obj
     except Exception as e:
         raise Exception("preprocess_prompt error", e)
-    
+
+
 def preprocessing_cell_prompt(cell, local_ns):
     import base64
+
     try:
         import json
+
         # 将JSON字符串解析成Python对象
         json_obj = json.loads(cell)
         prompt = json_obj.get("prompt")
         # 替换prompt content变量
-        if(prompt):
+        if prompt:
             for key, value in local_ns.items():
-                if not key.startswith("_"):
+                if key and not key.startswith("_"):
                     prompt = prompt.replace("{{" + key + "}}", str(value))
             json_obj["prompt"] = prompt
         return json_obj
     except Exception as e:
         raise Exception("preprocess_prompt error", e)
 
+
 class MimeTypeForPrompt(object):
     def __init__(self, smiles=None, val: object = None):
         self.smiles = smiles
         self.data = val
 
     def _repr_mimebundle_(self, include=None, exclude=None):
         return {
             "application/vnd.libro.prompt+json": self.data,
         }
 
+
 @magics_class
 class PromptMagic(Magics):
     """
-    %%prompt 
+    %%prompt
     {"chat_key":"MyGPT","prompt":"do something"}
     """
 
-    LLM_generate_res = ''
+    LLM_generate_res = ""
 
     def __init__(self, shell=None):
         super(PromptMagic, self).__init__(shell)
-    
+
     @line_cell_magic
     def prompt(self, line="", cell=None):
-        local_ns = self.shell.user_ns
+        local_ns = self.shell.user_ns  # type: ignore
         if cell is None:
-            (
-                args
-            ) = preprocessing_line_prompt(line, local_ns)
+            (args) = preprocessing_line_prompt(line, local_ns)
         else:
-            (
-                args
-            ) = preprocessing_cell_prompt(cell, local_ns)
-
+            (args) = preprocessing_cell_prompt(cell, local_ns)
 
-        chat_key:str = args["model_name"]
-        prompt:str = args["prompt"]
-        dict = chat_provider.get_provider_dict()
+        chat_key: str = args.get("chat_key")
+        if chat_key is None or chat_key == "":
+            chat_key = args.get("model_name")
+        prompt: str = args.get("prompt")
+        cell_id: str = args.get("cell_id")
+
+        if (
+            (chat_key is None or chat_key == "")
+            or (prompt is None or prompt == "")
+            or (cell_id is None or cell_id == "")
+        ):
+            raise Exception("Invalid prompt parameters!")
+
+        record_id: str = args.get("record")
+        variable_name: str = args.get("variable_name")
+        dict = chat_object_manager.get_object_dict()
         if chat_key in dict:
-            exist = dict.get(chat_key)
-            if exist:
-                executor = exist.to_executor()
+            object = dict.get(chat_key)
+            if object:
+                executor = object.to_executor()
                 # Use langchain prompt to support prompt templates and other features
                 template = PromptTemplate.from_template(prompt)
                 formattedPrompt = template.invoke(local_ns)
-                res = executor.run(formattedPrompt)
-                display_res = executor.display(res)
+
+                res = None
+                if cell_id and record_id:
+                    record = chat_record_provider.get_record(record_id)
+                    record.append_messages(
+                        cell_id, formattedPrompt.to_messages(), reset=True
+                    )
+                    res = executor.run(record.get_messages())
+                    if res and isinstance(res, BaseMessage):
+                        record.append_message(cell_id, res)
+                    if res and isinstance(res, str):
+                        record.append_message(cell_id, AIMessage(content=res))
+                else:
+                    res = executor.run(formattedPrompt)
+                executor.display(res)
                 # Set variable
                 try:
-                    if "variable_name" in args:
-                        variable_name:str = args["variable_name"]
-                        if variable_name and variable_name != "" and not variable_name.isidentifier():
-                            raise Exception('Invalid variable name "{}".'.format(variable_name))
+                    if variable_name is None or variable_name == "":
+                        return
+                    if not variable_name.isidentifier():
+                        raise Exception(
+                            'Invalid variable name "{}".'.format(variable_name)
+                        )
+                    else:
                         local_ns[variable_name] = res
                 except Exception as e:
                     raise Exception("set variable error", e)
         else:
             raise Exception("Chat executor for %s not found!" % chat_key)
```

### Comparing `libro_ai-0.1.0/src/libro_ai/utils/base.py` & `libro_ai-0.1.1/src/libro_ai/utils/base.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.0/src/libro_ai/utils/inspector.py` & `libro_ai-0.1.1/src/libro_ai/utils/inspector.py`

 * *Files identical despite different names*

