# Comparing `tmp/jhu-1.4.0.tar.gz` & `tmp/jhu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhu-1.4.0.tar", last modified: Tue Apr  9 08:33:41 2024, max compression
+gzip compressed data, was "jhu-1.4.1.tar", last modified: Wed Apr 10 01:50:53 2024, max compression
```

## Comparing `jhu-1.4.0.tar` & `jhu-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-09 08:33:41.961962 jhu-1.4.0/
--rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.4.0/LICENSE
--rw-r--r--   0 hujian     (501) staff       (20)      624 2024-04-09 08:33:41.960791 jhu-1.4.0/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)     1488 2024-04-09 08:30:27.000000 jhu-1.4.0/README.md
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-09 08:33:41.953254 jhu-1.4.0/jhu/
--rw-r--r--   0 hujian     (501) staff       (20)        0 2023-10-08 09:32:43.000000 jhu-1.4.0/jhu/__init__.py
--rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-01-05 07:00:28.000000 jhu-1.4.0/jhu/auth.py
--rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.4.0/jhu/email.py
--rw-r--r--   0 hujian     (501) staff       (20)     2686 2024-04-09 08:30:34.000000 jhu-1.4.0/jhu/security.py
--rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.4.0/jhu/webhook.py
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-09 08:33:41.959797 jhu-1.4.0/jhu.egg-info/
--rw-r--r--   0 hujian     (501) staff       (20)      624 2024-04-09 08:33:41.000000 jhu-1.4.0/jhu.egg-info/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)      254 2024-04-09 08:33:41.000000 jhu-1.4.0/jhu.egg-info/SOURCES.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-09 08:33:41.000000 jhu-1.4.0/jhu.egg-info/dependency_links.txt
--rw-r--r--   0 hujian     (501) staff       (20)       55 2024-04-09 08:33:41.000000 jhu-1.4.0/jhu.egg-info/requires.txt
--rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-09 08:33:41.000000 jhu-1.4.0/jhu.egg-info/top_level.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.4.0/jhu.egg-info/zip-safe
--rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-09 08:33:41.962242 jhu-1.4.0/setup.cfg
--rwxr-xr-x   0 hujian     (501) staff       (20)     1401 2024-04-09 08:27:04.000000 jhu-1.4.0/setup.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.611858 jhu-1.4.1/
+-rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.4.1/LICENSE
+-rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-10 01:50:53.609788 jhu-1.4.1/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)     1624 2024-04-10 01:50:15.000000 jhu-1.4.1/README.md
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.601236 jhu-1.4.1/jhu/
+-rw-r--r--   0 hujian     (501) staff       (20)       21 2024-04-10 01:48:06.000000 jhu-1.4.1/jhu/__init__.py
+-rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-01-05 07:00:28.000000 jhu-1.4.1/jhu/auth.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.4.1/jhu/email.py
+-rw-r--r--   0 hujian     (501) staff       (20)     3062 2024-04-10 01:48:10.000000 jhu-1.4.1/jhu/security.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.4.1/jhu/webhook.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.608638 jhu-1.4.1/jhu.egg-info/
+-rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)      254 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/SOURCES.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/dependency_links.txt
+-rw-r--r--   0 hujian     (501) staff       (20)       42 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/requires.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/top_level.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.4.1/jhu.egg-info/zip-safe
+-rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-10 01:50:53.612168 jhu-1.4.1/setup.cfg
+-rwxr-xr-x   0 hujian     (501) staff       (20)     1592 2024-04-10 01:47:56.000000 jhu-1.4.1/setup.py
```

### Comparing `jhu-1.4.0/LICENSE` & `jhu-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jhu-1.4.0/PKG-INFO` & `jhu-1.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.0
+Version: 1.4.1
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-jose
 Requires-Dist: bcrypt
-Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
```

### Comparing `jhu-1.4.0/README.md` & `jhu-1.4.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # JHU(Join Happy Utils)
 > 这个是我自己编写的一个python工具库,简化或者自动化的帮助我做一些工作
 
 # ChangeLog
+## V1.4.1(2024-04-10)
+### security.py
+- 废弃fernetAPI,改为AESAPI,并采用ECB模式; 同样的明文加密后的内容是一致的
+
 ## V1.4.0(2024-04-09)
 ### security.py
 - 追加了对称加密
 - JWTAPI中的datetime.utcnow函数弃用,用了其他替代方法
 
 ## V1.3.0
 - 2023-12-19:从v1.3.0版本开始,基于python3.12进行开发.并整合优化代码
```

### Comparing `jhu-1.4.0/jhu/auth.py` & `jhu-1.4.1/jhu/auth.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.0/jhu/email.py` & `jhu-1.4.1/jhu/email.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.0/jhu/security.py` & `jhu-1.4.1/jhu/security.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 """
 安全模块工具
 """
 from datetime import datetime,timedelta
 from zoneinfo import ZoneInfo
 from bcrypt import checkpw,gensalt,hashpw
-from base64 import b64decode
+from base64 import b64decode,b64encode
 from Cryptodome.Cipher import AES
-from Cryptodome.Util.Padding import unpad
-from cryptography.fernet import Fernet
+from Cryptodome.Util.Padding import pad,unpad
 from jose import jwt
 
-class FernetAPI:
+
+class AESAPI:
     def __init__(self,key:str) -> None:
-        """key可通过 Fernet.generate_key() 生成
-        """
-        self.__fernet = Fernet(key)
-    
-    @property
-    def fernet(self):
-        return self.__fernet
+        # ECB模式,加密结果固定
+        self.cipher = AES.new(key.encode(),AES.MODE_ECB)
     
-    def encrypt(self,plain_text:str)->str:
+    def encrypt(self,plain_text:str):
         """加密
         """
-        return self.fernet.encrypt(plain_text.encode()).decode()
-        
-    def decrypt(self,encrypted_text: str)->str:
+
+        # 对明文进行补全至块大小的填充
+        padded_text = pad(plain_text.encode(), AES.block_size)
+
+        # 加密
+        ciphertext = self.cipher.encrypt(padded_text)
+
+        # 返回Base64编码的密文
+        return b64encode(ciphertext).decode()
+    
+    def decrypt(self,encrypted_value:str):
         """解密
         """
-        return self.fernet.decrypt(encrypted_text).decode()
 
+        # 将Base64编码的密文解码为字节
+        ciphertext = b64decode(encrypted_value.encode())
+
+        # 解密
+        decrypted_text = unpad(self.cipher.decrypt(ciphertext), AES.block_size)
+
+        # 将解密后的字节串转换回字符串
+        original_message = decrypted_text.decode()
+
+        return original_message
         
 class HashAPI:
     def __init__(self,key:str) -> None:
        """Hash对象
        
        Args:
         key:str,加密密钥
```

### Comparing `jhu-1.4.0/jhu/webhook.py` & `jhu-1.4.1/jhu/webhook.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.0/jhu.egg-info/PKG-INFO` & `jhu-1.4.1/jhu.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.0
+Version: 1.4.1
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-jose
 Requires-Dist: bcrypt
-Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
```

### Comparing `jhu-1.4.0/setup.py` & `jhu-1.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #! /usr/bin/env python3
 
 """
 制作PIP包教程
 1. 先设置一个setup文件
 2. 运行setup.py sdist
 3. 然后会得到一个dist文件, 这个时候就可用pip install dist/xxxxx 来安装文件了
-4. twine upload dist/* 可上传安装,需要输入pypi的用户名和密码
+4. 到PYPI上创建一个API Token(现在不支持user/passwd模型上传package了)
+5. 在本地的创建一个$HOME/.pypirc文件
+    其中:
+    [pypi]
+    username = __token__
+    password = # 这里改成放申请下来的token
+6. twine upload dist/* 可上传安装,需要输入pypi的用户名和密码
 """
 from setuptools import setup, find_packages
 
 setup(
     name='jhu',  # 包的名称
-    version='1.4.0',  # 包的版本,每次更新或升级包都需要更新它
+    version='1.4.1',  # 包的版本,每次更新或升级包都需要更新它
     description='jhu是一个工具包,简化或自动化的做一些任务',  # 包的描述
     author='J.Hu',  # 作者
     email='joestarhu@163.com',  # 作者邮箱
     url='https://github.com/joestarhu/jhu',  # 项目地址
     packages=find_packages(
         exclude=['test', 'examples', 'script', 'tutorials']),   # 包内不需要引用的文件
     classifiers=[
@@ -26,12 +32,11 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 3.12',
     ],
     install_requires=[
         'requests',         # auth webhook
         'python-jose',      # security.py
         'bcrypt',           # security.py
-        'cryptography',     # security.py
         'pycryptodomex',    # security.py
         ],  # 依赖的包
     zip_safe=True
 )
```

