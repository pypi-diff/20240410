# Comparing `tmp/antchain_duanka-1.0.5.tar.gz` & `tmp/antchain_duanka-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_duanka-1.0.5.tar", last modified: Mon Mar 25 08:31:46 2024, max compression
+gzip compressed data, was "dist/antchain_duanka-1.0.6.tar", last modified: Wed Apr 10 07:18:07 2024, max compression
```

## Comparing `antchain_duanka-1.0.5.tar` & `antchain_duanka-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2180 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      813 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      999 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2180 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_duanka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/antchain_sdk_duanka/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/antchain_sdk_duanka/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21101 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/antchain_sdk_duanka/client.py
--rw-r--r--   0 root         (0) root         (0)    28591 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/antchain_sdk_duanka/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 08:31:46.000000 antchain_duanka-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2504 2024-03-25 08:31:45.000000 antchain_duanka-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23083 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/client.py
+-rw-r--r--   0 root         (0) root         (0)    35333 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/setup.py
```

### Comparing `antchain_duanka-1.0.5/LICENSE` & `antchain_duanka-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.5/PKG-INFO` & `antchain_duanka-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_duanka
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain DUANKA SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_duanka-1.0.5/README-CN.md` & `antchain_duanka-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.5/README.md` & `antchain_duanka-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.5/antchain_duanka.egg-info/PKG-INFO` & `antchain_duanka-1.0.6/antchain_duanka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-duanka
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain DUANKA SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_duanka-1.0.5/antchain_sdk_duanka/client.py` & `antchain_duanka-1.0.6/antchain_sdk_duanka/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
                     '_prod_code': 'DUANKA',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
                     '_prod_code': 'DUANKA',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -444,57 +444,113 @@
         )
 
     def query_common_score(
         self,
         request: duanka_models.QueryCommonScoreRequest,
     ) -> duanka_models.QueryCommonScoreResponse:
         """
-        Description: 公共查询链路
-        Summary: 公共查询链路
+        Description: 通用查询
+        Summary: 通用查询
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_common_score_ex(request, headers, runtime)
 
     async def query_common_score_async(
         self,
         request: duanka_models.QueryCommonScoreRequest,
     ) -> duanka_models.QueryCommonScoreResponse:
         """
-        Description: 公共查询链路
-        Summary: 公共查询链路
+        Description: 通用查询
+        Summary: 通用查询
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_common_score_ex_async(request, headers, runtime)
 
     def query_common_score_ex(
         self,
         request: duanka_models.QueryCommonScoreRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> duanka_models.QueryCommonScoreResponse:
         """
-        Description: 公共查询链路
-        Summary: 公共查询链路
+        Description: 通用查询
+        Summary: 通用查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             duanka_models.QueryCommonScoreResponse(),
             self.do_request('1.0', 'antcloud.duanka.common.score.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_common_score_ex_async(
         self,
         request: duanka_models.QueryCommonScoreRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> duanka_models.QueryCommonScoreResponse:
         """
-        Description: 公共查询链路
-        Summary: 公共查询链路
+        Description: 通用查询
+        Summary: 通用查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             duanka_models.QueryCommonScoreResponse(),
             await self.do_request_async('1.0', 'antcloud.duanka.common.score.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_ir_brand(
+        self,
+        request: duanka_models.QueryIrBrandRequest,
+    ) -> duanka_models.QueryIrBrandResponse:
+        """
+        Description: 品牌研究数据查询
+        Summary: 品牌研究数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_ir_brand_ex(request, headers, runtime)
+
+    async def query_ir_brand_async(
+        self,
+        request: duanka_models.QueryIrBrandRequest,
+    ) -> duanka_models.QueryIrBrandResponse:
+        """
+        Description: 品牌研究数据查询
+        Summary: 品牌研究数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_ir_brand_ex_async(request, headers, runtime)
+
+    def query_ir_brand_ex(
+        self,
+        request: duanka_models.QueryIrBrandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> duanka_models.QueryIrBrandResponse:
+        """
+        Description: 品牌研究数据查询
+        Summary: 品牌研究数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            duanka_models.QueryIrBrandResponse(),
+            self.do_request('1.0', 'antcloud.duanka.ir.brand.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_ir_brand_ex_async(
+        self,
+        request: duanka_models.QueryIrBrandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> duanka_models.QueryIrBrandResponse:
+        """
+        Description: 品牌研究数据查询
+        Summary: 品牌研究数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            duanka_models.QueryIrBrandResponse(),
+            await self.do_request_async('1.0', 'antcloud.duanka.ir.brand.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_duanka-1.0.5/antchain_sdk_duanka/models.py` & `antchain_duanka-1.0.6/antchain_sdk_duanka/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -217,14 +217,70 @@
         if m.get('bu_mail') is not None:
             self.bu_mail = m.get('bu_mail')
         if m.get('emp_type') is not None:
             self.emp_type = m.get('emp_type')
         return self
 
 
+class ZhxIrResultStruct(TeaModel):
+    def __init__(
+        self,
+        amt_index_v: str = None,
+        trans_num_index_v: str = None,
+        user_num_index_v: str = None,
+        dt: str = None,
+        city_level: str = None,
+    ):
+        # 日合计交易金额指数
+        self.amt_index_v = amt_index_v
+        # 日合计交易笔数指标
+        self.trans_num_index_v = trans_num_index_v
+        # 日合计交易人数指数
+        self.user_num_index_v = user_num_index_v
+        # 时间
+        self.dt = dt
+        # 城市等级
+        self.city_level = city_level
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
+        if self.amt_index_v is not None:
+            result['amt_index_v'] = self.amt_index_v
+        if self.trans_num_index_v is not None:
+            result['trans_num_index_v'] = self.trans_num_index_v
+        if self.user_num_index_v is not None:
+            result['user_num_index_v'] = self.user_num_index_v
+        if self.dt is not None:
+            result['dt'] = self.dt
+        if self.city_level is not None:
+            result['city_level'] = self.city_level
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('amt_index_v') is not None:
+            self.amt_index_v = m.get('amt_index_v')
+        if m.get('trans_num_index_v') is not None:
+            self.trans_num_index_v = m.get('trans_num_index_v')
+        if m.get('user_num_index_v') is not None:
+            self.user_num_index_v = m.get('user_num_index_v')
+        if m.get('dt') is not None:
+            self.dt = m.get('dt')
+        if m.get('city_level') is not None:
+            self.city_level = m.get('city_level')
+        return self
+
+
 class UserInfoResult(TeaModel):
     def __init__(
         self,
         success: bool = None,
         message: str = None,
         error_code: str = None,
         query_result_list: List[QueryResult] = None,
@@ -682,31 +738,37 @@
         auth_no: str = None,
         model_id: str = None,
         user_id: str = None,
         user_id_type: str = None,
         encrypt_type: str = None,
         customer_code: str = None,
         trans_no: str = None,
+        user_id_hash_encrypt: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 用户授权编码
         self.auth_no = auth_no
         # 模型id
         self.model_id = model_id
         # 用户id（客户身份证号/手机号的md5/sha256散列值）
         self.user_id = user_id
         # 用户id类型（身份证号：ID_NO；手机号：MOBILE_NO）
         self.user_id_type = user_id_type
-        # 加密类型: "MD5"：MD5（小写）, "SHA256" ： SHA256（小写）， "SM3"： SM3（小写）
+        # user_id 散列类型: "MD5"：MD5（小写）, "SHA256" ： SHA256（小写）， "SM3"： SM3（小写）
         self.encrypt_type = encrypt_type
         # 客户编码
         self.customer_code = customer_code
         # 流水号，串联链路用，非必填
         self.trans_no = trans_no
+        # encrypt_type类型的散列后的操作，默认为空不加密。
+        # 如启用，需要对散列后的user_id 加密，可选用如下算法，类型1、AES/ECB/PKCS5PADDING
+        # 在加密后的二进制需要以字符集UTF-8，编码base64 方式赋值给user_id传输。
+        # 示例：AES秘钥：base64_aes_key = "CZqWzQ5JL8s5Zx2XVpGZGw=="，报文：plaintext = "Hello, 蚂蚁。" ，使用算法： AES/ECB/PKCS5PADDING ；密文：SI1wU1ePSFoMy5YzuxclFkbZ/FIXUHPRDbKBW85WolY=，配置了此项user_id应该传输此密文。
+        self.user_id_hash_encrypt = user_id_hash_encrypt
 
     def validate(self):
         self.validate_required(self.auth_no, 'auth_no')
         self.validate_required(self.model_id, 'model_id')
         self.validate_required(self.user_id, 'user_id')
         self.validate_required(self.user_id_type, 'user_id_type')
         self.validate_required(self.encrypt_type, 'encrypt_type')
@@ -730,14 +792,16 @@
             result['user_id_type'] = self.user_id_type
         if self.encrypt_type is not None:
             result['encrypt_type'] = self.encrypt_type
         if self.customer_code is not None:
             result['customer_code'] = self.customer_code
         if self.trans_no is not None:
             result['trans_no'] = self.trans_no
+        if self.user_id_hash_encrypt is not None:
+            result['user_id_hash_encrypt'] = self.user_id_hash_encrypt
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('auth_no') is not None:
@@ -750,14 +814,16 @@
             self.user_id_type = m.get('user_id_type')
         if m.get('encrypt_type') is not None:
             self.encrypt_type = m.get('encrypt_type')
         if m.get('customer_code') is not None:
             self.customer_code = m.get('customer_code')
         if m.get('trans_no') is not None:
             self.trans_no = m.get('trans_no')
+        if m.get('user_id_hash_encrypt') is not None:
+            self.user_id_hash_encrypt = m.get('user_id_hash_encrypt')
         return self
 
 
 class QueryCommonScoreResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -809,7 +875,123 @@
         if m.get('score') is not None:
             self.score = m.get('score')
         if m.get('trans_no') is not None:
             self.trans_no = m.get('trans_no')
         return self
 
 
+class QueryIrBrandRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        brandmd_5: str = None,
+        begin_date: str = None,
+        end_date: str = None,
+        scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 品牌MD5的 32位小写
+        self.brandmd_5 = brandmd_5
+        # 开始日期，包含填写时间 ，目前与end_date最大间隔不大于7天
+        self.begin_date = begin_date
+        # 结束日期，包含填写时间， 目前与start_date最大间隔不大于7天
+        self.end_date = end_date
+        # 场景码,brand_overview 品牌汇总；brand_citylevel 品牌城市汇总
+        self.scene = scene
+
+    def validate(self):
+        self.validate_required(self.brandmd_5, 'brandmd_5')
+        self.validate_required(self.begin_date, 'begin_date')
+        self.validate_required(self.end_date, 'end_date')
+        self.validate_required(self.scene, 'scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.brandmd_5 is not None:
+            result['brandmd5'] = self.brandmd_5
+        if self.begin_date is not None:
+            result['begin_date'] = self.begin_date
+        if self.end_date is not None:
+            result['end_date'] = self.end_date
+        if self.scene is not None:
+            result['scene'] = self.scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('brandmd5') is not None:
+            self.brandmd_5 = m.get('brandmd5')
+        if m.get('begin_date') is not None:
+            self.begin_date = m.get('begin_date')
+        if m.get('end_date') is not None:
+            self.end_date = m.get('end_date')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        return self
+
+
+class QueryIrBrandResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data_list: List[ZhxIrResultStruct] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 结果
+        self.data_list = data_list
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['data_list'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['data_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.data_list = []
+        if m.get('data_list') is not None:
+            for k in m.get('data_list'):
+                temp_model = ZhxIrResultStruct()
+                self.data_list.append(temp_model.from_map(k))
+        return self
+
+
```

### Comparing `antchain_duanka-1.0.5/setup.py` & `antchain_duanka-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_duanka.
 
-Created on 25/03/2024
+Created on 10/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_duanka"
 NAME = "antchain_duanka" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DUANKA SDK Library for Python"
```

