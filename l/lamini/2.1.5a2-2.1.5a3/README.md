# Comparing `tmp/lamini-2.1.5a2-119-py3-none-any.whl.zip` & `tmp/lamini-2.1.5a3-119-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,52 @@
-Zip file size: 45886 bytes, number of entries: 41
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-09 20:32 lamini/__init__.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-09 20:25 lamini/api/classifier.py
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-09 20:25 lamini/api/embedding.py
--rw-r--r--  2.0 unx    12631 b- defN 24-Apr-09 20:25 lamini/api/lamini.py
--rw-r--r--  2.0 unx     2369 b- defN 24-Apr-09 20:25 lamini/api/lamini_config.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-09 20:25 lamini/api/precise_trainer.py
--rw-r--r--  2.0 unx     6208 b- defN 24-Apr-09 20:25 lamini/api/rest_requests.py
--rw-r--r--  2.0 unx     6732 b- defN 24-Apr-09 20:25 lamini/api/streaming_completion.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-09 20:25 lamini/api/synchronize.py
--rw-r--r--  2.0 unx     6617 b- defN 24-Apr-09 20:25 lamini/api/train.py
--rw-r--r--  2.0 unx     4605 b- defN 24-Apr-09 20:25 lamini/api/utils/async_inference_queue.py
--rw-r--r--  2.0 unx     5930 b- defN 24-Apr-09 20:25 lamini/api/utils/async_inference_queue_3_10.py
--rw-r--r--  2.0 unx     1494 b- defN 24-Apr-09 20:25 lamini/api/utils/base_async_inference_queue.py
--rw-r--r--  2.0 unx     1343 b- defN 24-Apr-09 20:25 lamini/api/utils/completion.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-09 20:25 lamini/api/utils/process_batch.py
--rw-r--r--  2.0 unx     5959 b- defN 24-Apr-09 20:25 lamini/api/utils/reservations.py
--rw-r--r--  2.0 unx      413 b- defN 24-Apr-09 20:25 lamini/api/utils/shutdown.py
--rw-r--r--  2.0 unx     1393 b- defN 24-Apr-09 20:25 lamini/api/utils/upload_client.py
--rw-r--r--  2.0 unx    23827 b- defN 24-Apr-09 20:25 lamini/classify/llama_classifier.py
--rw-r--r--  2.0 unx      896 b- defN 24-Apr-09 20:25 lamini/error/error.py
--rw-r--r--  2.0 unx     1273 b- defN 24-Apr-09 20:25 lamini/generation/base_generation_queue.py
--rw-r--r--  2.0 unx      594 b- defN 24-Apr-09 20:25 lamini/generation/base_node_object.py
--rw-r--r--  2.0 unx      797 b- defN 24-Apr-09 20:25 lamini/generation/base_prompt_object.py
--rw-r--r--  2.0 unx     1418 b- defN 24-Apr-09 20:25 lamini/generation/embedding_node.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-09 20:25 lamini/generation/generation_node.py
--rw-r--r--  2.0 unx     3868 b- defN 24-Apr-09 20:25 lamini/generation/generation_pipeline.py
--rw-r--r--  2.0 unx     6615 b- defN 24-Apr-09 20:25 lamini/generation/generation_queue_3_10.py
--rw-r--r--  2.0 unx      965 b- defN 24-Apr-09 20:25 lamini/generation/modify_node.py
--rw-r--r--  2.0 unx     3448 b- defN 24-Apr-09 20:25 lamini/generation/process_generation_batch.py
--rw-r--r--  2.0 unx     1390 b- defN 24-Apr-09 20:25 lamini/generation/split_response_node.py
--rw-r--r--  2.0 unx      557 b- defN 24-Apr-09 20:25 lamini/generation/token_optimizer.py
--rw-r--r--  2.0 unx     9354 b- defN 24-Apr-09 20:25 lamini/runners/base_runner.py
--rw-r--r--  2.0 unx      720 b- defN 24-Apr-09 20:25 lamini/runners/basic_model_runner.py
--rw-r--r--  2.0 unx     3062 b- defN 24-Apr-09 20:25 lamini/runners/llama_v2_runner.py
--rw-r--r--  2.0 unx     2625 b- defN 24-Apr-09 20:25 lamini/runners/mistral_runner.py
--rw-r--r--  2.0 unx       21 b- defN 24-Apr-09 20:25 llama/__init__.py
--rw-r--r--  2.0 unx    11340 b- defN 24-Apr-09 20:32 lamini-2.1.5a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1507 b- defN 24-Apr-09 20:32 lamini-2.1.5a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 20:32 lamini-2.1.5a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 20:32 lamini-2.1.5a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-09 20:32 lamini-2.1.5a2.dist-info/RECORD
-41 files, 150447 bytes uncompressed, 40096 bytes compressed:  73.3%
+Zip file size: 60326 bytes, number of entries: 50
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-09 22:00 lamini/__init__.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-Apr-09 21:57 lamini/api/classifier.py
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-09 21:57 lamini/api/embedding.py
+-rw-r--r--  2.0 unx    12631 b- defN 24-Apr-09 21:57 lamini/api/lamini.py
+-rw-r--r--  2.0 unx     2369 b- defN 24-Apr-09 21:57 lamini/api/lamini_config.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Apr-09 21:57 lamini/api/precise_trainer.py
+-rw-r--r--  2.0 unx     6208 b- defN 24-Apr-09 21:57 lamini/api/rest_requests.py
+-rw-r--r--  2.0 unx     6732 b- defN 24-Apr-09 21:57 lamini/api/streaming_completion.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Apr-09 21:57 lamini/api/synchronize.py
+-rw-r--r--  2.0 unx     6617 b- defN 24-Apr-09 21:57 lamini/api/train.py
+-rw-r--r--  2.0 unx     4605 b- defN 24-Apr-09 21:57 lamini/api/utils/async_inference_queue.py
+-rw-r--r--  2.0 unx     5930 b- defN 24-Apr-09 21:57 lamini/api/utils/async_inference_queue_3_10.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-Apr-09 21:57 lamini/api/utils/base_async_inference_queue.py
+-rw-r--r--  2.0 unx     1343 b- defN 24-Apr-09 21:57 lamini/api/utils/completion.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Apr-09 21:57 lamini/api/utils/process_batch.py
+-rw-r--r--  2.0 unx     5959 b- defN 24-Apr-09 21:57 lamini/api/utils/reservations.py
+-rw-r--r--  2.0 unx      413 b- defN 24-Apr-09 21:57 lamini/api/utils/shutdown.py
+-rw-r--r--  2.0 unx     1393 b- defN 24-Apr-09 21:57 lamini/api/utils/upload_client.py
+-rw-r--r--  2.0 unx    23827 b- defN 24-Apr-09 21:57 lamini/classify/llama_classifier.py
+-rw-r--r--  2.0 unx      896 b- defN 24-Apr-09 21:57 lamini/error/error.py
+-rw-r--r--  2.0 unx     2967 b- defN 24-Apr-09 21:57 lamini/evaluators/benchmark.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Apr-09 21:57 lamini/evaluators/custom/custom_evaluator.py
+-rw-r--r--  2.0 unx     9787 b- defN 24-Apr-09 21:57 lamini/evaluators/custom/earnings_call_evaluator.py
+-rw-r--r--  2.0 unx     9886 b- defN 24-Apr-09 21:57 lamini/evaluators/custom/ecommerce_evaluator.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-09 21:57 lamini/evaluators/custom/icd_evaluator.py
+-rw-r--r--  2.0 unx     5360 b- defN 24-Apr-09 21:57 lamini/evaluators/helm/harness_evaluator.py
+-rw-r--r--  2.0 unx      775 b- defN 24-Apr-09 21:57 lamini/evaluators/helm/mmlu_evaluator.py
+-rw-r--r--  2.0 unx      861 b- defN 24-Apr-09 21:57 lamini/evaluators/helm/truthfulqa_evaluator.py
+-rw-r--r--  2.0 unx     2441 b- defN 24-Apr-09 21:57 lamini/evaluators/utils/utils.py
+-rw-r--r--  2.0 unx     1273 b- defN 24-Apr-09 21:57 lamini/generation/base_generation_queue.py
+-rw-r--r--  2.0 unx      594 b- defN 24-Apr-09 21:57 lamini/generation/base_node_object.py
+-rw-r--r--  2.0 unx      797 b- defN 24-Apr-09 21:57 lamini/generation/base_prompt_object.py
+-rw-r--r--  2.0 unx     1418 b- defN 24-Apr-09 21:57 lamini/generation/embedding_node.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Apr-09 21:57 lamini/generation/generation_node.py
+-rw-r--r--  2.0 unx     3868 b- defN 24-Apr-09 21:57 lamini/generation/generation_pipeline.py
+-rw-r--r--  2.0 unx     6615 b- defN 24-Apr-09 21:57 lamini/generation/generation_queue_3_10.py
+-rw-r--r--  2.0 unx      965 b- defN 24-Apr-09 21:57 lamini/generation/modify_node.py
+-rw-r--r--  2.0 unx     3448 b- defN 24-Apr-09 21:57 lamini/generation/process_generation_batch.py
+-rw-r--r--  2.0 unx     1390 b- defN 24-Apr-09 21:57 lamini/generation/split_response_node.py
+-rw-r--r--  2.0 unx      557 b- defN 24-Apr-09 21:57 lamini/generation/token_optimizer.py
+-rw-r--r--  2.0 unx     9354 b- defN 24-Apr-09 21:57 lamini/runners/base_runner.py
+-rw-r--r--  2.0 unx      720 b- defN 24-Apr-09 21:57 lamini/runners/basic_model_runner.py
+-rw-r--r--  2.0 unx     3062 b- defN 24-Apr-09 21:57 lamini/runners/llama_v2_runner.py
+-rw-r--r--  2.0 unx     2625 b- defN 24-Apr-09 21:57 lamini/runners/mistral_runner.py
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-09 21:57 llama/__init__.py
+-rw-r--r--  2.0 unx    11340 b- defN 24-Apr-09 22:00 lamini-2.1.5a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-09 22:00 lamini-2.1.5a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 22:00 lamini-2.1.5a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 22:00 lamini-2.1.5a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4484 b- defN 24-Apr-09 22:00 lamini-2.1.5a3.dist-info/RECORD
+50 files, 195543 bytes uncompressed, 53104 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -54,14 +54,41 @@
 
 Filename: lamini/classify/llama_classifier.py
 Comment: 
 
 Filename: lamini/error/error.py
 Comment: 
 
+Filename: lamini/evaluators/benchmark.py
+Comment: 
+
+Filename: lamini/evaluators/custom/custom_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/custom/earnings_call_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/custom/ecommerce_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/custom/icd_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/helm/harness_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/helm/mmlu_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/helm/truthfulqa_evaluator.py
+Comment: 
+
+Filename: lamini/evaluators/utils/utils.py
+Comment: 
+
 Filename: lamini/generation/base_generation_queue.py
 Comment: 
 
 Filename: lamini/generation/base_node_object.py
 Comment: 
 
 Filename: lamini/generation/base_prompt_object.py
@@ -102,23 +129,23 @@
 
 Filename: lamini/runners/mistral_runner.py
 Comment: 
 
 Filename: llama/__init__.py
 Comment: 
 
-Filename: lamini-2.1.5a2.dist-info/LICENSE
+Filename: lamini-2.1.5a3.dist-info/LICENSE
 Comment: 
 
-Filename: lamini-2.1.5a2.dist-info/METADATA
+Filename: lamini-2.1.5a3.dist-info/METADATA
 Comment: 
 
-Filename: lamini-2.1.5a2.dist-info/WHEEL
+Filename: lamini-2.1.5a3.dist-info/WHEEL
 Comment: 
 
-Filename: lamini-2.1.5a2.dist-info/top_level.txt
+Filename: lamini-2.1.5a3.dist-info/top_level.txt
 Comment: 
 
-Filename: lamini-2.1.5a2.dist-info/RECORD
+Filename: lamini-2.1.5a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lamini-2.1.5a2.dist-info/LICENSE` & `lamini-2.1.5a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lamini-2.1.5a2.dist-info/METADATA` & `lamini-2.1.5a3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamini
-Version: 2.1.5a2
+Version: 2.1.5a3
 Summary: Build on large language models faster
 Author-email: PowerML <info@powerml.co>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `lamini-2.1.5a2.dist-info/RECORD` & `lamini-2.1.5a3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 lamini/api/utils/completion.py,sha256=37vn81fvpGR7HMuGQy1Cwz2ozIj0aZQTcxHzXl-cVpI,1343
 lamini/api/utils/process_batch.py,sha256=nNWu80NSeYig_MoO1GQs_JOiJMQgpts0F5Y-xQMDmG8,2865
 lamini/api/utils/reservations.py,sha256=yXnGPM1eQXgzRdQ1rjtoHMSxn4DhDPetxJfPl5221_4,5959
 lamini/api/utils/shutdown.py,sha256=oznFdh3JsE3CDH4Fx30c8_pVGBlIF0iPlFCFpoTE4iU,413
 lamini/api/utils/upload_client.py,sha256=n4VpSgg5n17NUr6PL7eT_aQESPz7GyrJb3x9jG-o1Kw,1393
 lamini/classify/llama_classifier.py,sha256=SrSCAf5tTiDyhRVzt9kn4lFqEC_A7Caq0lSrOB2SU08,23827
 lamini/error/error.py,sha256=C4SbfG3obNYGH8onkUkhUc61XRTwejCBlsG1QBNaEQI,896
+lamini/evaluators/benchmark.py,sha256=afndsoRYktnDSwsG5QdO6H6wZ5gSxwAfQAyr_hh06I8,2967
+lamini/evaluators/custom/custom_evaluator.py,sha256=yxACuA9wLzAp3zxMVRXhkSZABxwZOUnkyrqv0NIHzUM,2897
+lamini/evaluators/custom/earnings_call_evaluator.py,sha256=HxRnYicgnClwyoVv8coM5RpxrxDrEFI0S48AL6wXHX0,9787
+lamini/evaluators/custom/ecommerce_evaluator.py,sha256=2j6qMYK3XMZZLTlO6cBkdy3euho6E4ilmVMJfezmxXY,9886
+lamini/evaluators/custom/icd_evaluator.py,sha256=wCV2eWtn4jG3EdAs6OPBkkwA2z5y8sK0NCLFcdN4Ro8,9237
+lamini/evaluators/helm/harness_evaluator.py,sha256=oL-ecnfW4CtTH23OBkG6w1rGdZ7Fk70iKzwkuVZt_9M,5360
+lamini/evaluators/helm/mmlu_evaluator.py,sha256=TxsRjePTOd87LrpX9L2zC8EgEL7piNRKoHTtFlJ5Hj8,775
+lamini/evaluators/helm/truthfulqa_evaluator.py,sha256=xS8hpoKudf3K99eaEnbM5EShB_QTDOPffhFEOYntGww,861
+lamini/evaluators/utils/utils.py,sha256=DRevBVPgYChc46r3vpA_FXzfTFO0S976MI6mfyjpaic,2441
 lamini/generation/base_generation_queue.py,sha256=D_gav4v76N9Oo2r0dWYNuho2A8nKdr0Q-0xMjZMmyPk,1273
 lamini/generation/base_node_object.py,sha256=Q_t8eqCnf5HnLOHQTMpFaIq-_I2_YhXUhi64FeRF5-M,594
 lamini/generation/base_prompt_object.py,sha256=nC5VTLoiNzYoQquA2nPeqAvWY_zeSJlDtQnb5iuutSk,797
 lamini/generation/embedding_node.py,sha256=Iq2PlnI6yMTpwxG67w07029VDp_aJjKNbHhAgN4utnk,1418
 lamini/generation/generation_node.py,sha256=62X4Bm_qcdPd0J4Z6AyYWDOMNeiQgkT8EpIs77BZaWQ,5101
 lamini/generation/generation_pipeline.py,sha256=jbBYbVV4w8Tmrdzo84c-0GpSfM9a_ZIqJ6yqiXyWvks,3868
 lamini/generation/generation_queue_3_10.py,sha256=sm33jtLqN7HpIhWvJYX6v9pNPq3IXLWlYv068dOFK-k,6615
@@ -30,12 +39,12 @@
 lamini/generation/split_response_node.py,sha256=sZJaPj_4mdf-m-c4CAQ22O6nzA53fsHKzI5P7Irw7Do,1390
 lamini/generation/token_optimizer.py,sha256=LI7-APb8XM_Jg1WNL2DuQV4NcoY3y1FL-B3KlDPNe0E,557
 lamini/runners/base_runner.py,sha256=VYPlMdx2sR9BLXrO_jsyp-p0_3IQUXwPkVta8g6xFPE,9354
 lamini/runners/basic_model_runner.py,sha256=7e4xTotKGdmC0PH-ynAlOtXxHDvhH8HInqWCggG5DOA,720
 lamini/runners/llama_v2_runner.py,sha256=T2OjiJTC0goNpZebD1iKOKkuL5aAjfdrTvxss-d5ezM,3062
 lamini/runners/mistral_runner.py,sha256=uHS2ptK01JMGnvSi4zH6bcWquuZYjc3eIFgzWnFeg1Q,2625
 llama/__init__.py,sha256=E77xncFEWyRrg-MsjkiLrCkNJBIYIxr111hLd7WpgjY,21
-lamini-2.1.5a2.dist-info/LICENSE,sha256=-alRIf0b5B1SavU0njHUTAanPUn6GHxH9a2Q_ACz1HM,11340
-lamini-2.1.5a2.dist-info/METADATA,sha256=BbIkzpMauz9gZjrv1N6l7ckJBhV2Zu3p2we9lH4aaxs,1507
-lamini-2.1.5a2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lamini-2.1.5a2.dist-info/top_level.txt,sha256=5h0-n2aeXxQUxmNPPJ0AnsKIBAZV_qWqU0JIpA6Q2zo,13
-lamini-2.1.5a2.dist-info/RECORD,,
+lamini-2.1.5a3.dist-info/LICENSE,sha256=-alRIf0b5B1SavU0njHUTAanPUn6GHxH9a2Q_ACz1HM,11340
+lamini-2.1.5a3.dist-info/METADATA,sha256=sBkvDHFHiNJUEwOOxoFoMCXlr_f6W8UPHdwOPiFfMwQ,1507
+lamini-2.1.5a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lamini-2.1.5a3.dist-info/top_level.txt,sha256=5h0-n2aeXxQUxmNPPJ0AnsKIBAZV_qWqU0JIpA6Q2zo,13
+lamini-2.1.5a3.dist-info/RECORD,,
```

