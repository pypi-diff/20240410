# Comparing `tmp/markdown_pytest-0.3.0.tar.gz` & `tmp/markdown_pytest-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_pytest-0.3.0.tar", max compression
+gzip compressed data, was "markdown_pytest-0.3.1.tar", max compression
```

## Comparing `markdown_pytest-0.3.0.tar` & `markdown_pytest-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2022-12-26 14:39:22.443355 markdown_pytest-0.3.0/LICENSE
--rw-r--r--   0        0        0     5009 2023-02-01 09:13:10.820941 markdown_pytest-0.3.0/README.md
--rw-r--r--   0        0        0     5967 2023-02-01 09:13:10.822203 markdown_pytest-0.3.0/markdown_pytest.py
--rw-r--r--   0        0        0     1805 2023-02-01 09:13:10.823380 markdown_pytest-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 markdown_pytest-0.3.0/setup.py
--rw-r--r--   0        0        0     6964 1970-01-01 00:00:00.000000 markdown_pytest-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 22:23:16.117985 markdown_pytest-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5019 2024-04-09 22:23:16.118066 markdown_pytest-0.3.1/README.md
+-rw-r--r--   0        0        0     5967 2024-04-09 22:23:16.118140 markdown_pytest-0.3.1/markdown_pytest.py
+-rw-r--r--   0        0        0     1761 2024-04-09 22:27:16.514970 markdown_pytest-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 markdown_pytest-0.3.1/PKG-INFO
```

### Comparing `markdown_pytest-0.3.0/LICENSE` & `markdown_pytest-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_pytest-0.3.0/README.md` & `markdown_pytest-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -239,18 +239,20 @@
     exit(1)
 ```
 </details>
 
 Usage example
 -------------
 
-This README.md file might be tested like this:
+This README.md file can be tested like this:
 
 ```bash
 $ pytest -v README.md
+```
+```bash
 ======================= test session starts =======================
 plugins: subtests, markdown-pytest
 collected 3 items
 
 README.md::test_assert_true PASSED                           [ 33%]
 README.md::test_example PASSED                               [ 66%]
 README.md::test_counter SUBPASS                              [100%]
```

### Comparing `markdown_pytest-0.3.0/markdown_pytest.py` & `markdown_pytest-0.3.1/markdown_pytest.py`

 * *Files identical despite different names*

### Comparing `markdown_pytest-0.3.0/pyproject.toml` & `markdown_pytest-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markdown-pytest"
-version = "0.3.0"
+version = "0.3.1"
 license = "Apache-2.0"
 description = "Pytest plugin for runs tests directly from Markdown files"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 keywords=["pytest", "markdown", "documentation"]
 homepage = "https://github.com/mosquito/markdown-pytest"
 classifiers = [
@@ -17,31 +17,30 @@
     "Operating System :: MacOS",
     "Operating System :: Microsoft",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
 ]
 packages = [{include = "markdown_pytest.py"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pytest-subtests = "^0.9.0"
+python = "^3.8"
+pytest-subtests = ">=0.12.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
+pytest = ">=8.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins.pytest11]
 markdown-pytest = "markdown_pytest"
```

### Comparing `markdown_pytest-0.3.0/setup.py` & `markdown_pytest-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,299 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: markdown-pytest
+Version: 0.3.1
+Summary: Pytest plugin for runs tests directly from Markdown files
+Home-page: https://github.com/mosquito/markdown-pytest
+License: Apache-2.0
+Keywords: pytest,markdown,documentation
+Author: Dmitry Orlov
+Author-email: me@mosquito.su
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: pytest-subtests (>=0.12.0)
+Project-URL: Documentation, https://github.com/mosquito/markdown-pytest/blob/master/README.rst
+Project-URL: Source, https://github.com/mosquito/markdown-pytest
+Project-URL: Tracker, https://github.com/mosquito/markdown-pytest/issues
+Description-Content-Type: text/markdown
 
-modules = \
-['markdown_pytest']
-install_requires = \
-['pytest-subtests>=0.9.0,<0.10.0']
-
-entry_points = \
-{'pytest11': ['markdown-pytest = markdown_pytest']}
-
-setup_kwargs = {
-    'name': 'markdown-pytest',
-    'version': '0.3.0',
-    'description': 'Pytest plugin for runs tests directly from Markdown files',
-    'long_description': 'markdown-pytest\n===============\n\nThe `markdown-pytest` plugin is a `pytest` plugin that allows you to run tests\ndirectly from Markdown files.\n\nWith this plugin, you can write your tests inside Markdown files, making it\neasy to read, understand and maintain your documentation samples.\nThe tests are executed just like any other Pytest tests.\n\nSample of markdown file content:\n\n````markdown\n<!-- name: test_assert_true -->\n```python\nassert True\n```\n````\n\n<details>\n<summary>Will be shown as</summary>\n\n<!-- name: test_assert_true -->\n```python\nassert True\n```\n\n</details>\n\nRestrictions\n------------\n\nSince there is no way to add attributes to a block of code in markdown, this \nmodule only runs those tests that are marked with a special comment.\n\nThe general format of this comment is as follows: parts separated by semicolons\nare a colon separated key-value pairs, the last semicolon is optional,\nand parts not containing a colon bill be ignored.\n\nExample:\n\n```markdown\n<!-- key1: value1; key2: value2 -->\n```\n\nMultiline example:\n\n```markdown\n<!-- \n    key1: value1; \n    key2: value2;\n-->\n```\n\nThis comment should be placed right before the block of code, exactly upper \nthe backticks, for example: \n\n````\n<!-- name: test_name -->\n```python\n```\n````\n\nThe `name` key is required, and blocks that do not contain it will be ignored.\n\nSome Markdown parsers support two or three dashes around comments, this module \nsupports both variants. The `case` parameter is optional and might be used for\nsubtests, see "Code split" section.\n\nCommon parsing rules\n--------------------\n\nThis module uses its own, very simple Markdown parser, which only supports code \nblock parsing. In general, the parsing behavior of a file follows the following \nrules:\n\n* Code without `<!-- name: test_name -->` comment will not be executed.\n* Allowed two or three dashes in the comment symbols\n\n  For example following line will be parsed identically:\n\n  ````markdown\n  <!--  name: test_name -->\n  <!--- name: test_name --->\n  <!--  name: test_name --->\n  <!--- name: test_name -->\n  ````\n\n* Code blocks with same names will be merged in one code and executed once\n* The optional comment parameter `case` will execute the block as a subtest.\n* Indented code blocks will be shifted left.\n  \n  For example:\n\n  ````markdown\n      <!-- name: test_name -->\n      ```python\n      assert True\n      ```\n  ````\n\n  Is the same of:\n\n  ````markdown\n  <!-- name: test_name -->\n  ```python\n  assert True\n  ```\n  ````\n\nCode split\n----------\n\nYou can split a test into multiple blocks with the same test name:\n\nMarkdown:\n\n````markdown\nThis block performs import:\n\n<!-- name: test_example -->\n```python\nfrom itertools import chain\n```\n\n`chain` usage example:\n\n<!-- name: test_example -->\n```python\nassert list(chain(range(2), range(2))) == [0, 1, 0, 1]\n```\n````\n\n<details>\n<summary>Will be shown as</summary>\n\nThis block performs import:\n\n<!-- name: test_example -->\n```python\nfrom itertools import chain\n```\n\n`chain` usage example:\n\n<!-- name: test_example -->\n```python\nassert list(chain(range(2), range(2))) == [0, 1, 0, 1]\n```\n\n</details>\n\nsubtests support\n----------------\n\nOf course, you can break tests into subtests by simply adding `case: case_name` \nto the markdown comment.\n\n````markdown\n<!-- name: test_counter -->\n```python\nfrom collections import Counter\n```\n\n<!-- \n    name: test_counter;\n    case: initialize_counter\n-->\n```python\ncounter = Counter()\n```\n\n<!-- \n    name: test_counter;\n    case: assign_counter_value\n-->\n```python\ncounter["foo"] += 1\n\nassert counter["foo"] == 1\n```\n````\n\n<details>\n<summary>Will be shown as</summary>\n\n<!-- name: test_counter -->\n```python\nfrom collections import Counter\n```\n\n<!-- \n    name: test_counter;\n    case: initialize_counter\n-->\n```python\ncounter = Counter()\n```\n\n<!-- \n    name: test_counter;\n    case: assign_counter_value\n-->\n```python\ncounter["foo"] += 1\n\nassert counter["foo"] == 1\n```\n\n</details>\n\nFictional Code Examples\n-----------------------\n\nCode without `<!-- name: test_name -->` comment will not be executed.\n\n````markdown\n```python\nfrom universe import antigravity, WrongPlanet\n\ntry:\n    antigravity()\nexcept WrongPlanet:\n    print("You are on the wrong planet.")\n    exit(1)\n```\n````\n\n<details>\n<summary>Will be shown as</summary>\n\n```python\nfrom universe import antigravity, WrongPlanet\n\ntry:\n    antigravity()\nexcept WrongPlanet:\n    print("You are on the wrong planet.")\n    exit(1)\n```\n</details>\n\nUsage example\n-------------\n\nThis README.md file might be tested like this:\n\n```bash\n$ pytest -v README.md\n======================= test session starts =======================\nplugins: subtests, markdown-pytest\ncollected 3 items\n\nREADME.md::test_assert_true PASSED                           [ 33%]\nREADME.md::test_example PASSED                               [ 66%]\nREADME.md::test_counter SUBPASS                              [100%]\nREADME.md::test_counter SUBPASS                              [100%]\nREADME.md::test_counter PASSED                               [100%]\n```\n',
-    'author': 'Dmitry Orlov',
-    'author_email': 'me@mosquito.su',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mosquito/markdown-pytest',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+markdown-pytest
+===============
 
+The `markdown-pytest` plugin is a `pytest` plugin that allows you to run tests
+directly from Markdown files.
+
+With this plugin, you can write your tests inside Markdown files, making it
+easy to read, understand and maintain your documentation samples.
+The tests are executed just like any other Pytest tests.
+
+Sample of markdown file content:
+
+````markdown
+<!-- name: test_assert_true -->
+```python
+assert True
+```
+````
+
+<details>
+<summary>Will be shown as</summary>
+
+<!-- name: test_assert_true -->
+```python
+assert True
+```
+
+</details>
+
+Restrictions
+------------
+
+Since there is no way to add attributes to a block of code in markdown, this 
+module only runs those tests that are marked with a special comment.
+
+The general format of this comment is as follows: parts separated by semicolons
+are a colon separated key-value pairs, the last semicolon is optional,
+and parts not containing a colon bill be ignored.
+
+Example:
+
+```markdown
+<!-- key1: value1; key2: value2 -->
+```
+
+Multiline example:
+
+```markdown
+<!-- 
+    key1: value1; 
+    key2: value2;
+-->
+```
+
+This comment should be placed right before the block of code, exactly upper 
+the backticks, for example: 
+
+````
+<!-- name: test_name -->
+```python
+```
+````
+
+The `name` key is required, and blocks that do not contain it will be ignored.
+
+Some Markdown parsers support two or three dashes around comments, this module 
+supports both variants. The `case` parameter is optional and might be used for
+subtests, see "Code split" section.
+
+Common parsing rules
+--------------------
+
+This module uses its own, very simple Markdown parser, which only supports code 
+block parsing. In general, the parsing behavior of a file follows the following 
+rules:
+
+* Code without `<!-- name: test_name -->` comment will not be executed.
+* Allowed two or three dashes in the comment symbols
+
+  For example following line will be parsed identically:
+
+  ````markdown
+  <!--  name: test_name -->
+  <!--- name: test_name --->
+  <!--  name: test_name --->
+  <!--- name: test_name -->
+  ````
+
+* Code blocks with same names will be merged in one code and executed once
+* The optional comment parameter `case` will execute the block as a subtest.
+* Indented code blocks will be shifted left.
+  
+  For example:
+
+  ````markdown
+      <!-- name: test_name -->
+      ```python
+      assert True
+      ```
+  ````
+
+  Is the same of:
+
+  ````markdown
+  <!-- name: test_name -->
+  ```python
+  assert True
+  ```
+  ````
+
+Code split
+----------
+
+You can split a test into multiple blocks with the same test name:
+
+Markdown:
+
+````markdown
+This block performs import:
+
+<!-- name: test_example -->
+```python
+from itertools import chain
+```
+
+`chain` usage example:
+
+<!-- name: test_example -->
+```python
+assert list(chain(range(2), range(2))) == [0, 1, 0, 1]
+```
+````
+
+<details>
+<summary>Will be shown as</summary>
+
+This block performs import:
+
+<!-- name: test_example -->
+```python
+from itertools import chain
+```
+
+`chain` usage example:
+
+<!-- name: test_example -->
+```python
+assert list(chain(range(2), range(2))) == [0, 1, 0, 1]
+```
+
+</details>
+
+subtests support
+----------------
+
+Of course, you can break tests into subtests by simply adding `case: case_name` 
+to the markdown comment.
+
+````markdown
+<!-- name: test_counter -->
+```python
+from collections import Counter
+```
+
+<!-- 
+    name: test_counter;
+    case: initialize_counter
+-->
+```python
+counter = Counter()
+```
+
+<!-- 
+    name: test_counter;
+    case: assign_counter_value
+-->
+```python
+counter["foo"] += 1
+
+assert counter["foo"] == 1
+```
+````
+
+<details>
+<summary>Will be shown as</summary>
+
+<!-- name: test_counter -->
+```python
+from collections import Counter
+```
+
+<!-- 
+    name: test_counter;
+    case: initialize_counter
+-->
+```python
+counter = Counter()
+```
+
+<!-- 
+    name: test_counter;
+    case: assign_counter_value
+-->
+```python
+counter["foo"] += 1
+
+assert counter["foo"] == 1
+```
+
+</details>
+
+Fictional Code Examples
+-----------------------
+
+Code without `<!-- name: test_name -->` comment will not be executed.
+
+````markdown
+```python
+from universe import antigravity, WrongPlanet
+
+try:
+    antigravity()
+except WrongPlanet:
+    print("You are on the wrong planet.")
+    exit(1)
+```
+````
+
+<details>
+<summary>Will be shown as</summary>
+
+```python
+from universe import antigravity, WrongPlanet
+
+try:
+    antigravity()
+except WrongPlanet:
+    print("You are on the wrong planet.")
+    exit(1)
+```
+</details>
+
+Usage example
+-------------
+
+This README.md file can be tested like this:
+
+```bash
+$ pytest -v README.md
+```
+```bash
+======================= test session starts =======================
+plugins: subtests, markdown-pytest
+collected 3 items
+
+README.md::test_assert_true PASSED                           [ 33%]
+README.md::test_example PASSED                               [ 66%]
+README.md::test_counter SUBPASS                              [100%]
+README.md::test_counter SUBPASS                              [100%]
+README.md::test_counter PASSED                               [100%]
+```
 
-setup(**setup_kwargs)
```

