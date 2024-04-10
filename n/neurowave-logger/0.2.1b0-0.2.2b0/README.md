# Comparing `tmp/neurowave_logger-0.2.1b0.tar.gz` & `tmp/neurowave_logger-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurowave_logger-0.2.1b0.tar", max compression
+gzip compressed data, was "neurowave_logger-0.2.2b0.tar", max compression
```

## Comparing `neurowave_logger-0.2.1b0.tar` & `neurowave_logger-0.2.2b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       62 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/README.md
--rw-r--r--   0        0        0        0 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/__init__.py
--rw-r--r--   0        0        0     7312 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/langchain_tracer.py
--rw-r--r--   0        0        0     4100 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/tracer.py
--rw-r--r--   0        0        0        0 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/utils/__init__.py
--rw-r--r--   0        0        0     4878 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/utils/openai_info.py
--rw-r--r--   0        0        0     1105 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/nwlogger/utils/text_print.py
--rw-r--r--   0        0        0      501 2024-03-11 05:17:32.586806 neurowave_logger-0.2.1b0/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.1b0/PKG-INFO
+-rw-r--r--   0        0        0       62 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/__init__.py
+-rw-r--r--   0        0        0     7126 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/langchain_tracer.py
+-rw-r--r--   0        0        0     4150 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/tracer.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/__init__.py
+-rw-r--r--   0        0        0     4878 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/openai_info.py
+-rw-r--r--   0        0        0     1105 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/text_print.py
+-rw-r--r--   0        0        0      501 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.2b0/PKG-INFO
```

### Comparing `neurowave_logger-0.2.1b0/nwlogger/langchain_tracer.py` & `neurowave_logger-0.2.2b0/nwlogger/langchain_tracer.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,46 +106,43 @@
     def on_llm_start(
             self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
         ) -> None:
             """Print out the prompts."""
 
             # LLM start
             self.llm_start_time  = perf_counter()
-            self.get_prompts_messages(prompts[0].split("\n"))
-            # self.conversation["messages"] += messages
-
-    def get_prompts_messages(self, prompt_list: List[str]):
-        messages = []
-        for index, prompt_msg in enumerate(prompt_list):
-            if prompt_msg.startswith("System:"):
-                role = "system"
-                msg = prompt_msg.replace("System:", "").strip()
-            elif prompt_msg.startswith("AI:"):
-                role = "assistant"
-                msg = prompt_msg.replace("AI:", "").strip()
-            elif prompt_msg.startswith("Human:"):
-                role = "user"
-                msg = prompt_msg.replace("Human:", "").strip()
-            item = {
-                "content": msg,
-                "role": role,
-                "index": len(self.conversation["messages"]),
-            }
-            self.conversation["messages"].append(item)
-
-        # return messages
 
+            if len(self.conversation["messages"]) > 0 and self.conversation["messages"][-1].get("role") == "user":
+                self.conversation["messages"][-1]["prompts"] = prompts[0]
+            else:
+                pass
+
+    def log_question(self, question: str) -> None:
+        item = {
+            "content": question,
+            "role": "user",
+            "index": len(self.conversation["messages"]),
+        }
+        self.conversation["messages"].append(item)
+
+    def log_context(self, context: str) -> None:
+
+        if len(self.conversation["messages"]) > 0 and self.conversation["messages"][-1].get("role") == "assistant":
+            self.conversation["messages"][-1]["context"] = context
+        else:
+            pass
 
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> None:
         """Collect token usage."""
 
         if response.llm_output is None:
             return None
         if "token_usage" not in response.llm_output:
             return None
+
         token_usage = response.llm_output["token_usage"]
         completion_tokens = token_usage.get("completion_tokens", 0)
         prompt_tokens = token_usage.get("prompt_tokens", 0)
         llm_token_llm_token_usage = token_usage.get("total_tokens", 0)
 
         model_name = standardize_model_name(response.llm_output.get("model_name", ""))
         if model_name in MODEL_COST_PER_1K_TOKENS:
```

### Comparing `neurowave_logger-0.2.1b0/nwlogger/tracer.py` & `neurowave_logger-0.2.2b0/nwlogger/tracer.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,51 +26,50 @@
 
     # check if index in messages
     if "index" not in messages[-1]:
         for index, message in enumerate(messages):
             message["index"] = len(all_meta_data["conversation"]["messages"]) + index
     return messages
 
-def trace_llm(messages: List, response: List, latency: float) -> Dict:
+def trace_llm(messages: List, response: List, latency: float, context: str = None) -> Dict:
     '''get infor for each llm call'''
     print ("log the llm call infomation")
 
     messages = valid_message(messages)
-
     model_name = standardize_model_name(response.model)
 
     # ==== we get answers and usage information
     answer = response.choices[0].message.content
 
     completion_tokens = response.usage.completion_tokens
     prompt_tokens = response.usage.prompt_tokens
     total_tokens = response.usage.total_tokens
 
-    # import pdb; pdb.set_trace()
     if model_name in MODEL_COST_PER_1K_TOKENS:
         completion_cost = get_openai_token_cost_for_model(
             model_name, completion_tokens, is_completion=True
         )
         prompt_cost = get_openai_token_cost_for_model(model_name, prompt_tokens)
         llm_cost = prompt_cost + completion_cost
     else:
         llm_cost = 0
 
-    messages.append(
-        {
-            "index": messages[-1]["index"] + 1,
-            "role": "assistant",
-            "content": answer,
-            "llm_cost": round(llm_cost, 4),
-            "llm_latency": latency,
-            "llm_token_usage": total_tokens,
-            "model_name": model_name
-        }
-    )
-
+    item = {
+        "index": messages[-1]["index"] + 1,
+        "role": "assistant",
+        "content": answer,
+        "llm_cost": round(llm_cost, 4),
+        "llm_latency": latency,
+        "llm_token_usage": total_tokens,
+        "model_name": model_name
+    }
+
+    if context:
+        item["context"] = context
+    messages.append(item)
     return messages
 
 def trace_chain(session_id: str, meta_data: Dict):
     '''put all infor from each llm call together'''
     print ("log the chain infomation")
     all_meta_data["session_id"] = session_id
     all_meta_data.update(meta_data)
@@ -94,14 +93,15 @@
     all_meta_data["turn_latency"] = turn_latency
     all_meta_data["turn_cost"] = turn_cost
     all_meta_data["turn_token_usage"] = turn_token_usage
     # submit_to_server(all_meta_data)
     return all_meta_data
 
 def traceable(run_type: str,
+              context: str = None,
               session_id: Optional[str] = None,
               *,
               meta_data: Optional[Dict] = {},
               messages: Optional[List] = None,
              ):
     '''trace a OpenAI LLM call'''
 
@@ -112,15 +112,15 @@
             **kwargs: Any,
         ) -> Any:
             start_time  = perf_counter()
             result = func(*args, **kwargs)
             end_call_time = perf_counter()
             latency = end_call_time - start_time
             if run_type == "llm":
-                updated_messages = trace_llm(messages, result, latency)
+                updated_messages = trace_llm(messages, result, latency, context)
                 all_meta_data["conversation"]["messages"] += updated_messages
                 return result.choices[0].message.content
 
             if run_type == "chain":
                 data = trace_chain(session_id, meta_data)
             return data
         return wrapper
```

### Comparing `neurowave_logger-0.2.1b0/nwlogger/utils/openai_info.py` & `neurowave_logger-0.2.2b0/nwlogger/utils/openai_info.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.1b0/nwlogger/utils/text_print.py` & `neurowave_logger-0.2.2b0/nwlogger/utils/text_print.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.1b0/PKG-INFO` & `neurowave_logger-0.2.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurowave-logger
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: Log agent for Neurowave
 License: MIT
 Author: Neurowave AI
 Author-email: it@neurowave.ai
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

