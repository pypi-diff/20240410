# Comparing `tmp/alibabacloud_cloudauth20190307-2.4.0.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.4.0.tar", last modified: Wed Mar 13 03:09:06 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.5.0.tar", last modified: Wed Apr 10 17:14:47 2024, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.4.0.tar` & `alibabacloud_cloudauth20190307-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2449 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97165 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   157589 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2449 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2838 2024-03-13 03:09:06.000000 alibabacloud_cloudauth20190307-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   113253 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   186651 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-04-10 17:14:47.000000 alibabacloud_cloudauth20190307-2.5.0/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/ChangeLog.md` & `alibabacloud_cloudauth20190307-2.5.0/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-13 Version: 2.4.0
+- Support API AIGCFaceVerify.
+
+
 2024-02-22 Version: 2.3.0
 - Support API AIGCFaceVerify.
 
 
 2024-01-23 Version: 2.2.2
 - Update Tea.
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/LICENSE` & `alibabacloud_cloudauth20190307-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.4.0/PKG-INFO` & `alibabacloud_cloudauth20190307-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.4.0
+Version: 2.5.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/README-CN.md` & `alibabacloud_cloudauth20190307-2.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.4.0/README.md` & `alibabacloud_cloudauth20190307-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,14 +141,108 @@
     async def a_igcface_verify_async(
         self,
         request: cloudauth_20190307_models.AIGCFaceVerifyRequest,
     ) -> cloudauth_20190307_models.AIGCFaceVerifyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.a_igcface_verify_with_options_async(request, runtime)
 
+    def bank_meta_verify_with_options(
+        self,
+        request: cloudauth_20190307_models.BankMetaVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.bank_card):
+            query['BankCard'] = request.bank_card
+        if not UtilClient.is_unset(request.identify_num):
+            query['IdentifyNum'] = request.identify_num
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        if not UtilClient.is_unset(request.product_type):
+            query['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
+        if not UtilClient.is_unset(request.verify_mode):
+            query['VerifyMode'] = request.verify_mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BankMetaVerify',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.BankMetaVerifyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def bank_meta_verify_with_options_async(
+        self,
+        request: cloudauth_20190307_models.BankMetaVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.bank_card):
+            query['BankCard'] = request.bank_card
+        if not UtilClient.is_unset(request.identify_num):
+            query['IdentifyNum'] = request.identify_num
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        if not UtilClient.is_unset(request.product_type):
+            query['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
+        if not UtilClient.is_unset(request.verify_mode):
+            query['VerifyMode'] = request.verify_mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='BankMetaVerify',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.BankMetaVerifyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def bank_meta_verify(
+        self,
+        request: cloudauth_20190307_models.BankMetaVerifyRequest,
+    ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.bank_meta_verify_with_options(request, runtime)
+
+    async def bank_meta_verify_async(
+        self,
+        request: cloudauth_20190307_models.BankMetaVerifyRequest,
+    ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.bank_meta_verify_with_options_async(request, runtime)
+
     def compare_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.CompareFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CompareFaceVerifyResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1027,14 +1121,104 @@
         runtime = util_models.RuntimeOptions()
         return self.describe_oss_upload_token_with_options(runtime)
 
     async def describe_oss_upload_token_async(self) -> cloudauth_20190307_models.DescribeOssUploadTokenResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_oss_upload_token_with_options_async(runtime)
 
+    def describe_page_face_verify_data_with_options(
+        self,
+        request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.end_date):
+            query['EndDate'] = request.end_date
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.product_code):
+            query['ProductCode'] = request.product_code
+        if not UtilClient.is_unset(request.scene_id):
+            query['SceneId'] = request.scene_id
+        if not UtilClient.is_unset(request.start_date):
+            query['StartDate'] = request.start_date
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePageFaceVerifyData',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.DescribePageFaceVerifyDataResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_page_face_verify_data_with_options_async(
+        self,
+        request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.end_date):
+            query['EndDate'] = request.end_date
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.product_code):
+            query['ProductCode'] = request.product_code
+        if not UtilClient.is_unset(request.scene_id):
+            query['SceneId'] = request.scene_id
+        if not UtilClient.is_unset(request.start_date):
+            query['StartDate'] = request.start_date
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePageFaceVerifyData',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.DescribePageFaceVerifyDataResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_page_face_verify_data(
+        self,
+        request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
+    ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_page_face_verify_data_with_options(request, runtime)
+
+    async def describe_page_face_verify_data_async(
+        self,
+        request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
+    ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_page_face_verify_data_with_options_async(request, runtime)
+
     def describe_smart_statistics_page_list_with_options(
         self,
         request: cloudauth_20190307_models.DescribeSmartStatisticsPageListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeSmartStatisticsPageListResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2031,14 +2215,236 @@
     async def mobile_3meta_simple_verify_async(
         self,
         request: cloudauth_20190307_models.Mobile3MetaSimpleVerifyRequest,
     ) -> cloudauth_20190307_models.Mobile3MetaSimpleVerifyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.mobile_3meta_simple_verify_with_options_async(request, runtime)
 
+    def mobile_detect_with_options(
+        self,
+        request: cloudauth_20190307_models.MobileDetectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileDetectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobiles):
+            query['Mobiles'] = request.mobiles
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileDetect',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileDetectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def mobile_detect_with_options_async(
+        self,
+        request: cloudauth_20190307_models.MobileDetectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileDetectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobiles):
+            query['Mobiles'] = request.mobiles
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileDetect',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileDetectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def mobile_detect(
+        self,
+        request: cloudauth_20190307_models.MobileDetectRequest,
+    ) -> cloudauth_20190307_models.MobileDetectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_detect_with_options(request, runtime)
+
+    async def mobile_detect_async(
+        self,
+        request: cloudauth_20190307_models.MobileDetectRequest,
+    ) -> cloudauth_20190307_models.MobileDetectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.mobile_detect_with_options_async(request, runtime)
+
+    def mobile_online_status_with_options(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileOnlineStatus',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileOnlineStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def mobile_online_status_with_options_async(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileOnlineStatus',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileOnlineStatusResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def mobile_online_status(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineStatusRequest,
+    ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_online_status_with_options(request, runtime)
+
+    async def mobile_online_status_async(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineStatusRequest,
+    ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.mobile_online_status_with_options_async(request, runtime)
+
+    def mobile_online_time_with_options(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineTimeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileOnlineTime',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileOnlineTimeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def mobile_online_time_with_options_async(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineTimeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.param_type):
+            query['ParamType'] = request.param_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MobileOnlineTime',
+            version='2019-03-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudauth_20190307_models.MobileOnlineTimeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def mobile_online_time(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineTimeRequest,
+    ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_online_time_with_options(request, runtime)
+
+    async def mobile_online_time_async(
+        self,
+        request: cloudauth_20190307_models.MobileOnlineTimeRequest,
+    ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.mobile_online_time_with_options_async(request, runtime)
+
     def modify_device_info_with_options(
         self,
         request: cloudauth_20190307_models.ModifyDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ModifyDeviceInfoResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,198 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AIGCFaceVerifyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BankMetaVerifyRequest(TeaModel):
+    def __init__(
+        self,
+        bank_card: str = None,
+        identify_num: str = None,
+        mobile: str = None,
+        param_type: str = None,
+        product_type: str = None,
+        user_name: str = None,
+        verify_mode: str = None,
+    ):
+        self.bank_card = bank_card
+        self.identify_num = identify_num
+        self.mobile = mobile
+        self.param_type = param_type
+        self.product_type = product_type
+        self.user_name = user_name
+        self.verify_mode = verify_mode
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.bank_card is not None:
+            result['BankCard'] = self.bank_card
+        if self.identify_num is not None:
+            result['IdentifyNum'] = self.identify_num
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.param_type is not None:
+            result['ParamType'] = self.param_type
+        if self.product_type is not None:
+            result['ProductType'] = self.product_type
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.verify_mode is not None:
+            result['VerifyMode'] = self.verify_mode
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BankCard') is not None:
+            self.bank_card = m.get('BankCard')
+        if m.get('IdentifyNum') is not None:
+            self.identify_num = m.get('IdentifyNum')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        if m.get('ProductType') is not None:
+            self.product_type = m.get('ProductType')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('VerifyMode') is not None:
+            self.verify_mode = m.get('VerifyMode')
+        return self
+
+
+class BankMetaVerifyResponseBodyResultObject(TeaModel):
+    def __init__(
+        self,
+        biz_code: str = None,
+        sub_code: str = None,
+    ):
+        self.biz_code = biz_code
+        self.sub_code = sub_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_code is not None:
+            result['BizCode'] = self.biz_code
+        if self.sub_code is not None:
+            result['SubCode'] = self.sub_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizCode') is not None:
+            self.biz_code = m.get('BizCode')
+        if m.get('SubCode') is not None:
+            self.sub_code = m.get('SubCode')
+        return self
+
+
+class BankMetaVerifyResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result_object: BankMetaVerifyResponseBodyResultObject = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result_object = result_object
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_object is not None:
+            result['ResultObject'] = self.result_object.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultObject') is not None:
+            temp_model = BankMetaVerifyResponseBodyResultObject()
+            self.result_object = temp_model.from_map(m['ResultObject'])
+        return self
+
+
+class BankMetaVerifyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BankMetaVerifyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BankMetaVerifyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CompareFaceVerifyRequest(TeaModel):
     def __init__(
         self,
         crop: str = None,
         outer_order_no: str = None,
         product_code: str = None,
         scene_id: int = None,
@@ -1849,14 +2033,252 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeOssUploadTokenResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePageFaceVerifyDataRequest(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        end_date: str = None,
+        page_size: int = None,
+        product_code: str = None,
+        scene_id: int = None,
+        start_date: str = None,
+    ):
+        self.current_page = current_page
+        self.end_date = end_date
+        self.page_size = page_size
+        self.product_code = product_code
+        self.scene_id = scene_id
+        self.start_date = start_date
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.end_date is not None:
+            result['EndDate'] = self.end_date
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.product_code is not None:
+            result['ProductCode'] = self.product_code
+        if self.scene_id is not None:
+            result['SceneId'] = self.scene_id
+        if self.start_date is not None:
+            result['StartDate'] = self.start_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('EndDate') is not None:
+            self.end_date = m.get('EndDate')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ProductCode') is not None:
+            self.product_code = m.get('ProductCode')
+        if m.get('SceneId') is not None:
+            self.scene_id = m.get('SceneId')
+        if m.get('StartDate') is not None:
+            self.start_date = m.get('StartDate')
+        return self
+
+
+class DescribePageFaceVerifyDataResponseBodyItems(TeaModel):
+    def __init__(
+        self,
+        date: str = None,
+        product_code: str = None,
+        scene_id: str = None,
+        scene_name: str = None,
+        success_count: str = None,
+        total_count: str = None,
+    ):
+        self.date = date
+        self.product_code = product_code
+        self.scene_id = scene_id
+        self.scene_name = scene_name
+        self.success_count = success_count
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.date is not None:
+            result['Date'] = self.date
+        if self.product_code is not None:
+            result['ProductCode'] = self.product_code
+        if self.scene_id is not None:
+            result['SceneId'] = self.scene_id
+        if self.scene_name is not None:
+            result['SceneName'] = self.scene_name
+        if self.success_count is not None:
+            result['SuccessCount'] = self.success_count
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Date') is not None:
+            self.date = m.get('Date')
+        if m.get('ProductCode') is not None:
+            self.product_code = m.get('ProductCode')
+        if m.get('SceneId') is not None:
+            self.scene_id = m.get('SceneId')
+        if m.get('SceneName') is not None:
+            self.scene_name = m.get('SceneName')
+        if m.get('SuccessCount') is not None:
+            self.success_count = m.get('SuccessCount')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribePageFaceVerifyDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        current_page: str = None,
+        items: List[DescribePageFaceVerifyDataResponseBodyItems] = None,
+        message: str = None,
+        page_size: str = None,
+        request_id: str = None,
+        success: str = None,
+        total_count: str = None,
+        total_page: str = None,
+    ):
+        self.code = code
+        self.current_page = current_page
+        self.items = items
+        self.message = message
+        self.page_size = page_size
+        self.request_id = request_id
+        self.success = success
+        self.total_count = total_count
+        self.total_page = total_page
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        result['Items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['Items'].append(k.to_map() if k else None)
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        if self.total_page is not None:
+            result['TotalPage'] = self.total_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        self.items = []
+        if m.get('Items') is not None:
+            for k in m.get('Items'):
+                temp_model = DescribePageFaceVerifyDataResponseBodyItems()
+                self.items.append(temp_model.from_map(k))
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        if m.get('TotalPage') is not None:
+            self.total_page = m.get('TotalPage')
+        return self
+
+
+class DescribePageFaceVerifyDataResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePageFaceVerifyDataResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePageFaceVerifyDataResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeSmartStatisticsPageListRequest(TeaModel):
     def __init__(
         self,
         current_page: str = None,
         end_date: str = None,
         page_size: str = None,
         scene_id: str = None,
@@ -4225,14 +4647,547 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = Mobile3MetaSimpleVerifyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class MobileDetectRequest(TeaModel):
+    def __init__(
+        self,
+        mobiles: str = None,
+        param_type: str = None,
+    ):
+        self.mobiles = mobiles
+        self.param_type = param_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mobiles is not None:
+            result['Mobiles'] = self.mobiles
+        if self.param_type is not None:
+            result['ParamType'] = self.param_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Mobiles') is not None:
+            self.mobiles = m.get('Mobiles')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileDetectResponseBodyResultObjectItems(TeaModel):
+    def __init__(
+        self,
+        area: str = None,
+        biz_code: str = None,
+        isp_name: str = None,
+        mobile: str = None,
+        sub_code: str = None,
+    ):
+        self.area = area
+        self.biz_code = biz_code
+        self.isp_name = isp_name
+        self.mobile = mobile
+        self.sub_code = sub_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.area is not None:
+            result['Area'] = self.area
+        if self.biz_code is not None:
+            result['BizCode'] = self.biz_code
+        if self.isp_name is not None:
+            result['IspName'] = self.isp_name
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.sub_code is not None:
+            result['SubCode'] = self.sub_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Area') is not None:
+            self.area = m.get('Area')
+        if m.get('BizCode') is not None:
+            self.biz_code = m.get('BizCode')
+        if m.get('IspName') is not None:
+            self.isp_name = m.get('IspName')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('SubCode') is not None:
+            self.sub_code = m.get('SubCode')
+        return self
+
+
+class MobileDetectResponseBodyResultObject(TeaModel):
+    def __init__(
+        self,
+        charge_count: str = None,
+        items: List[MobileDetectResponseBodyResultObjectItems] = None,
+    ):
+        self.charge_count = charge_count
+        self.items = items
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.charge_count is not None:
+            result['ChargeCount'] = self.charge_count
+        result['Items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['Items'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ChargeCount') is not None:
+            self.charge_count = m.get('ChargeCount')
+        self.items = []
+        if m.get('Items') is not None:
+            for k in m.get('Items'):
+                temp_model = MobileDetectResponseBodyResultObjectItems()
+                self.items.append(temp_model.from_map(k))
+        return self
+
+
+class MobileDetectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result_object: MobileDetectResponseBodyResultObject = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result_object = result_object
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_object is not None:
+            result['ResultObject'] = self.result_object.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultObject') is not None:
+            temp_model = MobileDetectResponseBodyResultObject()
+            self.result_object = temp_model.from_map(m['ResultObject'])
+        return self
+
+
+class MobileDetectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MobileDetectResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MobileDetectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class MobileOnlineStatusRequest(TeaModel):
+    def __init__(
+        self,
+        mobile: str = None,
+        param_type: str = None,
+    ):
+        self.mobile = mobile
+        self.param_type = param_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.param_type is not None:
+            result['ParamType'] = self.param_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileOnlineStatusResponseBodyResultObject(TeaModel):
+    def __init__(
+        self,
+        biz_code: str = None,
+        isp_name: str = None,
+        sub_code: str = None,
+    ):
+        self.biz_code = biz_code
+        self.isp_name = isp_name
+        self.sub_code = sub_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_code is not None:
+            result['BizCode'] = self.biz_code
+        if self.isp_name is not None:
+            result['IspName'] = self.isp_name
+        if self.sub_code is not None:
+            result['SubCode'] = self.sub_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizCode') is not None:
+            self.biz_code = m.get('BizCode')
+        if m.get('IspName') is not None:
+            self.isp_name = m.get('IspName')
+        if m.get('SubCode') is not None:
+            self.sub_code = m.get('SubCode')
+        return self
+
+
+class MobileOnlineStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result_object: MobileOnlineStatusResponseBodyResultObject = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result_object = result_object
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_object is not None:
+            result['ResultObject'] = self.result_object.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultObject') is not None:
+            temp_model = MobileOnlineStatusResponseBodyResultObject()
+            self.result_object = temp_model.from_map(m['ResultObject'])
+        return self
+
+
+class MobileOnlineStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MobileOnlineStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MobileOnlineStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class MobileOnlineTimeRequest(TeaModel):
+    def __init__(
+        self,
+        mobile: str = None,
+        param_type: str = None,
+    ):
+        self.mobile = mobile
+        self.param_type = param_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.param_type is not None:
+            result['ParamType'] = self.param_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileOnlineTimeResponseBodyResultObject(TeaModel):
+    def __init__(
+        self,
+        biz_code: str = None,
+        isp_name: str = None,
+        time_code: str = None,
+    ):
+        self.biz_code = biz_code
+        self.isp_name = isp_name
+        self.time_code = time_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_code is not None:
+            result['BizCode'] = self.biz_code
+        if self.isp_name is not None:
+            result['IspName'] = self.isp_name
+        if self.time_code is not None:
+            result['TimeCode'] = self.time_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizCode') is not None:
+            self.biz_code = m.get('BizCode')
+        if m.get('IspName') is not None:
+            self.isp_name = m.get('IspName')
+        if m.get('TimeCode') is not None:
+            self.time_code = m.get('TimeCode')
+        return self
+
+
+class MobileOnlineTimeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        result_object: MobileOnlineTimeResponseBodyResultObject = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.result_object = result_object
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_object is not None:
+            result['ResultObject'] = self.result_object.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultObject') is not None:
+            temp_model = MobileOnlineTimeResponseBodyResultObject()
+            self.result_object = temp_model.from_map(m['ResultObject'])
+        return self
+
+
+class MobileOnlineTimeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MobileOnlineTimeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MobileOnlineTimeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyDeviceInfoRequest(TeaModel):
     def __init__(
         self,
         biz_type: str = None,
         device_id: str = None,
         duration: str = None,
         expired_day: str = None,
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.5.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.4.0
+Version: 2.5.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.4.0/setup.py` & `alibabacloud_cloudauth20190307-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 13/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
```

