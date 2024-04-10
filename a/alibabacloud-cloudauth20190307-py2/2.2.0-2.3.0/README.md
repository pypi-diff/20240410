# Comparing `tmp/alibabacloud_cloudauth20190307_py2-2.2.0.tar.gz` & `tmp/alibabacloud_cloudauth20190307_py2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307_py2-2.2.0.tar", last modified: Wed Mar 13 03:08:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307_py2-2.3.0.tar", last modified: Wed Apr 10 17:13:05 2024, max compression
```

## Comparing `alibabacloud_cloudauth20190307_py2-2.2.0.tar` & `alibabacloud_cloudauth20190307_py2-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/
--rw-r--r--   0 root         (0) root         (0)      320 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42665 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   158781 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3146 2024-03-13 03:08:44.000000 alibabacloud_cloudauth20190307_py2-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)      378 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49105 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   188030 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-10 17:13:05.000000 alibabacloud_cloudauth20190307_py2-2.3.0/setup.py
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/LICENSE` & `alibabacloud_cloudauth20190307_py2-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/PKG-INFO` & `alibabacloud_cloudauth20190307_py2-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307_py2
-Version: 2.2.0
+Version: 2.3.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/README-CN.md` & `alibabacloud_cloudauth20190307_py2-2.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/README.md` & `alibabacloud_cloudauth20190307_py2-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,54 @@
             self.call_api(params, req, runtime)
         )
 
     def a_igcface_verify(self, request):
         runtime = util_models.RuntimeOptions()
         return self.a_igcface_verify_with_options(request, runtime)
 
+    def bank_meta_verify_with_options(self, request, runtime):
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
+    def bank_meta_verify(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.bank_meta_verify_with_options(request, runtime)
+
     def compare_face_verify_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.crop):
             body['Crop'] = request.crop
         if not UtilClient.is_unset(request.outer_order_no):
             body['OuterOrderNo'] = request.outer_order_no
@@ -462,14 +502,52 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_oss_upload_token(self):
         runtime = util_models.RuntimeOptions()
         return self.describe_oss_upload_token_with_options(runtime)
 
+    def describe_page_face_verify_data_with_options(self, request, runtime):
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
+    def describe_page_face_verify_data(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_page_face_verify_data_with_options(request, runtime)
+
     def describe_smart_statistics_page_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
@@ -894,14 +972,104 @@
             self.call_api(params, req, runtime)
         )
 
     def mobile_3meta_simple_verify(self, request):
         runtime = util_models.RuntimeOptions()
         return self.mobile_3meta_simple_verify_with_options(request, runtime)
 
+    def mobile_detect_with_options(self, request, runtime):
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
+    def mobile_detect(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_detect_with_options(request, runtime)
+
+    def mobile_online_status_with_options(self, request, runtime):
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
+    def mobile_online_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_online_status_with_options(request, runtime)
+
+    def mobile_online_time_with_options(self, request, runtime):
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
+    def mobile_online_time(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.mobile_online_time_with_options(request, runtime)
+
     def modify_device_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.device_id):
             query['DeviceId'] = request.device_id
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AIGCFaceVerifyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BankMetaVerifyRequest(TeaModel):
+    def __init__(self, bank_card=None, identify_num=None, mobile=None, param_type=None, product_type=None,
+                 user_name=None, verify_mode=None):
+        self.bank_card = bank_card  # type: str
+        self.identify_num = identify_num  # type: str
+        self.mobile = mobile  # type: str
+        self.param_type = param_type  # type: str
+        self.product_type = product_type  # type: str
+        self.user_name = user_name  # type: str
+        self.verify_mode = verify_mode  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BankMetaVerifyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, biz_code=None, sub_code=None):
+        self.biz_code = biz_code  # type: str
+        self.sub_code = sub_code  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(BankMetaVerifyResponseBodyResultObject, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BizCode') is not None:
+            self.biz_code = m.get('BizCode')
+        if m.get('SubCode') is not None:
+            self.sub_code = m.get('SubCode')
+        return self
+
+
+class BankMetaVerifyResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None, result_object=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.result_object = result_object  # type: BankMetaVerifyResponseBodyResultObject
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super(BankMetaVerifyResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: BankMetaVerifyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(BankMetaVerifyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, crop=None, outer_order_no=None, product_code=None, scene_id=None, source_certify_id=None,
                  source_face_contrast_picture=None, source_face_contrast_picture_url=None, source_oss_bucket_name=None,
                  source_oss_object_name=None, target_certify_id=None, target_face_contrast_picture=None,
                  target_face_contrast_picture_url=None, target_oss_bucket_name=None, target_oss_object_name=None):
         self.crop = crop  # type: str
         self.outer_order_no = outer_order_no  # type: str
@@ -1613,14 +1774,223 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeOssUploadTokenResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePageFaceVerifyDataRequest(TeaModel):
+    def __init__(self, current_page=None, end_date=None, page_size=None, product_code=None, scene_id=None,
+                 start_date=None):
+        self.current_page = current_page  # type: long
+        self.end_date = end_date  # type: str
+        self.page_size = page_size  # type: long
+        self.product_code = product_code  # type: str
+        self.scene_id = scene_id  # type: long
+        self.start_date = start_date  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePageFaceVerifyDataRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, date=None, product_code=None, scene_id=None, scene_name=None, success_count=None,
+                 total_count=None):
+        self.date = date  # type: str
+        self.product_code = product_code  # type: str
+        self.scene_id = scene_id  # type: str
+        self.scene_name = scene_name  # type: str
+        self.success_count = success_count  # type: str
+        self.total_count = total_count  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePageFaceVerifyDataResponseBodyItems, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, current_page=None, items=None, message=None, page_size=None, request_id=None,
+                 success=None, total_count=None, total_page=None):
+        self.code = code  # type: str
+        self.current_page = current_page  # type: str
+        self.items = items  # type: list[DescribePageFaceVerifyDataResponseBodyItems]
+        self.message = message  # type: str
+        self.page_size = page_size  # type: str
+        self.request_id = request_id  # type: str
+        self.success = success  # type: str
+        self.total_count = total_count  # type: str
+        self.total_page = total_page  # type: str
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePageFaceVerifyDataResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePageFaceVerifyDataResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePageFaceVerifyDataResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, current_page=None, end_date=None, page_size=None, scene_id=None, service_code=None,
                  start_date=None):
         self.current_page = current_page  # type: str
         self.end_date = end_date  # type: str
         self.page_size = page_size  # type: str
         self.scene_id = scene_id  # type: str
@@ -3691,14 +4061,481 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = Mobile3MetaSimpleVerifyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class MobileDetectRequest(TeaModel):
+    def __init__(self, mobiles=None, param_type=None):
+        self.mobiles = mobiles  # type: str
+        self.param_type = param_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileDetectRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Mobiles') is not None:
+            self.mobiles = m.get('Mobiles')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileDetectResponseBodyResultObjectItems(TeaModel):
+    def __init__(self, area=None, biz_code=None, isp_name=None, mobile=None, sub_code=None):
+        self.area = area  # type: str
+        self.biz_code = biz_code  # type: str
+        self.isp_name = isp_name  # type: str
+        self.mobile = mobile  # type: str
+        self.sub_code = sub_code  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileDetectResponseBodyResultObjectItems, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, charge_count=None, items=None):
+        self.charge_count = charge_count  # type: str
+        self.items = items  # type: list[MobileDetectResponseBodyResultObjectItems]
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(MobileDetectResponseBodyResultObject, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, message=None, request_id=None, result_object=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.result_object = result_object  # type: MobileDetectResponseBodyResultObject
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super(MobileDetectResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: MobileDetectResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(MobileDetectResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, mobile=None, param_type=None):
+        self.mobile = mobile  # type: str
+        self.param_type = param_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileOnlineStatusRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileOnlineStatusResponseBodyResultObject(TeaModel):
+    def __init__(self, biz_code=None, isp_name=None, sub_code=None):
+        self.biz_code = biz_code  # type: str
+        self.isp_name = isp_name  # type: str
+        self.sub_code = sub_code  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileOnlineStatusResponseBodyResultObject, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, message=None, request_id=None, result_object=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.result_object = result_object  # type: MobileOnlineStatusResponseBodyResultObject
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super(MobileOnlineStatusResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: MobileOnlineStatusResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(MobileOnlineStatusResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, mobile=None, param_type=None):
+        self.mobile = mobile  # type: str
+        self.param_type = param_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileOnlineTimeRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('ParamType') is not None:
+            self.param_type = m.get('ParamType')
+        return self
+
+
+class MobileOnlineTimeResponseBodyResultObject(TeaModel):
+    def __init__(self, biz_code=None, isp_name=None, time_code=None):
+        self.biz_code = biz_code  # type: str
+        self.isp_name = isp_name  # type: str
+        self.time_code = time_code  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MobileOnlineTimeResponseBodyResultObject, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, message=None, request_id=None, result_object=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.result_object = result_object  # type: MobileOnlineTimeResponseBodyResultObject
+
+    def validate(self):
+        if self.result_object:
+            self.result_object.validate()
+
+    def to_map(self):
+        _map = super(MobileOnlineTimeResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: MobileOnlineTimeResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(MobileOnlineTimeResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, biz_type=None, device_id=None, duration=None, expired_day=None, user_device_id=None):
         self.biz_type = biz_type  # type: str
         self.device_id = device_id  # type: str
         self.duration = duration  # type: str
         self.expired_day = expired_day  # type: str
         self.user_device_id = user_device_id  # type: str
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307_py2-2.3.0/alibabacloud_cloudauth20190307_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307-py2
-Version: 2.2.0
+Version: 2.3.0
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307_py2-2.2.0/setup.py` & `alibabacloud_cloudauth20190307_py2-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307_py2.
 
-Created on 13/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python2"
```

