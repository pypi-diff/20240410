# Comparing `tmp/promptdown-0.1.0.tar.gz` & `tmp/promptdown-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptdown-0.1.0.tar", last modified: Mon Apr  8 21:02:31 2024, max compression
+gzip compressed data, was "promptdown-0.2.0.tar", last modified: Wed Apr 10 03:46:14 2024, max compression
```

## Comparing `promptdown-0.1.0.tar` & `promptdown-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-08 21:02:22.155122 promptdown-0.1.0/LICENSE
--rw-r--r--   0        0        0     2145 2024-04-08 21:02:22.155122 promptdown-0.1.0/README.md
--rw-r--r--   0        0        0      557 2024-04-08 21:02:31.507158 promptdown-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-08 21:02:22.155122 promptdown-0.1.0/src/promptdown/__init__.py
--rw-r--r--   0        0        0     5588 2024-04-08 21:02:22.155122 promptdown-0.1.0/src/promptdown/promptdown.py
--rw-r--r--   0        0        0        0 2024-04-08 21:02:22.155122 promptdown-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-08 21:02:22.155122 promptdown-0.1.0/tests/test_promptdown.py
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 promptdown-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 03:46:03.055501 promptdown-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2145 2024-04-10 03:46:03.055501 promptdown-0.2.0/README.md
+-rw-r--r--   0        0        0      606 2024-04-10 03:46:14.887629 promptdown-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-10 03:46:03.055501 promptdown-0.2.0/src/promptdown/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-10 03:46:13.603615 promptdown-0.2.0/src/promptdown/__init__.pyi
+-rw-r--r--   0        0        0     6050 2024-04-10 03:46:03.055501 promptdown-0.2.0/src/promptdown/promptdown.py
+-rw-r--r--   0        0        0      691 2024-04-10 03:46:13.603615 promptdown-0.2.0/src/promptdown/promptdown.pyi
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 promptdown-0.2.0/PKG-INFO
```

### Comparing `promptdown-0.1.0/LICENSE` & `promptdown-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptdown-0.1.0/README.md` & `promptdown-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `promptdown-0.1.0/pyproject.toml` & `promptdown-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptdown"
-version = "0.1.0"
+version = "0.2.0"
 description = "A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts"
 authors = [
     { name = "B.T. Franklin", email = "brandon.franklin@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
@@ -17,12 +17,17 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
+[tool.pdm.build]
+excludes = [
+    "tests/**",
+]
+
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.1.1",
     "flake8>=7.0.0",
 ]
```

### Comparing `promptdown-0.1.0/src/promptdown/promptdown.py` & `promptdown-0.2.0/src/promptdown/promptdown.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import logging
 from dataclasses import dataclass
 
+_LOGGER = logging.getLogger(__name__)
+
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = None
 
@@ -29,15 +32,15 @@
                 self.name == other.name
                 and self.system_message == other.system_message
                 and self.conversation == other.conversation
             )
         return False
 
     @classmethod
-    def parse_conversation(cls, lines: list[str]) -> list[Message]:
+    def _parse_conversation(cls, lines: list[str]) -> list[Message]:
         conversation: list[Message] = []
         headers: list[str] = []
 
         # Iterate over each line in the input lines
         for line in lines:
             # Check if the line starts with "|", indicating a conversation row
             if line.startswith("|"):
@@ -99,21 +102,27 @@
                 "No prompt name found in the promptdown string. A prompt name is required."
             )
         if system_message is None:
             raise ValueError(
                 "No system message found in the promptdown string. A system message is required."
             )
 
-        conversation = cls.parse_conversation(conversation_lines)
+        conversation = cls._parse_conversation(conversation_lines)
 
         return cls(name=name, system_message=system_message, conversation=conversation)
 
     @classmethod
     def from_promptdown_file(cls, file_path: str):
         promptdown_string = ""
+
+        # Check if the file path ends with ".prompt.md"
+        if not file_path.endswith(".prompt.md"):
+            _LOGGER.warning("Promptdown files should end with '.prompt.md'")
+
+        # Load the file from the path
         with open(file_path, "r") as file:
             promptdown_string = file.read()
 
         return cls.from_promptdown_string(promptdown_string)
 
     def to_promptdown_string(self) -> str:
         lines: list[str] = []
@@ -151,9 +160,14 @@
                 lines.append(f"| {role} | {name} | {content} |")
             else:
                 lines.append(f"| {role} | {content} |")
 
         return "\n".join(lines)
 
     def to_promptdown_file(self, file_path: str):
+
+        # Check if the file path ends with ".prompt.md"
+        if not file_path.endswith(".prompt.md"):
+            _LOGGER.warning("Promptdown files should end with '.prompt.md'")
+
         with open(file_path, "w") as file:
             file.write(self.to_promptdown_string())
```

### Comparing `promptdown-0.1.0/PKG-INFO` & `promptdown-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptdown
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts
 Author-Email: B.T. Franklin <brandon.franklin@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Promptdown
```

