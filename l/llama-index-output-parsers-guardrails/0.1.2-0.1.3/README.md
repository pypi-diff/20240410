# Comparing `tmp/llama_index_output_parsers_guardrails-0.1.2.tar.gz` & `tmp/llama_index_output_parsers_guardrails-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_output_parsers_guardrails-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_output_parsers_guardrails-0.1.3.tar", max compression
```

## Comparing `llama_index_output_parsers_guardrails-0.1.2.tar` & `llama_index_output_parsers_guardrails-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2024-02-13 13:53:01.706109 llama_index_output_parsers_guardrails-0.1.2/README.md
--rw-r--r--   0        0        0      116 2024-02-13 13:53:01.706351 llama_index_output_parsers_guardrails-0.1.2/llama_index/output_parsers/guardrails/__init__.py
--rw-r--r--   0        0        0     2848 2024-02-13 13:53:01.706420 llama_index_output_parsers_guardrails-0.1.2/llama_index/output_parsers/guardrails/base.py
--rw-r--r--   0        0        0     1504 2024-02-21 18:43:03.394440 llama_index_output_parsers_guardrails-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 llama_index_output_parsers_guardrails-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-04-10 02:55:36.384190 llama_index_output_parsers_guardrails-0.1.3/README.md
+-rw-r--r--   0        0        0      116 2024-04-10 02:55:36.384190 llama_index_output_parsers_guardrails-0.1.3/llama_index/output_parsers/guardrails/__init__.py
+-rw-r--r--   0        0        0     2187 2024-04-10 02:55:36.384190 llama_index_output_parsers_guardrails-0.1.3/llama_index/output_parsers/guardrails/base.py
+-rw-r--r--   0        0        0     1504 2024-04-10 02:55:36.384190 llama_index_output_parsers_guardrails-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_output_parsers_guardrails-0.1.3/PKG-INFO
```

### Comparing `llama_index_output_parsers_guardrails-0.1.2/llama_index/output_parsers/guardrails/base.py` & `llama_index_output_parsers_guardrails-0.1.3/llama_index/output_parsers/guardrails/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,60 @@
-"""Guardrails output parser.
+"""
+Guardrails output parser.
 
 See https://github.com/ShreyaR/guardrails.
 
 """
+
 from copy import deepcopy
-from typing import TYPE_CHECKING, Any, Callable, Optional
+from typing import Any, Optional
 
 from deprecated import deprecated
-from llama_index.core.output_parsers.base import ChainableOutputParser
-
 from guardrails import Guard
 
-if TYPE_CHECKING:
-    from llama_index.core.bridge.langchain import BaseLLM
-
-
-def get_callable(llm: Optional["BaseLLM"]) -> Optional[Callable]:
-    """Get callable."""
-    if llm is None:
-        return None
-
-    return llm.__call__
+from llama_index.core.output_parsers.base import ChainableOutputParser
 
 
 class GuardrailsOutputParser(ChainableOutputParser):
     """Guardrails output parser."""
 
     def __init__(
         self,
         guard: Guard,
-        llm: Optional["BaseLLM"] = None,
         format_key: Optional[str] = None,
     ):
         """Initialize a Guardrails output parser."""
         self.guard: Guard = guard
-        self.llm = llm
         self.format_key = format_key
 
     @classmethod
     @deprecated(version="0.8.46")
-    def from_rail(
-        cls, rail: str, llm: Optional["BaseLLM"] = None
-    ) -> "GuardrailsOutputParser":
+    def from_rail(cls, rail: str) -> "GuardrailsOutputParser":
         """From rail."""
         if Guard is None:
             raise ImportError(
                 "Guardrails is not installed. Run `pip install guardrails-ai`. "
             )
 
-        return cls(Guard.from_rail(rail), llm=llm)
+        return cls(Guard.from_rail(rail))
 
     @classmethod
     @deprecated(version="0.8.46")
-    def from_rail_string(
-        cls, rail_string: str, llm: Optional["BaseLLM"] = None
-    ) -> "GuardrailsOutputParser":
+    def from_rail_string(cls, rail_string: str) -> "GuardrailsOutputParser":
         """From rail string."""
         if Guard is None:
             raise ImportError(
                 "Guardrails is not installed. Run `pip install guardrails-ai`. "
             )
 
-        return cls(Guard.from_rail_string(rail_string), llm=llm)
+        return cls(Guard.from_rail_string(rail_string))
 
-    def parse(
-        self,
-        output: str,
-        llm: Optional["BaseLLM"] = None,
-        num_reasks: Optional[int] = 1,
-        *args: Any,
-        **kwargs: Any
-    ) -> Any:
+    def parse(self, output: str, *args: Any, **kwargs: Any) -> Any:
         """Parse, validate, and correct errors programmatically."""
-        llm = llm or self.llm
-        llm_fn = get_callable(llm)
-
-        return self.guard.parse(
-            output, llm_api=llm_fn, num_reasks=num_reasks, *args, **kwargs
-        )
+        return self.guard.parse(output, *args, **kwargs).validated_output
 
     def format(self, query: str) -> str:
         """Format a query with structured output formatting instructions."""
         output_schema_text = deepcopy(self.guard.rail.prompt)
 
         # Add format instructions here.
         format_instructions_tmpl = self.guard.raw_prompt.format_instructions
```

### Comparing `llama_index_output_parsers_guardrails-0.1.2/pyproject.toml` & `llama_index_output_parsers_guardrails-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index output_parsers guardrails integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-output-parsers-guardrails"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-guardrails-ai = "^0.3.2"
+guardrails-ai = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_output_parsers_guardrails-0.1.2/PKG-INFO` & `llama_index_output_parsers_guardrails-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-output-parsers-guardrails
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index output_parsers guardrails integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: guardrails-ai (>=0.3.2,<0.4.0)
+Requires-Dist: guardrails-ai (>=0.4.1,<0.5.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Output_Parsers Integration: Guardrails
```

