# Comparing `tmp/sparkproxy-0.2.1.tar.gz` & `tmp/sparkproxy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.2.1.tar", last modified: Tue Apr  9 07:47:14 2024, max compression
+gzip compressed data, was "sparkproxy-0.3.0.tar", last modified: Wed Apr 10 01:59:03 2024, max compression
```

## Comparing `sparkproxy-0.2.1.tar` & `sparkproxy-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.062101 sparkproxy-0.2.1/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.2.1/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-09 07:47:14.061970 sparkproxy-0.2.1/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     3717 2024-04-09 03:26:16.000000 sparkproxy-0.2.1/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-09 07:47:14.062137 sparkproxy-0.2.1/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.2.1/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.058983 sparkproxy-0.2.1/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-09 07:45:17.000000 sparkproxy-0.2.1/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2877 2024-04-09 03:14:04.000000 sparkproxy-0.2.1/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.2.1/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.060417 sparkproxy-0.2.1/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.2.1/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.2.1/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061276 sparkproxy-0.2.1/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.2.1/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.2.1/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1915 2024-04-09 07:45:11.000000 sparkproxy-0.2.1/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061609 sparkproxy-0.2.1/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.061793 sparkproxy-0.2.1/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.1/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5896 2024-04-09 07:38:03.000000 sparkproxy-0.2.1/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 07:47:14.059795 sparkproxy-0.2.1/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-09 07:47:14.000000 sparkproxy-0.2.1/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.344485 sparkproxy-0.3.0/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.3.0/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 01:59:03.344362 sparkproxy-0.3.0/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     4266 2024-04-10 01:58:30.000000 sparkproxy-0.3.0/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-10 01:59:03.344526 sparkproxy-0.3.0/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.3.0/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.341087 sparkproxy-0.3.0/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-10 01:56:26.000000 sparkproxy-0.3.0/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     3048 2024-04-10 01:27:54.000000 sparkproxy-0.3.0/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.3.0/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.342528 sparkproxy-0.3.0/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.3.0/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.3.0/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.343500 sparkproxy-0.3.0/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.3.0/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2511 2024-04-10 01:48:16.000000 sparkproxy-0.3.0/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.343839 sparkproxy-0.3.0/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.344041 sparkproxy-0.3.0/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     7059 2024-04-10 01:53:25.000000 sparkproxy-0.3.0/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.341913 sparkproxy-0.3.0/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.2.1/LICENSE` & `sparkproxy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/PKG-INFO` & `sparkproxy-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.2.1/README.md` & `sparkproxy-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,33 @@
 
 | sparkproxy SDK版本 |              Python 版本               |
 |:----------------:| :------------------------------------: |
 |       0.x        | 2.7, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9 |
 
 ## 使用方法
 
+### 检查接口是否已经配置好
+
+```python
+from sparkproxy import Auth
+from sparkproxy import SparkProxyClient
+
+supplier_no = 'test0001'
+with open("key.pem", 'rb') as pem_file:
+    private_key = pem_file.read().decode("utf-8")
+with open("spark.pub", 'rb') as pem_file:
+    rsa_public_key = pem_file.read().decode("utf-8")
+client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key, public_key=rsa_public_key))
+
+# 获取订单&实例信息
+ret, info = client.check_available()
+print(ret)
+print(info)
+```
+
 ### 调用sparkproxy的开放接口
 
 ```python
 from sparkproxy import Auth
 from sparkproxy import SparkProxyClient
 
 # 双方协商的商户号
@@ -100,15 +119,15 @@
         return ret, code
 
     ret = request.json
     if ret is not None:
         for ipInfo in ret['data']['ipInfo']:
             password = ipInfo["password"]
             if len(password) > 0:
-                ipInfo["password"] = auth.decrypt(password)
+                ipInfo["password"] = auth.decrypt_using_private_key(password)
 
     print(ret)
 
     return "", 200
 
 
 if __name__ == "__main__":
```

### Comparing `sparkproxy-0.2.1/setup.py` & `sparkproxy-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/auth.py` & `sparkproxy-0.3.0/sparkproxy/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import time
 
 from cryptography.exceptions import InvalidSignature
 
-from sparkproxy.rsa import rsa_load_pem_private_key, rsa_sign, rsa_decrypt, rsa_verify, rsa_load_pem_public_key
+from sparkproxy.rsa import rsa_load_pem_private_key, rsa_sign, rsa_verify, rsa_load_pem_public_key, \
+    rsa_public_encrypt, rsa_private_decrypt
 
 
 class Auth(object):
     """安全机制类
 
     该类主要内容是凭证的签名接口的实现，以及回调验证。
 
@@ -45,16 +46,19 @@
         return rsa_sign(message, self.__private_key)
 
     @staticmethod
     def __checkKey(access_key, secret_key):
         if not (access_key and secret_key):
             raise ValueError('invalid key')
 
-    def decrypt(self, encrypt_msg):
-        return rsa_decrypt(encrypt_msg, self.__private_key)
+    def encrypt_using_remote_public_key(self, msg):
+        return rsa_public_encrypt(msg, self.__public_key)
+
+    def decrypt_using_private_key(self, encrypt_msg):
+        return rsa_private_decrypt(encrypt_msg, self.__private_key)
 
     def verify_callback(
             self,
             supplier_no, sign, req_id, timestamp):
         """回调验证
 
         Args:
```

### Comparing `sparkproxy-0.2.1/sparkproxy/compat.py` & `sparkproxy-0.3.0/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/config.py` & `sparkproxy-0.3.0/sparkproxy/config.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/__init__.py` & `sparkproxy-0.3.0/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/client.py` & `sparkproxy-0.3.0/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/middleware/base.py` & `sparkproxy-0.3.0/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.3.0/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.3.0/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/http/response.py` & `sparkproxy-0.3.0/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.2.1/sparkproxy/rsa.py` & `sparkproxy-0.3.0/sparkproxy/rsa.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,33 @@
 # 兼容Python 2和3的编码函数
 def to_bytes(data, encoding='utf-8'):
     if isinstance(data, str):
         return data.encode(encoding)
     return data
 
 
+def to_string(data, encoding='utf-8'):
+    """
+    将数据转换为字符串。
+
+    Args:
+        data: 要转换的数据。
+        encoding: 字符串编码。
+
+    Returns:
+        str: 转换后的字符串。
+    """
+    if isinstance(data, bytes):
+        return data.decode(encoding)
+    elif isinstance(data, str):
+        return data
+    else:
+        return str(data)
+
+
 # 兼容Python 2和3的十六进制解码函数
 def from_hex(s):
     try:
         return bytes.fromhex(s)  # Python 3
     except AttributeError:
         return s.decode('hex')  # Python 2
 
@@ -42,15 +61,26 @@
     public_key = serialization.load_pem_public_key(
         to_bytes(pub_key),
         backend=default_backend()  # 显式指定后端
     )
     return public_key
 
 
-def rsa_decrypt(encrypted_msg_hex, private_key):
+def rsa_public_encrypt(msg, public_key):
+    decoded_msg = to_bytes(msg)
+
+    encrypted_msg = public_key.encrypt(
+        decoded_msg,
+        padding.PKCS1v15()
+    )
+
+    return to_hex(encrypted_msg)
+
+
+def rsa_private_decrypt(encrypted_msg_hex, private_key):
     encrypted_msg = from_hex(encrypted_msg_hex)
 
     decrypted_msg = private_key.decrypt(
         encrypted_msg,
         padding.PKCS1v15()
     )
```

### Comparing `sparkproxy-0.2.1/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.3.0/sparkproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.2.1/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.3.0/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

