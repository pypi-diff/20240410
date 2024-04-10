# Comparing `tmp/squidtools-0.0.1-py3-none-any.whl.zip` & `tmp/squidtools-0.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 12709 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 15:40 data-wrangler/__init__.py
--rw-r--r--  2.0 unx     2457 b- defN 23-Jul-27 15:38 data-wrangler/gpt-utils.py
--rw-r--r--  2.0 unx     5084 b- defN 23-Jul-27 15:38 data-wrangler/label-topic-copy.py
--rw-r--r--  2.0 unx     2457 b- defN 23-Jul-27 15:38 data-wrangler/label-topic.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 15:40 data_wrangler/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 23-Jul-27 15:58 data_wrangler/gpt_utils.py
--rw-r--r--  2.0 unx     5084 b- defN 23-Jul-27 15:38 data_wrangler/label-topic-copy.py
--rw-r--r--  2.0 unx     1027 b- defN 23-Jul-27 17:39 data_wrangler/proquest.py
--rw-r--r--  2.0 unx     1806 b- defN 23-Jul-27 17:00 data_wrangler/robust_task.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 15:40 src/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 23-Jul-27 15:58 src/gpt_utils.py
--rw-r--r--  2.0 unx     1027 b- defN 23-Jul-27 17:39 src/proquest.py
--rw-r--r--  2.0 unx     1806 b- defN 23-Jul-27 17:00 src/robust_task.py
--rw-r--r--  2.0 unx      261 b- defN 23-Jul-27 19:33 squidtools-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:33 squidtools-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-27 19:33 squidtools-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1353 b- defN 23-Jul-27 19:33 squidtools-0.0.1.dist-info/RECORD
-17 files, 27374 bytes uncompressed, 10489 bytes compressed:  61.7%
+Zip file size: 15983 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-20 21:33 squidtools/__init__.py
+-rw-r--r--  2.0 unx      582 b- defN 24-Feb-15 17:07 squidtools/gpt_utils.py
+-rw-r--r--  2.0 unx     4992 b- defN 24-Apr-06 21:53 squidtools/gpt_utils_async.py
+-rw-r--r--  2.0 unx     8373 b- defN 24-Mar-11 21:46 squidtools/linkedin.py
+-rw-r--r--  2.0 unx     5636 b- defN 24-Mar-13 01:39 squidtools/muckrack.py
+-rw-r--r--  2.0 unx     7245 b- defN 24-Mar-13 03:06 squidtools/names.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Mar-07 19:18 squidtools/proquest.py
+-rw-r--r--  2.0 unx      651 b- defN 24-Mar-24 13:18 squidtools/qualtrics.py
+-rw-r--r--  2.0 unx     5940 b- defN 24-Mar-06 23:50 squidtools/robust_task.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-02 16:09 squidtools/selenium_helpers.py
+-rw-r--r--  2.0 unx      116 b- defN 24-Mar-02 16:18 squidtools/strings.py
+-rw-r--r--  2.0 unx      862 b- defN 24-Mar-11 16:30 squidtools/util.py
+-rw-r--r--  2.0 unx     1283 b- defN 24-Mar-05 20:31 squidtools/webscraper.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Oct-12 14:55 squidtools/workflow.py
+-rw-r--r--  2.0 unx      262 b- defN 24-Apr-06 21:53 squidtools-0.0.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 21:53 squidtools-0.0.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-06 21:53 squidtools-0.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1422 b- defN 24-Apr-06 21:53 squidtools-0.0.11.dist-info/RECORD
+18 files, 40509 bytes uncompressed, 13661 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,52 +1,55 @@
-Filename: data-wrangler/__init__.py
+Filename: squidtools/__init__.py
 Comment: 
 
-Filename: data-wrangler/gpt-utils.py
+Filename: squidtools/gpt_utils.py
 Comment: 
 
-Filename: data-wrangler/label-topic-copy.py
+Filename: squidtools/gpt_utils_async.py
 Comment: 
 
-Filename: data-wrangler/label-topic.py
+Filename: squidtools/linkedin.py
 Comment: 
 
-Filename: data_wrangler/__init__.py
+Filename: squidtools/muckrack.py
 Comment: 
 
-Filename: data_wrangler/gpt_utils.py
+Filename: squidtools/names.py
 Comment: 
 
-Filename: data_wrangler/label-topic-copy.py
+Filename: squidtools/proquest.py
 Comment: 
 
-Filename: data_wrangler/proquest.py
+Filename: squidtools/qualtrics.py
 Comment: 
 
-Filename: data_wrangler/robust_task.py
+Filename: squidtools/robust_task.py
 Comment: 
 
-Filename: src/__init__.py
+Filename: squidtools/selenium_helpers.py
 Comment: 
 
-Filename: src/gpt_utils.py
+Filename: squidtools/strings.py
 Comment: 
 
-Filename: src/proquest.py
+Filename: squidtools/util.py
 Comment: 
 
-Filename: src/robust_task.py
+Filename: squidtools/webscraper.py
 Comment: 
 
-Filename: squidtools-0.0.1.dist-info/METADATA
+Filename: squidtools/workflow.py
 Comment: 
 
-Filename: squidtools-0.0.1.dist-info/WHEEL
+Filename: squidtools-0.0.11.dist-info/METADATA
 Comment: 
 
-Filename: squidtools-0.0.1.dist-info/top_level.txt
+Filename: squidtools-0.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: squidtools-0.0.1.dist-info/RECORD
+Filename: squidtools-0.0.11.dist-info/top_level.txt
+Comment: 
+
+Filename: squidtools-0.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

