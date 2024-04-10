# Comparing `tmp/windmill_model-1.0.0.8-py3-none-any.whl.zip` & `tmp/windmill_model-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 8159 bytes, number of entries: 9
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-30 06:56 windmillmodelv1/__init__.py
--rw-r--r--  2.0 unx      213 b- defN 23-Aug-21 07:58 windmillmodelv1/client/__init__.py
--rw-r--r--  2.0 unx     3119 b- defN 24-Mar-28 13:38 windmillmodelv1/client/model_api_model.py
--rw-r--r--  2.0 unx      908 b- defN 24-Mar-24 10:26 windmillmodelv1/client/model_api_modelstore.py
--rw-r--r--  2.0 unx    20925 b- defN 24-Mar-30 06:53 windmillmodelv1/client/model_client.py
--rw-r--r--  2.0 unx      750 b- defN 24-Mar-30 06:56 windmill_model-1.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-30 06:56 windmill_model-1.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-30 06:56 windmill_model-1.0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      802 b- defN 24-Mar-30 06:56 windmill_model-1.0.0.8.dist-info/RECORD
-9 files, 27038 bytes uncompressed, 6753 bytes compressed:  75.0%
+Zip file size: 12036 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      213 b- defN 24-Mar-25 11:01 modelv1/__init__.py
+-rw-r--r--  2.0 unx     3119 b- defN 24-Mar-25 11:01 modelv1/model_api_model.py
+-rw-r--r--  2.0 unx      908 b- defN 24-Mar-25 11:01 modelv1/model_api_modelstore.py
+-rw-r--r--  2.0 unx    20921 b- defN 24-Apr-10 13:17 modelv1/model_client.py
+-rw-r--r--  2.0 unx      213 b- defN 23-Aug-30 08:26 modelv1/client/__init__.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Sep-25 07:03 modelv1/client/model_api_modelstore.py
+-rw-r--r--  2.0 unx    14790 b- defN 23-Sep-25 06:55 modelv1/client/model_client.py
+-rw-r--r--  2.0 unx     1717 b- defN 23-Aug-30 08:26 modelv1/client/paging.py
+-rw-r--r--  2.0 unx      750 b- defN 24-Apr-10 13:19 windmill_model-1.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 13:19 windmill_model-1.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-10 13:19 windmill_model-1.0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1003 b- defN 24-Apr-10 13:19 windmill_model-1.0.0.9.dist-info/RECORD
+12 files, 44037 bytes uncompressed, 10340 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
-Filename: windmillmodelv1/__init__.py
+Filename: modelv1/__init__.py
 Comment: 
 
-Filename: windmillmodelv1/client/__init__.py
+Filename: modelv1/model_api_model.py
 Comment: 
 
-Filename: windmillmodelv1/client/model_api_model.py
+Filename: modelv1/model_api_modelstore.py
 Comment: 
 
-Filename: windmillmodelv1/client/model_api_modelstore.py
+Filename: modelv1/model_client.py
 Comment: 
 
-Filename: windmillmodelv1/client/model_client.py
+Filename: modelv1/client/__init__.py
 Comment: 
 
-Filename: windmill_model-1.0.0.8.dist-info/METADATA
+Filename: modelv1/client/model_api_modelstore.py
 Comment: 
 
-Filename: windmill_model-1.0.0.8.dist-info/WHEEL
+Filename: modelv1/client/model_client.py
 Comment: 
 
-Filename: windmill_model-1.0.0.8.dist-info/top_level.txt
+Filename: modelv1/client/paging.py
 Comment: 
 
-Filename: windmill_model-1.0.0.8.dist-info/RECORD
+Filename: windmill_model-1.0.0.9.dist-info/METADATA
+Comment: 
+
+Filename: windmill_model-1.0.0.9.dist-info/WHEEL
+Comment: 
+
+Filename: windmill_model-1.0.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: windmill_model-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `windmillmodelv1/client/model_api_model.py` & `modelv1/model_api_model.py`

 * *Files identical despite different names*

## Comparing `windmillmodelv1/client/model_api_modelstore.py` & `modelv1/model_api_modelstore.py`

 * *Files identical despite different names*

## Comparing `windmillmodelv1/client/model_client.py` & `modelv1/model_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,17 +515,17 @@
                                           local_name=model_name.model_store_name)
         compute_client = ComputeClient(config=self.config)
         filesystem = compute_client.suggest_first_filesystem(model_name.workspace_id, model_store_name.get_name())
 
         # b. 遍历manifest_list result，下载模型文件
         apply_models = []
         ensemble = None
-        for item in manifest_list.result:
+        for item in manifest_list.subModels:
             new_local_name = None
-            if rename and item["objectName"] == model_name.get_name():
+            if rename and item["name"] == model_name.get_name():
                 new_local_name = rename
 
             self._dump_model(filesystem, item, location_style, new_local_name, output_uri)
 
             if match(item["category"], Category.CategoryImageEnsemble.value):
                 ensemble = {"kind": "Model", "metadata": item}
                 continue
@@ -547,15 +547,15 @@
         Returns
             apply_obj: apply object
         """
         # 1. 获取model dump列表文件
         if rename:
             output_uri = output_uri.rstrip("/") + "/" + rename
         else:
-            output_uri = output_uri.rstrip("/") + "/" + model["local_name"]
+            output_uri = output_uri.rstrip("/") + "/" + model["localName"]
 
         output_uri = get_location_path(output_uri, location_style, str(model["artifact"]["version"]))
         if not os.path.exists(output_uri):
             os.makedirs(output_uri)
 
         # 2. 下载模型文件
         download_by_filesystem(filesystem, model["artifact"]["uri"], output_uri)
```

## Comparing `windmill_model-1.0.0.8.dist-info/METADATA` & `windmill_model-1.0.0.9.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-model
-Version: 1.0.0.8
+Version: 1.0.0.9
 Summary: sdk in python for windmill model
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-model/tree/master
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

