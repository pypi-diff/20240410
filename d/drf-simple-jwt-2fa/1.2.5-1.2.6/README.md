# Comparing `tmp/drf-simple-jwt-2fa-1.2.5.tar.gz` & `tmp/drf-simple-jwt-2fa-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-simple-jwt-2fa-1.2.5.tar", last modified: Thu Oct 27 08:56:21 2022, max compression
+gzip compressed data, was "drf-simple-jwt-2fa-1.2.6.tar", last modified: Wed Apr 10 08:11:07 2024, max compression
```

## Comparing `drf-simple-jwt-2fa-1.2.5.tar` & `drf-simple-jwt-2fa-1.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-10-27 08:56:21.975417 drf-simple-jwt-2fa-1.2.5/
--rw-rw-rw-   0        0        0     1092 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     5059 2022-10-27 08:56:21.975417 drf-simple-jwt-2fa-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2022-01-11 13:33:30.000000 drf-simple-jwt-2fa-1.2.5/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-27 08:56:21.955008 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/
--rw-rw-rw-   0        0        0      186 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/__init__.py
--rw-rw-rw-   0        0        0      131 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/authentication.py
--rw-rw-rw-   0        0        0      588 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/exceptions.py
--rw-rw-rw-   0        0        0     1343 2022-10-27 08:56:07.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/sending.py
--rw-rw-rw-   0        0        0     6198 2022-01-19 14:00:23.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/serializers.py
--rw-rw-rw-   0        0        0     1714 2022-01-11 15:44:49.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/settings.py
-drwxrwxrwx   0        0        0        0 2022-10-27 08:56:21.975417 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/
--rw-rw-rw-   0        0        0        0 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/__init__.py
--rw-rw-rw-   0        0        0      308 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/factories.py
--rw-rw-rw-   0        0        0     3712 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_endpoints.py
--rw-rw-rw-   0        0        0     6985 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_throttling.py
--rw-rw-rw-   0        0        0     4473 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_token_manager.py
--rw-rw-rw-   0        0        0     3188 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/utils.py
--rw-rw-rw-   0        0        0     1799 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/throttling.py
--rw-rw-rw-   0        0        0     4319 2022-01-19 14:01:00.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/token_manager.py
--rw-rw-rw-   0        0        0      320 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/urls.py
--rw-rw-rw-   0        0        0     1125 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/utils.py
--rw-rw-rw-   0        0        0      774 2022-01-04 10:58:27.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/views.py
-drwxrwxrwx   0        0        0        0 2022-10-27 08:56:21.965563 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/
--rw-rw-rw-   0        0        0     5059 2022-10-27 08:56:21.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      837 2022-10-27 08:56:21.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-27 08:56:21.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-10-27 08:56:21.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-10-27 08:56:21.000000 drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1568 2022-10-27 08:56:21.975417 drf-simple-jwt-2fa-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      161 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:11:07.890527 drf-simple-jwt-2fa-1.2.6/
+-rw-rw-rw-   0        0        0     1092 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     5059 2024-04-10 08:11:07.890527 drf-simple-jwt-2fa-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2022-01-11 13:33:30.000000 drf-simple-jwt-2fa-1.2.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 08:11:07.872571 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/
+-rw-rw-rw-   0        0        0      186 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/__init__.py
+-rw-rw-rw-   0        0        0      131 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/authentication.py
+-rw-rw-rw-   0        0        0      588 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/exceptions.py
+-rw-rw-rw-   0        0        0     1343 2022-10-27 08:56:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/sending.py
+-rw-rw-rw-   0        0        0     6198 2022-01-19 14:00:23.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/serializers.py
+-rw-rw-rw-   0        0        0     1714 2022-01-11 15:44:49.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:11:07.889526 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/__init__.py
+-rw-rw-rw-   0        0        0      308 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/factories.py
+-rw-rw-rw-   0        0        0     3712 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_endpoints.py
+-rw-rw-rw-   0        0        0     6985 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_throttling.py
+-rw-rw-rw-   0        0        0     4473 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_token_manager.py
+-rw-rw-rw-   0        0        0     3188 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/utils.py
+-rw-rw-rw-   0        0        0     1799 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/throttling.py
+-rw-rw-rw-   0        0        0     4319 2022-01-19 14:01:00.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/token_manager.py
+-rw-rw-rw-   0        0        0      335 2024-04-10 08:08:02.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/urls.py
+-rw-rw-rw-   0        0        0     1125 2022-01-03 11:13:01.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/utils.py
+-rw-rw-rw-   0        0        0      774 2022-01-04 10:58:27.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/views.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:11:07.879593 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/
+-rw-rw-rw-   0        0        0     5059 2024-04-10 08:11:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      837 2024-04-10 08:11:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:11:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-10 08:11:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 08:11:07.000000 drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1568 2024-04-10 08:11:07.892525 drf-simple-jwt-2fa-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      161 2022-01-11 12:45:54.000000 drf-simple-jwt-2fa-1.2.6/setup.py
```

### Comparing `drf-simple-jwt-2fa-1.2.5/LICENSE` & `drf-simple-jwt-2fa-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/PKG-INFO` & `drf-simple-jwt-2fa-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: drf-simple-jwt-2fa
-Version: 1.2.5
+Version: 1.2.6
 Summary: Django Rest Framework Simple JWT 2FA
 Home-page: https://github.com/GauthierSgds/drf-simple-jwt-2fa
 Maintainer: Gauthier Segonds
 Maintainer-email: gauthier.segonds@lugos.fr
 License: MIT
 Keywords: Authentication,Two Factor,Django Rest Framework,JSON Web Token,Simple JWT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django Rest Framework JWT 2FA
 =============================
```

### Comparing `drf-simple-jwt-2fa-1.2.5/README.rst` & `drf-simple-jwt-2fa-1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/exceptions.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/sending.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/sending.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/serializers.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/settings.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/settings.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_endpoints.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_throttling.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_throttling.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/test_token_manager.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/tests/utils.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/tests/utils.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/throttling.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/throttling.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/token_manager.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/token_manager.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/utils.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/utils.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa/views.py` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa/views.py`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/PKG-INFO` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: drf-simple-jwt-2fa
-Version: 1.2.5
+Version: 1.2.6
 Summary: Django Rest Framework Simple JWT 2FA
 Home-page: https://github.com/GauthierSgds/drf-simple-jwt-2fa
 Maintainer: Gauthier Segonds
 Maintainer-email: gauthier.segonds@lugos.fr
 License: MIT
 Keywords: Authentication,Two Factor,Django Rest Framework,JSON Web Token,Simple JWT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django Rest Framework JWT 2FA
 =============================
```

### Comparing `drf-simple-jwt-2fa-1.2.5/drf_simple_jwt_2fa.egg-info/SOURCES.txt` & `drf-simple-jwt-2fa-1.2.6/drf_simple_jwt_2fa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-simple-jwt-2fa-1.2.5/setup.cfg` & `drf-simple-jwt-2fa-1.2.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d73 696d 706c 652d 6a77   = drf-simple-jw
 00000020: 742d 3266 610d 0a76 6572 7369 6f6e 203d  t-2fa..version =
-00000030: 2031 2e32 2e35 0d0a 6465 7363 7269 7074   1.2.5..descript
+00000030: 2031 2e32 2e36 0d0a 6465 7363 7269 7074   1.2.6..descript
 00000040: 696f 6e20 3d20 446a 616e 676f 2052 6573  ion = Django Res
 00000050: 7420 4672 616d 6577 6f72 6b20 5369 6d70  t Framework Simp
 00000060: 6c65 204a 5754 2032 4641 0d0a 6c6f 6e67  le JWT 2FA..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
 00000080: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
 00000090: 2f6d 6172 6b64 6f77 6e0d 0a6c 6f6e 675f  /markdown..long_
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
@@ -31,22 +31,22 @@
 000001e0: 6965 7273 203d 200d 0a09 4465 7665 6c6f  iers = ...Develo
 000001f0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
 00000200: 3420 2d20 4265 7461 0d0a 0945 6e76 6972  4 - Beta...Envir
 00000210: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
 00000220: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
 00000230: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
 00000240: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000250: 6a61 6e67 6f20 3a3a 2033 2e30 0d0a 0949  jango :: 3.0...I
+00000250: 6a61 6e67 6f20 3a3a 2034 2e30 0d0a 0949  jango :: 4.0...I
 00000260: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
 00000270: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
 00000280: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
 00000290: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
 000002a0: 656e 740d 0a09 5072 6f67 7261 6d6d 696e  ent...Programmin
 000002b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002c0: 7468 6f6e 203a 3a20 332e 370d 0a09 546f  thon :: 3.7...To
+000002c0: 7468 6f6e 203a 3a20 332e 380d 0a09 546f  thon :: 3.8...To
 000002d0: 7069 6320 3a3a 2049 6e74 6572 6e65 7420  pic :: Internet 
 000002e0: 3a3a 2057 5757 2f48 5454 5020 3a3a 2053  :: WWW/HTTP :: S
 000002f0: 6573 7369 6f6e 0d0a 0d0a 5b6f 7074 696f  ession....[optio
 00000300: 6e73 5d0d 0a69 6e63 6c75 6465 5f70 6163  ns]..include_pac
 00000310: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
 00000320: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000330: 643a 0d0a 696e 7374 616c 6c5f 7265 7175  d:..install_requ
```

