# Comparing `tmp/crewai_tools-0.1.6.tar.gz` & `tmp/crewai_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.1.6.tar", max compression
+gzip compressed data, was "crewai_tools-0.1.7.tar", max compression
```

## Comparing `crewai_tools-0.1.6.tar` & `crewai_tools-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.6/LICENSE
--rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.6/README.md
--rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.6/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.6/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.6/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.6/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.6/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.6/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1682 2024-04-04 16:45:56.494162 crewai_tools-0.1.6/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.6/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.494340 crewai_tools-0.1.6/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.6/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.6/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.6/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1739 2024-04-04 16:45:56.494732 crewai_tools-0.1.6/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.6/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1601 2024-04-04 16:45:56.494892 crewai_tools-0.1.6/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.6/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.6/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.6/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     2226 2024-04-06 01:44:50.972453 crewai_tools-0.1.6/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.6/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1636 2024-04-04 18:15:36.456434 crewai_tools-0.1.6/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.6/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.495395 crewai_tools-0.1.6/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.6/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.6/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.6/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.1.6/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.6/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.6/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.6/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.6/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.6/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.1.6/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.6/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.6/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.6/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.6/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.6/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1586 2024-04-04 16:45:56.495704 crewai_tools-0.1.6/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.6/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1672 2024-04-04 16:45:56.495856 crewai_tools-0.1.6/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.6/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.496107 crewai_tools-0.1.6/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.6/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     2030 2024-04-04 16:45:56.496381 crewai_tools-0.1.6/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.6/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1804 2024-04-04 16:45:56.496557 crewai_tools-0.1.6/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-04-07 17:18:46.967562 crewai_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.7/README.md
+-rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.7/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.7/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.7/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.7/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.7/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1642 2024-04-10 14:50:04.965572 crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.7/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.7/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.7/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.7/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.7/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.1.7/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      730 2024-04-10 14:50:15.447576 crewai_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.7/PKG-INFO
```

### Comparing `crewai_tools-0.1.6/LICENSE` & `crewai_tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/README.md` & `crewai_tools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.1.7/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.1.7/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/__init__.py` & `crewai_tools-0.1.7/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/base_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, docs_url: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if docs_url is not None:
             self.add(docs_url)
             self.description = f"A tool that can be used to semantic search a query the {docs_url} Code Docs content."
             self.args_schema = FixedCodeDocsSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.DOCS_SITE
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, csv: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if csv is not None:
             self.add(csv)
             self.description = f"A tool that can be used to semantic search a query the {csv} CSV's content."
             self.args_schema = FixedCSVSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.CSV
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, directory: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if directory is not None:
             self.add(directory)
             self.description = f"A tool that can be used to semantic search a query the {directory} directory's content."
             self.args_schema = FixedDirectorySearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["loader"] = DirectoryLoader(config=dict(recursive=True))
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/docx_search_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, docx: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if docx is not None:
             self.add(docx)
             self.description = f"A tool that can be used to semantic search a query the {docx} DOCX's content."
             self.args_schema = FixedDOCXSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.DOCX
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-# GitHubSearchTool
+# GithubSearchTool
 
 ## Description
-The GitHubSearchTool is a Read, Append, and Generate (RAG) tool specifically designed for conducting semantic searches within GitHub repositories. Utilizing advanced semantic search capabilities, it sifts through code, pull requests, issues, and repositories, making it an essential tool for developers, researchers, or anyone in need of precise information from GitHub.
+The GithubSearchTool is a Read, Append, and Generate (RAG) tool specifically designed for conducting semantic searches within GitHub repositories. Utilizing advanced semantic search capabilities, it sifts through code, pull requests, issues, and repositories, making it an essential tool for developers, researchers, or anyone in need of precise information from GitHub.
 
 ## Installation
-To use the GitHubSearchTool, first ensure the crewai_tools package is installed in your Python environment:
+To use the GithubSearchTool, first ensure the crewai_tools package is installed in your Python environment:
 
 ```shell
 pip install 'crewai[tools]'
 ```
 
-This command installs the necessary package to run the GitHubSearchTool along with any other tools included in the crewai_tools package.
+This command installs the necessary package to run the GithubSearchTool along with any other tools included in the crewai_tools package.
 
 ## Example
-Here’s how you can use the GitHubSearchTool to perform semantic searches within a GitHub repository:
+Here’s how you can use the GithubSearchTool to perform semantic searches within a GitHub repository:
 ```python
-from crewai_tools import GitHubSearchTool
+from crewai_tools import GithubSearchTool
 
 # Initialize the tool for semantic searches within a specific GitHub repository
-tool = GitHubSearchTool(
+tool = GithubSearchTool(
+    gh_token='...',
 	github_repo='https://github.com/example/repo',
 	content_types=['code', 'issue'] # Options: code, repo, pr, issue
 )
 
 # OR
 
 # Initialize the tool for semantic searches within a specific GitHub repository, so the agent can search any repository if it learns about during its execution
-tool = GitHubSearchTool(
+tool = GithubSearchTool(
+    gh_token='...',
 	content_types=['code', 'issue'] # Options: code, repo, pr, issue
 )
 ```
 
 ## Arguments
+- `gh_token` : The GitHub token used to authenticate the search. This is a mandatory field and allows the tool to access the GitHub API for conducting searches.
 - `github_repo` : The URL of the GitHub repository where the search will be conducted. This is a mandatory field and specifies the target repository for your search.
 - `content_types` : Specifies the types of content to include in your search. You must provide a list of content types from the following options: `code` for searching within the code, `repo` for searching within the repository's general information, `pr` for searching within pull requests, and `issue` for searching within issues. This field is mandatory and allows tailoring the search to specific content types within the GitHub repository.
 
 ## Custom model and embeddings
 
 By default, the tool uses OpenAI for both embeddings and summarization. To customize the model, you can use a config dictionary as follows:
 
 ```python
-tool = GitHubSearchTool(
+tool = GithubSearchTool(
     config=dict(
         llm=dict(
             provider="ollama", # or google, openai, anthropic, llama2, ...
             config=dict(
                 model="llama2",
                 # temperature=0.5,
                 # top_p=1,
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,27 @@
         ...,
         description="Mandatory content types you want to be included search, options: [code, repo, pr, issue]",
     )
 
 
 class GithubSearchTool(RagTool):
     name: str = "Search a github repo's content"
-    description: str = "A tool that can be used to semantic search a query from a github repo's content."
+    description: str = "A tool that can be used to semantic search a query from a github repo's content. This is not the GitHub API, but instead a tool that can provide semantic search capabilities."
     summarize: bool = False
     gh_token: str
     args_schema: Type[BaseModel] = GithubSearchToolSchema
     content_types: List[str]
 
     def __init__(self, github_repo: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if github_repo is not None:
             self.add(repo=github_repo)
-            self.description = f"A tool that can be used to semantic search a query the {github_repo} github repo's content."
+            self.description = f"A tool that can be used to semantic search a query the {github_repo} github repo's content. This is not the GitHub API, but instead a tool that can provide semantic search capabilities."
             self.args_schema = FixedGithubSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         repo: str,
         content_types: List[str] | None = None,
         **kwargs: Any,
     ) -> None:
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, json_path: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if json_path is not None:
             self.add(json_path)
             self.description = f"A tool that can be used to semantic search a query the {json_path} JSON's content."
             self.args_schema = FixedJSONSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.JSON
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, mdx: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if mdx is not None:
             self.add(mdx)
             self.description = f"A tool that can be used to semantic search a query the {mdx} MDX's content."
             self.args_schema = FixedMDXSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.MDX
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     def __init__(self, pdf: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if pdf is not None:
             self.add(pdf)
             self.description = f"A tool that can be used to semantic search a query the {pdf} PDF's content."
             self.args_schema = FixedPDFSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.PDF_FILE
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/rag/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.1.7/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, txt: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if txt is not None:
             self.add(txt)
             self.description = f"A tool that can be used to semantic search a query the {txt} txt's content."
             self.args_schema = FixedTXTSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.TEXT_FILE
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, website: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if website is not None:
             self.add(website)
             self.description = f"A tool that can be used to semantic search a query from {website} website content."
             self.args_schema = FixedWebsiteSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.WEB_PAGE
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/xml_search_tool/xml_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, xml: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if xml is not None:
             self.add(xml)
             self.description = f"A tool that can be used to semantic search a query the {xml} XML's content."
             self.args_schema = FixedXMLSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.XML
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, youtube_channel_handle: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if youtube_channel_handle is not None:
             self.add(youtube_channel_handle)
             self.description = f"A tool that can be used to semantic search a query the {youtube_channel_handle} Youtube Channels content."
             self.args_schema = FixedYoutubeChannelSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         youtube_channel_handle: str,
         **kwargs: Any,
     ) -> None:
         if not youtube_channel_handle.startswith("@"):
```

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.6/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(self, youtube_video_url: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if youtube_video_url is not None:
             self.add(youtube_video_url)
             self.description = f"A tool that can be used to semantic search a query the {youtube_video_url} Youtube Video content."
             self.args_schema = FixedYoutubeVideoSearchToolSchema
+            self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs["data_type"] = DataType.YOUTUBE_VIDEO
```

### Comparing `crewai_tools-0.1.6/pyproject.toml` & `crewai_tools-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.1.6"
+version = "0.1.7"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.1.6/PKG-INFO` & `crewai_tools-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

