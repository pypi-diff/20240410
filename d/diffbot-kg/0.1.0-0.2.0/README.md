# Comparing `tmp/diffbot_kg-0.1.0.tar.gz` & `tmp/diffbot_kg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffbot_kg-0.1.0.tar", max compression
+gzip compressed data, was "diffbot_kg-0.2.0.tar", max compression
```

## Comparing `diffbot_kg-0.1.0.tar` & `diffbot_kg-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0     1074 2024-02-21 20:44:17.634370 diffbot_kg-0.1.0/LICENSE
--rw-r--r--   0        0        0      871 2024-02-23 10:02:08.347504 diffbot_kg-0.1.0/README.md
--rw-r--r--   0        0        0      603 2024-02-23 10:01:37.275310 diffbot_kg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      178 2024-02-23 04:47:02.154434 diffbot_kg-0.1.0/src/diffbot_kg/__init__.py
--rw-r--r--   0        0        0     7229 2024-02-23 10:00:58.828571 diffbot_kg-0.1.0/src/diffbot_kg/clients.py
--rw-r--r--   0        0        0     3892 2024-02-23 07:22:47.732614 diffbot_kg-0.1.0/src/diffbot_kg/session.py
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 diffbot_kg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-10 21:01:10.627504 diffbot_kg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1311 2024-04-10 21:01:10.627504 diffbot_kg-0.2.0/README.md
+-rw-r--r--   0        0        0      648 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/__init__.py
+-rw-r--r--   0        0        0     3819 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/base.py
+-rw-r--r--   0        0        0     5850 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/enhance.py
+-rw-r--r--   0        0        0     2050 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/search.py
+-rw-r--r--   0        0        0     3224 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/session.py
+-rw-r--r--   0        0        0      644 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/__init__.py
+-rw-r--r--   0        0        0     1767 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/base.py
+-rw-r--r--   0        0        0      573 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_create.py
+-rw-r--r--   0        0        0      471 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_list.py
+-rw-r--r--   0        0        0     1011 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_results.py
+-rw-r--r--   0        0        0      786 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_status.py
+-rw-r--r--   0        0        0      141 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/coverage_report.py
+-rw-r--r--   0        0        0      865 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/entities.py
+-rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 diffbot_kg-0.2.0/PKG-INFO
```

### Comparing `diffbot_kg-0.1.0/LICENSE` & `diffbot_kg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.1.0/pyproject.toml` & `diffbot_kg-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "diffbot-kg"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python client for the Diffbot Knowledge Graph API."
 authors = ["Brendan C. Smith"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -14,16 +14,17 @@
 yarl = "^1.9.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
 pytest-asyncio = "^0.23.5"
 pytest-mock = "^3.12.0"
 ruff = "^0.2.2"
-black = "^24.2.0"
-pre-commit = "^3.6.2"
+python-dotenv = "^1.0.1"
+pytest-vcr = "^1.0.2"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
+addopts = ["--import-mode=importlib"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `diffbot_kg-0.1.0/src/diffbot_kg/clients.py` & `diffbot_kg-0.2.0/src/diffbot_kg/clients/enhance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,172 @@
-import logging
-from typing import Any
+from typing import cast
 
-from yarl import URL
+from diffbot_kg.clients.base import BaseDiffbotKGClient
+from diffbot_kg.models.response import (
+    DiffbotBulkJobCreateResponse,
+    DiffbotBulkJobStatusResponse,
+    DiffbotCoverageReportResponse,
+    DiffbotEntitiesResponse,
+    DiffbotListBulkJobsResponse,
+)
+from diffbot_kg.models.response.bulkjob_results import DiffbotBulkJobResultsResponse
 
-from diffbot_kg.session import DiffbotResponse, DiffbotSession
 
-log = logging.getLogger(__name__)
-
-
-class BaseDiffbotKGClient:
-    url = URL("https://kg.diffbot.com/kg/v3/")
-
-    def __init__(self, token, **kwargs) -> None:
-        for kwarg in kwargs:
-            if kwarg not in ["token", "useCache", "jsonmode", "size"]:
-                raise ValueError(f"Invalid kwarg: {kwarg}")
-
-        self.default_params = {"token": token, **kwargs}
-        self.s = DiffbotSession()
-
-    def _merge_params(self, params) -> dict[str, Any]:
-        params = params or {}
-        params = {**self.default_params, **params}
-        params = {k: v for k, v in params.items() if v is not None}
-        return params
-
-    async def _get(self, url: str | URL, params=None, headers=None) -> DiffbotResponse:
-        resp = await self.s.get(str(url), params=params, headers=headers)
-        return resp
-
-    async def _post(
-        self, url: str | URL, params: dict | None = None
-    ) -> DiffbotResponse:
-        """POST request to Diffbot API as alternative to GET for large queries.
-        All params except token are placed in the body of the request."""
-
-        token = params.pop("token", None) if params else None
-        json, params = params, {"token": token}
-
-        # headers = {"accept": "application/json", "content-type": "application/json"}
-        headers = {"content-type": "application/json"}
-
-        resp = await self.s.post(str(url), params=params, headers=headers, json=json)
-        return resp
-
-    async def _post_or_put(self, url: str | URL, params: dict | None = None):
-        # Diffbot uses nginx, which has a 4096 byte limit on URL by default
-        # but there are other factors, so we'll play it safe.
-        # 250 chars == 2000 bytes
-        if params is None:
-            params = {}
-        else:
-            params = {k: v for k, v in params.items() if v is not None}
-
-        url_len = len(str(url % params))
-        if url_len > 250:
-            resp = await self._post(url, params=params)
-        else:
-            resp = await self._get(url, params=params)
-
-        return resp
-
-
-class DiffbotSearchClient(BaseDiffbotKGClient):
-    search_url = BaseDiffbotKGClient.url / "dql"
-    report_url = BaseDiffbotKGClient.url / "dql/report"
-    report_by_id_url = BaseDiffbotKGClient.url / "dql/report/{id}"
+class DiffbotEnhanceClient(BaseDiffbotKGClient):
+    """
+    A client for interacting with the Diffbot Enhance API.
 
-    async def search(self, params: dict) -> DiffbotResponse:
-        """Search Dreport_urliffbot's Knowledge Graph.
+    This client provides methods for enhancing content using the Diffbot Enhance API,
+    managing bulk jobs, and retrieving job results and coverage reports.
+    """
 
-        Args:
-            params (dict): Dict of params to send in request
+    enhance_url = BaseDiffbotKGClient.url / "enhance"
+    bulk_job_url = enhance_url / "bulk"
+    list_bulk_jobs_url = bulk_job_url / "status"
+    bulk_job_status_url = bulk_job_url / "{bulkjobId}" / "status"
+    bulk_job_results_url = bulk_job_url / "{bulkjobId}"
+    bulk_job_single_result_url = bulk_job_results_url / "{jobIdx}"
+    bulk_job_coverage_report_url = bulk_job_url / "report/{bulkjobId}/{reportId}"
+    bulk_job_stop_url = bulk_job_url / "{bulkjobId}/stop"
 
-        Returns:
-            response: requests.Response object
+    async def enhance(self, params) -> DiffbotEntitiesResponse:
         """
-        resp = await self._post_or_put(self.search_url, params=params)
-
-        return resp
-
-    async def coverage_report_by_id(self, report_id: str) -> DiffbotResponse:
-        """Download coverage report by report ID.
+        Enhance content using the Diffbot Enhance API.
 
         Args:
-            report_id (str): The report ID string.
+            params (dict): The parameters for enhancing the content.
 
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
-        url = str(self.report_by_id_url).format(id=report_id)
-        resp = await self._get(url)
-        return resp
 
-    async def coverage_report_by_query(self, query: str) -> DiffbotResponse:
-        """Download coverage report by DQL query.
+        resp = await self._get(self.enhance_url, params=params)
+        resp.__class__ = DiffbotEntitiesResponse
+        return cast(DiffbotEntitiesResponse, resp)
+
+    async def create_bulkjob(
+        self, json: list[dict], params=None
+    ) -> DiffbotBulkJobCreateResponse:
+        """
+        Create a bulk job for enhancing multiple content items.
 
         Args:
-            query (str): The DQL query string.
+            data (list[dict]): The content items to enhance.
+            params (dict): The parameters for creating the bulk job.
 
         Returns:
-            DiffbotResponse: The response from the Diffbot API.
+            DiffbotBulkJobResponse: The response from the Diffbot API.
         """
-        params = {"query": query}
-        resp = await self._get(self.report_url, params=params)
-        return resp
-
-
-class DiffbotEnhanceClient(BaseDiffbotKGClient):
-    enhance_url = BaseDiffbotKGClient.url / "enhance"
-    bulk_enhance_url = enhance_url / "bulk"
-    bulk_status_url = BaseDiffbotKGClient.url / "enhance/bulk/status"
-    single_bulkjob_result_url = (
-        BaseDiffbotKGClient.url / "enhance/bulk/{bulkjobId}/{jobIdx}"
-    )
-    bulk_job_results_url = BaseDiffbotKGClient.url / "enhance/bulk/{bulkjobId}"
-    bulk_job_coverage_report_url = (
-        BaseDiffbotKGClient.url / "enhance/bulk/{bulkjobId}/coverage/{reportId}"
-    )
 
-    async def enhance(self, params) -> DiffbotResponse:
-        resp = await self._get(self.enhance_url, params=params)
-        return resp
+        if json is None or not json:
+            raise ValueError("data must be provided")
 
-    bulk_job_stop_url = BaseDiffbotKGClient.url / "enhance/bulk/{bulkjobId}/stop"
-    ...  # Other methods
+        resp = await self._post(self.bulk_job_url, params=params, json=json)
+        resp.__class__ = DiffbotBulkJobCreateResponse
+        return cast(DiffbotBulkJobCreateResponse, resp)
 
-    async def stop_bulkjob(self, bulkjobId: str) -> DiffbotResponse:
+    async def bulkjob_status(self, bulkjobId: str) -> DiffbotBulkJobStatusResponse:
         """
-        Stop an active Enhance Bulkjob by its ID.
+        Poll the status of an Enhance Bulkjob by its ID.
 
         Args:
             bulkjobId (str): The ID of the bulk job.
 
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
-        url = str(self.bulk_job_stop_url).format(bulkjobId=bulkjobId)
-        return await self._get(url)
 
-    async def download_single_bulkjob_result(
-        self, bulkjobId: str, jobIdx: str
-    ) -> DiffbotResponse:
-        """
-        Download the result of a single job within a bulkjob by specifying the index of the job.
+        url = self.bulk_job_status_url.human_repr().format(bulkjobId=bulkjobId)
+        resp = await self._get(url)
+        resp.__class__ = DiffbotBulkJobStatusResponse
+        return cast(DiffbotBulkJobStatusResponse, resp)
 
-        Args:
-            bulkjobId (str): The ID of the bulk job.
-            jobIdx (str): The index of the job within the bulk job.
+    async def list_bulkjobs(self) -> DiffbotListBulkJobsResponse:
+        """
+        Poll the status of all Enhance Bulkjobs for a token.
 
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
-        url = str(self.single_bulkjob_result_url).format(
-            bulkjobId=bulkjobId, jobIdx=jobIdx
-        )
-        return await self._get(url)
 
-    async def create_bulkjob(self, params) -> DiffbotResponse:
-        resp = await self._post(self.bulk_enhance_url, params=params)
-        return resp
+        resp = await self._get(self.list_bulk_jobs_url)
+        resp.__class__ = DiffbotListBulkJobsResponse
+        return cast(DiffbotListBulkJobsResponse, resp)
 
-    async def list_bulkjobs_for_token(self) -> DiffbotResponse:
+    async def bulkjob_results(self, bulkjobId: str) -> DiffbotBulkJobResultsResponse:
         """
-        Poll the status of all Enhance Bulkjobs for a token.
+        Download the results of a completed Enhance Bulkjob by its ID.
+
+        Args:
+            bulkjobId (str): The ID of the bulk job.
 
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
-        return await self._get(self.bulk_status_url)
 
-    async def poll_bulkjob_status(self, bulkjobId: str) -> DiffbotResponse:
+        url = self.bulk_job_results_url.human_repr().format(bulkjobId=bulkjobId)
+        resp = await self._get(url)
+        resp.__class__ = DiffbotBulkJobResultsResponse
+        return cast(DiffbotBulkJobResultsResponse, resp)
+
+    async def bulkjob_coverage_report(
+        self, bulkjobId: str, reportId: str
+    ) -> DiffbotCoverageReportResponse:
         """
-        Poll the status of an Enhance Bulkjob by its ID.
+        Download the coverage report of a completed Enhance Bulkjob by its ID and report ID.
 
         Args:
             bulkjobId (str): The ID of the bulk job.
+            reportId (str): The ID of the report.
 
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
-        url = str(self.bulk_status_url).format(bulkjobId=bulkjobId)
-        return await self._get(url)
 
-    async def download_bulkjob_results(self, bulkjobId: str) -> DiffbotResponse:
+        url = self.bulk_job_coverage_report_url.human_repr().format(
+            bulkjobId=bulkjobId, reportId=reportId
+        )
+        resp = await self._get(url)
+        resp.__class__ = DiffbotCoverageReportResponse
+        return cast(DiffbotCoverageReportResponse, resp)
+
+    async def single_bulkjob_result(
+        self,
+        bulkjobId: str,
+        jobIdx: int,
+    ) -> DiffbotEntitiesResponse:
         """
-        Download the results of a completed Enhance Bulkjob by its ID.
+        Download the result of a single job within a bulkjob by specifying the index of the job.
 
         Args:
             bulkjobId (str): The ID of the bulk job.
+            jobIdx (int): The index of the job within the bulk job.
 
         Returns:
-            DiffbotResponse: The response from the Diffbot API.
+            DiffbotEntitiesResponse: The response from the Diffbot API.
         """
-        url = str(self.bulk_job_results_url).format(bulkjobId=bulkjobId)
-        return await self._get(url)
 
-    async def download_bulkjob_coverage_report(
-        self, bulkjobId: str, reportId: str
-    ) -> DiffbotResponse:
+        url = self.bulk_job_single_result_url.human_repr().format(
+            bulkjobId=bulkjobId, jobIdx=jobIdx
+        )
+        resp = await self._get(url)
+        resp.__class__ = DiffbotEntitiesResponse
+        return cast(DiffbotEntitiesResponse, resp)
+
+    async def stop_bulkjob(
+        self,
+        bulkJobId: str,
+    ) -> DiffbotBulkJobStatusResponse:
         """
-        Download the coverage report of a completed Enhance Bulkjob by its ID and report ID.
+        Stop an active Enhance Bulkjob by its ID.
 
         Args:
             bulkjobId (str): The ID of the bulk job.
-            reportId (str): The ID of the report.
 
         Returns:
-            DiffbotResponse: The response from the Diffbot API.
+            DiffbotEntitiesResponse: The response from the Diffbot API.
         """
-        url = str(self.bulk_job_coverage_report_url).format(
-            bulkjobId=bulkjobId, reportId=reportId
-        )
-        return await self._get(url)
+
+        url = self.bulk_job_stop_url.human_repr().format(bulkjobId=bulkJobId)
+        resp = await self._get(url)
+        resp.__class__ = DiffbotBulkJobStatusResponse
+        return cast(DiffbotBulkJobStatusResponse, resp)
```

### Comparing `diffbot_kg-0.1.0/src/diffbot_kg/session.py` & `diffbot_kg-0.2.0/src/diffbot_kg/clients/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,31 @@
 import logging
 from http import HTTPMethod
-from typing import Any, List, Self
+from typing import Self
 
 import aiohttp
 import aiolimiter
-from multidict import CIMultiDictProxy
 from tenacity import (
     after_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 
-log = logging.getLogger(__name__)
-
-
-class DiffbotResponse:
-    """DiffbotResponse represents the response from a Diffbot API request.
+from diffbot_kg.models.response.base import BaseDiffbotResponse
 
-    It contains the response status, headers, and JSON content. Provides
-    convenience properties to access the 'data' and 'entities' portions
-    of the JSON content.
+log = logging.getLogger(__name__)
 
-    The create classmethod is the main constructor, which handles converting
-    an aiohttp response into a DiffbotResponse.
-    """
 
-    def __init__(
-        self, status: int, headers: CIMultiDictProxy[str], content: dict[str, Any]
-    ):
-        self.status = status
-        self.headers = headers
-        self.content = content
-
-    @property
-    def data(self) -> List[dict]:
-        return self.content["data"]
-
-    @property
-    def entities(self) -> List[dict]:
-        # Note: this class/method will not be compatible with facet queries
-        # (no entities returned)
-        return [d["entity"] for d in self.data]
-
-    @classmethod
-    async def create(cls, resp: aiohttp.ClientResponse) -> Self:
-        """Unpack an aiohttp response object and return a DiffbotResponse instance."""
-        return cls(resp.status, resp.headers, await resp.json())
+class RetryableException(Exception):
+    pass
 
 
-class RetryableException(Exception):
+class URLTooLongException(Exception):
     pass
 
 
 # TODO: Should this be a subclass of ClientSession?
 class DiffbotSession:
     """
     A class representing a session with the Diffbot API.
@@ -66,54 +37,66 @@
 
     def __init__(self) -> None:
         headers = {"accept": "application/json"}
         timeout = aiohttp.ClientTimeout(total=60, sock_connect=5)
         self._session = aiohttp.ClientSession(headers=headers, timeout=timeout)
         self._limiter = aiolimiter.AsyncLimiter(max_rate=5, time_period=1)
 
-    async def get(self, url, **kwargs) -> DiffbotResponse:
+    async def get(self, url, **kwargs) -> BaseDiffbotResponse:
         resp = await self._request(HTTPMethod.GET, url, **kwargs)
         return resp
 
-    async def post(self, url, **kwargs) -> DiffbotResponse:
+    async def post(self, url, **kwargs) -> BaseDiffbotResponse:
         resp = await self._request(HTTPMethod.POST, url, **kwargs)
         return resp
 
     async def close(self) -> None:
         if not self._session.closed:
             await self._session.close()
 
     @retry(
         retry=retry_if_exception_type(RetryableException),
         reraise=True,
         stop=stop_after_attempt(5),
         wait=wait_random_exponential(multiplier=0.5, min=2, max=30),
         after=after_log(log, logging.DEBUG),
     )
-    async def _request(self, method, url, **kwargs) -> DiffbotResponse:
+    async def _request(self, method, url, **kwargs) -> BaseDiffbotResponse:
         async with self._limiter:
             async with await self._session.request(method, url, **kwargs) as resp:
                 try:
                     resp.raise_for_status()
                 except Exception as e:
                     if resp.status in [408, 429] or resp.status >= 500:
                         log.debug(
                             "Retryable exception: %s (%s %s %s)",
                             e,
                             resp.status,
                             resp.reason,
                             resp.headers,
                         )
+
                         raise RetryableException from e
 
+                    elif resp.status == 414:
+                        log.debug(
+                            "URLTooLongException: %s (%s %s %s)",
+                            e,
+                            resp.status,
+                            resp.reason,
+                            resp.headers,
+                        )
+
+                        raise URLTooLongException from e
+
                     log.exception(
                         "%s (%s %s %s)", e, resp.status, resp.reason, resp.headers
                     )
                     raise e
 
-                return await DiffbotResponse.create(resp)
+                return await BaseDiffbotResponse.create(resp)
 
     async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(self, *args, **kwargs) -> None:
         await self.close()
```

### Comparing `diffbot_kg-0.1.0/PKG-INFO` & `diffbot_kg-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffbot-kg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python client for the Diffbot Knowledge Graph API.
 License: MIT
 Author: Brendan C. Smith
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -16,14 +16,21 @@
 Description-Content-Type: text/markdown
 
 Diffbot Knowledge Graph Client
 =============
 
 ![](https://www.diffbot.com/assets/img/diffbot-logo-darkbg.svg)
 
+
+[![CodeFactor](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg/badge)](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/brendancsmith/diffbot-kg/python-package.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/diffbot-kg)
+![GitHub License](https://img.shields.io/github/license/brendancsmith/diffbot-kg)
+
+
 Description
 -----------
 
 Python client for the Diffbot Knowledge Graph API.
 
 Installation
 ------------
```

