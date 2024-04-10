# Comparing `tmp/flexdown-0.1.5a7.tar.gz` & `tmp/flexdown-0.1.5a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexdown-0.1.5a7.tar", max compression
+gzip compressed data, was "flexdown-0.1.5a8.tar", max compression
```

## Comparing `flexdown-0.1.5a7.tar` & `flexdown-0.1.5a8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-09-29 06:06:18.701607 flexdown-0.1.5a7/README.md
--rw-r--r--   0        0        0     1789 2024-01-10 19:15:39.538550 flexdown-0.1.5a7/flexdown/__init__.py
--rw-r--r--   0        0        0      182 2024-01-10 19:57:07.542793 flexdown-0.1.5a7/flexdown/blocks/__init__.py
--rw-r--r--   0        0        0     4348 2024-01-10 19:15:22.621925 flexdown-0.1.5a7/flexdown/blocks/block.py
--rw-r--r--   0        0        0      977 2024-03-06 00:30:50.912988 flexdown-0.1.5a7/flexdown/blocks/code_block.py
--rw-r--r--   0        0        0      358 2024-01-10 01:22:58.245149 flexdown-0.1.5a7/flexdown/blocks/eval_block.py
--rw-r--r--   0        0        0      874 2024-01-23 23:25:11.905369 flexdown-0.1.5a7/flexdown/blocks/exec_block.py
--rw-r--r--   0        0        0      670 2024-01-09 22:38:44.491006 flexdown-0.1.5a7/flexdown/blocks/markdown_block.py
--rw-r--r--   0        0        0      768 2024-03-06 00:30:46.703475 flexdown-0.1.5a7/flexdown/cli.py
--rw-r--r--   0        0        0      665 2024-01-10 19:26:38.744435 flexdown-0.1.5a7/flexdown/constants.py
--rw-r--r--   0        0        0     1576 2023-10-09 00:40:28.366561 flexdown-0.1.5a7/flexdown/document.py
--rw-r--r--   0        0        0     7282 2024-03-06 00:30:46.704368 flexdown-0.1.5a7/flexdown/flexdown.py
--rw-r--r--   0        0        0      361 2023-10-05 22:32:42.955213 flexdown-0.1.5a7/flexdown/types.py
--rw-r--r--   0        0        0     1678 2024-01-24 00:01:29.105079 flexdown-0.1.5a7/flexdown/utils.py
--rw-r--r--   0        0        0      486 2024-03-06 00:31:40.297378 flexdown-0.1.5a7/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 flexdown-0.1.5a7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-09-29 06:06:18.701607 flexdown-0.1.5a8/README.md
+-rw-r--r--   0        0        0     1789 2024-01-10 19:15:39.538550 flexdown-0.1.5a8/flexdown/__init__.py
+-rw-r--r--   0        0        0      182 2024-01-10 19:57:07.542793 flexdown-0.1.5a8/flexdown/blocks/__init__.py
+-rw-r--r--   0        0        0     4348 2024-01-10 19:15:22.621925 flexdown-0.1.5a8/flexdown/blocks/block.py
+-rw-r--r--   0        0        0      977 2024-03-06 00:30:50.912988 flexdown-0.1.5a8/flexdown/blocks/code_block.py
+-rw-r--r--   0        0        0      358 2024-01-10 01:22:58.245149 flexdown-0.1.5a8/flexdown/blocks/eval_block.py
+-rw-r--r--   0        0        0      874 2024-01-23 23:25:11.905369 flexdown-0.1.5a8/flexdown/blocks/exec_block.py
+-rw-r--r--   0        0        0      397 2024-04-10 20:22:21.767870 flexdown-0.1.5a8/flexdown/blocks/markdown_block.py
+-rw-r--r--   0        0        0      768 2024-03-06 00:30:46.703475 flexdown-0.1.5a8/flexdown/cli.py
+-rw-r--r--   0        0        0      665 2024-01-10 19:26:38.744435 flexdown-0.1.5a8/flexdown/constants.py
+-rw-r--r--   0        0        0     1576 2023-10-09 00:40:28.366561 flexdown-0.1.5a8/flexdown/document.py
+-rw-r--r--   0        0        0     8248 2024-04-10 20:21:59.058713 flexdown-0.1.5a8/flexdown/flexdown.py
+-rw-r--r--   0        0        0      361 2023-10-05 22:32:42.955213 flexdown-0.1.5a8/flexdown/types.py
+-rw-r--r--   0        0        0     1678 2024-01-24 00:01:29.105079 flexdown-0.1.5a8/flexdown/utils.py
+-rw-r--r--   0        0        0      486 2024-04-10 21:18:26.154202 flexdown-0.1.5a8/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 flexdown-0.1.5a8/PKG-INFO
```

### Comparing `flexdown-0.1.5a7/flexdown/__init__.py` & `flexdown-0.1.5a8/flexdown/__init__.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/blocks/block.py` & `flexdown-0.1.5a8/flexdown/blocks/block.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/blocks/code_block.py` & `flexdown-0.1.5a8/flexdown/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/blocks/exec_block.py` & `flexdown-0.1.5a8/flexdown/blocks/exec_block.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/cli.py` & `flexdown-0.1.5a8/flexdown/cli.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/constants.py` & `flexdown-0.1.5a8/flexdown/constants.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/document.py` & `flexdown-0.1.5a8/flexdown/document.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/flexdown/flexdown.py` & `flexdown-0.1.5a8/flexdown/flexdown.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The main flexdown module."""
+
 import importlib
 import os
 import shutil
 import sys
 from typing import Callable, Iterator
 
 import reflex as rx
@@ -36,14 +37,37 @@
 
     # Mapping from markdown tag to a rendering function for Reflex components.
     component_map: types.ComponentMap = {}
 
     # The directory to save modules to.
     module_dir: str = "modules"
 
+    def get_default_block(self) -> Block:
+        """Get the default block type.
+
+        Returns:
+            The default block type.
+        """
+        block = self.default_block_type()
+        if isinstance(block, blocks.MarkdownBlock):
+            block.render_fn = self.flexdown_memo
+        return block
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        def flexdown_memo(content: str) -> rx.Component:
+            return rx.markdown(content, component_map=self.component_map)
+
+        # Give the function a unique name.
+        import random
+
+        flexdown_memo.__name__ = f"flexdown_memo_{random.randint(0, 100000)}"
+        self.flexdown_memo = rx.memo(flexdown_memo)
+
     def clear_modules(self):
         """Clear the modules directory."""
         # Get the path to the directory where the module should be saved.
         flexdown_dir = os.path.dirname(os.path.abspath(__file__))
         module_dir = os.path.join(flexdown_dir, self.module_dir)
 
         # Delete the directory.
@@ -67,21 +91,24 @@
             # Try to create a block from the line.
             block = block_type.from_line(
                 line,
                 line_number=line_number,
                 component_map=self.component_map,
                 filename=filename,
             )
+            if isinstance(block, blocks.MarkdownBlock):
+                block.render_fn = self.flexdown_memo
 
             # If a block was created, then return it.
             if block is not None:
                 return block
 
         # If no block was created, then return the default block type.
-        return self.default_block_type().append(line)
+        block = self.default_block_type().append(line)
+        return block
 
     def exec(self, content: str, env: types.Env = {}, filename: str | None = None):
         # Get the path to the directory where the module should be saved.
         flexdown_dir = os.path.dirname(os.path.abspath(__file__))
         module_dir = os.path.join(flexdown_dir, self.module_dir)
 
         # Write the content to a file in the module directory.
@@ -164,14 +191,16 @@
 
         # Get the content of the document.
         source = source.content
 
         # Render each block.
         out: list[rx.Component] = []
         for block in self.get_blocks(source, filename):
+            if isinstance(block, blocks.MarkdownBlock):
+                block.render_fn = self.flexdown_memo
             try:
                 out.append(block.render(env=env))
             except Exception as e:
                 print(
                     f"Error while rendering {type(block)} on line {block.start_line_number}. "
                     f"\n{block.get_content(env)}"
                 )
```

### Comparing `flexdown-0.1.5a7/flexdown/utils.py` & `flexdown-0.1.5a8/flexdown/utils.py`

 * *Files identical despite different names*

### Comparing `flexdown-0.1.5a7/PKG-INFO` & `flexdown-0.1.5a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexdown
-Version: 0.1.5a7
+Version: 0.1.5a8
 Summary: Write interactive documentation with Markdown and Python.
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

