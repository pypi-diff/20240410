# Comparing `tmp/llm_structured_output-0.0.1.tar.gz` & `tmp/llm_structured_output-0.0.2.tar.gz`

## Comparing `llm_structured_output-0.0.1.tar` & `llm_structured_output-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/_/_eval.sh
--rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/_/_server.sh
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/examples/llm_schema.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/examples/server.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21180 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/LICENSE
--rw-r--r--   0        0        0    12474 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/_/_eval.sh
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/_/_server.sh
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/_/x.py
+-rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/examples/llm_schema.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    21187 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/LICENSE
+-rw-r--r--   0        0        0    13427 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 llm_structured_output-0.0.2/PKG-INFO
```

### Comparing `llm_structured_output-0.0.1/_/_mistral_schema.sh` & `llm_structured_output-0.0.2/_/_mistral_schema.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 cd `dirname $0`/../src
 
 LLM=examples.llm_schema
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=./mistral/mlx_model_q4
-#MODEL=mistralai/Mistral-7B-Instruct-v0.2
-MODEL=mlx-community/Mistral-7B-v0.2-4bit
+MODEL=mistralai/Mistral-7B-Instruct-v0.2
+#MODEL=mlx-community/Mistral-7B-v0.2-4bit
 OPTIONS="--max-tokens 1000 --repeat-prompt --temp 0.8"
 
 PROMPT='[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}. Do not explain the result, just output it. Do not add any additional information. [/INST]'
 
 if [ "$1" == "--mixtral" ]; then
   shift
   MODEL=./mixtral/mlx_model_q4
   #MODEL=./mixtral/mlx_model_q8
   #MODEL=./mixtral/mlx_model_f16
   MODEL_TYPE="--model-type mixtral"
 fi
 if [ "$1" == "--encapsulated" ]; then
   shift
-  PROMPT='[INST] Your mission is to parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}.
+  PROMPT='<s>[INST] Your mission is to parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}.
 First, think through the mission, and then output a JSON object wrapped between the lines ```json and ```. [/INST]'
 fi
 
 if [ "$1" == "--no-schema" ]; then
   shift
   python3 -m $LLM --model-path $MODEL $MODEL_TYPE $OPTIONS --prompt "$PROMPT" $@
 else
```

### Comparing `llm_structured_output-0.0.1/src/examples/llm_schema.py` & `llm_structured_output-0.0.2/src/examples/llm_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 """
 Example of JSON schema decoding for Mixtral with MLX.
 """
 import argparse
 import json
 import time
 from operator import itemgetter
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
 from mlx_lm.utils import load
 
-from llm_structured_output import JsonSchemaAcceptorDriver, extract_vocabulary, bias_logits
-from llm_structured_output.util.bitmap import count_set_bits, enumerate_set_bits
+from llm_structured_output import JsonSchemaAcceptorDriver
+from llm_structured_output.util.bitmap import bias_logits, count_set_bits, enumerate_set_bits
 from llm_structured_output.util.output import info, bold, bolddim, debug
+from llm_structured_output.util.tokenization import HuggingfaceTokenizerHelper
 
 
 class RejectedCompletion(Exception):
     """
     It's rare, but sometimes we reach a state where it's not possible to
     advance the acceptor. For example, when closing a JSON string we get
     a higher probability for slanted quotes than straight ones and select
@@ -40,25 +41,20 @@
         self.vocabulary = None
         self.eos_id = None
 
     def load(self, model_path: str):
         """
         Load locally or download from Huggingface hub.
         """
-        self.model, self.tokenizer = load(model_path)
-        self.vocabulary, self.eos_id = extract_vocabulary(self.tokenizer)
+        self.model, tokenizer = load(model_path)
+        self.tokenizer = HuggingfaceTokenizerHelper(tokenizer)
+        self.vocabulary, self.eos_id = self.tokenizer.extract_vocabulary()
 
     def _decode(self, tokens):
-        """
-        Allows to decode without removing the initial space.
-        The Huggingface tokenizer doesn't seem to have an easy way to do this.
-        It's a bit scary that we may be leaving out some extra magic that the
-        tokenizer decoder may do in some particular LLM, so YMMV.
-        """
-        return "".join([ self.vocabulary[token] for token in tokens ])
+        return self.tokenizer.no_strip_decode(tokens)
 
     def sample(self, logits, temp):
         if temp == 0:
             result = mx.argmax(logits, axis=-1)
         else:
             result = mx.random.categorical(logits * (1 / temp))
         return result.item()
@@ -143,21 +139,25 @@
             logits, cache = self._run_model(mx.array(batch), cache)
             mx.eval(logits)
 
             first_token_logits = bias_logits(mx, logits[0, 0, :], accepted_token_bitmap)
             first_token = self.sample(first_token_logits, temp)
             tokens = [first_token]
 
+            if first_token == self.eos_id:
+                yield tokens
+                break
+
             token_acceptor.advance_token(self._decode([first_token]))
             accepted_token_bitmap = token_acceptor.select_valid_tokens()
             if not accepted_token_bitmap:
                 raise RejectedCompletion()
 
             # If we had submitted 2-token continuations, we can decode a second token
-            if len(batch[0]) > 1 and first_token != self.eos_id:
+            if len(batch[0]) > 1:
                 index = next(  # Find which of the second tokens was selected
                     i
                     for i, batch_item in enumerate(batch)
                     if batch_item[1] == first_token
                 )
                 second_token_logits = bias_logits(
                     mx, logits[index, 1, :], accepted_token_bitmap
@@ -219,14 +219,18 @@
             logits, cache = self._run_model(batch_array, cache)
             mx.eval(logits)
 
             first_token_logits = bias_logits(mx, logits[0, 0, :], accepted_token_bitmap)
             first_token = self.sample(first_token_logits, temp)
             tokens = [first_token]
 
+            if first_token == self.eos_id:
+                yield tokens
+                break
+
             token_acceptor.advance_token(self._decode([first_token]))
             accepted_token_bitmap = token_acceptor.select_valid_tokens()
             if not accepted_token_bitmap:
                 raise RejectedCompletion()
 
             # If we had submitted 2-token continuations, we can decode a second token
             if len(batch[0]) > 1:
@@ -282,31 +286,31 @@
             h, cache[e] = layer(h, mask, cache[e])
 
         out = model.norm(h)
         return self.model.lm_head(out), cache
 
     def completion(
         self,
-        prompt: str,
+        prompt: Union[str, Iterable[dict[str, str]]],
         schema: dict,
         encapsulated: bool = False,
         max_tokens: int = 1000,
         temp: float = 0.0,
         seed: int = None,
         preemptive_batch_size: int = 0,
     ):
         if seed is not None:
             mx.random.seed(seed)
 
-        prompt_tokens = self.tokenizer.encode(prompt)
+        prompt_tokens = self.tokenizer.encode_prompt(prompt)
 
         if schema:
             token_acceptor = JsonSchemaAcceptorDriver(
                 schema,
-                self.vocabulary.items(),
+                self.vocabulary,
                 self.eos_id,
                 is_encapsulated_json=encapsulated,
             )
             if preemptive_batch_size > 0:
                 generator = self.generate_with_preemptive_decoding(
                     prompt_tokens,
                     token_acceptor,
```

### Comparing `llm_structured_output-0.0.1/src/examples/server.py` & `llm_structured_output-0.0.2/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.2/src/llm_structured_output/acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.2/src/llm_structured_output/json_acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.2/src/llm_structured_output/json_schema_acceptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Acceptors for JSON schema validation or constraning LLM generation to JSON
 outputs complying with a JSON schema.
 """
 from __future__ import annotations
 
 import re
 from collections import defaultdict
-from typing import Iterable
+from typing import Iterable, Tuple
 
 from .acceptor import (
     TokenAcceptor,
     StateMachineAcceptor,
     SequenceAcceptor,
     TextAcceptor,
     WaitForAcceptor,
```

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.2/src/llm_structured_output/util/bitmap.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.2/src/llm_structured_output/util/output.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.2/src/llm_structured_output/util/tokentrie.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         self.ids: int = 0
 
     def insert_all(self, vocabulary: Iterable[Tuple[int, str]]):
         """
         Insert all the tokens in the vocabulary in the trie, with the id of
         each token being its index in the vocabulary.
         """
-        for i, token in vocabulary:
+        for _id, token in vocabulary:
             if len(token) > 0:
-                self.insert(token, i)
+                self.insert(token, _id)
 
     def insert(self, token, _id):
         """
         Insert one token in the trie, with the given id.
         """
         if len(token) == 0:
             self.ids |= 1 << _id
```

### Comparing `llm_structured_output-0.0.1/src/tests/eval.py` & `llm_structured_output-0.0.2/src/tests/eval.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,14 @@
 
 
 def run_eval_case(model, case, header):
     messages = case["prompt"]
     gold_completion = json.loads(case["completion"].partition("<functioncall>")[2])
     tools = json.loads(case["tools"])
 
-    prompt = "\n".join(
-        (
-            message.content
-            if message["role"] == "assistant"
-            else f"[INST] {message['content']} [/INST]"
-        )
-        for message in messages
-    )
-
     schema = {
         "anyOf": [
             {
                 "type": "object",
                 "properties": {
                     "function_call": {
                         "type": "object",
@@ -40,27 +31,28 @@
                                 "const": tool["function"]["name"],
                             },
                             "arguments": tool["function"]["parameters"],
                         },
                         "required": ["name", "arguments"],
                     }
                 },
+                "required": ["function_call"],
             }
             for tool in tools
         ]
     }
 
     info(f"{header} Starting generation...")
     content = ""
     prompt_tokens = 0
     completion_tokens = 0
     completion_time = 0
 
     for result in model.completion(
-        prompt,
+        messages,
         schema=schema,
         max_tokens=4000,
         temp=0,
     ):
         if result["op"] == "evaluatedPrompt":
             prompt_tokens += result["token_count"]
             prompt_time = result["time_ms"]
```

### Comparing `llm_structured_output-0.0.1/LICENSE` & `llm_structured_output-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.1/README.md` & `llm_structured_output-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -117,40 +117,65 @@
 
 ### Using the JSON schema acceptor in your project
 
 Install in your project with `pip install llm-structured-output` and
 use a `JsonSchemaAcceptorDriver` within your normal generation loop:
 
 ```python
-from llm_structured_output import JsonSchemaAcceptorDriver, extract_vocabulary, bias_logits
+import json
+import mlx.core as mx
+from mlx_lm.utils import load # Needs pip import mlx_lm
+from llm_structured_output import JsonSchemaAcceptorDriver, HuggingfaceTokenizerHelper, bias_logits
+
+
+MODEL_PATH = "mistralai/Mistral-7B-Instruct-v0.2"
+SCHEMA = {
+    "type": "object",
+    "properties": {
+        "streetNumber": {"type": "number"},
+        "streetName": {"type": "string"},
+        "city": {"type": "string"},
+        "state": {"type": "string"},
+        "zipCode": {"type": "number"},
+    },
+}
+PROMPT = f'''
+[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014".
+Your answer should be only a JSON object according to this schema: {json.dumps(SCHEMA)}
+Do not explain the result, just output it. Do not add any additional information. [/INST]
+'''
 
-# ...
 
 # Load the model as usual.
-model, tokenizer = load(model_path)
+model, tokenizer = load(MODEL_PATH)
 
 # Instantiate a token acceptor
-vocabulary, eos_id = extract_vocabulary(tokenizer)
-token_acceptor = JsonSchemaAcceptorDriver(schema, vocabulary, eos_id)
+tokenizer_helper = HuggingfaceTokenizerHelper(tokenizer)
+vocabulary, eos_id = tokenizer_helper.extract_vocabulary()
+token_acceptor = JsonSchemaAcceptorDriver(SCHEMA, vocabulary, eos_id)
 
 cache = None
-tokens = tokenizer.encode(prompt)
+tokens = tokenizer_helper.encode_prompt(PROMPT)
 
 while tokens[-1] != eos_id:
-
     # Evaluate the model as usual. 
     logits, cache = model(mx.array(tokens)[None], cache)
 
     # Set probability to -inf for invalid tokens.
     accepted_token_bitmap = token_acceptor.select_valid_tokens()
     logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
 
-    # Sample as usual.
-    tokens = [sample(logits, temp)]
-    text = tokenizer.decode(tokens)
+    # Sample as usual, e.g.:
+    tokens = [mx.argmax(logits, axis=-1).item()]
+
+    if tokens[0] == eos_id:
+      break
+
+    # Decode the tokens as you go to be able to advance the acceptor.
+    text = tokenizer_helper.no_strip_decode(tokens)
     print(text, end="")
 
     # Advance the acceptor to the next state.
     token_acceptor.advance_token(text)
 ```
 
 ## A note about guarantees on the output
@@ -215,15 +240,15 @@
 general it can also considerably slow it down, depending on model and
 quantization. We are investigating whether this is an effect of Apple hardware
 architecture, the MLX library, or our own implementation mistakes.
 
 ### Benchmarks
 
 - The following tests were perfomed on an Apple Studio with an M2 Ultra (24 core)
-with 192GB of RAM using MLX version 0.9.0.
+with 192GB of RAM using MLX version 0.9.0, with models converted to MLX format.
 
 - The results are the average of 5 runs on a simple data extraction task with a
 127-token prompt.
 
 - Pre-emptive decoding was tested in two different forms: with a constant batch
   size, where we always sent the same size matrices for evaluation, and variable-
   size batching, where we made the batch large or shorter depending on the numer
```

### Comparing `llm_structured_output-0.0.1/pyproject.toml` & `llm_structured_output-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.1/PKG-INFO` & `llm_structured_output-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.1
+Version: 0.0.2
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -131,40 +131,65 @@
 
 ### Using the JSON schema acceptor in your project
 
 Install in your project with `pip install llm-structured-output` and
 use a `JsonSchemaAcceptorDriver` within your normal generation loop:
 
 ```python
-from llm_structured_output import JsonSchemaAcceptorDriver, extract_vocabulary, bias_logits
+import json
+import mlx.core as mx
+from mlx_lm.utils import load # Needs pip import mlx_lm
+from llm_structured_output import JsonSchemaAcceptorDriver, HuggingfaceTokenizerHelper, bias_logits
+
+
+MODEL_PATH = "mistralai/Mistral-7B-Instruct-v0.2"
+SCHEMA = {
+    "type": "object",
+    "properties": {
+        "streetNumber": {"type": "number"},
+        "streetName": {"type": "string"},
+        "city": {"type": "string"},
+        "state": {"type": "string"},
+        "zipCode": {"type": "number"},
+    },
+}
+PROMPT = f'''
+[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014".
+Your answer should be only a JSON object according to this schema: {json.dumps(SCHEMA)}
+Do not explain the result, just output it. Do not add any additional information. [/INST]
+'''
 
-# ...
 
 # Load the model as usual.
-model, tokenizer = load(model_path)
+model, tokenizer = load(MODEL_PATH)
 
 # Instantiate a token acceptor
-vocabulary, eos_id = extract_vocabulary(tokenizer)
-token_acceptor = JsonSchemaAcceptorDriver(schema, vocabulary, eos_id)
+tokenizer_helper = HuggingfaceTokenizerHelper(tokenizer)
+vocabulary, eos_id = tokenizer_helper.extract_vocabulary()
+token_acceptor = JsonSchemaAcceptorDriver(SCHEMA, vocabulary, eos_id)
 
 cache = None
-tokens = tokenizer.encode(prompt)
+tokens = tokenizer_helper.encode_prompt(PROMPT)
 
 while tokens[-1] != eos_id:
-
     # Evaluate the model as usual. 
     logits, cache = model(mx.array(tokens)[None], cache)
 
     # Set probability to -inf for invalid tokens.
     accepted_token_bitmap = token_acceptor.select_valid_tokens()
     logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
 
-    # Sample as usual.
-    tokens = [sample(logits, temp)]
-    text = tokenizer.decode(tokens)
+    # Sample as usual, e.g.:
+    tokens = [mx.argmax(logits, axis=-1).item()]
+
+    if tokens[0] == eos_id:
+      break
+
+    # Decode the tokens as you go to be able to advance the acceptor.
+    text = tokenizer_helper.no_strip_decode(tokens)
     print(text, end="")
 
     # Advance the acceptor to the next state.
     token_acceptor.advance_token(text)
 ```
 
 ## A note about guarantees on the output
@@ -229,15 +254,15 @@
 general it can also considerably slow it down, depending on model and
 quantization. We are investigating whether this is an effect of Apple hardware
 architecture, the MLX library, or our own implementation mistakes.
 
 ### Benchmarks
 
 - The following tests were perfomed on an Apple Studio with an M2 Ultra (24 core)
-with 192GB of RAM using MLX version 0.9.0.
+with 192GB of RAM using MLX version 0.9.0, with models converted to MLX format.
 
 - The results are the average of 5 runs on a simple data extraction task with a
 127-token prompt.
 
 - Pre-emptive decoding was tested in two different forms: with a constant batch
   size, where we always sent the same size matrices for evaluation, and variable-
   size batching, where we made the batch large or shorter depending on the numer
```

