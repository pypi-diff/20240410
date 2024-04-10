# Comparing `tmp/pulumi_venafi-1.8.0a1712403151.tar.gz` & `tmp/pulumi_venafi-1.8.0a1712653977.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.8.0a1712403151.tar", last modified: Sat Apr  6 11:38:17 2024, max compression
+gzip compressed data, was "pulumi_venafi-1.8.0a1712653977.tar", last modified: Tue Apr  9 09:16:51 2024, max compression
```

## Comparing `pulumi_venafi-1.8.0a1712403151.tar` & `pulumi_venafi-1.8.0a1712653977.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    48936 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21014 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53759 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48936 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53759 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-09 09:16:51.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 09:16:51.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:16:51.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 09:16:51.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 09:16:51.000000 pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 09:16:44.000000 pulumi_venafi-1.8.0a1712653977/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:16:51.303233 pulumi_venafi-1.8.0a1712653977/setup.cfg
```

### Comparing `pulumi_venafi-1.8.0a1712403151/PKG-INFO` & `pulumi_venafi-1.8.0a1712653977/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.8.0a1712403151
+Version: 1.8.0a1712653977
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.8.0a1712403151/README.md` & `pulumi_venafi-1.8.0a1712653977/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/__init__.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/certificate.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.pyi` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,41 +12,51 @@
 accessToken: Optional[str]
 """
 Access token for Venafi TLSPDC, user should use this for authentication
 """
 
 apiKey: Optional[str]
 """
-API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
 """
 
 clientId: Optional[str]
 """
 application that will be using the token
 """
 
 devMode: Optional[bool]
 """
 When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
 Venafi as a Service or Trust Protection Platform. Useful for development and testing.
 """
 
+idpJwt: Optional[str]
+"""
+JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+"""
+
 p12CertFilename: Optional[str]
 """
 Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
 TLSPDC
 """
 
 p12CertPassword: Optional[str]
 """
 Password for the PKCS#12 keystore declared in p12_cert
 """
 
 skipRetirement: Optional[bool]
 
+tokenUrl: Optional[str]
+"""
+Endpoint URL to request new Venafi Control Plane access tokens
+"""
+
 tppPassword: Optional[str]
 """
 Password for WebSDK user. Example: password
 """
 
 tppUsername: Optional[str]
 """
```

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/config/vars.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Access token for Venafi TLSPDC, user should use this for authentication
         """
         return __config__.get('accessToken')
 
     @property
     def api_key(self) -> Optional[str]:
         """
-        API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+        API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         """
         return __config__.get('apiKey')
 
     @property
     def client_id(self) -> Optional[str]:
         """
         application that will be using the token
@@ -41,14 +41,21 @@
         """
         When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
         Venafi as a Service or Trust Protection Platform. Useful for development and testing.
         """
         return __config__.get_bool('devMode')
 
     @property
+    def idp_jwt(self) -> Optional[str]:
+        """
+        JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+        """
+        return __config__.get('idpJwt')
+
+    @property
     def p12_cert_filename(self) -> Optional[str]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
         """
         return __config__.get('p12CertFilename')
 
@@ -60,14 +67,21 @@
         return __config__.get('p12CertPassword')
 
     @property
     def skip_retirement(self) -> Optional[bool]:
         return __config__.get_bool('skipRetirement')
 
     @property
+    def token_url(self) -> Optional[str]:
+        """
+        Endpoint URL to request new Venafi Control Plane access tokens
+        """
+        return __config__.get('tokenUrl')
+
+    @property
     def tpp_password(self) -> Optional[str]:
         """
         Password for WebSDK user. Example: password
         """
         return __config__.get('tppPassword')
 
     @property
```

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/policy.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/provider.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,33 +14,37 @@
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
+                 idp_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
+                 token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] access_token: Access token for Venafi TLSPDC, user should use this for authentication
-        :param pulumi.Input[str] api_key: API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+        :param pulumi.Input[str] api_key: API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         :param pulumi.Input[str] client_id: application that will be using the token
         :param pulumi.Input[bool] dev_mode: When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
                Venafi as a Service or Trust Protection Platform. Useful for development and testing.
+        :param pulumi.Input[str] idp_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         :param pulumi.Input[str] p12_cert_filename: Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
                TLSPDC
         :param pulumi.Input[str] p12_cert_password: Password for the PKCS#12 keystore declared in p12_cert
         :param pulumi.Input[bool] skip_retirement: When true, certificates will not be retired on Venafi platforms when terraform destroy is run. Default is false.
+        :param pulumi.Input[str] token_url: Endpoint URL to request new Venafi Control Plane access tokens
         :param pulumi.Input[str] tpp_password: Password for WebSDK user. Example: password
         :param pulumi.Input[str] tpp_username: WebSDK user for Venafi TLSPDC. Example: admin
         :param pulumi.Input[str] trust_bundle: Use to specify a PEM-formatted file that contains certificates to be trust anchors for all communications with the
                Venafi Web Service. Example: trust_bundle = "${file("chain.pem")}"
         :param pulumi.Input[str] url: The Venafi Platform URL. Example: https://tpp.venafi.example/vedsdk
         :param pulumi.Input[str] zone: DN of the Venafi TLSPDC policy folder or name of the Venafi as a Service application plus issuing template alias.
                Example for Platform: testPolicy\\\\vault Example for Venafi as a Service: myApp\\\\Default
@@ -49,20 +53,24 @@
             pulumi.set(__self__, "access_token", access_token)
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if dev_mode is not None:
             pulumi.set(__self__, "dev_mode", dev_mode)
+        if idp_jwt is not None:
+            pulumi.set(__self__, "idp_jwt", idp_jwt)
         if p12_cert_filename is not None:
             pulumi.set(__self__, "p12_cert_filename", p12_cert_filename)
         if p12_cert_password is not None:
             pulumi.set(__self__, "p12_cert_password", p12_cert_password)
         if skip_retirement is not None:
             pulumi.set(__self__, "skip_retirement", skip_retirement)
+        if token_url is not None:
+            pulumi.set(__self__, "token_url", token_url)
         if tpp_password is not None:
             warnings.warn(""", please use access_token instead""", DeprecationWarning)
             pulumi.log.warn("""tpp_password is deprecated: , please use access_token instead""")
         if tpp_password is not None:
             pulumi.set(__self__, "tpp_password", tpp_password)
         if tpp_username is not None:
             warnings.warn(""", please use access_token instead""", DeprecationWarning)
@@ -88,15 +96,15 @@
     def access_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_token", value)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> Optional[pulumi.Input[str]]:
         """
-        API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+        API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         """
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
@@ -122,14 +130,26 @@
         return pulumi.get(self, "dev_mode")
 
     @dev_mode.setter
     def dev_mode(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dev_mode", value)
 
     @property
+    @pulumi.getter(name="idpJwt")
+    def idp_jwt(self) -> Optional[pulumi.Input[str]]:
+        """
+        JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+        """
+        return pulumi.get(self, "idp_jwt")
+
+    @idp_jwt.setter
+    def idp_jwt(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "idp_jwt", value)
+
+    @property
     @pulumi.getter(name="p12CertFilename")
     def p12_cert_filename(self) -> Optional[pulumi.Input[str]]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
         """
         return pulumi.get(self, "p12_cert_filename")
@@ -159,14 +179,26 @@
         return pulumi.get(self, "skip_retirement")
 
     @skip_retirement.setter
     def skip_retirement(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_retirement", value)
 
     @property
+    @pulumi.getter(name="tokenUrl")
+    def token_url(self) -> Optional[pulumi.Input[str]]:
+        """
+        Endpoint URL to request new Venafi Control Plane access tokens
+        """
+        return pulumi.get(self, "token_url")
+
+    @token_url.setter
+    def token_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_url", value)
+
+    @property
     @pulumi.getter(name="tppPassword")
     def tpp_password(self) -> Optional[pulumi.Input[str]]:
         """
         Password for WebSDK user. Example: password
         """
         warnings.warn(""", please use access_token instead""", DeprecationWarning)
         pulumi.log.warn("""tpp_password is deprecated: , please use access_token instead""")
@@ -236,17 +268,19 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
+                 idp_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
+                 token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -254,22 +288,24 @@
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_token: Access token for Venafi TLSPDC, user should use this for authentication
-        :param pulumi.Input[str] api_key: API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+        :param pulumi.Input[str] api_key: API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         :param pulumi.Input[str] client_id: application that will be using the token
         :param pulumi.Input[bool] dev_mode: When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
                Venafi as a Service or Trust Protection Platform. Useful for development and testing.
+        :param pulumi.Input[str] idp_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         :param pulumi.Input[str] p12_cert_filename: Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
                TLSPDC
         :param pulumi.Input[str] p12_cert_password: Password for the PKCS#12 keystore declared in p12_cert
         :param pulumi.Input[bool] skip_retirement: When true, certificates will not be retired on Venafi platforms when terraform destroy is run. Default is false.
+        :param pulumi.Input[str] token_url: Endpoint URL to request new Venafi Control Plane access tokens
         :param pulumi.Input[str] tpp_password: Password for WebSDK user. Example: password
         :param pulumi.Input[str] tpp_username: WebSDK user for Venafi TLSPDC. Example: admin
         :param pulumi.Input[str] trust_bundle: Use to specify a PEM-formatted file that contains certificates to be trust anchors for all communications with the
                Venafi Web Service. Example: trust_bundle = "${file("chain.pem")}"
         :param pulumi.Input[str] url: The Venafi Platform URL. Example: https://tpp.venafi.example/vedsdk
         :param pulumi.Input[str] zone: DN of the Venafi TLSPDC policy folder or name of the Venafi as a Service application plus issuing template alias.
                Example for Platform: testPolicy\\\\vault Example for Venafi as a Service: myApp\\\\Default
@@ -301,17 +337,19 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
+                 idp_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
+                 token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -322,23 +360,25 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["access_token"] = None if access_token is None else pulumi.Output.secret(access_token)
             __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["dev_mode"] = pulumi.Output.from_input(dev_mode).apply(pulumi.runtime.to_json) if dev_mode is not None else None
+            __props__.__dict__["idp_jwt"] = None if idp_jwt is None else pulumi.Output.secret(idp_jwt)
             __props__.__dict__["p12_cert_filename"] = p12_cert_filename
             __props__.__dict__["p12_cert_password"] = None if p12_cert_password is None else pulumi.Output.secret(p12_cert_password)
             __props__.__dict__["skip_retirement"] = pulumi.Output.from_input(skip_retirement).apply(pulumi.runtime.to_json) if skip_retirement is not None else None
+            __props__.__dict__["token_url"] = None if token_url is None else pulumi.Output.secret(token_url)
             __props__.__dict__["tpp_password"] = None if tpp_password is None else pulumi.Output.secret(tpp_password)
             __props__.__dict__["tpp_username"] = tpp_username
             __props__.__dict__["trust_bundle"] = trust_bundle
             __props__.__dict__["url"] = url
             __props__.__dict__["zone"] = zone
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "apiKey", "p12CertPassword", "tppPassword"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "apiKey", "idpJwt", "p12CertPassword", "tokenUrl", "tppPassword"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'venafi',
             resource_name,
             __props__,
             opts)
 
@@ -350,27 +390,35 @@
         """
         return pulumi.get(self, "access_token")
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Output[Optional[str]]:
         """
-        API key for Venafi as a Service. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
+        API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         """
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Output[Optional[str]]:
         """
         application that will be using the token
         """
         return pulumi.get(self, "client_id")
 
     @property
+    @pulumi.getter(name="idpJwt")
+    def idp_jwt(self) -> pulumi.Output[Optional[str]]:
+        """
+        JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+        """
+        return pulumi.get(self, "idp_jwt")
+
+    @property
     @pulumi.getter(name="p12CertFilename")
     def p12_cert_filename(self) -> pulumi.Output[Optional[str]]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
         """
         return pulumi.get(self, "p12_cert_filename")
@@ -380,14 +428,22 @@
     def p12_cert_password(self) -> pulumi.Output[Optional[str]]:
         """
         Password for the PKCS#12 keystore declared in p12_cert
         """
         return pulumi.get(self, "p12_cert_password")
 
     @property
+    @pulumi.getter(name="tokenUrl")
+    def token_url(self) -> pulumi.Output[Optional[str]]:
+        """
+        Endpoint URL to request new Venafi Control Plane access tokens
+        """
+        return pulumi.get(self, "token_url")
+
+    @property
     @pulumi.getter(name="tppPassword")
     def tpp_password(self) -> pulumi.Output[Optional[str]]:
         """
         Password for WebSDK user. Example: password
         """
         warnings.warn(""", please use access_token instead""", DeprecationWarning)
         pulumi.log.warn("""tpp_password is deprecated: , please use access_token instead""")
```

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.8.0a1712403151
+Version: 1.8.0a1712653977
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.8.0a1712653977/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1712403151/pyproject.toml` & `pulumi_venafi-1.8.0a1712653977/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_venafi"
   description = "A Pulumi package for creating and managing venafi cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "venafi"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.8.0a1712403151"
+  version = "1.8.0a1712653977"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-venafi"
 
 [build-system]
```

