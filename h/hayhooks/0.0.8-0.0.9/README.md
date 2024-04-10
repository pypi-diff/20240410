# Comparing `tmp/hayhooks-0.0.8.tar.gz` & `tmp/hayhooks-0.0.9.tar.gz`

## Comparing `hayhooks-0.0.8.tar` & `hayhooks-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hayhooks-0.0.8/Dockerfile
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hayhooks-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 hayhooks-0.0.8/img/test_pipeline_01.png
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/__main__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/cli/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/cli/deploy/__init__.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/cli/run/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/cli/status/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/cli/undeploy/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/__init__.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/app.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/handlers/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/handlers/deploy.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/handlers/draw.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/handlers/status.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/handlers/undeploy.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/pipelines/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/pipelines/models.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/pipelines/registry.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/utils/__init__.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/server/utils/deploy_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/testing/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hayhooks-0.0.8/src/hayhooks/testing/components.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hayhooks-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 hayhooks-0.0.8/tests/test_files/test_pipeline_01.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hayhooks-0.0.8/tests/test_files/test_pipeline_02.yml
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hayhooks-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hayhooks-0.0.8/LICENSE
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 hayhooks-0.0.8/README.md
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 hayhooks-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 hayhooks-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hayhooks-0.0.9/Dockerfile
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hayhooks-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 hayhooks-0.0.9/img/test_pipeline_01.png
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/__main__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/cli/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/cli/deploy/__init__.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/cli/run/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/cli/status/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/cli/undeploy/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/app.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/handlers/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/handlers/deploy.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/handlers/draw.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/handlers/status.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/handlers/undeploy.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/pipelines/__init__.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/pipelines/models.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/pipelines/registry.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/utils/__init__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/server/utils/deploy_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/testing/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hayhooks-0.0.9/src/hayhooks/testing/components.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hayhooks-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 hayhooks-0.0.9/tests/test_files/test_pipeline_01.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hayhooks-0.0.9/tests/test_files/test_pipeline_02.yml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hayhooks-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hayhooks-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 hayhooks-0.0.9/README.md
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 hayhooks-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 hayhooks-0.0.9/PKG-INFO
```

### Comparing `hayhooks-0.0.8/img/test_pipeline_01.png` & `hayhooks-0.0.9/img/test_pipeline_01.png`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/cli/__init__.py` & `hayhooks-0.0.9/src/hayhooks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/cli/deploy/__init__.py` & `hayhooks-0.0.9/src/hayhooks/cli/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/cli/status/__init__.py` & `hayhooks-0.0.9/src/hayhooks/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/cli/undeploy/__init__.py` & `hayhooks-0.0.9/src/hayhooks/cli/undeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/server/app.py` & `hayhooks-0.0.9/src/hayhooks/server/app.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/server/handlers/undeploy.py` & `hayhooks-0.0.9/src/hayhooks/server/handlers/undeploy.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/server/pipelines/models.py` & `hayhooks-0.0.9/src/hayhooks/server/pipelines/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import get_args, get_origin, List
 
-from pydantic import BaseModel, create_model
+from pydantic import BaseModel, create_model, ConfigDict
 from haystack.dataclasses import Document
 
 
 class HaystackDocument(BaseModel):
     id: str
     content: str
 
@@ -22,14 +22,16 @@
             'value': {'type': <class 'int'>, 'is_mandatory': True}, <-- Input
             'add': {'type': typing.Optional[int], 'is_mandatory': False, 'default_value': None}, <-- Input
         },
         'second_addition': {'add': {'type': typing.Optional[int], 'is_mandatory': False}},
     }
     """
     request_model = {}
+    config = ConfigDict(arbitrary_types_allowed=True)
+
     for component_name, inputs in pipeline_inputs.items():
 
         component_model = {}
         for name, typedef in inputs.items():
             component_model[name] = (typedef["type"], typedef.get("default_value", ...))
         request_model[component_name] = (create_model('ComponentParams', **component_model, __config__=config), ...)
 
@@ -42,15 +44,17 @@
     {
         'second_addition': { <-- Component Name
             'result': {'type': "<class 'int'>"}  <-- Output
         },
     }
     """
     response_model = {}
-    for component_name, outputs in pipe.outputs().items():
+    config = ConfigDict(arbitrary_types_allowed=True)
+
+    for component_name, outputs in pipeline_outputs.items():
         component_model = {}
         for name, typedef in outputs.items():
             output_type = typedef["type"]
             if get_origin(output_type) == list and get_args(output_type)[0] == Document:
                 component_model[name] = (List[HaystackDocument], ...)
             else:
                 component_model[name] = (typedef["type"], ...)
```

### Comparing `hayhooks-0.0.8/src/hayhooks/server/pipelines/registry.py` & `hayhooks-0.0.9/src/hayhooks/server/pipelines/registry.py`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/src/hayhooks/server/utils/deploy_utils.py` & `hayhooks-0.0.9/src/hayhooks/server/utils/deploy_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from fastapi import HTTPException
 from fastapi.responses import JSONResponse
-from pydantic import ConfigDict
+
 
 from hayhooks.server.pipelines import registry
 from hayhooks.server.pipelines.models import (
-    HaystackDocument,
     PipelineDefinition,
     get_request_model,
     get_response_model,
     convert_component_output,
 )
-from haystack.dataclasses import Document
 
 
 def deploy_pipeline_def(app, pipeline_def: PipelineDefinition):
     try:
         pipe = registry.add(pipeline_def.name, pipeline_def.source_code)
     except ValueError as e:
         raise HTTPException(status_code=409, detail=f"{e}") from e
 
-    config = ConfigDict(arbitrary_types_allowed=True)
-
     PipelineRunRequest = get_request_model(pipeline_def.name, pipe.inputs())
     PipelineRunResponse = get_response_model(pipeline_def.name, pipe.outputs())
 
     # There's no way in FastAPI to define the type of the request body other than annotating
     # the endpoint handler. We have to ignore the type here to make FastAPI happy while
     # silencing static type checkers (that would have good reasons to trigger!).
     async def pipeline_run(pipeline_run_req: PipelineRunRequest) -> JSONResponse:  # type: ignore
```

### Comparing `hayhooks-0.0.8/.gitignore` & `hayhooks-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/LICENSE` & `hayhooks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/README.md` & `hayhooks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/pyproject.toml` & `hayhooks-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hayhooks-0.0.8/PKG-INFO` & `hayhooks-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayhooks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Grab and deploy Haystack pipelines
 Project-URL: Documentation, https://github.com/unknown/hayhooks#readme
 Project-URL: Issues, https://github.com/unknown/hayhooks/issues
 Project-URL: Source, https://github.com/unknown/hayhooks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

