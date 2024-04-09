# Comparing `tmp/arxiv_client-0.2.1.tar.gz` & `tmp/arxiv_client-0.2.2.tar.gz`

## Comparing `arxiv_client-0.2.1.tar` & `arxiv_client-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/link.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/LICENSE
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/PKG-INFO
```

### Comparing `arxiv_client-0.2.1/src/arxiv_client/article.py` & `arxiv_client-0.2.2/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/src/arxiv_client/author.py` & `arxiv_client-0.2.2/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/src/arxiv_client/category.py` & `arxiv_client-0.2.2/src/arxiv_client/category.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/src/arxiv_client/client.py` & `arxiv_client-0.2.2/src/arxiv_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from arxiv_client import Article, Query
 
 logger = logging.getLogger(__name__)
 
 
 class Client:
     """
-    Python wrapper for the Arxiv API
+    Structured Python3 client for the Arxiv API
     """
 
     base_search_url = "https://export.arxiv.org/api/query"
     """
     Base URL for Arxiv API
     """
 
@@ -62,23 +62,23 @@
         total_retrieved = 0
         while total_retrieved < query.max_results:
             feed = self._get_sub_page(subquery, paging_delay_ms, paging_max_retries)
             total_retrieved += len(feed.entries)
             total_results = int(feed.feed.opensearch_totalresults)
 
             logger.debug("Retrieved %d of %d total articles", total_retrieved, total_results)
-            if not feed.entries:
-                return
-
             for entry in feed.entries:
                 yield Article.from_feed_entry(entry)
 
-            subquery.max_results = min(query.max_results - total_retrieved, page_size)
+            if not feed.entries or total_retrieved >= total_results:
+                return
+
             if page_size is not None:
                 subquery.start += page_size
+                subquery.max_results = min(query.max_results - total_retrieved, page_size)
 
     def _get_sub_page(self, query: Query, chunk_delay_ms, chunk_max_retries: int) -> feedparser.FeedParserDict:
         """
         Get a chunk of search results from the Arxiv API.
 
         Will raise a RuntimeError if the chunk request fails after `chunk_max_retries` attempts.
 
@@ -88,26 +88,26 @@
         :return: The search results
         """
         try_count = 0
         while try_count <= chunk_max_retries:
             try:
                 self._apply_paging_delay(chunk_delay_ms)
                 response = self._session.get(self.base_search_url, params=query._to_url_params())
-                response.raise_for_status()
                 self._last_request_dt = datetime.now()
+                response.raise_for_status()
 
                 feed = feedparser.parse(response.content)
-                logger.debug("Successfully retrieved chunk of %d articles", len(feed.entries))
+                logger.debug("Successfully retrieved page of %d articles", len(feed.entries))
                 return feed
             except (requests.HTTPError, requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout) as e:
-                logger.warning("Failed to retrieve chunk of articles: %s", e)
+                logger.warning("Failed to retrieve page of articles: %s", e)
                 try_count += 1
 
-        msg = f"Failed to retrieve chunk of articles after {chunk_max_retries} retries"
-        logger.error(msg, extra={"query": query})
+        msg = f"Failed to retrieve page of articles after {chunk_max_retries} retries"
+        logger.error(msg, extra={"page_query": query})
         raise RuntimeError(msg)
 
     def _apply_paging_delay(self, delay_ms: int) -> None:
         """
         Ensure a minimum delay of delay_ms since the last request. This is to avoid violating arXiv rate limit
         while fetching results in chunks.
         """
```

### Comparing `arxiv_client-0.2.1/src/arxiv_client/link.py` & `arxiv_client-0.2.2/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/src/arxiv_client/query.py` & `arxiv_client-0.2.2/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/.gitignore` & `arxiv_client-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/LICENSE` & `arxiv_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/README.md` & `arxiv_client-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
-Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
+Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) from PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 ## Basic Features
```

### Comparing `arxiv_client-0.2.1/pyproject.toml` & `arxiv_client-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.1/PKG-INFO` & `arxiv_client-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -34,15 +34,15 @@
 Requires-Dist: feedparser>=6.0.11
 Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
-Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
+Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) from PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 ## Basic Features
```

