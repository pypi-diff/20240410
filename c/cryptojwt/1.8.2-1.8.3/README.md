# Comparing `tmp/cryptojwt-1.8.2.tar.gz` & `tmp/cryptojwt-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptojwt-1.8.2.tar", max compression
+gzip compressed data, was "cryptojwt-1.8.3.tar", max compression
```

## Comparing `cryptojwt-1.8.2.tar` & `cryptojwt-1.8.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rwxr-xr-x   0        0        0    10759 2022-04-27 12:41:12.237425 cryptojwt-1.8.2/LICENSE
--rw-r--r--   0        0        0      575 2022-04-27 12:41:12.237425 cryptojwt-1.8.2/README.md
--rw-r--r--   0        0        0     1342 2022-04-27 12:41:12.237425 cryptojwt-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      877 2022-04-27 12:41:12.237425 cryptojwt-1.8.2/src/cryptojwt/__init__.py
--rw-r--r--   0        0        0     1821 2022-04-27 12:41:12.237425 cryptojwt-1.8.2/src/cryptojwt/exception.py
--rw-r--r--   0        0        0     1119 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/__init__.py
--rw-r--r--   0        0        0     4388 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/aes.py
--rw-r--r--   0        0        0      606 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/exception.py
--rw-r--r--   0        0        0     2064 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/fernet.py
--rw-r--r--   0        0        0     7204 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwe.py
--rw-r--r--   0        0        0     7770 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_ec.py
--rw-r--r--   0        0        0     3050 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_hmac.py
--rw-r--r--   0        0        0     3638 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_rsa.py
--rw-r--r--   0        0        0     2749 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwekey.py
--rw-r--r--   0        0        0     1414 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/jwenc.py
--rw-r--r--   0        0        0     1775 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/rsa.py
--rw-r--r--   0        0        0     2910 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwe/utils.py
--rw-r--r--   0        0        0    10598 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/__init__.py
--rw-r--r--   0        0        0     1906 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/asym.py
--rw-r--r--   0        0        0    11266 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/ec.py
--rw-r--r--   0        0        0     4607 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/hmac.py
--rw-r--r--   0        0        0     6948 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/jwk.py
--rw-r--r--   0        0        0    15334 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/rsa.py
--rw-r--r--   0        0        0      728 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/utils.py
--rw-r--r--   0        0        0      905 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/wrap.py
--rw-r--r--   0        0        0     4102 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwk/x509.py
--rw-r--r--   0        0        0      354 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/__init__.py
--rw-r--r--   0        0        0     3837 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/dsa.py
--rw-r--r--   0        0        0      329 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/exception.py
--rw-r--r--   0        0        0     1535 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/hmac.py
--rw-r--r--   0        0        0    15209 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/jws.py
--rw-r--r--   0        0        0     2183 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/pss.py
--rw-r--r--   0        0        0     1580 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/rsa.py
--rw-r--r--   0        0        0     2690 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jws/utils.py
--rwxr-xr-x   0        0        0    12355 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwt.py
--rw-r--r--   0        0        0     8704 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/jwx.py
--rwxr-xr-x   0        0        0    38936 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/key_bundle.py
--rwxr-xr-x   0        0        0    21120 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/key_issuer.py
--rwxr-xr-x   0        0        0    29366 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/key_jar.py
--rw-r--r--   0        0        0        0 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/serialize/__init__.py
--rw-r--r--   0        0        0      472 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/serialize/item.py
--rw-r--r--   0        0        0     4497 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/simple_jwt.py
--rw-r--r--   0        0        0        0 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/tools/__init__.py
--rwxr-xr-x   0        0        0     4221 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/tools/jwtpeek.py
--rw-r--r--   0        0        0     6695 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/tools/keyconv.py
--rw-r--r--   0        0        0     2172 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/tools/keygen.py
--rw-r--r--   0        0        0     6837 2022-04-27 12:41:12.241425 cryptojwt-1.8.2/src/cryptojwt/utils.py
--rw-r--r--   0        0        0     1705 2022-04-27 12:41:25.174682 cryptojwt-1.8.2/setup.py
--rw-r--r--   0        0        0     1387 2022-04-27 12:41:25.175222 cryptojwt-1.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0    10759 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/LICENSE
+-rw-r--r--   0        0        0      575 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/README.md
+-rw-r--r--   0        0        0     1342 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      877 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/__init__.py
+-rw-r--r--   0        0        0     1821 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/exception.py
+-rw-r--r--   0        0        0     1119 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/__init__.py
+-rw-r--r--   0        0        0     4388 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/aes.py
+-rw-r--r--   0        0        0      606 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/exception.py
+-rw-r--r--   0        0        0     2064 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/fernet.py
+-rw-r--r--   0        0        0     7204 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwe.py
+-rw-r--r--   0        0        0     7770 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_ec.py
+-rw-r--r--   0        0        0     3050 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_hmac.py
+-rw-r--r--   0        0        0     3638 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_rsa.py
+-rw-r--r--   0        0        0     2749 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwekey.py
+-rw-r--r--   0        0        0     1414 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/jwenc.py
+-rw-r--r--   0        0        0     1775 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/rsa.py
+-rw-r--r--   0        0        0     2910 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwe/utils.py
+-rw-r--r--   0        0        0    10598 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/__init__.py
+-rw-r--r--   0        0        0     1906 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/asym.py
+-rw-r--r--   0        0        0    11266 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/ec.py
+-rw-r--r--   0        0        0     4607 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/hmac.py
+-rw-r--r--   0        0        0     6948 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/jwk.py
+-rw-r--r--   0        0        0    15334 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/rsa.py
+-rw-r--r--   0        0        0      728 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/utils.py
+-rw-r--r--   0        0        0      905 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/wrap.py
+-rw-r--r--   0        0        0     4102 2022-06-22 09:14:16.617725 cryptojwt-1.8.3/src/cryptojwt/jwk/x509.py
+-rw-r--r--   0        0        0      354 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/__init__.py
+-rw-r--r--   0        0        0     3837 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/dsa.py
+-rw-r--r--   0        0        0      329 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/exception.py
+-rw-r--r--   0        0        0     1535 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/hmac.py
+-rw-r--r--   0        0        0    15208 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/jws.py
+-rw-r--r--   0        0        0     2183 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/pss.py
+-rw-r--r--   0        0        0     1580 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/rsa.py
+-rw-r--r--   0        0        0     2690 2022-06-22 09:14:16.625725 cryptojwt-1.8.3/src/cryptojwt/jws/utils.py
+-rwxr-xr-x   0        0        0    12355 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/jwt.py
+-rw-r--r--   0        0        0     8704 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/jwx.py
+-rwxr-xr-x   0        0        0    38936 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/key_bundle.py
+-rwxr-xr-x   0        0        0    21120 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/key_issuer.py
+-rwxr-xr-x   0        0        0    29366 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/key_jar.py
+-rw-r--r--   0        0        0        0 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/serialize/__init__.py
+-rw-r--r--   0        0        0      472 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/serialize/item.py
+-rw-r--r--   0        0        0     4497 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/simple_jwt.py
+-rw-r--r--   0        0        0        0 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/tools/__init__.py
+-rwxr-xr-x   0        0        0     4221 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/tools/jwtpeek.py
+-rw-r--r--   0        0        0     6695 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/tools/keyconv.py
+-rw-r--r--   0        0        0     2172 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/tools/keygen.py
+-rw-r--r--   0        0        0     6837 2022-06-22 09:14:16.629725 cryptojwt-1.8.3/src/cryptojwt/utils.py
+-rw-r--r--   0        0        0     1705 2022-06-22 09:14:30.676236 cryptojwt-1.8.3/setup.py
+-rw-r--r--   0        0        0     1387 2022-06-22 09:14:30.676630 cryptojwt-1.8.3/PKG-INFO
```

### Comparing `cryptojwt-1.8.2/LICENSE` & `cryptojwt-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/README.md` & `cryptojwt-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/pyproject.toml` & `cryptojwt-1.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
 ]
 
 [tool.poetry]
 name = "cryptojwt"
-version = "1.8.2"
+version = "1.8.3"
 description = "Python implementation of JWT, JWE, JWS and JWK"
 authors = ["Roland Hedberg <roland@catalogix.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT"
 readme = "README.md"
 packages = [
     { include = "cryptojwt", from = "src" }
```

### Comparing `cryptojwt-1.8.2/src/cryptojwt/__init__.py` & `cryptojwt-1.8.3/src/cryptojwt/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/exception.py` & `cryptojwt-1.8.3/src/cryptojwt/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/__init__.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/aes.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/aes.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/exception.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/fernet.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/fernet.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwe.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwe.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_ec.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_ec.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_hmac.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwe_rsa.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwe_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwekey.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwekey.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/jwenc.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/jwenc.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/rsa.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwe/utils.py` & `cryptojwt-1.8.3/src/cryptojwt/jwe/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/__init__.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/asym.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/asym.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/ec.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/ec.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/hmac.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/jwk.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/jwk.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/rsa.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/utils.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/wrap.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/wrap.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwk/x509.py` & `cryptojwt-1.8.3/src/cryptojwt/jwk/x509.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/dsa.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/hmac.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/jws.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/jws.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         _headers = self._header
         _headers.update(kwargs)
 
         key, xargs, _alg = self.alg_keys(keys, "sig", protected)
 
         if "typ" in self:
-            xargs["type"] = self["typ"]
+            xargs["typ"] = self["typ"]
 
         _headers.update(xargs)
         jwt = JWSig(**_headers)
         if _alg == "none":
             return jwt.pack(parts=[self.msg, ""])
 
         # All other cases
```

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/pss.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/pss.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/rsa.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jws/utils.py` & `cryptojwt-1.8.3/src/cryptojwt/jws/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwt.py` & `cryptojwt-1.8.3/src/cryptojwt/jwt.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/jwx.py` & `cryptojwt-1.8.3/src/cryptojwt/jwx.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/key_bundle.py` & `cryptojwt-1.8.3/src/cryptojwt/key_bundle.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/key_issuer.py` & `cryptojwt-1.8.3/src/cryptojwt/key_issuer.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/key_jar.py` & `cryptojwt-1.8.3/src/cryptojwt/key_jar.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/simple_jwt.py` & `cryptojwt-1.8.3/src/cryptojwt/simple_jwt.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/tools/jwtpeek.py` & `cryptojwt-1.8.3/src/cryptojwt/tools/jwtpeek.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/tools/keyconv.py` & `cryptojwt-1.8.3/src/cryptojwt/tools/keyconv.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/tools/keygen.py` & `cryptojwt-1.8.3/src/cryptojwt/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/src/cryptojwt/utils.py` & `cryptojwt-1.8.3/src/cryptojwt/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.2/setup.py` & `cryptojwt-1.8.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 entry_points = \
 {'console_scripts': ['jwkconv = cryptojwt.tools.keyconv:main',
                      'jwkgen = cryptojwt.tools.keygen:main',
                      'jwtpeek = cryptojwt.tools.jwtpeek:main']}
 
 setup_kwargs = {
     'name': 'cryptojwt',
-    'version': '1.8.2',
+    'version': '1.8.3',
     'description': 'Python implementation of JWT, JWE, JWS and JWK',
     'long_description': '# cryptojwt\n\n![License](https://img.shields.io/badge/license-Apache%202-blue.svg)\n![Python version](https://img.shields.io/badge/python-3.6%20%7C%203.7%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nAn implementation of the JSON cryptographic specs JWS, JWE, JWK, and JWA [RFC 7515-7518] and JSON Web Token (JWT) [RFC 7519]\n\nPlease read the [Official Documentation](https://cryptojwt.readthedocs.io/en/latest/) for getting usage examples and further informations.\n',
     'author': 'Roland Hedberg',
     'author_email': 'roland@catalogix.se',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT',
```

### Comparing `cryptojwt-1.8.2/PKG-INFO` & `cryptojwt-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptojwt
-Version: 1.8.2
+Version: 1.8.3
 Summary: Python implementation of JWT, JWE, JWS and JWK
 Home-page: https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT
 License: Apache-2.0
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

