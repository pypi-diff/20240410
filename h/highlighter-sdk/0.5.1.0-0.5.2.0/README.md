# Comparing `tmp/highlighter_sdk-0.5.1.0.tar.gz` & `tmp/highlighter_sdk-0.5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `highlighter_sdk-0.5.1.0.tar` & `highlighter_sdk-0.5.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/_colors.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/assessments.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/aws_s3.py
--rw-r--r--   0        0        0    10903 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/base_models.py
--rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/capabilities.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/const.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cropping.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/data_files.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/entity_avro_schema.py
--rw-r--r--   0        0        0    16291 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/gql_base.py
--rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/gql_client.py
--rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/io.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/itertools.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/labeled_uuid.py
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/logging.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/object_classes.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/pagination.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/presigned_url.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/shape_utils.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/tasks.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/training_config.py
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/training_runs.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/__init__.py
--rw-r--r--   0        0        0    11612 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/assessment.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/common.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/config.py
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/data_files.py
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/dataset.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/experiment.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/highlighter.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/object_class.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/step.py
--rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/task.py
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/cli/training_run.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/__init__.py
--rw-r--r--   0        0        0    10743 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/base_models.py
--rw-r--r--   0        0        0    38549 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/dataset.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/interfaces.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/__init__.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/writer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/__init__.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/common.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/reader.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/writer.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/__init__.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/reader.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/__init__.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/reader.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/writer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/splits/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/highlighter/splits/random_split.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/LICENSE
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/README.md
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/pyproject.toml
--rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 highlighter_sdk-0.5.1.0/PKG-INFO
+-rw-r--r--   0        0        0      592 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/__init__.py
+-rw-r--r--   0        0        0     2474 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/_colors.py
+-rw-r--r--   0        0        0     1412 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/assessments.py
+-rw-r--r--   0        0        0    11111 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/aws_s3.py
+-rw-r--r--   0        0        0    10903 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/base_models.py
+-rw-r--r--   0        0        0     8229 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/capabilities.py
+-rw-r--r--   0        0        0     1128 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/const.py
+-rw-r--r--   0        0        0     8431 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cropping.py
+-rw-r--r--   0        0        0     3260 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/data_files.py
+-rw-r--r--   0        0        0     3632 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/entity_avro_schema.py
+-rw-r--r--   0        0        0    16291 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/gql_base.py
+-rw-r--r--   0        0        0    14632 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/gql_client.py
+-rw-r--r--   0        0        0    13415 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/io.py
+-rw-r--r--   0        0        0      397 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/itertools.py
+-rw-r--r--   0        0        0     2938 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/labeled_uuid.py
+-rwxr-xr-x   0        0        0      400 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/logging.py
+-rw-r--r--   0        0        0     2154 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/object_classes.py
+-rw-r--r--   0        0        0     1712 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/pagination.py
+-rw-r--r--   0        0        0      973 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/presigned_url.py
+-rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/tasks.py
+-rw-r--r--   0        0        0    10450 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/training_config.py
+-rw-r--r--   0        0        0     9383 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/training_runs.py
+-rw-r--r--   0        0        0     1493 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/workflow.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/__init__.py
+-rw-r--r--   0        0        0    11031 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/assessment.py
+-rw-r--r--   0        0        0     1185 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/common.py
+-rw-r--r--   0        0        0     3689 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/config.py
+-rw-r--r--   0        0        0     9802 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/data_files.py
+-rw-r--r--   0        0        0     8187 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/dataset.py
+-rw-r--r--   0        0        0     1612 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/experiment.py
+-rw-r--r--   0        0        0     4038 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/highlighter.py
+-rw-r--r--   0        0        0     1109 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/object_class.py
+-rw-r--r--   0        0        0     1357 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/step.py
+-rw-r--r--   0        0        0    11701 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/task.py
+-rw-r--r--   0        0        0     7585 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/cli/training_run.py
+-rw-r--r--   0        0        0     2257 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/__init__.py
+-rw-r--r--   0        0        0    12340 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/base_models.py
+-rw-r--r--   0        0        0    39615 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/dataset.py
+-rw-r--r--   0        0        0      454 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/interfaces.py
+-rw-r--r--   0        0        0      847 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/aws_s3/__init__.py
+-rw-r--r--   0        0        0     4485 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/aws_s3/writer.py
+-rw-r--r--   0        0        0       62 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/__init__.py
+-rw-r--r--   0        0        0     5753 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/common.py
+-rw-r--r--   0        0        0     5426 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/reader.py
+-rw-r--r--   0        0        0    10120 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/writer.py
+-rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/highlighter/__init__.py
+-rw-r--r--   0        0        0     5605 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/highlighter/reader.py
+-rw-r--r--   0        0        0     6001 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/highlighter/writer.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/torch_image_folder/__init__.py
+-rw-r--r--   0        0        0     2863 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/torch_image_folder/reader.py
+-rw-r--r--   0        0        0     8947 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/datasets/formats/torch_image_folder/writer.py
+-rw-r--r--   0        0        0      186 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/splits/__init__.py
+-rw-r--r--   0        0        0      292 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/splits/base_splitter.py
+-rw-r--r--   0        0        0     2518 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/highlighter/splits/random_split.py
+-rw-r--r--   0        0        0       45 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/LICENSE
+-rw-r--r--   0        0        0     5323 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/README.md
+-rw-r--r--   0        0        0     3070 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6751 1980-01-01 00:00:00.000000 highlighter_sdk-0.5.2.0/PKG-INFO
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/__init__.py` & `highlighter_sdk-0.5.2.0/highlighter/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/_colors.py` & `highlighter_sdk-0.5.2.0/highlighter/_colors.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/assessments.py` & `highlighter_sdk-0.5.2.0/highlighter/assessments.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/aws_s3.py` & `highlighter_sdk-0.5.2.0/highlighter/aws_s3.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/base_models.py` & `highlighter_sdk-0.5.2.0/highlighter/base_models.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/capabilities.py` & `highlighter_sdk-0.5.2.0/highlighter/capabilities.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/const.py` & `highlighter_sdk-0.5.2.0/highlighter/const.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cropping.py` & `highlighter_sdk-0.5.2.0/highlighter/cropping.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/data_files.py` & `highlighter_sdk-0.5.2.0/highlighter/data_files.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/entity_avro_schema.py` & `highlighter_sdk-0.5.2.0/highlighter/entity_avro_schema.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/gql_base.py` & `highlighter_sdk-0.5.2.0/highlighter/gql_base.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/gql_client.py` & `highlighter_sdk-0.5.2.0/highlighter/gql_client.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/io.py` & `highlighter_sdk-0.5.2.0/highlighter/io.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/labeled_uuid.py` & `highlighter_sdk-0.5.2.0/highlighter/labeled_uuid.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/object_classes.py` & `highlighter_sdk-0.5.2.0/highlighter/object_classes.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/pagination.py` & `highlighter_sdk-0.5.2.0/highlighter/pagination.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/presigned_url.py` & `highlighter_sdk-0.5.2.0/highlighter/presigned_url.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/tasks.py` & `highlighter_sdk-0.5.2.0/highlighter/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import highlighter as hl
 from highlighter.base_models import SubmissionType
 
 __all__ = ["update_task_result"]
 
 class UpdateTaskResultPayload(BaseModel):
-    assessment: SubmissionType
+    submission: SubmissionType
     errors: List[Any]
 
 def update_task_result(client: hl.HLClient,
                        task_id: str,
                        status: str,
                        observations: List[Dict] = [],
                        background_info_layer_file_data: Optional[Dict]=None,
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/training_config.py` & `highlighter_sdk-0.5.2.0/highlighter/training_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-"""
-TODO remove this as it's now duplicated in sdk/python/training_config.py
-"""
-
 import json
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import yaml
-from pydantic import BaseModel, Extra, Field, confloat, validator
+from pydantic import BaseModel, Extra, Field, ValidationError, confloat, validator
 
 from highlighter import HLClient
 
 __all__ = [
     "get_training_config",
     "MetricType",
     "EntityAttributeValueTypeEnum",
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/training_runs.py` & `highlighter_sdk-0.5.2.0/highlighter/training_runs.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/workflow.py` & `highlighter_sdk-0.5.2.0/highlighter/workflow.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/assessment.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/assessment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import json
 from typing import Dict, List
 
 import click
 import fastavro as avro
 import yaml
 from pydantic import BaseModel
-from shapely.wkt import loads as wkt_loads
 
 from highlighter import ENTITY_AVRO_SCHEMA, SubmissionType
 from highlighter.aws_s3 import upload_file_to_s3
 from highlighter.base_models import PageInfo
-from highlighter.const import PIXEL_LOCATION_ATTRIBUTE_UUID
 from highlighter.datasets import Dataset
 from highlighter.datasets.formats.coco.reader import CocoReader
 from highlighter.datasets.formats.highlighter.writer import (
     CreateSubmissionPayload, HighlighterAssessmentsWriter)
 from highlighter.pagination import paginate
 from highlighter.assessments import (
     create_assessment_with_avro_file, get_latest_assessments_gen)
-from highlighter.shape_utils import polygon_to_multipolygon_if_self_intersecting
 
 
 ASSESSMENT_FIELDS = list(SubmissionType.__annotations__.keys())
 
 
 class AnnotationsAttributesParamType(click.ParamType):
     name = "dict"
@@ -251,15 +248,15 @@
     default=None,
     multiple=True,
 )
 @click.option(
     "--fix-invalid-polygons/--no-fix-invalid-polygons",
     type=bool,
     required=False,
-    help="Try to convert self-intersecting Polygons to MultiPolygon",
+    help="Try to convert self-intersecting Polygons to MultiPolygon from 'coco' dataset",
     default=False,
 )
 
 @click.pass_context
 def create_from_dataset(
     ctx, dataset_format, data_path, workflow_id, user_id, data_source_ids,
     fix_invalid_polygons,
@@ -273,19 +270,23 @@
     the Highlighter data_file_id to the original file path. We recommend this workflow
     in most cases.
     
     """
     client = ctx.obj["client"]
 
     if dataset_format == "hdf":
+        if fix_invalid_polygons:
+            click.echo("--fix-invalid-polygons only used for --dataset-format 'coco'. It has no effect when using 'hdf'")
         ds = Dataset.read_hdf(path=data_path)
     elif dataset_format == "json":
+        if fix_invalid_polygons:
+            click.echo("--fix-invalid-polygons only used for --dataset-format 'coco'. It has no effect when using 'json'")
         ds = Dataset.read_json(path=data_path)
     elif dataset_format == "coco":
-        reader = CocoReader(data_path)
+        reader = CocoReader(data_path, fix_invalid_polygons=fix_invalid_polygons)
         ds = Dataset.load_from_reader(reader)
     else:
         raise ValueError(f"Invalid dataset_format: {dataset_format}")
 
     # Get data_file ids in data_source
     class Image(BaseModel):
         id: int
@@ -309,32 +310,14 @@
             old_id: original_source_url_to_id[filename] for old_id, filename in old_id_filename
         }
         ds.data_files_df.loc[:, "data_file_id"] = ds.data_files_df.data_file_id.map(old_id_to_new_id)
         ds.annotations_df.loc[:, "data_file_id"] = ds.annotations_df.data_file_id.map(
             old_id_to_new_id
         )
 
-
-
-    def validate_polygons(wkt_str, fix_invalid_polygons=fix_invalid_polygons):
-        result = wkt_loads(wkt_str)
-        if (result.geom_type == "Polygon") and fix_invalid_polygons:
-            result = polygon_to_multipolygon_if_self_intersecting(result)
-
-        if not result.is_valid:
-            raise ValueError(f"Invalid pixel location shape: {result}. "
-                             "Possibly self-intersecting or un-closed Polygon. "
-                             "Try using --fix-invalid-polygons flag")
-        return result.wkt
-
-    adf = ds.annotations_df
-    validated_polys = adf[adf.attribute_id == PIXEL_LOCATION_ATTRIBUTE_UUID].value.apply(validate_polygons)
-    adf.loc[validated_polys.index, "value"] = validated_polys
-    ds.annotations_df = adf
-
     writer = HighlighterAssessmentsWriter(client, workflow_id, user_id=user_id)
     writer.write(ds)
 
 @assessment_group.command("create-from-avro")
 @click.option(
     "--avro-file",
     type=click.Path(dir_okay=False, exists=True),
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/common.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/common.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/config.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/config.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/data_files.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/data_files.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/dataset.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         help = (
             "Add assessments from existing dataset(s), see Note in help string "
             " for more context and a warrning."
             )
         )
 @click.option("--split-type",
         type=click.Choice(SUPPORTED_SPLIT_FNS.keys()), required=False,
-        default="random_split", show_default=True,
+        default="RandomSplitter", show_default=True,
         )
 @click.option("--split-seed",
         type=int, required=False, default=42,
         show_default=True,
         )
 @click.option("--split-frac",
         type=click.Tuple([str, float]), required=False, multiple=True,
@@ -169,25 +169,26 @@
                 ("Base Datasets", base_dataset_links_str)
                 )
 
 
 
     dataset = Dataset.combine(datasets)
 
-    split_fn = get_split_fn(split_type)
     split_names = [s[0] for s in split_frac]
     fracs = [s[1] for s in split_frac]
-    split_args = dict(
-            seed=split_seed,
-            fracs=fracs,
-            names=split_names,
-            )
-    dataset.apply_split(split_fn, split_args)
+    splitter = get_split_fn(split_type)(split_seed, fracs, split_names)
+
+    dataset.apply_split(splitter)
+
+    split_args = {"type": splitter.__class__.__name__,
+                  "seed": splitter.seed,
+                  "fracs": splitter.fracs,
+                  "names": splitter.names
+                  }
 
-    split_args["type"] = split_fn.__name__
     split_str = yaml.safe_dump(split_args)
     split_str = f"<pre>" + split_str + "</pre> \n"
 
     query_str = yaml.safe_dump(query_args)
     query_str = f"<pre>" + query_str + "</pre> \n"
 
     # List of tuples with e[0] being the heading and e[1]
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/experiment.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/highlighter.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/highlighter.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/object_class.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/object_class.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/step.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/step.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/task.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/task.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/cli/training_run.py` & `highlighter_sdk-0.5.2.0/highlighter/cli/training_run.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/__init__.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/dataset.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import tempfile
 import tarfile
 import zipfile
 import json
 import yaml
 from datetime import datetime
 from uuid import UUID
-from typing import Any, Optional, List, Dict, Tuple, Callable, Union
+from typing import Optional, List, Dict, Tuple, Union, Any
 from pathlib import Path
 import pandas as pd
 import numpy as np
 from pydantic import BaseModel
+from shapely.wkt import loads as wkt_loads
+from shapely.geometry.base import BaseGeometry as ShapelyShape
 from highlighter import HLClient, read_object_classes
 from highlighter.base_models import (
         DatasetSubmissionTypeConnection,
         )
 from highlighter.const import (
         OBJECT_CLASS_ATTRIBUTE_UUID,
         PIXEL_LOCATION_ATTRIBUTE_UUID,
@@ -389,17 +391,17 @@
 
         for dataset in datasets:
             self.data_files_df = self.data_files_df.append(dataset.data_files_df)
             self.annotations_df = self.annotations_df.append(dataset.annotations_df)
             self.cloud_files_info.extend(dataset.cloud_files_info)
 
 
-    def apply_split(self, split_fn: Callable, split_args: Dict):
+    def apply_split(self, dataset_splitter: "DatasetSplitter"):
         (self.data_files_df,
-         self.annotations_df) = split_fn(self, **split_args)
+         self.annotations_df) = dataset_splitter.split(self)
 
 
     def get_stats(self, split=None, uuid_to_name=None):
         stats_dict = dict(data_files=dict(), attributes=[])
 
         if split is not None:
             data_files_df = self.data_files_df[self.data_files_df.split == split]
@@ -808,17 +810,25 @@
         payload = {}
         if len(self.cloud_files_info) > 0:
             payload[CLOUD_FILES_INFO_KEY] = [c.dict() for c in self.cloud_files_info]
 
         payload[annotations_key] = self.annotations_df.to_dict("records")
         payload[data_files_key] = self.data_files_df.to_dict("records")
 
+        
+        class ShapelyGeometryEncoder(json.JSONEncoder):
+            def default(self, obj: Any) -> Any:
+                if isinstance(obj, ShapelyShape):
+                    return obj.wkt  # Convert BaseGeometry instances to WKT
+                # Let the base class default method raise the TypeError
+                return json.JSONEncoder.default(self, obj)
+
         path = Path(path)
         with path.open("w") as f:
-            json.dump(payload, f)
+            json.dump(payload, f, cls=ShapelyGeometryEncoder)
 
     @classmethod
     def read_data_file_folder(cls,
                           *,
                           path: Path,
                           attribute_id: str = str(OBJECT_CLASS_ATTRIBUTE_UUID),
                           attribute_name: str = OBJECT_CLASS_ATTRIBUTE_UUID.label,
@@ -860,16 +870,26 @@
         If you need to download accompanying data_files you can
         either use the generic `Dataset.read` classmethod or use
         `Dataset.download_dataset_files`
         """
         # Make sure path is a Path object
         path = Path(path)
 
+        class ShapelyGeometryDecoder(json.JSONDecoder):
+            def __init__(self, *args, **kwargs):
+                super().__init__(object_hook=self.dict_to_object, *args, **kwargs)
+                self.WKT_INDICATORS = ("POLYGON", "MULTIPOLYGON", "POINT", "LINESTRING")
+        
+            def dict_to_object(self, d: dict) -> dict:
+                if ("value" in d)  and isinstance(d["value"], str) and (d["value"].split(" ")[0] in self.WKT_INDICATORS):
+                    d["value"] = wkt_loads(d["value"])
+                return d
+
         with path.open("r") as f:
-            data = json.load(f)
+            data = json.load(f, cls=ShapelyGeometryDecoder)
 
         if annotations_key in data:
             attr_list = data[annotations_key]
         else:
             attr_list = data["attributes"]
 
         annotations_df = pd.DataFrame(attr_list)
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/__init__.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/aws_s3/writer.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/aws_s3/writer.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/common.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,36 +88,39 @@
     points = []
     for poly in multi_poly.geoms:
         points.append(
                 shapely_poly_to_segmentation(poly)[0],
                 )
     return points
 
-def wkt_to_segmentation(wkt_str):
-    """Convert WKT Polygon or MultiPolygon to
-    coco segmentation
-    ie:
-    [[xa0,ya0,xa1,ya1,xa2,ya2,xa3,ya3],
-     [xb0,yb0,xb1,yb1,xb2,yb2,xb3,yb3],
-     ...]
-
-    """
+def shapely_to_segmentation(shape):
     conversion_fns = {
             Polygon: shapely_poly_to_segmentation,
             MultiPolygon: shapely_multipoly_to_segmentation,
             }
-    shape = wkt.loads(wkt_str)
     to_segmentation = conversion_fns.get(type(shape), None)
     if to_segmentation is None:
         raise KeyError((
             f"Cannot convert shapely geometry '{type(shape)}' to segmentation."
         ))
     else:
         return to_segmentation(shape)
 
+def wkt_to_segmentation(wkt_str):
+    """Convert WKT Polygon or MultiPolygon to
+    coco segmentation
+    ie:
+    [[xa0,ya0,xa1,ya1,xa2,ya2,xa3,ya3],
+     [xb0,yb0,xb1,yb1,xb2,yb2,xb3,yb3],
+     ...]
+
+    """
+    shape = wkt.loads(wkt_str)
+    return shapely_to_segmentation(shape)
+
 def segmentation_to_wkt(seg: List[List[int]]):
     """Convert segmentation polygon [[x0, y0, x1, y1, ...],...] to a WKT string
     
     Top left is 0,0
     Positive x-axis is right
     Positive y-axis is down
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/reader.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,34 @@
 from uuid import uuid4
 from pathlib import Path
 from typing import List, Tuple, Union
 
 from highlighter.datasets.interfaces import IReader
 from highlighter.const import (
         OBJECT_CLASS_ATTRIBUTE_UUID,
-        PIXEL_LOCATION_ATTRIBUTE_UUID,
         )
 from highlighter.datasets.formats.coco.common import (
-        segmentation_to_wkt,
-        bbox_to_wkt,
         CocoKeys
         )
 
 from highlighter.datasets.base_models import (
         AttributeRecord,
         ImageRecord,
+        PixelLocationAttributeValue,
         )
 
 PathLike = Union[str, Path]
 
 class CocoReader(IReader):
     format_name = "coco"
 
     def __init__(self,
                  annotations_file: PathLike,
                  bbox_only: bool=False,
+                 fix_invalid_polygons: bool=False,
                  ):
         """Read a coco dataset from disk into highlighter DataFrame format
 
         By default, the coco reader will preference the segmentation label
         over the bbox label because we can always infer a bbox from a segmentation
         but not vice versa. You can optionally override this behavior by setting
         the bbox_only option to True. This can be useful if the segmentation labels
@@ -39,42 +38,52 @@
         Args:
           annotations_file: Where to save coco json
           bbox_only: Preference bbox label over segmentation
 
         """
         self.annotations_file = Path(annotations_file)
         self.bbox_only = bbox_only
+        self.fix_invalid_polygons = fix_invalid_polygons
 
     def read(self) -> Tuple[List[AttributeRecord], List[ImageRecord]]:
 
         with self.annotations_file.open("r") as f:
             coco_data = json.load(f)
 
         id_to_name = {ele.pop(CocoKeys.ID): ele for ele in coco_data[CocoKeys.CATS]}
         def get_category_name(cat_id):
             return id_to_name[cat_id][CocoKeys.NAME]
 
         def get_uuid():
             return str(uuid4())
 
-        def get_wkt_str(anno, bbox_only=self.bbox_only):
+        def get_pixel_location_attribute_value(anno, bbox_only=self.bbox_only):
             if bbox_only:
-                wkt = bbox_to_wkt(anno[CocoKeys.BBOX])
+                value = PixelLocationAttributeValue.from_left_top_width_height_coords(anno[CocoKeys.BBOX])
+
             elif CocoKeys.SEG in anno:
-                wkt = segmentation_to_wkt(anno[CocoKeys.SEG])
+
+                multi_poly_pts = []
+                for seg_xy_flat in anno[CocoKeys.SEG]:
+                    seg_xy_pts = [(x,y) for x, y in zip(seg_xy_flat[:-1:2], seg_xy_flat[1::2])]
+                    multi_poly_pts.append(seg_xy_pts)
+                value = PixelLocationAttributeValue.from_multpolygon_coords(multi_poly_pts, fix_invalid_polygons=self.fix_invalid_polygons)
+
             elif CocoKeys.BBOX in anno:
-                wkt = bbox_to_wkt(anno[CocoKeys.BBOX])
+                value = PixelLocationAttributeValue.from_left_top_width_height_coords(anno[CocoKeys.BBOX])
+
             else:
                 ValueError((
-                        f"Each coco annotation must have either a {SEG} or "
-                        f"{BBOX}, got: {anno}"
+                        f"Each coco annotation must have either a {CocoKeys.SEG} or "
+                        f"{CocoKeys.BBOX}, got: {anno}"
                         ))
-            return wkt
+            return value
 
         data_files = {ele.pop(CocoKeys.ID): ele for ele in coco_data[CocoKeys.IMAGES]}
+
         # Annotations can be polygons or masks. We just want the polygons.
         # https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocotools/coco.py#L255
         attribute_records = []
         data_file_records = []
         processed_data_file_ids = set()
         for anno in coco_data[CocoKeys.ANNOS]:
             # print(coco_data[CocoKeys.ANNOS])
@@ -102,20 +111,18 @@
                         attribute_id = str(OBJECT_CLASS_ATTRIBUTE_UUID),
                         attribute_name = OBJECT_CLASS_ATTRIBUTE_UUID.label,
                         value = get_category_name(anno[CocoKeys.CAT_ID])
                         )
                     )
 
             attribute_records.append(
-                    AttributeRecord(
-                        data_file_id=data_file_id,
+                    AttributeRecord.from_attribute_value(
+                        data_file_id,
+                        get_pixel_location_attribute_value(anno),
                         entity_id = entity_uuid,
-                        attribute_id = str(PIXEL_LOCATION_ATTRIBUTE_UUID),
-                        attribute_name = PIXEL_LOCATION_ATTRIBUTE_UUID.label,
-                        value = get_wkt_str(anno),
                         )
                     )
 
             for key, value in extra_fields.items():
                 attribute_records.append(
                         AttributeRecord(
                             data_file_id=data_file_id,
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/coco/writer.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/coco/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 import json
 from pathlib import Path
 from typing import Union, List, Dict, Optional
 
+from shapely import wkt
 from highlighter.datasets.formats.coco.common import (
     CocoAnnotationRecord,
     CocoImageRecord,
     CocoCategory,
-    wkt_to_segmentation,
+    shapely_to_segmentation,
     segmentation_to_bbox,
     get_bbox_area,
 )
 
 from highlighter.const import (
     OBJECT_CLASS_ATTRIBUTE_UUID,
     PIXEL_LOCATION_ATTRIBUTE_UUID,
         )
 from highlighter.datasets.interfaces import IWriter
 
 PathLike = Union[str, Path]
 
 def validate_categories(
-        categories: List[Union[Dict, CocoCategory]],
+        categories: List[CocoCategory],
         unique_object_classes,
         ):
-
-    def to_base_model(c):
-        if isinstance(c, dict):
-            return CocoCategory(**c)
-        return c
-    
-    # Ensure we're working with the CocoCategory BaseModel
-    categories = [to_base_model(c) for c in categories]
     
     # Validate no duplicate ids
     unique_ids = set([c.id for c in categories])
     if len(unique_ids) != len(categories):
         raise ValueError(
                 f"Got dupliate category ids in: {categories}"
                 )
@@ -49,31 +42,51 @@
     # Validate all unique_object_classes are accounted for in
     # categories
     category_names = [c.name for c in categories]
     if (
             (len(category_names) != len(unique_object_classes)) or \
             (len(set(category_names) - set(unique_object_classes)) > 0)
        ):
-        raise ValueError(
-                "categories dont match unique_object_classes, got: "
-                f"{category_names} and {unique_object_classes} respectivly")
+
+        diff_table = _tabulate_list_diff(sorted(category_names), sorted(unique_object_classes), "coco_categories", "hl dataset classes")
+        raise ValueError( f"categories dont match unique_object_classes, got: \n{diff_table}")
 
     return categories
 
 
+def _tabulate_list_diff(a, b, a_title, b_title):
+    """Create a readable diff for 2 lists
+
+    abc | abc
+    xyz | ---
+    --- | foo
+    bar | bar
+
+    """
+    ab = sorted(set(a+b))
+    left_cols = []
+    right_cols = []
+    for ele in ab:
+        left_cols.append(ele if ele in a else "-"*len(ele))
+        right_cols.append(ele if ele in b else "-"*len(ele))
+
+    table = [f"{a_title:<40} | {b_title}"]
+    table.extend([f"{l:40} | {r}" for l,r in zip(left_cols, right_cols)])
+    return "\n".join(table)
+
 class CocoWriter(IWriter):
 
     format_name = "coco"
     annotation_count = -1
     image_count = -1
     def __init__(
         self,
         annotations_dir: PathLike,
         category_attribute_id: str = OBJECT_CLASS_ATTRIBUTE_UUID,
-        categories: Optional[List[CocoCategory]] = None,
+        categories: Optional[List[Union[CocoCategory, Dict]]] = None,
     ):
         """Write annotations files.
 
         Args:
             annotations_dir: the dir to store the JSON file
             class_attribute_intentifier: value from the annotations_df.attribute_id  column select categories from
             categories: value from the annotations_df.values column to use as categories
@@ -98,15 +111,25 @@
             the we would create a coco dataset with the categories [a,c]
 
             If category_attribute_id="2" and categories=None
             the we would create a coco dataset with the categories [x,y]
         """
         self.annotations_dir = Path(annotations_dir)
         self.category_attribute_id = category_attribute_id
-        self.categories = categories
+    
+        def to_base_model(c):
+            if isinstance(c, dict):
+                return CocoCategory(**c)
+            return c
+        
+        # Ensure we're working with the CocoCategory BaseModel
+        if categories is None:
+            self.categories = None
+        else:
+            self.categories: List[CocoCategory] = [to_base_model(c) for c in categories]
 
 
     def write(
         self,
         dataset: "Dataset",
     ):
         self.annotations_dir.mkdir(parents=True, exist_ok=True)
@@ -184,15 +207,18 @@
                     f"entity: {entity_id}, No LOCATION"
                     ))
                     #"expected a location attribute for each entity "
                     #f"got: {grp}"))
                 return None
 
             location = location_attr["value"]
-            segmentation = wkt_to_segmentation(location)
+            if isinstance(location, str):
+                location = wkt.loads(location)
+
+            segmentation = shapely_to_segmentation(location)
             bbox = segmentation_to_bbox(segmentation)
             area = get_bbox_area(bbox)
 
             extra_fields = {attr_id: attr["value"] for attr_id, attr in data.items()}
             extra_fields["entity_id"] = str(entity_id)
             self.annotation_count += 1
             return CocoAnnotationRecord(
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/reader.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/highlighter/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import mimetypes
 from pathlib import Path
 from typing import List, Tuple
 from highlighter.datasets.interfaces import IReader
 from highlighter.datasets.base_models import (
         AttributeRecord,
         ImageRecord,
+        PixelLocationAttributeValue,
         )
 from highlighter.const import (
         OBJECT_CLASS_ATTRIBUTE_UUID,
         PIXEL_LOCATION_ATTRIBUTE_UUID,
         )
 from warnings import warn
 
@@ -108,21 +109,20 @@
                             attribute_id=str(OBJECT_CLASS_ATTRIBUTE_UUID),
                             attribute_name=OBJECT_CLASS_ATTRIBUTE_UUID.label,
                             value=object_class.uuid,
                             frame_id=annotation.frameId,
                             confidence=confidence,
                             )
                         )
+                
+                pixel_location_attribute_value = PixelLocationAttributeValue.from_wkt(annotation.location, confidence=confidence)
                 attribute_records.append(
-                        AttributeRecord(
-                            data_file_id=data_file_id,
+                        AttributeRecord.from_attribute_value(
+                            data_file_id,
+                            pixel_location_attribute_value,
                             entity_id=annotation.entityId,
-                            attribute_id=str(PIXEL_LOCATION_ATTRIBUTE_UUID),
-                            attribute_name=PIXEL_LOCATION_ATTRIBUTE_UUID.label,
-                            value=annotation.location,
                             frame_id=annotation.frameId,
-                            confidence=confidence,
                             )
                         )
 
         return data_file_records, attribute_records
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/highlighter/writer.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/highlighter/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 from tqdm import tqdm
 from datetime import datetime
 
 from pydantic import BaseModel, StrictBool, StrictFloat, StrictInt, StrictStr, validator, conlist
+from shapely.geometry.base import BaseGeometry
 
 from highlighter.base_models import ObjectClass, SubmissionType
 from highlighter.datasets.interfaces import IWriter
 from highlighter.gql_client import HLClient
 from highlighter.labeled_uuid import LabeledUUID
 
 tqdm.pandas()
@@ -121,14 +122,18 @@
                 if is_valid_uuid(attr_id):
                     # Cast/validate attribute value
                     value = attr["value"]
 
                     if isinstance(value, str):
                         value = str(self.object_class_uuid_lookup.get(value, value))
 
+                    # Is a shapely object
+                    if isinstance(value, BaseGeometry):
+                        value = value.wkt
+
                     eavt_attrs.append(
                         EAVTInputType(
                             entityId=entity_id,
                             attributeId=attr_id,
                             value=value,
                             datumSource=DatumSourceInputType(
                                 confidence=float(attr["confidence"])
```

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/reader.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/torch_image_folder/reader.py`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/highlighter/datasets/formats/torch_image_folder/writer.py` & `highlighter_sdk-0.5.2.0/highlighter/datasets/formats/torch_image_folder/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,15 @@
             warn(f"value not found for pixel location record '{grp.to_dict()}', skipping.")
             return None
 
         if "value" not in attr_record:
             warn(f"value not found for attr record '{grp.to_dict()}', skipping.")
             return None
 
-        wkt_str = pix_loc_record["value"]
-        poly: Union[gm.Polygon, gm.MultiPolygon] = wkt.loads(wkt_str)
+        poly: Union[gm.Polygon, gm.MultiPolygon] = pix_loc_record["value"]
         if not isinstance(poly, (gm.Polygon, gm.MultiPolygon)):
             warn(f"pixel location is not a Polygon {poly}, skipping")
             return None
 
         try:
             bbox = [(int(x), int(y)) for x, y in poly.envelope.exterior.coords]
         except AttributeError:
```

### Comparing `highlighter_sdk-0.5.1.0/LICENSE` & `highlighter_sdk-0.5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/README.md` & `highlighter_sdk-0.5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `highlighter_sdk-0.5.1.0/pyproject.toml` & `highlighter_sdk-0.5.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "highlighter-sdk"
-version =  "0.5.1.0"
+version =  "0.5.2.0"
 readme = "README.md"
 description = "Package to interact with the Highlighter Perception System"
 requires-python = ">=3.7,<4.0"
 
 # From pep 0639:
 # https://peps.python.org/pep-0639/#i-have-a-private-package-that-won-t-be-distributed
 license-files = { paths = ["LICENSE"] }
```

### Comparing `highlighter_sdk-0.5.1.0/PKG-INFO` & `highlighter_sdk-0.5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: highlighter-sdk
-Version: 0.5.1.0
+Version: 0.5.2.0
 Summary: Package to interact with the Highlighter Perception System
 Project-URL: Documentation, https://highlighter-docs.netlify.app/
 Author-email: Joshua Patterson <joshua.patterson@silverpond.com.au>, Jono Chang <jonathan.chang@silverpond.com.au>, Simon Hudson <simon.hudson@silverpond.com.au>
 License-File: LICENSE
 Keywords: enterprise perception system
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

