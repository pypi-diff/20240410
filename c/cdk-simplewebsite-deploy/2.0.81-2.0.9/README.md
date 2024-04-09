# Comparing `tmp/cdk-simplewebsite-deploy-2.0.81.tar.gz` & `tmp/cdk-simplewebsite-deploy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-simplewebsite-deploy-2.0.81.tar", last modified: Tue Apr  9 22:48:19 2024, max compression
+gzip compressed data, was "cdk-simplewebsite-deploy-2.0.9.tar", last modified: Sun Feb 13 00:42:55 2022, max compression
```

## Comparing `cdk-simplewebsite-deploy-2.0.81.tar` & `cdk-simplewebsite-deploy-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:19.596637 cdk-simplewebsite-deploy-2.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-09 22:48:19.596637 cdk-simplewebsite-deploy-2.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:48:19.596637 cdk-simplewebsite-deploy-2.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:19.592637 cdk-simplewebsite-deploy-2.0.81/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:19.592637 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:19.592637 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.81.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:48:07.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:19.592637 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-09 22:48:19.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 22:48:19.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:48:19.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 22:48:19.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 22:48:19.000000 cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6263 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.214831 cdk-simplewebsite-deploy-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.214831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/
+-rw-r--r--   0 runner    (1001) docker     (121)    17904 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23921 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 00:42:37.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 00:42:55.218831 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-02-13 00:42:55.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-13 00:42:54.000000 cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/top_level.txt
```

### Comparing `cdk-simplewebsite-deploy-2.0.81/LICENSE` & `cdk-simplewebsite-deploy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-simplewebsite-deploy-2.0.81/PKG-INFO` & `cdk-simplewebsite-deploy-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk-simplewebsite-deploy
-Version: 2.0.81
+Version: 2.0.9
 Summary: This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.
 Home-page: https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Author: Thon Becker<thon.becker@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SnapPetal/cdk-simplewebsite-deploy
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Build](https://github.com/SnapPetal/cdk-simplewebsite-deploy/workflows/build/badge.svg)
 ![Release](https://github.com/SnapPetal/cdk-simplewebsite-deploy/workflows/release/badge.svg?branch=main)
 
@@ -252,7 +253,9 @@
                              hosted_zone='example.com',
                              sub_domain='www.example.com')
 ```
 
 ## License
 
 Distributed under the [Apache-2.0](./LICENSE) license.
+
+
```

### Comparing `cdk-simplewebsite-deploy-2.0.81/README.md` & `cdk-simplewebsite-deploy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-simplewebsite-deploy-2.0.81/setup.py` & `cdk-simplewebsite-deploy-2.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-simplewebsite-deploy",
-    "version": "2.0.81",
+    "version": "2.0.9",
     "description": "This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.",
     "license": "Apache-2.0",
     "url": "https://github.com/SnapPetal/cdk-simplewebsite-deploy",
     "long_description_content_type": "text/markdown",
     "author": "Thon Becker<thon.becker@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,36 @@
     },
     "packages": [
         "cdk_simplewebsite_deploy",
         "cdk_simplewebsite_deploy._jsii"
     ],
     "package_data": {
         "cdk_simplewebsite_deploy._jsii": [
-            "cdk-simplewebsite-deploy@2.0.81.jsii.tgz"
+            "cdk-simplewebsite-deploy@2.0.9.jsii.tgz"
         ],
         "cdk_simplewebsite_deploy": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.8",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib>=2.102.0, <3.0.0",
-        "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "aws-cdk-lib>=2.12.0, <3.0.0",
+        "constructs>=10.0.61, <11.0.0",
+        "jsii>=1.53.0, <2.0.0",
+        "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy/__init__.py` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -231,32 +231,27 @@
                              sub_domain='www.example.com')
 ```
 
 ## License
 
 Distributed under the [Apache-2.0](./LICENSE) license.
 '''
-from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
-
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
-from typeguard import check_type
-
 from ._jsii import *
 
-import constructs as _constructs_77d1e7e8
+import constructs
 
 
 @jsii.data_type(
     jsii_type="cdk-simplewebsite-deploy.BasicSiteConfiguration",
     jsii_struct_bases=[],
     name_mapping={
         "hosted_zone": "hostedZone",
@@ -276,21 +271,15 @@
     ) -> None:
         '''
         :param hosted_zone: Hosted Zone used to create the DNS record for the website.
         :param index_doc: The index document of the website.
         :param website_folder: Local path to the website folder you want to deploy on S3.
         :param error_doc: The error document of the website. Default: - No error document.
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__55e1d457f7f88b408ecc128e65052c3c69d68b852e2406239079c5f4b76a672d)
-            check_type(argname="argument hosted_zone", value=hosted_zone, expected_type=type_hints["hosted_zone"])
-            check_type(argname="argument index_doc", value=index_doc, expected_type=type_hints["index_doc"])
-            check_type(argname="argument website_folder", value=website_folder, expected_type=type_hints["website_folder"])
-            check_type(argname="argument error_doc", value=error_doc, expected_type=type_hints["error_doc"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "hosted_zone": hosted_zone,
             "index_doc": index_doc,
             "website_folder": website_folder,
         }
         if error_doc is not None:
             self._values["error_doc"] = error_doc
 
@@ -366,24 +355,15 @@
         :param index_doc: The index document of the website.
         :param website_folder: Local path to the website folder you want to deploy on S3.
         :param domain: Used to deploy a Cloudfront site with a single domain. e.g. sample.example.com If you include a value for both domain and subDomain, an error will be thrown. Default: - no value
         :param error_doc: The error document of the website. Default: - No error document.
         :param price_class: The price class determines how many edge locations CloudFront will use for your distribution. Default: PriceClass.PRICE_CLASS_100.
         :param sub_domain: The sub-domain name you want to deploy. e.g. www.example.com If you include a value for both domain and subDomain, an error will be thrown. Default: - no value
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0e850e19fcfb3492790ff3ec407df63abfa515b2415ed714c8499dc3239a822f)
-            check_type(argname="argument hosted_zone", value=hosted_zone, expected_type=type_hints["hosted_zone"])
-            check_type(argname="argument index_doc", value=index_doc, expected_type=type_hints["index_doc"])
-            check_type(argname="argument website_folder", value=website_folder, expected_type=type_hints["website_folder"])
-            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument error_doc", value=error_doc, expected_type=type_hints["error_doc"])
-            check_type(argname="argument price_class", value=price_class, expected_type=type_hints["price_class"])
-            check_type(argname="argument sub_domain", value=sub_domain, expected_type=type_hints["sub_domain"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "hosted_zone": hosted_zone,
             "index_doc": index_doc,
             "website_folder": website_folder,
         }
         if domain is not None:
             self._values["domain"] = domain
         if error_doc is not None:
@@ -469,21 +449,21 @@
     def __repr__(self) -> str:
         return "CloudfrontSiteConfiguration(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class CreateBasicSite(
-    _constructs_77d1e7e8.Construct,
+    constructs.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-simplewebsite-deploy.CreateBasicSite",
 ):
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         hosted_zone: builtins.str,
         index_doc: builtins.str,
         website_folder: builtins.str,
         error_doc: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -491,36 +471,32 @@
         :param scope: -
         :param id: -
         :param hosted_zone: Hosted Zone used to create the DNS record for the website.
         :param index_doc: The index document of the website.
         :param website_folder: Local path to the website folder you want to deploy on S3.
         :param error_doc: The error document of the website. Default: - No error document.
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9b1cd29a96c6c8b996276e29a8e2730cf2a3c15a5c12e1c5bc0e23986cb136f7)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = BasicSiteConfiguration(
             hosted_zone=hosted_zone,
             index_doc=index_doc,
             website_folder=website_folder,
             error_doc=error_doc,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 class CreateCloudfrontSite(
-    _constructs_77d1e7e8.Construct,
+    constructs.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-simplewebsite-deploy.CreateCloudfrontSite",
 ):
     def __init__(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         *,
         hosted_zone: builtins.str,
         index_doc: builtins.str,
         website_folder: builtins.str,
         domain: typing.Optional[builtins.str] = None,
         error_doc: typing.Optional[builtins.str] = None,
@@ -534,18 +510,14 @@
         :param index_doc: The index document of the website.
         :param website_folder: Local path to the website folder you want to deploy on S3.
         :param domain: Used to deploy a Cloudfront site with a single domain. e.g. sample.example.com If you include a value for both domain and subDomain, an error will be thrown. Default: - no value
         :param error_doc: The error document of the website. Default: - No error document.
         :param price_class: The price class determines how many edge locations CloudFront will use for your distribution. Default: PriceClass.PRICE_CLASS_100.
         :param sub_domain: The sub-domain name you want to deploy. e.g. www.example.com If you include a value for both domain and subDomain, an error will be thrown. Default: - no value
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__35939f41a1cbd87bd7b3fa20b126e3c79332b77b538ed266f3ea73f154b3c68a)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CloudfrontSiteConfiguration(
             hosted_zone=hosted_zone,
             index_doc=index_doc,
             website_folder=website_folder,
             domain=domain,
             error_doc=error_doc,
             price_class=price_class,
@@ -570,57 +542,7 @@
     "CloudfrontSiteConfiguration",
     "CreateBasicSite",
     "CreateCloudfrontSite",
     "PriceClass",
 ]
 
 publication.publish()
-
-def _typecheckingstub__55e1d457f7f88b408ecc128e65052c3c69d68b852e2406239079c5f4b76a672d(
-    *,
-    hosted_zone: builtins.str,
-    index_doc: builtins.str,
-    website_folder: builtins.str,
-    error_doc: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0e850e19fcfb3492790ff3ec407df63abfa515b2415ed714c8499dc3239a822f(
-    *,
-    hosted_zone: builtins.str,
-    index_doc: builtins.str,
-    website_folder: builtins.str,
-    domain: typing.Optional[builtins.str] = None,
-    error_doc: typing.Optional[builtins.str] = None,
-    price_class: typing.Optional[PriceClass] = None,
-    sub_domain: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9b1cd29a96c6c8b996276e29a8e2730cf2a3c15a5c12e1c5bc0e23986cb136f7(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    hosted_zone: builtins.str,
-    index_doc: builtins.str,
-    website_folder: builtins.str,
-    error_doc: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__35939f41a1cbd87bd7b3fa20b126e3c79332b77b538ed266f3ea73f154b3c68a(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    *,
-    hosted_zone: builtins.str,
-    index_doc: builtins.str,
-    website_folder: builtins.str,
-    domain: typing.Optional[builtins.str] = None,
-    error_doc: typing.Optional[builtins.str] = None,
-    price_class: typing.Optional[PriceClass] = None,
-    sub_domain: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk-simplewebsite-deploy
-Version: 2.0.81
+Version: 2.0.9
 Summary: This is an AWS CDK v2 Construct to simplify deploying a single-page website use CloudFront distributions.
 Home-page: https://github.com/SnapPetal/cdk-simplewebsite-deploy
 Author: Thon Becker<thon.becker@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SnapPetal/cdk-simplewebsite-deploy
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Build](https://github.com/SnapPetal/cdk-simplewebsite-deploy/workflows/build/badge.svg)
 ![Release](https://github.com/SnapPetal/cdk-simplewebsite-deploy/workflows/release/badge.svg?branch=main)
 
@@ -252,7 +253,9 @@
                              hosted_zone='example.com',
                              sub_domain='www.example.com')
 ```
 
 ## License
 
 Distributed under the [Apache-2.0](./LICENSE) license.
+
+
```

### Comparing `cdk-simplewebsite-deploy-2.0.81/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt` & `cdk-simplewebsite-deploy-2.0.9/src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_simplewebsite_deploy/py.typed
 src/cdk_simplewebsite_deploy.egg-info/PKG-INFO
 src/cdk_simplewebsite_deploy.egg-info/SOURCES.txt
 src/cdk_simplewebsite_deploy.egg-info/dependency_links.txt
 src/cdk_simplewebsite_deploy.egg-info/requires.txt
 src/cdk_simplewebsite_deploy.egg-info/top_level.txt
 src/cdk_simplewebsite_deploy/_jsii/__init__.py
-src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.81.jsii.tgz
+src/cdk_simplewebsite_deploy/_jsii/cdk-simplewebsite-deploy@2.0.9.jsii.tgz
```

