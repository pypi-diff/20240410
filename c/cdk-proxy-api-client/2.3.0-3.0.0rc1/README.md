# Comparing `tmp/cdk_proxy_api_client-2.3.0.tar.gz` & `tmp/cdk_proxy_api_client-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-2.3.0.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-3.0.0rc1.tar", max compression
```

## Comparing `cdk_proxy_api_client-2.3.0.tar` & `cdk_proxy_api_client-3.0.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-2.3.0/LICENSE
--rw-r--r--   0        0        0      222 2023-10-03 07:30:35.881560 cdk_proxy_api_client-2.3.0/README.md
--rw-r--r--   0        0        0      181 2024-02-15 21:37:19.947461 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     5728 2023-08-03 06:09:54.327251 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0       93 2023-10-03 07:40:54.094102 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1937 2023-10-03 07:41:27.578445 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0      426 2023-09-01 10:03:29.445084 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/exceptions.py
--rw-r--r--   0        0        0     6012 2023-10-24 13:07:52.460103 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/interceptors/__init__.py
--rw-r--r--   0        0        0     1046 2023-10-18 20:18:22.878099 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/plugins/__init__.py
--rw-r--r--   0        0        0      890 2023-09-01 10:03:29.446084 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0     1680 2023-11-30 20:23:36.900165 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/usermappings/__init__.py
--rw-r--r--   0        0        0     5567 2023-11-30 20:23:36.900165 cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/vclusters/__init__.py
--rw-r--r--   0        0        0     1943 2024-02-15 21:37:19.947461 cdk_proxy_api_client-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 cdk_proxy_api_client-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-3.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      222 2023-10-03 07:30:35.881560 cdk_proxy_api_client-3.0.0rc1/README.md
+-rw-r--r--   0        0        0      185 2024-04-09 06:04:25.917364 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     5889 2024-04-08 16:25:03.929937 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0       93 2024-04-08 14:50:57.285009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1937 2023-10-03 07:41:27.578445 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     3012 2024-04-08 14:50:57.281009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0      426 2024-04-08 14:50:57.287009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/exceptions.py
+-rw-r--r--   0        0        0     8629 2024-04-08 17:43:00.455397 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/interceptors/__init__.py
+-rw-r--r--   0        0        0     1040 2024-04-08 16:25:03.927937 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/plugins/__init__.py
+-rw-r--r--   0        0        0      890 2024-04-08 14:50:57.289009 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0     4635 2024-04-08 21:50:09.929832 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/user_mappings/__init__.py
+-rw-r--r--   0        0        0     8138 2024-04-08 22:17:53.442884 cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/vclusters/__init__.py
+-rw-r--r--   0        0        0     2072 2024-04-09 06:04:25.917364 cdk_proxy_api_client-3.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 cdk_proxy_api_client-3.0.0rc1/PKG-INFO
```

### Comparing `cdk_proxy_api_client-2.3.0/LICENSE` & `cdk_proxy_api_client-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/client_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #   SPDX-License-Identifier: Apache-2.0
-#   Copyright 2023 John Mille <john@ews-network.net>
+#   Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union
 
+import requests
+
 if TYPE_CHECKING:
     from requests import Response
 
 import re
 
-from requests import delete, get, post, put
 from requests.auth import HTTPBasicAuth
 
 from .errors import evaluate_api_return
 
 
 class ApiClient:
     """HTTP Calls wrapper"""
@@ -29,14 +30,15 @@
         hostname: str = None,
         port: int = None,
         url: str = None,
         protocol: str = None,
         ignore_ssl_errors: bool = False,
         username: str = None,
         password: str = None,
+        session: requests.session = None,
     ):
         """
 
         :param str hostname:
         :param int port: The endpoint port
         :param str protocol: http or https
         :param bool ignore_ssl_errors: Ignore SSL errors, for self-signed endpoints. Use at own risks
@@ -53,26 +55,28 @@
         self._port = None
         self._protocol = "http"
         self._ignore_ssl_errors = ignore_ssl_errors
 
         self.protocol = protocol
         self.port = port
         self.url = url
+        if session is None:
+            self.session = requests.session()
 
     def __repr__(self):
         return self.url
 
     @property
     def verify_ssl(self) -> bool:
         if not self._ignore_ssl_errors and self.protocol == "http":
             return False
         return not self._ignore_ssl_errors
 
     @property
-    def basic_auth(self) -> Union[HTTPBasicAuth, None]:
+    def basic_auth(self) -> HTTPBasicAuth | None:
         """Returns basic auth information. If both the username and password are not set, raises AttributeError"""
         if self.username and self.password:
             return HTTPBasicAuth(self.username, self.password)
         if (self.username and not self.password) or (
             self.password and not self.username
         ):
             raise AttributeError("You must specify both username and password")
@@ -91,15 +95,15 @@
                 return f"{self.protocol}://{self.hostname}:{self.port}"
         else:
             raise AttributeError(
                 "Unable to form a URL", self._url, self.hostname, self.port
             )
 
     @url.setter
-    def url(self, value: Union[str, None]):
+    def url(self, value: str | None):
         if value is None:
             return
         if re.match(r"^https://(.*)$", value):
             self.protocol = "https"
         elif not re.match(r"(http://|https://)", value):
             print(f"URL Does not contain a protocol. Using default {self.protocol}")
             value = f"{self.protocol}://{value}"
@@ -108,30 +112,30 @@
     @property
     def protocol(self) -> str:
         if self._protocol:
             return self._protocol
         return "http"
 
     @protocol.setter
-    def protocol(self, value: Union[str, None]) -> None:
+    def protocol(self, value: str | None) -> None:
         if value is None:
             return
         valid_values: list = ["http", "https", "HTTP", "HTTPS"]
         if value not in valid_values:
             raise ValueError("protocol must be one of", valid_values, "got", value)
         self._protocol = value.lower()
 
     @property
     def port(self) -> int:
         if self._port:
             return self._port
         return 80
 
     @port.setter
-    def port(self, value: Union[int, None]) -> None:
+    def port(self, value: int | None) -> None:
         if value is None and self.protocol == "http":
             value = 80
         elif value is None and self.protocol == "https":
             value = 443
         elif isinstance(value, str):
             value = int(value)
 
@@ -142,43 +146,47 @@
         self._port = value
 
     @evaluate_api_return
     def get(self, query_path, **kwargs) -> Response:
         if not query_path.startswith(r"/"):
             query_path = f"/{query_path}"
         url = f"{self.url}{query_path}"
-        req = get(url, auth=self.basic_auth, verify=self.verify_ssl, **kwargs)
+        req = self.session.get(
+            url, auth=self.basic_auth, verify=self.verify_ssl, **kwargs
+        )
         return req
 
     @evaluate_api_return
     def post(self, query_path, **kwargs) -> Response:
         if not query_path.startswith(r"/"):
             query_path = f"/{query_path}"
         url = f"{self.url}{query_path}"
-        req = post(
+        req = self.session.post(
             url,
             auth=self.basic_auth,
             verify=self.verify_ssl,
             **kwargs,
         )
         return req
 
     @evaluate_api_return
     def put(self, query_path, **kwargs) -> Response:
         if not query_path.startswith(r"/"):
             query_path = f"/{query_path}"
         url = f"{self.url}{query_path}"
-        req = put(
+        req = self.session.put(
             url,
             auth=self.basic_auth,
             verify=self.verify_ssl,
             **kwargs,
         )
         return req
 
     @evaluate_api_return
     def delete(self, query_path, **kwargs) -> Response:
         if not query_path.startswith(r"/"):
             query_path = f"/{query_path}"
         url = f"{self.url}{query_path}"
-        req = delete(url, auth=self.basic_auth, verify=self.verify_ssl, **kwargs)
+        req = self.session.delete(
+            url, auth=self.basic_auth, verify=self.verify_ssl, **kwargs
+        )
         return req
```

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #  SPDX-License-Identifier: Apache-2.0
-#  Copyright 2023 John Mille <john@ews-network.net>
+#  Copyright 2024 John Mille <john@ews-network.net>
 
 from requests import exceptions as req_exceptions
 
 KEYISSET = lambda key, obj: isinstance(obj, dict) and key in obj and obj[key]
 
 
 class ProxyGenericException(Exception):
```

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/plugins/__init__.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/plugins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: Apache-2.0
-# Copyright 2023 John Mille <john@ews-network.net>
+# Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from typing import Union
 
 from requests import Response
 
@@ -12,15 +12,15 @@
 
 
 class Plugins(ApiApplication):
     app_path: str = "admin/plugins"
 
     def list_all_plugins(
         self, extended: bool = False, as_list: bool = False
-    ) -> Union[Response, list]:
+    ) -> Response | list:
         """
         Docs: https://developers.conduktor.io/#tag/Plugins/operation/Plugins_v1_getPlugins
         Path: /admin/plugins/v1
         Docs: https://developers.conduktor.io/#tag/Plugins/operation/Plugins_v1_getPluginsExtended
         Path: /admin/plugins/v1/extended
         """
         _path = self.base_path
```

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/proxy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #   SPDX-License-Identifier: Apache-2.0
-#   Copyright 2023 John Mille <john@ews-network.net>
+#   Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from cdk_proxy_api_client.client_wrapper import ApiClient
```

### Comparing `cdk_proxy_api_client-2.3.0/cdk_proxy_api_client/vclusters/__init__.py` & `cdk_proxy_api_client-3.0.0rc1/cdk_proxy_api_client/vclusters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #   SPDX-License-Identifier: Apache-2.0
-#   Copyright 2023 John Mille <john@ews-network.net>
+#   Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from typing import Union
 from urllib.parse import quote
 
 from requests import Response
@@ -13,32 +13,32 @@
 from cdk_proxy_api_client.exceptions import (
     TopicOrVirtualClusterNotFound,
     VirtualClusterNotFound,
 )
 from cdk_proxy_api_client.proxy_api import ApiApplication
 
 
-class VirturalClusters(ApiApplication):
+class VirtualClusters(ApiApplication):
     app_path: str = "admin/vclusters"
 
-    def list_vclusters(self, as_list: bool = False) -> Union[Response, list[str]]:
+    def list_vclusters(self, as_list: bool = False) -> Response | dict:
         _path: str = f"{self.base_path}/"
         LOG.debug(f"list_vclusters path {_path}")
         req = self.proxy.client.get(_path, headers={"Accept": "application/json"})
         if as_list:
             return req.json()
         return req
 
     def create_vcluster_user_token(
         self,
         vcluster: str,
         username: str = None,
         lifetime_in_seconds: int = 86400,
         token_only: bool = False,
-    ) -> Union[Response, str]:
+    ) -> Response | str:
         """
         Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/Auth_v1_createClusterAccountToken
         Path: /admin/vclusters/v1/vcluster/{vcluster}/username/{username}
         """
         if not username:
             username = vcluster
         payload = {"lifeTimeSeconds": lifetime_in_seconds}
@@ -47,60 +47,123 @@
         req = self.proxy.client.post(
             _path, headers={"Accept": "application/json"}, json=payload
         )
         if token_only:
             return req.json()["token"]
         return req
 
+    def create_concentration_rule(
+        self,
+        vcluster_name: str,
+        pattern: str,
+        delete_topic_name: str,
+        compact_topic_name: str = None,
+        compact_delete_topic_name: str = None,
+        cluster_id: str = None,
+    ) -> Response:
+        """
+        Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/ConcentrationRule_createConcentrationRule
+        Path: /admin/vclusters/v1/vcluster/{vcluster}/concentration-rules
+        """
+        _path: str = f"{self.base_path}/vcluster/{vcluster_name}/concentration-rules"
+        LOG.debug(f"create_concentration_rule path {_path}")
+        payload: dict = {
+            "pattern": pattern,
+            "physicalTopicName": delete_topic_name,
+            "physicalTopicCompactedName": compact_topic_name
+            if compact_topic_name
+            else f"{delete_topic_name}_compacted",
+            "physicalTopicCompactedDeletedName": compact_delete_topic_name
+            if compact_delete_topic_name
+            else f"{delete_topic_name}_compact_delete",
+        }
+        if cluster_id:
+            payload["clusterId"] = cluster_id
+        req = self.proxy.client.post(
+            _path, headers={"Accept": "application/json"}, json=payload
+        )
+        return req
+
+    def get_concentration_rules(self, vcluster_name: str) -> Response:
+        """
+        Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/ConcentrationRule_getConcentrationRules
+        Path: /admin/vclusters/v1/vcluster/{vcluster}/concentration-rules
+        """
+        _path: str = f"{self.base_path}/vcluster/{vcluster_name}/concentration-rules"
+        LOG.debug(f"get_concentration_rules path {_path}")
+        req = self.proxy.client.get(
+            _path,
+        )
+        return req
+
+    def delete_concentration_rule(
+        self, vcluster_name: str, pattern: str = None
+    ) -> Response:
+        """
+        Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/ConcentrationRule_deleteConcentrationRule
+        Path: /admin/vclusters/v1/vcluster/{vcluster}/concentration-rules
+        """
+        if pattern:
+            _path: str = f"{self.base_path}/vcluster/{vcluster_name}/concentration-rules?{quote(pattern)}"
+        else:
+            _path: str = (
+                f"{self.base_path}/vcluster/{vcluster_name}/concentration-rules"
+            )
+        LOG.debug(f"delete_concentration_rule path {_path}")
+        req = self.proxy.client.delete(
+            _path,
+        )
+        return req
+
     def create_vcluster_topic_mapping(
         self,
         vcluster: str,
         logical_topic_name: str,
         physical_topic_name: str,
+        mapping_type: str = "alias",
         read_only: bool = False,
-        concentrated: bool = False,
         cluster_id: str = None,
     ) -> Response:
         """
         Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/Clusters_v1_createClusterTopicMapping
         Path: /admin/vclusters/v1/vcluster/{vcluster}/topics/{logicalTopicName}
         """
+        if mapping_type not in ["alias", "concentrated"]:
+            raise ValueError("mapping_type must be alias or concentrated")
+        if mapping_type == "concentrated":
+            raise ValueError("Must use concentration rules functions.")
         _path: str = (
             f"{self.base_path}/vcluster/{vcluster}/topics/{quote(logical_topic_name)}"
         )
         payload: dict = {
             "physicalTopicName": physical_topic_name,
             "readOnly": read_only,
-            "concentrated": concentrated,
+            "type": mapping_type,
         }
         if cluster_id:
             payload["clusterId"] = cluster_id
-        if payload["concentrated"] and payload["readOnly"]:
-            raise ValueError(
-                f"{_path} - concentrated is true, read_only cannot be true."
-            )
         LOG.debug(f"create_vcluster_topic_mapping path: {_path}")
         req = self.proxy.client.post(_path, json=payload)
         return req
 
     def list_vcluster_topic_mappings(
         self, vcluster: str, as_list: bool = False
-    ) -> Union[Response, list]:
+    ) -> Response | list[dict]:
         """
         Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/Clusters_v1_listClusterTopicMapping
         Path: /admin/vclusters/v1/vcluster/{vcluster}/topics
         """
         _path = f"{self.base_path}/vcluster/{vcluster}/topics"
         LOG.debug(f"list_vcluster_topic_mappings path: {_path}")
         try:
             req = self.proxy.client.get(_path, headers={"Accept": "application/json"})
             if as_list:
                 return req.json()
             return req
-        except GenericNotFound as error:
+        except GenericNotFound:
             raise VirtualClusterNotFound(vcluster)
 
     def delete_vcluster_topics_mappings(self, vcluster: str) -> Response:
         """
         Docs: https://developers.conduktor.io/#tag/Virtual-Clusters/operation/Clusters_v1_deleteClusters
         Path: /admin/vclusters/v1/vcluster/{vcluster}/topics
         """
```

### Comparing `cdk_proxy_api_client-2.3.0/pyproject.toml` & `cdk_proxy_api_client-3.0.0rc1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "2.3.0"
+version = "3.0.0-rc1"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{ include = "cdk_proxy_api_client" }]
 keywords = ["conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 exclude = ["*.pyc", "*~", "*pycache*"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/JohnPreston/cdk-proxy-api-client/issues"
 "Source (GitHub)" = "https://github.com/JohnPreston/cdk-proxy-api-client"
 "CLI & Tools" = "https://github.com/johnpreston/cdk-gw-tools"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 requests = "^2.31"
 pyjwt = "^2.8"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 black = "^23.9"
 isort = "^5.12"
 pyupgrade = "^3.3.1"
 pydantic = "^1.10.5"
 tbump = "^6.9.0"
 
+[tool.poetry.group.testing.dependencies]
+coverage = "^7.4.4"
+pytest = "^8.1.1"
+testcontainers = "^4.3.2"
+confluent-kafka = "^3.0.0-rc1"
+pytest-timeout = "^2.3.1"
+
+
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "2.3.0"
+current = "3.0.0-rc1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-2.3.0/PKG-INFO` & `cdk_proxy_api_client-3.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cdk-proxy-api-client
-Version: 2.3.0
+Version: 3.0.0rc1
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyjwt (>=2.8,<3.0)
 Requires-Dist: requests (>=2.31,<3.0)
 Project-URL: Bug Tracker, https://github.com/JohnPreston/cdk-proxy-api-client/issues
 Project-URL: CLI & Tools, https://github.com/johnpreston/cdk-gw-tools
```

