# Comparing `tmp/arxiv_client-0.2.2.tar.gz` & `tmp/arxiv_client-0.2.3.tar.gz`

## Comparing `arxiv_client-0.2.2.tar` & `arxiv_client-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/link.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/LICENSE
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 arxiv_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/PKG-INFO
```

### Comparing `arxiv_client-0.2.2/src/arxiv_client/article.py` & `arxiv_client-0.2.3/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/src/arxiv_client/author.py` & `arxiv_client-0.2.3/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/src/arxiv_client/category.py` & `arxiv_client-0.2.3/src/arxiv_client/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Category(Enum):
     """
     All the categories in the arXiv subject taxonomy, mapped to their codes.
 
     See [Arxiv category taxonomy](https://arxiv.org/category_taxonomy)
     """
 
-    def __new__(cls, value: str, description: str | None = None) -> Self:  # noqa
+    def __new__(cls, value: str, description: str | None = None) -> Self:
         """Allows for custom descriptions for each enum value"""
         obj = object.__new__(cls)
         obj._value_ = value
         if description is not None:
             obj.__doc__ = description
         return obj
```

### Comparing `arxiv_client-0.2.2/src/arxiv_client/client.py` & `arxiv_client-0.2.3/src/arxiv_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import logging
 import time
 from collections.abc import Iterator
-from datetime import datetime, timedelta
+from datetime import UTC, datetime, timedelta
 
 import feedparser  # type: ignore
 import requests
 
 from arxiv_client import Article, Query
 
 logger = logging.getLogger(__name__)
@@ -56,67 +56,68 @@
         """
         logger.debug("Searching arXiv with query: %r", query)
         subquery = copy.deepcopy(query)
         if page_size is not None:
             subquery.max_results = page_size
 
         total_retrieved = 0
-        while total_retrieved < query.max_results:
+        while total_retrieved < (query.max_results or float("inf")):
             feed = self._get_sub_page(subquery, paging_delay_ms, paging_max_retries)
             total_retrieved += len(feed.entries)
             total_results = int(feed.feed.opensearch_totalresults)
 
             logger.debug("Retrieved %d of %d total articles", total_retrieved, total_results)
             for entry in feed.entries:
                 yield Article.from_feed_entry(entry)
 
             if not feed.entries or total_retrieved >= total_results:
                 return
 
             if page_size is not None:
                 subquery.start += page_size
-                subquery.max_results = min(query.max_results - total_retrieved, page_size)
+                if query.max_results is not None:
+                    subquery.max_results = min(query.max_results - total_retrieved, page_size)
 
-    def _get_sub_page(self, query: Query, chunk_delay_ms, chunk_max_retries: int) -> feedparser.FeedParserDict:
+    def _get_sub_page(self, query: Query, paging_delay_ms: int, paging_max_retries: int) -> feedparser.FeedParserDict:
         """
         Get a chunk of search results from the Arxiv API.
 
         Will raise a RuntimeError if the chunk request fails after `chunk_max_retries` attempts.
 
         :param query: The query to search with
-        :param chunk_delay_ms: The delay in milliseconds between each chunk request
-        :param chunk_max_retries: The max number of retries for each chunk request
+        :param paging_delay_ms: The delay in milliseconds between each chunk request
+        :param paging_max_retries: The max number of retries for each chunk request
         :return: The search results
         """
         try_count = 0
-        while try_count <= chunk_max_retries:
+        while try_count <= paging_max_retries:
             try:
-                self._apply_paging_delay(chunk_delay_ms)
-                response = self._session.get(self.base_search_url, params=query._to_url_params())
-                self._last_request_dt = datetime.now()
+                self._apply_paging_delay(paging_delay_ms)
+                response = self._session.get(self.base_search_url, params=query._to_url_params())  # noqa SLF001
+                self._last_request_dt = datetime.now(tz=UTC)
                 response.raise_for_status()
-
                 feed = feedparser.parse(response.content)
-                logger.debug("Successfully retrieved page of %d articles", len(feed.entries))
-                return feed
             except (requests.HTTPError, requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout) as e:
                 logger.warning("Failed to retrieve page of articles: %s", e)
                 try_count += 1
+            else:
+                logger.debug("Successfully retrieved page of %d articles", len(feed.entries))
+                return feed
 
-        msg = f"Failed to retrieve page of articles after {chunk_max_retries} retries"
+        msg = f"Failed to retrieve page of articles after {paging_max_retries} retries"
         logger.error(msg, extra={"page_query": query})
         raise RuntimeError(msg)
 
     def _apply_paging_delay(self, delay_ms: int) -> None:
         """
         Ensure a minimum delay of delay_ms since the last request. This is to avoid violating arXiv rate limit
         while fetching results in chunks.
         """
         if self._last_request_dt is None:
             return
 
         min_delay = timedelta(milliseconds=delay_ms)
-        elapsed = datetime.now() - self._last_request_dt
+        elapsed = datetime.now(tz=UTC) - self._last_request_dt
         if elapsed < min_delay:
             wait_time = (min_delay - elapsed).total_seconds()
             logger.debug("Waiting %s seconds before next request", wait_time)
             time.sleep(wait_time)
```

### Comparing `arxiv_client-0.2.2/src/arxiv_client/link.py` & `arxiv_client-0.2.3/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/src/arxiv_client/query.py` & `arxiv_client-0.2.3/src/arxiv_client/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,19 +80,14 @@
 
     For more advanced query logic, use the `custom_params` field to pass in a raw query string.
 
     See [Arxiv Query Interface](https://info.arxiv.org/help/api/user-manual.html#311-query-interface)
     [Arxiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#query_details)
     """
 
-    # TODO: Support for remaining searchable fields
-    #   - abstract
-    #   - comment
-    #   - journal reference
-    #   - report number
     keywords: list[str]
     """
     Keywords to search across all fields.
     """
     title_keywords: list[str]
     """
     Title keywords to filter on.
@@ -101,14 +96,22 @@
     """
     Author names to filter on.
     """
     categories: list[Category]
     """
     Subject categories to filter on.
     """
+    abstract_keywords: list[str]
+    """
+    Keywords to search for in the article's abstract
+    """
+    comment_keywords: list[str]
+    """
+    Keywords to search for in the author's comment
+    """
     article_ids: list[str]
     """
     ArXiv article IDs to filter on.
     """
     custom_params: str | None
     """
     Query param string for advanced users. This is helpful if query logic is not supported, e.g.,
@@ -130,35 +133,41 @@
 
     def __init__(
         self,
         keywords: list[str] | None = None,
         title_keywords: list[str] | None = None,
         author_names: list[str] | None = None,
         categories: list[Category] | None = None,
+        abstract_keywords: list[str] | None = None,
+        comment_keywords: list[str] | None = None,
         article_ids: list[str] | None = None,
         custom_params: str | None = None,
         sort_criterion: SortCriterion | None = None,
         start: int = 0,
         max_results: int | None = 10,
     ) -> None:
         """
         :param keywords: Keywords to search across all fields
         :param title_keywords: Title keywords to filter on
         :param author_names: Author names to filter on
         :param categories: Categories to filter on
+        :param abstract_keywords: Keywords to search for in the article's abstract
+        :param comment_keywords: Keywords to search for in the author's comment
         :param article_ids: ArXiv article IDs to filter on. If you want to retrieve a specific version, simply append
             `v{version#}` to the article ID, e.g., `2103.12345v1` for version 1 of article `2103.12345`
         :param custom_params: Raw query string for advanced users
         :param sort_criterion: Sort criterion for the query results
         :param max_results: The max number of results to get
         """
         self.keywords = [] if keywords is None else keywords
         self.title_keywords = [] if title_keywords is None else title_keywords
         self.author_names = [] if author_names is None else author_names
         self.categories = [] if categories is None else categories
+        self.abstract_keywords = [] if abstract_keywords is None else abstract_keywords
+        self.comment_keywords = [] if comment_keywords is None else comment_keywords
         self.article_ids = [] if article_ids is None else article_ids
         self.custom_params = custom_params
         self.sort_criterion = SortCriterion() if sort_criterion is None else sort_criterion
         self.start = start
         self.max_results = max_results
 
     def __str__(self) -> str:
@@ -183,24 +192,38 @@
             else ""
         )
         categories = (
             " OR ".join([f"{Field.CATEGORY.value}:{category.value}" for category in self.categories])
             if self.categories
             else ""
         )
+        abs_keywords = (
+            " OR ".join(f'{Field.ABSTRACT.value}:"{keyword}"' for keyword in self.abstract_keywords)
+            if self.abstract_keywords
+            else ""
+        )
+        comment_keywords = (
+            " OR ".join(f'{Field.COMMENT.value}:"{keyword}"' for keyword in self.comment_keywords)
+            if self.comment_keywords
+            else ""
+        )
 
         partials: list[str] = []
         if keywords:
             partials.append(f"({keywords})")
         if title_keywords:
             partials.append(f"({title_keywords})")
         if authors:
             partials.append(f"({authors})")
         if categories:
             partials.append(f"({categories})")
+        if abs_keywords:
+            partials.append(f"({abs_keywords})")
+        if comment_keywords:
+            partials.append(f"({comment_keywords})")
         if self.custom_params:
             partials.append(f"({self.custom_params})")
 
         return {
             "search_query": " AND ".join(partials),
             "id_list": ",".join(self.article_ids),
             **(
```

### Comparing `arxiv_client-0.2.2/.gitignore` & `arxiv_client-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/LICENSE` & `arxiv_client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/README.md` & `arxiv_client-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 The `Query` object accepts the following field filters:
 
 - `keywords`: terms across all fields
 - `title_keywords`: terms in the article title
 - `author_names`: names in the author list
 - `categories`: arXiv subject categories
+- `abstract_keywords`: terms in the article abstract
+- `comment_keywords`: terms in the author provided comment
 - `article_ids`: arXiv article IDs
 - `custom_params`: custom query string
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
```

### Comparing `arxiv_client-0.2.2/pyproject.toml` & `arxiv_client-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.2/PKG-INFO` & `arxiv_client-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -75,14 +75,16 @@
 
 The `Query` object accepts the following field filters:
 
 - `keywords`: terms across all fields
 - `title_keywords`: terms in the article title
 - `author_names`: names in the author list
 - `categories`: arXiv subject categories
+- `abstract_keywords`: terms in the article abstract
+- `comment_keywords`: terms in the author provided comment
 - `article_ids`: arXiv article IDs
 - `custom_params`: custom query string
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
```

