# Comparing `tmp/promptdown-0.2.0.tar.gz` & `tmp/promptdown-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptdown-0.2.0.tar", last modified: Wed Apr 10 03:46:14 2024, max compression
+gzip compressed data, was "promptdown-0.2.1.tar", last modified: Wed Apr 10 04:31:01 2024, max compression
```

## Comparing `promptdown-0.2.0.tar` & `promptdown-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-10 03:46:03.055501 promptdown-0.2.0/LICENSE
--rw-r--r--   0        0        0     2145 2024-04-10 03:46:03.055501 promptdown-0.2.0/README.md
--rw-r--r--   0        0        0      606 2024-04-10 03:46:14.887629 promptdown-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-10 03:46:03.055501 promptdown-0.2.0/src/promptdown/__init__.py
--rw-r--r--   0        0        0      124 2024-04-10 03:46:13.603615 promptdown-0.2.0/src/promptdown/__init__.pyi
--rw-r--r--   0        0        0     6050 2024-04-10 03:46:03.055501 promptdown-0.2.0/src/promptdown/promptdown.py
--rw-r--r--   0        0        0      691 2024-04-10 03:46:13.603615 promptdown-0.2.0/src/promptdown/promptdown.pyi
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 promptdown-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 04:30:47.433758 promptdown-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2145 2024-04-10 04:30:47.433758 promptdown-0.2.1/README.md
+-rw-r--r--   0        0        0      606 2024-04-10 04:31:01.873674 promptdown-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-10 04:30:47.433758 promptdown-0.2.1/src/promptdown/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-10 04:31:00.377682 promptdown-0.2.1/src/promptdown/__init__.pyi
+-rw-r--r--   0        0        0     6149 2024-04-10 04:30:47.433758 promptdown-0.2.1/src/promptdown/promptdown.py
+-rw-r--r--   0        0        0      755 2024-04-10 04:31:00.377682 promptdown-0.2.1/src/promptdown/promptdown.pyi
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 promptdown-0.2.1/PKG-INFO
```

### Comparing `promptdown-0.2.0/LICENSE` & `promptdown-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptdown-0.2.0/README.md` & `promptdown-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `promptdown-0.2.0/pyproject.toml` & `promptdown-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptdown"
-version = "0.2.0"
+version = "0.2.1"
 description = "A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts"
 authors = [
     { name = "B.T. Franklin", email = "brandon.franklin@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `promptdown-0.2.0/src/promptdown/promptdown.py` & `promptdown-0.2.1/src/promptdown/promptdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from __future__ import annotations
 import logging
 from dataclasses import dataclass
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = None
 
-    def __eq__(self, other: object):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, Message):
             return (
                 self.role.lower() == other.role.lower()
                 and self.content == other.content
                 and self.name == other.name
             )
         return False
@@ -22,15 +23,15 @@
 
 @dataclass
 class StructuredPrompt:
     name: str
     system_message: str
     conversation: list[Message]
 
-    def __eq__(self, other: object):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, StructuredPrompt):
             return (
                 self.name == other.name
                 and self.system_message == other.system_message
                 and self.conversation == other.conversation
             )
         return False
@@ -73,15 +74,15 @@
                         )
                     )
 
         # Return the parsed conversation list
         return conversation
 
     @classmethod
-    def from_promptdown_string(cls, promptdown_string: str):
+    def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt:
         name: str | None = None
         system_message: str | None = None
         conversation: list[Message] = []
         current_section: str | None = None
         conversation_lines: list[str] = []
 
         lines = promptdown_string.split("\n")
@@ -107,15 +108,15 @@
             )
 
         conversation = cls._parse_conversation(conversation_lines)
 
         return cls(name=name, system_message=system_message, conversation=conversation)
 
     @classmethod
-    def from_promptdown_file(cls, file_path: str):
+    def from_promptdown_file(cls, file_path: str) -> StructuredPrompt:
         promptdown_string = ""
 
         # Check if the file path ends with ".prompt.md"
         if not file_path.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
         # Load the file from the path
@@ -159,15 +160,15 @@
                 name = message.name if message.name is not None else ""
                 lines.append(f"| {role} | {name} | {content} |")
             else:
                 lines.append(f"| {role} | {content} |")
 
         return "\n".join(lines)
 
-    def to_promptdown_file(self, file_path: str):
+    def to_promptdown_file(self, file_path: str) -> None:
 
         # Check if the file path ends with ".prompt.md"
         if not file_path.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
         with open(file_path, "w") as file:
             file.write(self.to_promptdown_string())
```

### Comparing `promptdown-0.2.0/src/promptdown/promptdown.pyi` & `promptdown-0.2.1/src/promptdown/promptdown.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import dataclass
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = ...
-    def __eq__(self, other: object): ...
+    def __eq__(self, other: object) -> bool: ...
     def __init__(self, role, content, name) -> None: ...
 
 @dataclass
 class StructuredPrompt:
     name: str
     system_message: str
     conversation: list[Message]
-    def __eq__(self, other: object): ...
+    def __eq__(self, other: object) -> bool: ...
     @classmethod
-    def from_promptdown_string(cls, promptdown_string: str): ...
+    def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt: ...
     @classmethod
-    def from_promptdown_file(cls, file_path: str): ...
+    def from_promptdown_file(cls, file_path: str) -> StructuredPrompt: ...
     def to_promptdown_string(self) -> str: ...
-    def to_promptdown_file(self, file_path: str): ...
+    def to_promptdown_file(self, file_path: str) -> None: ...
     def __init__(self, name, system_message, conversation) -> None: ...
```

### Comparing `promptdown-0.2.0/PKG-INFO` & `promptdown-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptdown
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts
 Author-Email: B.T. Franklin <brandon.franklin@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Promptdown
```

