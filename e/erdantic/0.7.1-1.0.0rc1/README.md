# Comparing `tmp/erdantic-0.7.1.tar.gz` & `tmp/erdantic-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdantic-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "erdantic-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `erdantic-0.7.1.tar` & `erdantic-1.0.0rc1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-04-10 01:49:58.162600 erdantic-0.7.1/LICENSE
--rw-r--r--   0        0        0     3720 2024-04-10 01:49:58.162600 erdantic-0.7.1/README.md
--rw-r--r--   0        0        0      336 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/__init__.py
--rw-r--r--   0        0        0       66 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/__main__.py
--rw-r--r--   0        0        0     7542 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/base.py
--rw-r--r--   0        0        0     4622 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/cli.py
--rw-r--r--   0        0        0     2126 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/dataclasses.py
--rw-r--r--   0        0        0    13858 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/erd.py
--rw-r--r--   0        0        0      137 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/examples/__init__.py
--rw-r--r--   0        0        0     2246 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/examples/dataclasses.py
--rw-r--r--   0        0        0     2199 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/examples/pydantic.py
--rw-r--r--   0        0        0     3708 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/exceptions.py
--rw-r--r--   0        0        0     4023 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/pydantic.py
--rw-r--r--   0        0        0     4027 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/pydantic1.py
--rw-r--r--   0        0        0     4815 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/typing.py
--rw-r--r--   0        0        0      205 2024-04-10 01:49:58.166600 erdantic-0.7.1/erdantic/version.py
--rw-r--r--   0        0        0     1946 2024-04-10 01:49:58.166600 erdantic-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 erdantic-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4154 2024-03-31 00:41:27.886743 erdantic-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      426 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__main__.py
+-rw-r--r--   0        0        0      112 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_logging.py
+-rw-r--r--   0        0        0     2656 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_repr_utils.py
+-rw-r--r--   0        0        0       80 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_version.py
+-rw-r--r--   0        0        0     7502 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/cli.py
+-rw-r--r--   0        0        0     8420 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/convenience.py
+-rw-r--r--   0        0        0    28058 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/core.py
+-rw-r--r--   0        0        0      189 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2302 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/attrs.py
+-rw-r--r--   0        0        0     2330 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2251 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     2307 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py
+-rw-r--r--   0        0        0     5000 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/exceptions.py
+-rw-r--r--   0        0        0     3446 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/__init__.py
+-rw-r--r--   0        0        0     2184 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/attrs.py
+-rw-r--r--   0        0        0     3847 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/dataclasses.py
+-rw-r--r--   0        0        0     4797 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/pydantic.py
+-rw-r--r--   0        0        0        0 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/py.typed
+-rw-r--r--   0        0        0     3526 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/typing_utils.py
+-rw-r--r--   0        0        0     2123 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 erdantic-1.0.0rc1/PKG-INFO
```

### Comparing `erdantic-0.7.1/README.md` & `erdantic-1.0.0rc1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 [![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
 [![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
 [![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
 [![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
 [![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
 
+> [!NOTE]
+> erdantic v1.0 is coming soon and involves big backend changes. See the [changelog](./HISTORY.md) for more information.
+
 **erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
 
 - [Pydantic V2](https://docs.pydantic.dev/latest/)
 - [Pydantic V1 legacy](https://docs.pydantic.dev/latest/migration/#continue-using-pydantic-v1-features)
+- [attrs](https://www.attrs.org/en/stable/)
 - [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
 
-Features include a convenient CLI, automatic native rendering in Jupyter notebooks, and easy extensibility to other data modeling frameworks. Docstrings are even accessible as tooltips for SVG outputs. Great for adding a simple and clean data model reference to your documentation.
+You can use erdantic either as a convenient CLI or as a Python library. Great for adding a simple and clean data model reference to your documentation.
 
-<object type="image/svg+xml" data="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg"></object>
+<object type="image/svg+xml" data="./docs/docs/assets/example_diagram.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="./docs/docs/assets/example_diagram.svg"></object>
 
 ## Installation
 
 erdantic's graph modeling depends on [pygraphviz](https://pygraphviz.github.io/documentation/stable/index.html) and [Graphviz](https://graphviz.org/), an open-source C library. If you are on Linux or macOS, the easiest way to install everything together is to use conda and conda-forge:
 
 ```bash
 conda install erdantic -c conda-forge
@@ -35,32 +39,37 @@
 
 You can get the development version from GitHub with:
 
 ```bash
 pip install git+https://github.com/drivendataorg/erdantic.git#egg=erdantic
 ```
 
-## Quick Usage
+## Quick usage
+
+First, make sure that the data model classes that you want to include in your diagram are importable. This means the code with your models should either be available on your [`sys.path`](https://docs.python.org/3/library/sys_path_init.html) or installed into the same virtual environment as erdantic.
 
-The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted path to your data model class and an output path. The rendered format is interpreted from the filename extension.
+The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted import path to your model and an output file path. The rendered format is interpreted from the filename extension.
 
 ```bash
 erdantic erdantic.examples.pydantic.Party -o diagram.png
 ```
 
-You can also import the erdantic Python library and use its functions.
+You can also import the erdantic Python library. This lets you inspect the diagram data and potentially modify it. You will have greater ability to customize the diagram in Python.
 
 ```python
 import erdantic as erd
 from erdantic.examples.pydantic import Party
 
 # Easy one-liner
 erd.draw(Party, out="diagram.png")
 
 # Or create a diagram object that you can inspect and do stuff with
 diagram = erd.create(Party)
-diagram.models
-#> [PydanticModel(Adventurer), PydanticModel(Party), PydanticModel(Quest), PydanticModel(QuestGiver)]
+list(diagram.models.keys())
+#> [ 'erdantic.examples.pydantic.Adventurer',
+#>   'erdantic.examples.pydantic.Party',
+#>   'erdantic.examples.pydantic.Quest',
+#>   'erdantic.examples.pydantic.QuestGiver']
 diagram.draw("diagram.png")
 ```
 
 Check out the "Usage Examples" section of our [docs](https://erdantic.drivendata.org/) to see more.
```

### Comparing `erdantic-0.7.1/erdantic/examples/dataclasses.py` & `erdantic-1.0.0rc1/erdantic/examples/dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Example data model classes using standard library's
 [`dataclasses`](https://docs.python.org/3/library/dataclasses.html) module."""
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 
 class Alignment(str, Enum):
     LAWFUL_GOOD = "lawful_good"
@@ -22,52 +22,52 @@
 @dataclass
 class Adventurer:
     """A person often late for dinner but with a tale or two to tell.
 
     Attributes:
         name (str): Name of this adventurer
         profession (str): Profession of this adventurer
-        level (int): Level of this adventurer
         alignment (Alignment): Alignment of this adventurer
+        level (int): Level of this adventurer
     """
 
     name: str
     profession: str
-    level: int
     alignment: Alignment
+    level: int = 1
 
 
 @dataclass
 class QuestGiver:
     """A person who offers a task that needs completing.
 
     Attributes:
         name (str): Name of this quest giver
         faction (str): Faction that this quest giver belongs to
         location (str): Location this quest giver can be found
     """
 
     name: str
-    faction: Optional[str]
-    location: str
+    faction: Optional[str] = None
+    location: str = "Adventurer's Guild"
 
 
 @dataclass
 class Quest:
     """A task to complete, with some monetary reward.
 
     Attributes:
         name (str): Name by which this quest is referred to
         giver (QuestGiver): Person who offered the quest
         reward_gold (int): Amount of gold to be rewarded for quest completion
     """
 
     name: str
     giver: QuestGiver
-    reward_gold: int
+    reward_gold: int = 100
 
 
 @dataclass
 class Party:
     """A group of adventurers finding themselves doing and saying things altogether unexpected.
 
     Attributes:
@@ -75,9 +75,9 @@
         formed_datetime (datetime): Timestamp of when the party was formed
         members (List[Adventurer]): Adventurers that belong to this party
         active_quest (Optional[Quest]): Current quest that party is actively tackling
     """
 
     name: str
     formed_datetime: datetime
-    members: List[Adventurer]
-    active_quest: Optional[Quest]
+    members: List[Adventurer] = field(default_factory=list)
+    active_quest: Optional[Quest] = None
```

### Comparing `erdantic-0.7.1/erdantic/examples/pydantic.py` & `erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Example data model classes using [Pydantic](https://pydantic-docs.helpmanual.io/)."""
+"""Example data model classes using legacy
+[Pydantic V1](https://docs.pydantic.dev/latest/migration/#continue-using-pydantic-v1-features)."""
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 
 
 class Alignment(str, Enum):
     LAWFUL_GOOD = "lawful_good"
     NEUTRAL_GOOD = "neutral_good"
     CHAOTIC_GOOD = "chaotic_good"
     LAWFUL_NEUTRAL = "lawful_neutral"
@@ -21,59 +22,59 @@
 
 class Adventurer(BaseModel):
     """A person often late for dinner but with a tale or two to tell.
 
     Attributes:
         name (str): Name of this adventurer
         profession (str): Profession of this adventurer
-        level (int): Level of this adventurer
         alignment (Alignment): Alignment of this adventurer
+        level (int): Level of this adventurer
     """
 
     name: str
     profession: str
-    level: int
     alignment: Alignment
+    level: int = 1
 
 
 class QuestGiver(BaseModel):
     """A person who offers a task that needs completing.
 
     Attributes:
         name (str): Name of this quest giver
         faction (str): Faction that this quest giver belongs to
         location (str): Location this quest giver can be found
     """
 
     name: str
-    faction: Optional[str]
-    location: str
+    faction: Optional[str] = None
+    location: str = "Adventurer's Guild"
 
 
 class Quest(BaseModel):
     """A task to complete, with some monetary reward.
 
     Attributes:
         name (str): Name by which this quest is referred to
         giver (QuestGiver): Person who offered the quest
         reward_gold (int): Amount of gold to be rewarded for quest completion
     """
 
     name: str
     giver: QuestGiver
-    reward_gold: int
+    reward_gold: int = 100
 
 
 class Party(BaseModel):
     """A group of adventurers finding themselves doing and saying things altogether unexpected.
 
     Attributes:
         name (str): Name that party is known by
         formed_datetime (datetime): Timestamp of when the party was formed
         members (List[Adventurer]): Adventurers that belong to this party
         active_quest (Optional[Quest]): Current quest that party is actively tackling
     """
 
     name: str
     formed_datetime: datetime
-    members: List[Adventurer]
-    active_quest: Optional[Quest]
+    members: List[Adventurer] = []
+    active_quest: Optional[Quest] = None
```

### Comparing `erdantic-0.7.1/pyproject.toml` & `erdantic-1.0.0rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "erdantic"
-version = "0.7.1"
+version = "1.0.0rc1"
 description = "Entity relationship diagrams for Python data model classes like Pydantic."
 readme = "README.md"
-authors = [{ name = "DrivenData", email = "info@drivendata.org" }]
-license = { file = "LICENSE" }
-keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic"]
+authors = [{ name = "DrivenData", email = "info@drivendata.org" }, { name = "Jay Qi" }]
+license = { text = "MIT License" }
+keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic", "attrs"]
 classifiers = [
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Code Generators",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Framework :: Pydantic",
+  "Framework :: Pydantic :: 2",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-  "importlib_metadata ; python_version < '3.8'",
   "pydantic >= 2",
   "pydantic-core",
   "pygraphviz",
-  "typer < 0.10.0",
-  "typing_extensions > 4 ; python_version < '3.8'",
+  "sortedcontainers-pydantic",
+  "typenames",
+  "typer",
 ]
 
+[project.optional-dependencies]
+attrs = ["attrs"]
+
 [project.scripts]
 erdantic = "erdantic.cli:app"
 
 [project.urls]
 "Repository" = "https://github.com/drivendataorg/erdantic"
 "Documentation" = "https://erdantic.drivendata.org/"
 "Bug Tracker" = "https://github.com/drivendataorg/erdantic/issues"
 "Changelog" = "https://erdantic.drivendata.org/stable/changelog/"
 
 [tool.ruff]
 line-length = 99
-src = ["erdantic/**/*.py", "tests/**/*.py"]
+src = ["erdantic/**/*.py", "tests/**/*.py", "docs/**/*.py"]
 
 [tool.ruff.lint]
 select = [
   "E", # Pyflakes
   "F", # Pycodestyle
   "I", # isort
 ]
 unfixable = ["F"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["erdantic"]
 force-sort-within-sections = true
 
 [tool.mypy]
-ignore_missing_imports = true
+files = ["erdantic", "tests/typechecks.py"]
+plugins = ["pydantic.mypy"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--cov=erdantic --cov-report=term --cov-report=html --cov-report=xml"
+addopts = "--cov=erdantic --cov-report=term --cov-report=html --cov-report=xml --cov-append"
 testpaths = ["tests"]
 
 [tool.coverage.run]
 source = ["erdantic"]
+
+[tool.coverage.report]
+exclude_also = [
+  "if TYPE_CHECKING:",
+]
```

### Comparing `erdantic-0.7.1/PKG-INFO` & `erdantic-1.0.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 Metadata-Version: 2.1
 Name: erdantic
-Version: 0.7.1
+Version: 1.0.0rc1
 Summary: Entity relationship diagrams for Python data model classes like Pydantic.
-Keywords: erd,entity relationship diagram,dataclasses,pydantic
+Keywords: erd,entity relationship diagram,dataclasses,pydantic,attrs
+Author: Jay Qi
 Author-email: DrivenData <info@drivendata.org>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: importlib_metadata ; python_version < '3.8'
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
 Requires-Dist: pydantic >= 2
 Requires-Dist: pydantic-core
 Requires-Dist: pygraphviz
-Requires-Dist: typer < 0.10.0
-Requires-Dist: typing_extensions > 4 ; python_version < '3.8'
+Requires-Dist: sortedcontainers-pydantic
+Requires-Dist: typenames
+Requires-Dist: typer
+Requires-Dist: attrs ; extra == "attrs"
 Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
 Project-URL: Changelog, https://erdantic.drivendata.org/stable/changelog/
 Project-URL: Documentation, https://erdantic.drivendata.org/
 Project-URL: Repository, https://github.com/drivendataorg/erdantic
+Provides-Extra: attrs
 
 # erdantic: Entity Relationship Diagrams
 
 [![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
 [![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
 [![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
 [![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
 [![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
 
+> [!NOTE]
+> erdantic v1.0 is coming soon and involves big backend changes. See the [changelog](./HISTORY.md) for more information.
+
 **erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
 
 - [Pydantic V2](https://docs.pydantic.dev/latest/)
 - [Pydantic V1 legacy](https://docs.pydantic.dev/latest/migration/#continue-using-pydantic-v1-features)
+- [attrs](https://www.attrs.org/en/stable/)
 - [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
 
-Features include a convenient CLI, automatic native rendering in Jupyter notebooks, and easy extensibility to other data modeling frameworks. Docstrings are even accessible as tooltips for SVG outputs. Great for adding a simple and clean data model reference to your documentation.
+You can use erdantic either as a convenient CLI or as a Python library. Great for adding a simple and clean data model reference to your documentation.
 
-<object type="image/svg+xml" data="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg"></object>
+<object type="image/svg+xml" data="./docs/docs/assets/example_diagram.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="./docs/docs/assets/example_diagram.svg"></object>
 
 ## Installation
 
 erdantic's graph modeling depends on [pygraphviz](https://pygraphviz.github.io/documentation/stable/index.html) and [Graphviz](https://graphviz.org/), an open-source C library. If you are on Linux or macOS, the easiest way to install everything together is to use conda and conda-forge:
 
 ```bash
 conda install erdantic -c conda-forge
@@ -65,33 +73,38 @@
 
 You can get the development version from GitHub with:
 
 ```bash
 pip install git+https://github.com/drivendataorg/erdantic.git#egg=erdantic
 ```
 
-## Quick Usage
+## Quick usage
+
+First, make sure that the data model classes that you want to include in your diagram are importable. This means the code with your models should either be available on your [`sys.path`](https://docs.python.org/3/library/sys_path_init.html) or installed into the same virtual environment as erdantic.
 
-The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted path to your data model class and an output path. The rendered format is interpreted from the filename extension.
+The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted import path to your model and an output file path. The rendered format is interpreted from the filename extension.
 
 ```bash
 erdantic erdantic.examples.pydantic.Party -o diagram.png
 ```
 
-You can also import the erdantic Python library and use its functions.
+You can also import the erdantic Python library. This lets you inspect the diagram data and potentially modify it. You will have greater ability to customize the diagram in Python.
 
 ```python
 import erdantic as erd
 from erdantic.examples.pydantic import Party
 
 # Easy one-liner
 erd.draw(Party, out="diagram.png")
 
 # Or create a diagram object that you can inspect and do stuff with
 diagram = erd.create(Party)
-diagram.models
-#> [PydanticModel(Adventurer), PydanticModel(Party), PydanticModel(Quest), PydanticModel(QuestGiver)]
+list(diagram.models.keys())
+#> [ 'erdantic.examples.pydantic.Adventurer',
+#>   'erdantic.examples.pydantic.Party',
+#>   'erdantic.examples.pydantic.Quest',
+#>   'erdantic.examples.pydantic.QuestGiver']
 diagram.draw("diagram.png")
 ```
 
 Check out the "Usage Examples" section of our [docs](https://erdantic.drivendata.org/) to see more.
```

