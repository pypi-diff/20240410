# Comparing `tmp/scale_egp-1.0.5.tar.gz` & `tmp/scale_egp-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_egp-1.0.5.tar", max compression
+gzip compressed data, was "scale_egp-1.1.5.tar", max compression
```

## Comparing `scale_egp-1.0.5.tar` & `scale_egp-1.1.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    17859 2024-03-28 12:58:46.893521 scale_egp-1.0.5/README.md
--rw-r--r--   0        0        0     1100 2024-03-28 12:58:46.893521 scale_egp-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/__init__.py
--rw-r--r--   0        0        0       74 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/__init__.py
--rw-r--r--   0        0        0     4533 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/cli_main.py
--rw-r--r--   0        0        0    17966 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/collections.py
--rw-r--r--   0        0        0     7729 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/formatter.py
--rw-r--r--   0        0        0     1469 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/model_instance_description.py
--rw-r--r--   0        0        0     1828 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/cli/parser.py
--rw-r--r--   0        0        0     1733 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/__init__.py
--rw-r--r--   0        0        0    12689 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/client.py
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/__init__.py
--rw-r--r--   0        0        0     2914 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/application_specs.py
--rw-r--r--   0        0        0     3170 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/chunks.py
--rw-r--r--   0        0        0     5272 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/completions.py
--rw-r--r--   0        0        0     2500 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/evaluation_configs.py
--rw-r--r--   0        0        0    25007 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/evaluation_datasets.py
--rw-r--r--   0        0        0     8055 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/evaluations.py
--rw-r--r--   0        0        0     4918 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/fine_tuning.py
--rw-r--r--   0        0        0    14039 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/knowledge_bases.py
--rw-r--r--   0        0        0     2685 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/model_groups.py
--rw-r--r--   0        0        0     4798 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/model_templates.py
--rw-r--r--   0        0        0     7572 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/models.py
--rw-r--r--   0        0        0     1862 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/question_sets.py
--rw-r--r--   0        0        0     2588 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/questions.py
--rw-r--r--   0        0        0     1510 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/collections/users.py
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/constants/__init__.py
--rw-r--r--   0        0        0      762 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/constants/model_schemas.py
--rw-r--r--   0        0        0     9049 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/enums.py
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/models/__init__.py
--rw-r--r--   0        0        0     2387 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/models/fine_tuning_jobs.py
--rw-r--r--   0        0        0     2069 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/models/model_enums.py
--rw-r--r--   0        0        0     8403 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/models/model_vendor_configuration.py
--rw-r--r--   0        0        0      647 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/__init__.py
--rw-r--r--   0        0        0     4651 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/agents.py
--rw-r--r--   0        0        0      741 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/application_specs.py
--rw-r--r--   0        0        0     6125 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/chunks.py
--rw-r--r--   0        0        0     6553 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/completions.py
--rw-r--r--   0        0        0     1016 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/embeddings.py
--rw-r--r--   0        0        0     1019 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/evaluation_configs.py
--rw-r--r--   0        0        0     3474 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py
--rw-r--r--   0        0        0     1686 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/evaluation_datasets.py
--rw-r--r--   0        0        0     4747 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/evaluation_test_case_results.py
--rw-r--r--   0        0        0     1398 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/evaluations.py
--rw-r--r--   0        0        0     3333 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/fine_tuning.py
--rw-r--r--   0        0        0     1860 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_artifacts.py
--rw-r--r--   0        0        0     1559 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_chunks.py
--rw-r--r--   0        0        0    11128 2024-03-28 12:58:46.889521 scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_uploads.py
--rw-r--r--   0        0        0     1863 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/knowledge_bases.py
--rw-r--r--   0        0        0     1112 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/memory_strategy.py
--rw-r--r--   0        0        0     2478 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/message.py
--rw-r--r--   0        0        0     3557 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/model_templates.py
--rw-r--r--   0        0        0    14065 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/models.py
--rw-r--r--   0        0        0     1086 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/models_group.py
--rw-r--r--   0        0        0      891 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/question_sets.py
--rw-r--r--   0        0        0     5234 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/questions.py
--rw-r--r--   0        0        0      410 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/sdk/types/user_info.py
--rw-r--r--   0        0        0        0 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/utils/__init__.py
--rw-r--r--   0        0        0    11431 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/utils/api_utils.py
--rw-r--r--   0        0        0     3541 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/utils/model_utils.py
--rw-r--r--   0        0        0      107 2024-03-28 12:58:46.893521 scale_egp-1.0.5/scale_egp/utils/strenum_compat.py
--rw-r--r--   0        0        0    18855 1970-01-01 00:00:00.000000 scale_egp-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    17859 2024-04-09 22:10:29.167863 scale_egp-1.1.5/README.md
+-rw-r--r--   0        0        0     1100 2024-04-09 22:10:29.167863 scale_egp-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/__init__.py
+-rw-r--r--   0        0        0     4533 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/cli_main.py
+-rw-r--r--   0        0        0    17966 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/collections.py
+-rw-r--r--   0        0        0     7857 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/formatter.py
+-rw-r--r--   0        0        0     1469 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/model_instance_description.py
+-rw-r--r--   0        0        0     1828 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/parser.py
+-rw-r--r--   0        0        0     1733 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/client.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/__init__.py
+-rw-r--r--   0        0        0     2914 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/application_specs.py
+-rw-r--r--   0        0        0     3170 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/chunks.py
+-rw-r--r--   0        0        0     5272 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/completions.py
+-rw-r--r--   0        0        0     2500 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_configs.py
+-rw-r--r--   0        0        0    25007 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_datasets.py
+-rw-r--r--   0        0        0     8055 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluations.py
+-rw-r--r--   0        0        0     4918 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/fine_tuning.py
+-rw-r--r--   0        0        0    25810 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/knowledge_bases.py
+-rw-r--r--   0        0        0     2685 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/model_groups.py
+-rw-r--r--   0        0        0     4798 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/model_templates.py
+-rw-r--r--   0        0        0     7572 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/models.py
+-rw-r--r--   0        0        0     1862 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/question_sets.py
+-rw-r--r--   0        0        0     2588 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/questions.py
+-rw-r--r--   0        0        0     1510 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/users.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/constants/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/constants/model_schemas.py
+-rw-r--r--   0        0        0     9225 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/enums.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/__init__.py
+-rw-r--r--   0        0        0     2387 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/fine_tuning_jobs.py
+-rw-r--r--   0        0        0     2069 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/model_enums.py
+-rw-r--r--   0        0        0     8403 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/model_vendor_configuration.py
+-rw-r--r--   0        0        0      647 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/__init__.py
+-rw-r--r--   0        0        0     4651 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/agents.py
+-rw-r--r--   0        0        0      741 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/application_specs.py
+-rw-r--r--   0        0        0     6125 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/chunks.py
+-rw-r--r--   0        0        0     6553 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/completions.py
+-rw-r--r--   0        0        0     1016 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/embeddings.py
+-rw-r--r--   0        0        0     1019 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_configs.py
+-rw-r--r--   0        0        0     3474 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py
+-rw-r--r--   0        0        0     1686 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_datasets.py
+-rw-r--r--   0        0        0     4747 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_test_case_results.py
+-rw-r--r--   0        0        0     1398 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluations.py
+-rw-r--r--   0        0        0     3401 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/fine_tuning.py
+-rw-r--r--   0        0        0     1860 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_artifacts.py
+-rw-r--r--   0        0        0     1559 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_chunks.py
+-rw-r--r--   0        0        0    15686 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_uploads.py
+-rw-r--r--   0        0        0     1863 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_bases.py
+-rw-r--r--   0        0        0     1112 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/memory_strategy.py
+-rw-r--r--   0        0        0     2478 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/message.py
+-rw-r--r--   0        0        0     3557 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/model_templates.py
+-rw-r--r--   0        0        0    14065 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/models.py
+-rw-r--r--   0        0        0     1086 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/models_group.py
+-rw-r--r--   0        0        0      891 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/question_sets.py
+-rw-r--r--   0        0        0     5234 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/questions.py
+-rw-r--r--   0        0        0      410 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/user_info.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/__init__.py
+-rw-r--r--   0        0        0    11461 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/api_utils.py
+-rw-r--r--   0        0        0     3541 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/model_utils.py
+-rw-r--r--   0        0        0      107 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/strenum_compat.py
+-rw-r--r--   0        0        0    18855 1970-01-01 00:00:00.000000 scale_egp-1.1.5/PKG-INFO
```

### Comparing `scale_egp-1.0.5/README.md` & `scale_egp-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/pyproject.toml` & `scale_egp-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scale-egp"
-version = "1.0.5"
+version = "1.1.5"
 description = "SDK for Scale SGP API"
 license = "Apache 2.0 modified with Commons Clause"
 authors = ["Scale SGP team"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/sgp-py/"
 repository = "https://github.com/scaleapi/egp-py"
 packages = [{include = "scale_egp"}]
```

### Comparing `scale_egp-1.0.5/scale_egp/cli/cli_main.py` & `scale_egp-1.1.5/scale_egp/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/cli/collections.py` & `scale_egp-1.1.5/scale_egp/cli/collections.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/cli/formatter.py` & `scale_egp-1.1.5/scale_egp/cli/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,18 @@
 
 class RichFormatter(Formatter):
     LIST_JOINER = ", "
     name = "rich"
 
     def stringify_one(self, value: Any) -> str:
         if isinstance(value, list):
-            return f"[{self.LIST_JOINER.join([self.stringify_one(element) for element in value])}]"
+            # The opening square bracket to avoid Rich rendering the list is a markdown link.
+            return (
+                f"\\[{self.LIST_JOINER.join([self.stringify_one(element) for element in value])}]"
+            )
         if is_str_enum(type(value)):
             return value.value
         if isinstance(value, Markdownable):
             return value.to_markdown()
         if isinstance(value, BaseModel):
             return value.json(indent=2)
         if isinstance(value, dict):
```

### Comparing `scale_egp-1.0.5/scale_egp/cli/model_instance_description.py` & `scale_egp-1.1.5/scale_egp/cli/model_instance_description.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/cli/parser.py` & `scale_egp-1.1.5/scale_egp/cli/parser.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/exceptions.py` & `scale_egp-1.1.5/scale_egp/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/client.py` & `scale_egp-1.1.5/scale_egp/sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 from scale_egp.sdk.collections.application_specs import ApplicationSpecCollection
 from scale_egp.sdk.collections.chunks import ChunkCollection
 from scale_egp.sdk.collections.completions import CompletionCollection
 from scale_egp.sdk.collections.evaluation_configs import EvaluationConfigCollection
 from scale_egp.sdk.collections.evaluation_datasets import EvaluationDatasetCollection
 from scale_egp.sdk.collections.evaluations import EvaluationCollection
-from scale_egp.sdk.collections.knowledge_bases import KnowledgeBaseCollection
+from scale_egp.sdk.collections.knowledge_bases import (
+    KnowledgeBaseCollection,
+    KnowledgeBaseDataSourceCollection,
+)
 from scale_egp.sdk.collections.model_groups import ModelGroupCollection
 from scale_egp.sdk.collections.model_templates import ModelTemplateCollection
 from scale_egp.sdk.collections.models import ModelInstanceCollection
 from scale_egp.sdk.collections.question_sets import QuestionSetCollection
 from scale_egp.sdk.collections.questions import QuestionCollection
 from scale_egp.sdk.collections.users import UsersCollection
 from scale_egp.sdk.types.user_info import UserInfoResponse
@@ -154,14 +157,25 @@
         Use this collection to create and manage Knowledge Bases.
 
         Returns:
             The Knowledge Base Collection.
         """
         return KnowledgeBaseCollection(self)
 
+    def knowledge_base_data_sources(self) -> KnowledgeBaseDataSourceCollection:
+        """
+        Returns the Knowledge Base Data Source Collection.
+
+        Use this collection to create and manage Knowledge Bases.
+
+        Returns:
+            The Knowledge Base Data Source Collection.
+        """
+        return KnowledgeBaseDataSourceCollection(self)
+
     def chunks(self) -> ChunkCollection:
         """
         Returns the Chunk Collection.
 
         Use this collection to create and manage Chunks.
 
         Returns:
```

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/application_specs.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/chunks.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/completions.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/evaluation_configs.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/evaluation_datasets.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/evaluations.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/fine_tuning.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/model_groups.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/model_groups.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/model_templates.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/models.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/question_sets.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/questions.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/collections/users.py` & `scale_egp-1.1.5/scale_egp/sdk/collections/users.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/constants/model_schemas.py` & `scale_egp-1.1.5/scale_egp/sdk/constants/model_schemas.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/enums.py` & `scale_egp-1.1.5/scale_egp/sdk/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,16 @@
     An enum representing the different types of chunking strategies supported.
 
     Attributes:
         CHARACTER: Denotes that the chunking strategy is to chunk by character.
     """
 
     CHARACTER = "character"
+    TOKEN = "token"
+    CUSTOM = "custom"
 
 
 class ArtifactSource(str, Enum):
     """
     An enum representing the different types of artifact sources supported.
 
     Attributes:
@@ -273,7 +275,13 @@
     NVIDIA_AMPERE_A100e = "nvidia-ampere-a100e"
 
 
 class EmbeddingConfigType(str, Enum):
     BASE = "base"
     MODELS_API = "models_api"
 
+
+class UploadScheduleStatus(str, Enum):
+    HEALTHY = "HEALTHY"
+    UNHEALTHY = "UNHEALTHY"
+    ERROR = "ERROR"
+    PAUSED = "PAUSED"
```

### Comparing `scale_egp-1.0.5/scale_egp/sdk/models/fine_tuning_jobs.py` & `scale_egp-1.1.5/scale_egp/sdk/models/fine_tuning_jobs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/models/model_enums.py` & `scale_egp-1.1.5/scale_egp/sdk/models/model_enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/models/model_vendor_configuration.py` & `scale_egp-1.1.5/scale_egp/sdk/models/model_vendor_configuration.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/__init__.py` & `scale_egp-1.1.5/scale_egp/sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/agents.py` & `scale_egp-1.1.5/scale_egp/sdk/types/agents.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/application_specs.py` & `scale_egp-1.1.5/scale_egp/sdk/types/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/chunks.py` & `scale_egp-1.1.5/scale_egp/sdk/types/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/completions.py` & `scale_egp-1.1.5/scale_egp/sdk/types/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/embeddings.py` & `scale_egp-1.1.5/scale_egp/sdk/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/evaluation_configs.py` & `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py` & `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/evaluation_datasets.py` & `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/evaluation_test_case_results.py` & `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_test_case_results.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/evaluations.py` & `scale_egp-1.1.5/scale_egp/sdk/types/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/fine_tuning.py` & `scale_egp-1.1.5/scale_egp/sdk/types/fine_tuning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # !!!!! DO NOT EVER CHANGE THIS FILE MANUALLY -- AUTOGENERATED by orm2pydantic.py !!!!!
-# Generated on 2024-03-19 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
+# Generated on 2024-04-08 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
 # To regenerate this file, run:
 # scaleapi/packages/egp-api-backend/scripts/orm2pydantic.sh
 
 from scale_egp.utils.model_utils import BaseModel, Entity
 from pydantic import Field
 
 from datetime import (datetime)
@@ -12,42 +12,42 @@
 from scale_egp.utils.strenum_compat import (StrEnum)
 from typing import (Optional)
 DataSource = StrEnum('DataSource', [('S3', 'S3'), ('SHARE_POINT', 'SharePoint'), ('LOCAL_FILE', 'LocalFile'), ('LOCAL_CHUNKS', 'LocalChunks'), ('GOOGLE_DRIVE', 'GoogleDrive'), ('AZURE_BLOB_STORAGE', 'AzureBlobStorage')])
 class TrainingDatasetRequest(BaseModel):
     name: str = Field(..., description="The name of the dataset")
     schema_type: TrainingDatasetORMSchemaTypeEnum = Field(..., description="The schema type of the dataset, currently only GENERATION is supported")
     data_source: DataSource = Field(..., description="The data source of the dataset, used to determine how to parse the location")
-    account_id: str = Field(..., description="The ID of the account that owns the given entity.")
+    account_id: str = Field(..., description="The ID of the account that owns the given entity.", can_patch=False)
 
 
 class TrainingDataset(Entity):
     name: str = Field(..., description="The name of the dataset")
     schema_type: TrainingDatasetORMSchemaTypeEnum = Field(..., description="The schema type of the dataset, currently only GENERATION is supported")
     data_source: DataSource = Field(..., description="The data source of the dataset, used to determine how to parse the location")
     id: str = Field(..., description="The unique identifier of the entity.")
     created_at: datetime = Field(..., description="The date and time when the entity was created in ISO format.")
-    account_id: str = Field(..., description="The ID of the account that owns the given entity.")
+    account_id: str = Field(..., description="The ID of the account that owns the given entity.", can_patch=False)
     created_by_user_id: str = Field(..., description="The user who originally created the entity.")
 
 
 class FineTuningJobRequest(BaseModel):
     base_model_id: Optional[str] = Field(None)
     vendor_configuration: Optional[FineTuningJobVendorConfiguration] = Field(None)
     fine_tuned_model_id: Optional[str] = Field(None)
     training_dataset_id: str
     validation_dataset_id: Optional[str] = Field(None)
-    account_id: str = Field(..., description="The ID of the account that owns the given entity.")
+    account_id: str = Field(..., description="The ID of the account that owns the given entity.", can_patch=False)
 
 
 class FineTuningJob(Entity):
     base_model_id: Optional[str] = Field(None)
     vendor_configuration: Optional[FineTuningJobVendorConfiguration] = Field(None)
     fine_tuned_model_id: Optional[str] = Field(None)
     training_dataset_id: str
     validation_dataset_id: Optional[str] = Field(None)
     status: FineTuningJobStatus
     id: str = Field(..., description="The unique identifier of the entity.")
     created_at: datetime = Field(..., description="The date and time when the entity was created in ISO format.")
-    account_id: str = Field(..., description="The ID of the account that owns the given entity.")
+    account_id: str = Field(..., description="The ID of the account that owns the given entity.", can_patch=False)
     created_by_user_id: str = Field(..., description="The user who originally created the entity.")
```

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_artifacts.py` & `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_artifacts.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_chunks.py` & `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/knowledge_base_uploads.py` & `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_uploads.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from __future__ import annotations
 
+from datetime import datetime, timedelta
 from typing import Optional, Union, List, Literal, Dict, Any
 
 from pydantic import Field
 
-from scale_egp.sdk.enums import UploadJobStatus, DataSource, DeduplicationStrategy, ChunkingStrategy
+from scale_egp.sdk.enums import (
+    UploadJobStatus,
+    DataSource,
+    DeduplicationStrategy,
+    ChunkingStrategy,
+    UploadScheduleStatus,
+)
 from scale_egp.sdk.types.knowledge_base_artifacts import KnowledgeBaseArtifact
 from scale_egp.utils.model_utils import Entity, RootModel, BaseModel
 
 
 class KnowledgeBaseUploadResponse(BaseModel):
     upload_id: str = Field(..., description="ID of the created knowledge base upload job.")
 
@@ -117,19 +124,20 @@
     Attributes:
         source: The data source type. Must be 'GoogleDrive'.
         client_email: The service account's client email
         private_key: The service account's private_key
         token_uri: The service account's token_uri
         client_id: The service account's client_id
     """
+
     source: Literal[DataSource.GOOGLE_DRIVE] = DataSource.GOOGLE_DRIVE.value
-    client_email: Optional[str]
-    private_key: Optional[str]
-    token_uri: Optional[str]
-    client_id: Optional[str]
+    client_email: str
+    private_key: str
+    token_uri: str
+    client_id: str
 
 
 class SharePointDataSourceAuthConfig(BaseModel):
     """
     A data model representing the configuration of a SharePoint data source.
 
     Attributes:
@@ -146,16 +154,17 @@
     A data model representing the configuration of a S3 data source.
 
     Attributes:
         source: The data source type. Must be 'S3'.
         s3_role: Name of the role that a client will be initialized via AssumeRole of AWS sts
         external_id: External ID defined by the customer for the IAM role
     """
+
     source: Literal[DataSource.S3] = DataSource.S3.value
-    s3_role: str
+    s3_role: Optional[str]
     external_id: Optional[str]
 
     class Config(BaseModel.Config):
         title = "S3 DataSource Auth Config"
 
 
 class AzureBlobStorageDataSourceConfig(BaseModel):
@@ -211,14 +220,38 @@
 
     strategy: Literal[ChunkingStrategy.CHARACTER] = ChunkingStrategy.CHARACTER.value
     separator: Optional[str] = "\n\n"
     chunk_size: Optional[int] = 1000
     chunk_overlap: Optional[int] = 200
 
 
+class TokenChunkingStrategyConfig(BaseModel):
+    """
+    A data model representing the configuration of a token chunking strategy.
+
+    Attributes:
+        strategy: The chunking strategy type. Must be 'token'.
+        separator: Character designating breaks in input data. Text data will first be split
+            into sections by this separator, then each section will be split into chunks
+            of size `chunk_size`.
+        target_chunk_size: Target number of tokens in each chunk. If not specified, a target chunk
+            size of 200 will be used.
+        max_chunk_size: Maximum number of tokens in each chunk. If not specified, a maximum chunk
+            size of 200 will be used.
+        chunk_overlap: Number of tokens to overlap between chunks. If not specified, an overlap
+            of 0 will be used. Note this is only followed approximately.
+    """
+
+    strategy: Literal[ChunkingStrategy.TOKEN] = ChunkingStrategy.TOKEN.value
+    separator: Optional[str] = "\n\n"
+    target_chunk_size: Optional[int] = 200
+    max_chunk_size: Optional[int] = 600
+    chunk_overlap: Optional[int] = 0
+
+
 class ChunkToUpload(BaseModel):
     """
     A data model representing a local chunk.
 
     Attributes:
         text: The text associated with the chunk
         chunk_position: The position of the chunk in the artifact
@@ -234,26 +267,65 @@
     """
     A type alias for a Union of all data source types.
 
     Attributes:
         __root__: Instead of directly using this class, please use the appropriate data source type
             for your use case.
     """
+
     __root__: Union[
         S3DataSourceConfig,
         SharePointDataSourceConfig,
         GoogleDriveDataSourceConfig,
         AzureBlobStorageDataSourceConfig,
         LocalChunksSourceConfig,
     ] = Field(
         ...,
         discriminator="source",
     )
 
 
+class RemoteDataSourceConfig(RootModel):
+    """
+    A type alias for a Union of all remote data source types.
+
+    Attributes:
+        __root__: Instead of directly using this class, please use the appropriate data source type
+            for your use case.
+    """
+
+    __root__: Union[
+        S3DataSourceConfig,
+        SharePointDataSourceConfig,
+        GoogleDriveDataSourceConfig,
+        AzureBlobStorageDataSourceConfig,
+    ] = Field(
+        ...,
+        discriminator="source",
+    )
+
+
+class ChunkingStrategyConfig(RootModel):
+    """
+    A type alias for a Union of all chunking strategy types.
+
+    Attributes:
+        __root__: Instead of directly using this class, please use the appropriate chunking strategy
+            type for your use case.
+    """
+
+    __root__: Union[
+        CharacterChunkingStrategyConfig,
+        TokenChunkingStrategyConfig,
+    ] = Field(
+        ...,
+        discriminator="strategy",
+    )
+
+
 class KnowledgeBaseUpload(Entity):
     """
     A data model representing a knowledge base upload.
 
     Attributes:
         upload_id: Unique ID of the upload job
         data_source_config: Configuration for downloading data from source
@@ -264,35 +336,45 @@
         status_reason: Reason for the upload job's status
         artifacts_status: Number of artifacts pending, completed, and failed
         artifacts: List of info for each artifacts
     """
 
     upload_id: str
     data_source_config: DataSourceConfig
-    chunking_strategy_config: Optional[Union[CharacterChunkingStrategyConfig]]
+    chunking_strategy_config: Optional[ChunkingStrategyConfig]
     created_at: str
     updated_at: str
     status: UploadJobStatus
     status_reason: Optional[str] = None
     artifacts_status: Optional[ArtifactsStatus]
     artifacts: Optional[List[KnowledgeBaseArtifact]]
 
 
 class KnowledgeBaseRemoteUploadRequest(BaseModel):
     upload_type: Literal["remote"] = "remote"
-    data_source_config: DataSourceConfig
+    data_source_config: RemoteDataSourceConfig
     data_source_auth_config: Optional[DataSourceAuthConfig] = Field(
         None,
         description="Configuration for the data source which describes how to "
-                    "authenticate to the data source.",
+        "authenticate to the data source.",
+    )
+    chunking_strategy_config: ChunkingStrategyConfig = Field(
+        None,
+        description="Configuration for the chunking strategy which describes how to chunk the "
+        "data.",
     )
-    chunking_strategy_config: CharacterChunkingStrategyConfig = Field(
+
+
+class KnowledgeBaseDataSourceUploadRequest(BaseModel):
+    upload_type: Literal["data_source"] = "data_source"
+    data_source_id: str = Field(description="The ID of the data source to upload from.")
+    chunking_strategy_config: ChunkingStrategyConfig = Field(
         None,
         description="Configuration for the chunking strategy which describes how to chunk the "
-                    "data.",
+        "data.",
     )
 
 
 class ListKnowledgeBaseUploadsResponse(BaseModel):
     uploads: List[KnowledgeBaseUpload] = Field(..., description="List of knowledge base uploads.")
 
 
@@ -305,11 +387,72 @@
     chunks: List[ChunkToUpload] = Field(..., description="List of chunks.")
 
 
 class KnowledgeBaseUploadRequest(RootModel):
     __root__: Union[
         KnowledgeBaseRemoteUploadRequest,
         KnowledgeBaseLocalChunkUploadRequest,
+        KnowledgeBaseDataSourceUploadRequest,
     ] = Field(
         ...,
         discriminator="upload_type",
     )
+
+
+class KnowledgeBaseDataSourceRequest(BaseModel):
+    name: str = Field(..., description="A unique name for the data source.")
+    description: Optional[str] = Field(None, description="A description of the data source.")
+    data_source_config: RemoteDataSourceConfig
+    data_source_auth_config: Optional[DataSourceAuthConfig] = Field(
+        None,
+        description="Configuration for the data source which describes how to "
+        "authenticate to the data source.",
+    )
+    account_id: str = Field(..., description="The ID of the account that owns the data source.")
+
+
+class KnowledgeBaseDataSource(Entity):
+    id: str
+    name: str
+    description: Optional[str]
+    data_source_config: RemoteDataSourceConfig
+    created_at: datetime
+    updated_at: datetime
+    created_by_user_id: str
+    account_id: str
+
+
+class KnowledgeBaseUploadScheduleRequest(BaseModel):
+    knowledge_base_data_source_id: str = Field(
+        ..., description="The ID of the knowledge base data source to upload from."
+    )
+    chunking_strategy_config: ChunkingStrategyConfig = Field(
+        None,
+        description="Configuration for the chunking strategy which describes how to chunk the "
+        "data.",
+    )
+    interval: float = Field(
+        ..., description="The interval at which to run uploads from the data source."
+    )
+    next_run_at: Optional[str] = Field(
+        None, description="The time at which the next upload will run."
+    )
+    account_id: str = Field(..., description="The ID of the account that owns the upload schedule.")
+
+
+class KnowledgeBaseUploadSchedulePauseRequest(BaseModel):
+    next_run_at: None = None
+
+
+class KnowledgeBaseUploadSchedule(Entity):
+    id: str
+    knowledge_base_id: str
+    knowledge_base_data_source_id: str
+    chunking_strategy_config: ChunkingStrategyConfig
+    status: UploadScheduleStatus
+    status_reason: Optional[str]
+    interval: timedelta
+    next_run_at: Optional[datetime]
+    created_at: datetime
+    updated_at: datetime
+    created_by_user_id: str
+    account_id: str
```

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/knowledge_bases.py` & `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/memory_strategy.py` & `scale_egp-1.1.5/scale_egp/sdk/types/memory_strategy.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/message.py` & `scale_egp-1.1.5/scale_egp/sdk/types/message.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/model_templates.py` & `scale_egp-1.1.5/scale_egp/sdk/types/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/models.py` & `scale_egp-1.1.5/scale_egp/sdk/types/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/models_group.py` & `scale_egp-1.1.5/scale_egp/sdk/types/models_group.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/question_sets.py` & `scale_egp-1.1.5/scale_egp/sdk/types/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/sdk/types/questions.py` & `scale_egp-1.1.5/scale_egp/sdk/types/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/scale_egp/utils/api_utils.py` & `scale_egp-1.1.5/scale_egp/utils/api_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,23 +258,23 @@
             )
 
     @handle_api_exceptions
     def _raw_get(
         self,
         sub_path: str,
         timeout: Optional[int] = None,
-        query_params: Optional[Dict[str, str]] = None,
+        query_params: Optional[Dict[str, Union[str, List[str]]]] = None,
         additional_headers: Optional[Dict[str, str]] = None,
     ) -> Response:
         with self._httpx_client() as httpx_client:
             url = urljoin(self._api_client.endpoint_url, sub_path)
             self._log_curl_command(
                 client=httpx_client,
                 method="GET",
-                url=url if query_params is None else f"{url}?{urlencode(query_params)}",
+                url=url if query_params is None else f"{url}?{urlencode(query_params, doseq=True)}",
                 additional_headers=additional_headers,
             )
             response = httpx_client.get(
                 url,
                 params=query_params,
                 **self._universal_request_kwargs(
                     timeout=timeout,
```

### Comparing `scale_egp-1.0.5/scale_egp/utils/model_utils.py` & `scale_egp-1.1.5/scale_egp/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.0.5/PKG-INFO` & `scale_egp-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-egp
-Version: 1.0.5
+Version: 1.1.5
 Summary: SDK for Scale SGP API
 Home-page: https://scaleapi.github.io/sgp-py/
 License: Apache 2.0 modified with Commons Clause
 Author: Scale SGP team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

