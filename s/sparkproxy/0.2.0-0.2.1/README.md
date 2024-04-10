# Comparing `tmp/sparkproxy-0.2.0.tar.gz` & `tmp/sparkproxy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.2.0.tar", last modified: Tue Apr  9 03:20:31 2024, max compression
+gzip compressed data, was "sparkproxy-0.2.1.tar", last modified: Tue Apr  9 07:47:14 2024, max compression
```

## Comparing `sparkproxy-0.2.0.tar` & `sparkproxy-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.384274 sparkproxy-0.2.0/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.2.0/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1130 2024-04-09 03:20:31.384146 sparkproxy-0.2.0/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     3719 2024-04-09 03:20:05.000000 sparkproxy-0.2.0/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-09 03:20:31.384339 sparkproxy-0.2.0/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.2.0/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.380857 sparkproxy-0.2.0/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-09 03:18:58.000000 sparkproxy-0.2.0/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2877 2024-04-09 03:14:04.000000 sparkproxy-0.2.0/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.2.0/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.382286 sparkproxy-0.2.0/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.2.0/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.2.0/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383243 sparkproxy-0.2.0/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.2.0/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1555 2024-04-09 02:53:50.000000 sparkproxy-0.2.0/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383576 sparkproxy-0.2.0/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383802 sparkproxy-0.2.0/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5916 2024-04-09 03:16:16.000000 sparkproxy-0.2.0/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.381702 sparkproxy-0.2.0/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1130 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       55 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.062101 sparkproxy-0.2.1/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.2.1/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-09 07:47:14.061970 sparkproxy-0.2.1/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     3717 2024-04-09 03:26:16.000000 sparkproxy-0.2.1/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-09 07:47:14.062137 sparkproxy-0.2.1/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.2.1/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.058983 sparkproxy-0.2.1/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-09 07:45:17.000000 sparkproxy-0.2.1/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2877 2024-04-09 03:14:04.000000 sparkproxy-0.2.1/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.2.1/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.060417 sparkproxy-0.2.1/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.2.1/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.2.1/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061276 sparkproxy-0.2.1/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.2.1/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1915 2024-04-09 07:45:11.000000 sparkproxy-0.2.1/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061609 sparkproxy-0.2.1/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061793 sparkproxy-0.2.1/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5896 2024-04-09 07:38:03.000000 sparkproxy-0.2.1/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.059795 sparkproxy-0.2.1/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.2.0/LICENSE` & `sparkproxy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/PKG-INFO` & `sparkproxy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
@@ -24,9 +24,7 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 License-File: LICENSE
 
 see:
 https://github.com/yungoo/spark-sdk-python
-
-
```

### Comparing `sparkproxy-0.2.0/README.md` & `sparkproxy-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Sparkproxy OpenApi SDK for Python
 
 [![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)
 [![GitHub release](https://img.shields.io/github/v/tag/sparkpoxy/spark-sdk-python.svg?label=release)](https://github.com/yungoo/spark-sdk-python/releases)
-[![Latest Stable Version](https://img.shields.io/pypi/v/sparkproxy.svg)](https://pypi.python.org/pypi/spark-proxy)
-[![Download Times](https://img.shields.io/pypi/dm/sparkproxy.svg)](https://pypi.python.org/pypi/spark-proxy)
+[![Latest Stable Version](https://img.shields.io/pypi/v/sparkproxy.svg)](https://pypi.python.org/pypi/sparkproxy)
+[![Download Times](https://img.shields.io/pypi/dm/sparkproxy.svg)](https://pypi.python.org/pypi/sparkproxy)
 
 ## 安装
 
 通过pip
 
 ```bash
 $ pip install sparkproxy
```

### Comparing `sparkproxy-0.2.0/setup.py` & `sparkproxy-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/auth.py` & `sparkproxy-0.2.1/sparkproxy/auth.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/compat.py` & `sparkproxy-0.2.1/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/config.py` & `sparkproxy-0.2.1/sparkproxy/config.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/__init__.py` & `sparkproxy-0.2.1/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/client.py` & `sparkproxy-0.2.1/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/middleware/base.py` & `sparkproxy-0.2.1/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.2.1/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.2.1/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/http/response.py` & `sparkproxy-0.2.1/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.0/sparkproxy/rsa.py` & `sparkproxy-0.2.1/sparkproxy/rsa.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,80 @@
-import base64
+import binascii
 
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.serialization import load_pem_private_key
-import os
+
+
+# 兼容Python 2和3的编码函数
+def to_bytes(data, encoding='utf-8'):
+    if isinstance(data, str):
+        return data.encode(encoding)
+    return data
+
+
+# 兼容Python 2和3的十六进制解码函数
+def from_hex(s):
+    try:
+        return bytes.fromhex(s)  # Python 3
+    except AttributeError:
+        return s.decode('hex')  # Python 2
+
+
+# 兼容Python 2和3的十六进制编码函数
+def to_hex(data):
+    try:
+        return data.hex()  # Python 3
+    except AttributeError:
+        return binascii.hexlify(data)  # Python 2
 
 
 def rsa_load_pem_private_key(pri_key):
     private_key = serialization.load_pem_private_key(
-        pri_key.encode(),
+        to_bytes(pri_key),
         password=None,
         backend=default_backend()
     )
     return private_key
 
 
 def rsa_load_pem_public_key(pub_key):
     public_key = serialization.load_pem_public_key(
-        pub_key.encode(),
-        backend=None  # Uses the default backend
+        to_bytes(pub_key),
+        backend=default_backend()  # 显式指定后端
     )
     return public_key
 
 
 def rsa_decrypt(encrypted_msg_hex, private_key):
-    # 十六进制解码
-    encrypted_msg = bytes.fromhex(encrypted_msg_hex)
-    
-    # 使用PKCS1v15解密
+    encrypted_msg = from_hex(encrypted_msg_hex)
+
     decrypted_msg = private_key.decrypt(
         encrypted_msg,
         padding.PKCS1v15()
     )
-    
+
     return decrypted_msg
 
 
 def rsa_sign(message, private_key):
-    # 使用私钥对哈希值进行签名
     signature = private_key.sign(
-        message.encode(),
+        to_bytes(message),
         padding.PKCS1v15(),
         hashes.SHA256()
     )
-    return signature.hex()
+    return to_hex(signature)
 
 
 def rsa_verify(sign, message, public_key):
     try:
-        decoded_sign = base64.b64decode(sign)
+        decoded_sign = from_hex(sign)
     except Exception as e:
-        raise ValueError(f"签名解码失败: {e}")
+        raise ValueError("签名解码失败: {}".format(e))
 
     public_key.verify(
         decoded_sign,
-        message.encode(),
+        to_bytes(message),
         padding.PKCS1v15(),
         hashes.SHA256()
     )
```

### Comparing `sparkproxy-0.2.0/sparkproxy/services/openapi/client.py` & `sparkproxy-0.2.1/sparkproxy/services/openapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,17 +137,17 @@
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
         ret, info = self.__post('GetInstance', {"instanceId": instance_id})
         if ret is not None:
-            password = ret['data']['IpInfo']["password"]
+            password = ret['data']["password"]
             if len(password) > 0:
-                ret['data']['IpInfo']["password"] = self.auth.decrypt(password)
+                ret['data']["password"] = self.auth.decrypt(password)
         return ret, info
 
     def __request_params(self, method, args):
         base_params = {
             "method": method,
             "version": "2024-04-08",
             "reqId": str(uuid.uuid4()),
```

### Comparing `sparkproxy-0.2.0/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.2.1/sparkproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
@@ -24,9 +24,7 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 License-File: LICENSE
 
 see:
 https://github.com/yungoo/spark-sdk-python
-
-
```

### Comparing `sparkproxy-0.2.0/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.2.1/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

