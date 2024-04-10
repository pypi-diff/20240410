# Comparing `tmp/reasoner-pydantic-4.1.6.tar.gz` & `tmp/reasoner-pydantic-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.1.6.tar", last modified: Thu Dec 14 01:22:29 2023, max compression
+gzip compressed data, was "reasoner-pydantic-5.0.0.tar", last modified: Wed Apr 10 19:01:55 2024, max compression
```

## Comparing `reasoner-pydantic-4.1.6.tar` & `reasoner-pydantic-5.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 01:22:29.590693 reasoner-pydantic-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-12-14 01:22:29.590693 reasoner-pydantic-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 01:22:29.586693 reasoner-pydantic-4.1.6/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 01:22:29.590693 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-14 01:22:29.000000 reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 01:22:29.590693 reasoner-pydantic-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-12-14 01:22:22.000000 reasoner-pydantic-4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/setup.py
```

### Comparing `reasoner-pydantic-4.1.6/PKG-INFO` & `reasoner-pydantic-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.1.6
+Version: 5.0.0
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.1.6/README.md` & `reasoner-pydantic-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/__init__.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/auxgraphs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Auxiliary Graphs model"""
+
 from typing import Optional
 
 from pydantic import Field, parse_obj_as
 
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSet
 from .shared import Attribute, CURIE
 
 
 class AuxiliaryGraph(BaseModel):
     """Auxiliary Graph"""
 
     edges: HashableSet[str] = Field(..., title="edges in auxiliary graph")
 
-    attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
+    attributes: HashableSet[Attribute] = Field(..., nullable=False)
 
     class Config:
         title = "auxiliary graph"
         extra = "allow"
 
 
 class AuxiliaryGraphs(BaseModel):
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/base_model.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/kgraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Knowledge graph models."""
+
 from typing import Optional
 
 from pydantic import Field
 
 from .shared import (
     Attribute,
     BiolinkEntity,
@@ -15,21 +16,22 @@
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSet
 
 
 class Node(BaseModel):
     """Knowledge graph node."""
 
-    categories: Optional[HashableSet[BiolinkEntity]] = Field(
-        None,
+    categories: HashableSet[BiolinkEntity] = Field(
+        ...,
         title="categories",
-        nullable=True,
+        nullable=False,
     )
     name: Optional[str] = Field(None, nullable=True)
-    attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
+    attributes: HashableSet[Attribute] = Field(..., nullable=False)
+    is_set: Optional[bool]
 
     class Config:
         title = "knowledge-graph node"
         schema_extra = {
             "example": {
                 "category": "string",
             },
@@ -88,15 +90,15 @@
         title="object node id",
     )
     predicate: BiolinkPredicate = Field(..., title="edge predicate")
     sources: HashableSet[RetrievalSource] = Field(
         ..., title="list of source retrievals"
     )
     qualifiers: Optional[HashableSet[Qualifier]] = Field(None, nullable=True)
-    attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
+    attributes: Optional[HashableSet[Attribute]] = Field(..., nullable=False)
 
     class Config:
         title = "knowledge-graph edge"
         extra = "forbid"
 
     def update(self, other):
         if other.attributes:
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/message.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reasoner API models."""
+
 import copy
 import hashlib
 
 from typing import Optional, Callable
 
 from pydantic import constr, Field, parse_obj_as
 
@@ -171,51 +172,47 @@
     )
     log_level: Optional[LogLevel] = Field(
         None,
         title="log_level",
         nullable=True,
     )
     workflow: Optional[Workflow]
+    bypass_cache: Optional[bool]
 
     class Config:
         title = "query"
         extra = "allow"
         schema_extra = {"x-body-name": "request_body"}
 
 
 class AsyncQuery(BaseModel):
     """AsyncQuery."""
 
-    callback: constr(regex=r"^https?://") = Field(..., format="uri")
-    message: Message = Field(
-        ...,
-        title="message",
-    )
+    callback: constr(regex=r"^https?://") = Field(..., format="uri", nullable=False)
+    message: Message = Field(..., title="message", nullable=False)
     log_level: Optional[LogLevel] = Field(
         None,
         title="log_level",
         nullable=True,
     )
     workflow: Optional[Workflow]
+    bypass_cache: Optional[bool]
 
     class Config:
         title = "query"
         extra = "allow"
         schema_extra = {"x-body-name": "request_body"}
 
 
 class Response(BaseModel):
     """Response."""
 
-    message: Message = Field(
-        ...,
-        title="message",
-    )
+    message: Message = Field(..., title="message", nullable=False)
 
-    logs: Optional[HashableSequence[LogEntry]] = Field(None, nullable=True)
+    logs: Optional[HashableSequence[LogEntry]] = Field(..., nullable=False)
 
     status: Optional[str] = Field(None, nullable=True)
 
     workflow: Optional[Workflow]
 
     class Config:
         title = "response"
@@ -244,14 +241,14 @@
 class AsyncQueryStatusResponse(BaseModel):
     """Async Query Status Response."""
 
     status: str = Field(..., title="status")
 
     description: str = Field(..., title="description")
 
-    logs: Optional[HashableSet[LogEntry]] = Field(None, nullable=True)
+    logs: HashableSet[LogEntry] = Field(..., nullable=False)
 
     response_url: Optional[str] = Field(None, nullable=True)
 
     class Config:
         title = "async query status response"
         extra = "allow"
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/metakg.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/qgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query graph models."""
+
 from enum import Enum
 
 from pydantic.class_validators import validator
 from reasoner_pydantic.utils import HashableMapping
 from typing import Any, Optional
 
 from pydantic import Field
@@ -71,14 +72,22 @@
 
     qualifier_set: HashableSequence[Qualifier] = Field(
         default=HashableSequence[Qualifier](__root__=[]),
         title="qualifier set",
     )
 
 
+class SetInterpretationEnum(str, Enum):
+    """Enumeration for set interpretation."""
+
+    BATCH = "BATCH"
+    ALL = "ALL"
+    MANY = "MANY"
+
+
 class QNode(BaseModel):
     """Query node."""
 
     ids: Optional[HashableSequence[CURIE]] = Field(
         None,
         title="ids",
         nullable=True,
@@ -88,15 +97,15 @@
     categories: Optional[HashableSequence[BiolinkEntity]] = Field(
         None,
         title="categories",
         nullable=True,
     )
     _nonzero_categories = validator("categories", allow_reuse=True)(nonzero_validator)
 
-    is_set: bool = False
+    set_interpretation: Optional[SetInterpretationEnum] = Field(None, nullable=True)
     constraints: Optional[HashableSequence[AttributeConstraint]] = Field(
         default=HashableSequence[AttributeConstraint](__root__=[]),
         title="attribute constraints",
     )
 
     class Config:
         title = "query-graph node"
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/results.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Results models."""
+
 import copy
 from typing import Optional
 
 from pydantic import Field, parse_obj_as
 
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSet, HashableSequence
 from .shared import Attribute, CURIE
 
 
 class EdgeBinding(BaseModel):
     """Edge binding."""
 
-    id: str = Field(
-        ...,
-        title="knowledge graph id",
-    )
+    id: str = Field(..., title="knowledge graph id", nullable=False)
 
-    attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
+    attributes: HashableSet[Attribute] = Field(..., nullable=False)
 
     class Config:
         title = "edge binding"
         schema_extra = {
             "example": {
                 "id": "string",
             },
@@ -85,22 +83,19 @@
             else:
                 self.support_graphs = other.support_graphs
 
 
 class NodeBinding(BaseModel):
     """Node binding."""
 
-    id: CURIE = Field(
-        ...,
-        title="knowledge graph id",
-    )
+    id: CURIE = Field(..., title="knowledge graph id", nullable=False)
 
     query_id: Optional[CURIE] = Field(None, title="query graph id")
 
-    attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
+    attributes: HashableSet[Attribute] = Field(..., nullable=False)
 
     class Config:
         title = "node binding"
         schema_extra = {
             "example": {
                 "id": "x:string",
             },
@@ -108,21 +103,19 @@
         extra = "allow"
 
 
 class Result(BaseModel):
     """Result."""
 
     node_bindings: HashableMapping[str, HashableSet[NodeBinding]] = Field(
-        ...,
-        title="list of node bindings",
+        ..., title="list of node bindings", nullable=False
     )
 
     analyses: HashableSet[Analysis] = Field(
-        ...,
-        title="list of anlysis blocks",
+        ..., title="list of anlysis blocks", nullable=False
     )
 
     class Config:
         title = "result"
         extra = "allow"
 
     def update(self, other):
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/shared.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shared models."""
+
 from __future__ import annotations
 
 import re
 from datetime import datetime
 from enum import Enum
 import string
 from typing import Any, Optional
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/utils.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic/workflow.py` & `reasoner-pydantic-5.0.0/reasoner_pydantic/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Operations models."""
+
 from enum import Enum
 from typing import Any, Optional, Union
 from pydantic.class_validators import validator
 
 from pydantic.types import confloat, conint
 
 from .base_model import BaseModel
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.1.6
+Version: 5.0.0
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.1.6/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.6/setup.py` & `reasoner-pydantic-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Setup file for reasoner package."""
+
 from setuptools import setup
 
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.1.6",
+    version="5.0.0",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

