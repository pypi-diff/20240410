# Comparing `tmp/f_tools_pkg-0.0.6.tar.gz` & `tmp/f_tools_pkg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\f_tools_pkg-0.0.6.tar", last modified: Wed Mar 27 07:17:00 2024, max compression
+gzip compressed data, was "dist\f_tools_pkg-0.0.7.tar", last modified: Wed Apr 10 12:48:46 2024, max compression
```

## Comparing `f_tools_pkg-0.0.6.tar` & `f_tools_pkg-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/
--rw-rw-rw-   0        0        0      517 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-03-27 06:58:04.000000 f_tools_pkg-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg/
--rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.6/f_tools_pkg/__init__.py
--rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_bmp.py
--rw-rw-rw-   0        0        0     5300 2022-03-17 06:25:08.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_crypt.py
--rw-rw-rw-   0        0        0     3393 2024-03-27 06:54:20.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_e.py
--rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_ecc.py
--rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_excel.py
--rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_log.py
--rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.6/f_tools_pkg/f_serial.py
-drwxrwxrwx   0        0        0        0 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/
--rw-rw-rw-   0        0        0      517 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/f_tools_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 07:17:00.000000 f_tools_pkg-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-03-27 06:55:32.000000 f_tools_pkg-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/
+-rw-rw-rw-   0        0        0      584 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-04-10 12:48:00.000000 f_tools_pkg-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg/
+-rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.7/f_tools_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_bmp.py
+-rw-rw-rw-   0        0        0     5667 2024-04-10 12:46:32.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_crypt.py
+-rw-rw-rw-   0        0        0     3393 2024-03-27 06:54:20.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_e.py
+-rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_ecc.py
+-rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_excel.py
+-rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_log.py
+-rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/
+-rw-rw-rw-   0        0        0      584 2024-04-10 12:48:45.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:48:45.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-04-10 12:48:06.000000 f_tools_pkg-0.0.7/setup.py
```

### Comparing `f_tools_pkg-0.0.6/PKG-INFO` & `f_tools_pkg-0.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f_tools_pkg
-Version: 0.0.6
+Version: 0.0.7
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,10 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 2022-7-20 V0.0.4  add bmp_scale function
 
 2024-3-27 V0.06  e bu add "type" parameter
 
+2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
+
```

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_bmp.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_bmp.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_crypt.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_crypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from Crypto.Cipher import AES
 from Crypto.Cipher import DES3 
+from Crypto.Cipher import DES
 
 class f_crypt:
     def __init__(self):
         self.crc_table=[
         0x00000000, 0x04c11db7, 0x09823b6e, 0x0d4326d9, 0x130476dc, 0x17c56b6b,
 		0x1a864db2, 0x1e475005, 0x2608edb8, 0x22c9f00f, 0x2f8ad6d6, 0x2b4bcb61,
 		0x350c9b64, 0x31cd86d3, 0x3c8ea00a, 0x384fbdbd, 0x4c11db70, 0x48d0c6c7,
@@ -72,22 +73,32 @@
         aes = AES.new(bytes(ikey), AES.MODE_ECB)  # 初始化加密器
         tdata = aes.decrypt(bytes(idata))   # 加密
         odata.extend(list(tdata))
         return odata
     
     def tdes_enc(self,ikey,idata,odata):
         odata.clear()
-        tdes = DES3.new(bytes(ikey), AES.MODE_ECB)
+        t=""
+        for i in range(0,16): t+=str(ikey[i])
+        if int(t,10) ==0:
+            tdes = DES.new(bytes(ikey[16:]), DES.MODE_ECB)
+        else:
+            tdes = DES3.new(bytes(ikey), DES3.MODE_ECB)
         tdata = tdes.encrypt(bytes(idata))
         odata.extend(list(tdata))
         return odata
     
     def tdes_dec(self,ikey,idata,odata):
         odata.clear()
-        tdes = DES3.new(bytes(ikey), AES.MODE_ECB)
+        t=""
+        for i in range(0,16): t+=str(ikey[i])
+        if int(t,10) ==0:
+            tdes = DES.new(bytes(ikey[16:]), DES.MODE_ECB)
+        else:
+            tdes = DES3.new(bytes(ikey), DES3.MODE_ECB)
         tdata = tdes.decrypt(bytes(idata))
         odata.extend(list(tdata))
         return odata
     
 
 # test = f_crypt()
 # keybuf=[0x8B,0x25,0x9A,0x39,0x9D,0xE5,0xCE,0x47,0x51,0xD5,0xE7,0xCB,0xE7,0x2D,0x0C,0x77]
```

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_e.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_e.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_excel.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_excel.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_log.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_log.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg/f_serial.py` & `f_tools_pkg-0.0.7/f_tools_pkg/f_serial.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.6/f_tools_pkg.egg-info/PKG-INFO` & `f_tools_pkg-0.0.7/f_tools_pkg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f-tools-pkg
-Version: 0.0.6
+Version: 0.0.7
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,8 +13,10 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 2022-7-20 V0.0.4  add bmp_scale function
 
 2024-3-27 V0.06  e bu add "type" parameter
 
+2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
+
```

### Comparing `f_tools_pkg-0.0.6/setup.py` & `f_tools_pkg-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='f_tools_pkg',
-    version='0.0.6',
+    version='0.0.7',
     packages=setuptools.find_packages(),
     url='',
     license='MIT',
     author='wushengyan',
     author_email='WUSY1991@163.com',
     description='some common tools(bmp/crypt/excel/log ...)',
     long_description=long_description,
```

