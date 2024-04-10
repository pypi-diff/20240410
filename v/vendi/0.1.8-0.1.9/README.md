# Comparing `tmp/vendi-0.1.8.tar.gz` & `tmp/vendi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vendi-0.1.8.tar", max compression
+gzip compressed data, was "vendi-0.1.9.tar", max compression
```

## Comparing `vendi-0.1.8.tar` & `vendi-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     9758 2024-01-07 13:54:19.458407 vendi-0.1.8/README.md
--rw-r--r--   0        0        0      484 2024-01-07 13:54:37.390559 vendi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1592 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/__init__.py
--rw-r--r--   0        0        0      146 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/completions/__init__.py
--rw-r--r--   0        0        0     8132 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/completions/completions.py
--rw-r--r--   0        0        0     1610 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/completions/schema.py
--rw-r--r--   0        0        0       94 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/core/__init__.py
--rw-r--r--   0        0        0      418 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/core/config.py
--rw-r--r--   0        0        0     3838 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/core/http_client.py
--rw-r--r--   0        0        0      462 2024-01-07 13:54:19.458407 vendi-0.1.8/vendi/src/vendi/core/schema.py
--rw-r--r--   0        0        0      134 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/datasets/__init__.py
--rw-r--r--   0        0        0     3443 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/datasets/datasets.py
--rw-r--r--   0        0        0     1238 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/datasets/schema.py
--rw-r--r--   0        0        0      437 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/deployments/__init__.py
--rw-r--r--   0        0        0     6061 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/deployments/deployments.py
--rw-r--r--   0        0        0     2761 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/deployments/schema.py
--rw-r--r--   0        0        0      564 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/endpoints/__init__.py
--rw-r--r--   0        0        0     1243 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/endpoints/endpoints.py
--rw-r--r--   0        0        0     1823 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/endpoints/schema.py
--rw-r--r--   0        0        0        0 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/__init__.py
--rw-r--r--   0        0        0     3283 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/evaluation.py
--rw-r--r--   0        0        0      273 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/metrics/__init__.py
--rw-r--r--   0        0        0      186 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/metrics/base.py
--rw-r--r--   0        0        0      300 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/metrics/charachter_based.py
--rw-r--r--   0        0        0      269 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/metrics/model_based.py
--rw-r--r--   0        0        0      850 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/metrics/vector_based.py
--rw-r--r--   0        0        0        0 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/evaluations/service.py
--rw-r--r--   0        0        0      288 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/models/__init__.py
--rw-r--r--   0        0        0     2035 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/models/models.py
--rw-r--r--   0        0        0     1329 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/models/schema.py
--rw-r--r--   0        0        0      260 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/prompte_templates/__init__.py
--rw-r--r--   0        0        0     2765 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/prompte_templates/prompt_templates.py
--rw-r--r--   0        0        0     1248 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/prompte_templates/schema.py
--rw-r--r--   0        0        0      448 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/providers/__init__.py
--rw-r--r--   0        0        0     1956 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/providers/providers.py
--rw-r--r--   0        0        0      781 2024-01-07 13:54:19.462407 vendi-0.1.8/vendi/src/vendi/providers/schema.py
--rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 vendi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     9758 2024-01-07 14:11:06.946026 vendi-0.1.9/README.md
+-rw-r--r--   0        0        0      540 2024-01-07 14:11:22.818141 vendi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/__init__.py
+-rw-r--r--   0        0        0      146 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/completions/__init__.py
+-rw-r--r--   0        0        0     8132 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/completions/completions.py
+-rw-r--r--   0        0        0     1610 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/completions/schema.py
+-rw-r--r--   0        0        0       94 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/core/__init__.py
+-rw-r--r--   0        0        0      434 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/core/config.py
+-rw-r--r--   0        0        0     3838 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/core/http_client.py
+-rw-r--r--   0        0        0      462 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/core/schema.py
+-rw-r--r--   0        0        0      134 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/datasets/__init__.py
+-rw-r--r--   0        0        0     3443 2024-01-07 14:11:06.946026 vendi-0.1.9/src/vendi/datasets/datasets.py
+-rw-r--r--   0        0        0     1238 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/datasets/schema.py
+-rw-r--r--   0        0        0      437 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/deployments/__init__.py
+-rw-r--r--   0        0        0     6061 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/deployments/deployments.py
+-rw-r--r--   0        0        0     2831 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/deployments/schema.py
+-rw-r--r--   0        0        0      564 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/endpoints/__init__.py
+-rw-r--r--   0        0        0     1243 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/endpoints/endpoints.py
+-rw-r--r--   0        0        0     1905 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/endpoints/schema.py
+-rw-r--r--   0        0        0        0 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/__init__.py
+-rw-r--r--   0        0        0     3283 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/evaluation.py
+-rw-r--r--   0        0        0      265 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/metrics/__init__.py
+-rw-r--r--   0        0        0      186 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/metrics/base.py
+-rw-r--r--   0        0        0      300 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/metrics/charachter_based.py
+-rw-r--r--   0        0        0      269 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/metrics/model_based.py
+-rw-r--r--   0        0        0      850 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/metrics/vector_based.py
+-rw-r--r--   0        0        0        0 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/evaluations/service.py
+-rw-r--r--   0        0        0      288 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/models/__init__.py
+-rw-r--r--   0        0        0     2035 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/models/models.py
+-rw-r--r--   0        0        0     1329 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/models/schema.py
+-rw-r--r--   0        0        0      260 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/prompte_templates/__init__.py
+-rw-r--r--   0        0        0     2765 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/prompte_templates/prompt_templates.py
+-rw-r--r--   0        0        0     1248 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/prompte_templates/schema.py
+-rw-r--r--   0        0        0      448 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/providers/__init__.py
+-rw-r--r--   0        0        0     1956 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/providers/providers.py
+-rw-r--r--   0        0        0      781 2024-01-07 14:11:06.950026 vendi-0.1.9/src/vendi/providers/schema.py
+-rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 vendi-0.1.9/PKG-INFO
```

### Comparing `vendi-0.1.8/README.md` & `vendi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/__init__.py` & `vendi-0.1.9/src/vendi/__init__.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/completions/completions.py` & `vendi-0.1.9/src/vendi/completions/completions.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/completions/schema.py` & `vendi-0.1.9/src/vendi/completions/schema.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/core/http_client.py` & `vendi-0.1.9/src/vendi/core/http_client.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/datasets/datasets.py` & `vendi-0.1.9/src/vendi/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/datasets/schema.py` & `vendi-0.1.9/src/vendi/datasets/schema.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/deployments/deployments.py` & `vendi-0.1.9/src/vendi/deployments/deployments.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/deployments/schema.py` & `vendi-0.1.9/src/vendi/deployments/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,7 +67,11 @@
     """The provider of the deployment. vendi/azure/gcp/aws/tenant"""
     model_configuration: ModelConfig
     """The model configuration of the deployment."""
     deploy_configuration: DeploymentConfig
     """The deployment configuration of the deployment."""
     status: DeploymentStatus
     """The status of the deployment."""
+
+    model_config = ConfigDict(
+        protected_namespaces=(),
+    )
```

### Comparing `vendi-0.1.8/vendi/src/vendi/endpoints/__init__.py` & `vendi-0.1.9/src/vendi/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/endpoints/endpoints.py` & `vendi-0.1.9/src/vendi/endpoints/endpoints.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/endpoints/schema.py` & `vendi-0.1.9/src/vendi/endpoints/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from enum import Enum
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from vendi.core.schema import SchemaMixin
 from vendi.deployments.schema import DeploymentStatus
 
 
 class UsableEndpoint(BaseModel):
     id: uuid.UUID | str
@@ -35,13 +35,16 @@
     """
     The ID of the deployment to use for the endpoint. This value must be the ID of a deployment that is live and ready to be used.
     Each endpoint must be associated with a single deployment.
     """
     model_id: uuid.UUID | None = None  # For fine-tune endpoints
     """The ID of the model to use for the endpoint. This value shows the model id that runs within the deployment id."""
 
+    model_config = ConfigDict(
+        protected_namespaces=(),
+    )
 
 class Endpoint(CreateEndpointSchema):
     provider: str | None = None
     """The provider of the endpoint. vendi/openai/google/etc.."""
     status: DeploymentStatus | None = None
     """The status of the endpoint. A replica of the deployment id status"""
```

### Comparing `vendi-0.1.8/vendi/src/vendi/evaluations/evaluation.py` & `vendi-0.1.9/src/vendi/evaluations/evaluation.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/evaluations/metrics/vector_based.py` & `vendi-0.1.9/src/vendi/evaluations/metrics/vector_based.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/models/models.py` & `vendi-0.1.9/src/vendi/models/models.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/models/schema.py` & `vendi-0.1.9/src/vendi/models/schema.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/prompte_templates/prompt_templates.py` & `vendi-0.1.9/src/vendi/prompte_templates/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/prompte_templates/schema.py` & `vendi-0.1.9/src/vendi/prompte_templates/schema.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/providers/providers.py` & `vendi-0.1.9/src/vendi/providers/providers.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/vendi/src/vendi/providers/schema.py` & `vendi-0.1.9/src/vendi/providers/schema.py`

 * *Files identical despite different names*

### Comparing `vendi-0.1.8/PKG-INFO` & `vendi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vendi
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Aviv.a
 Author-email: aviv@vendi-ai.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

