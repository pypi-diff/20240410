# Comparing `tmp/document_ingestor-0.0.5.tar.gz` & `tmp/document_ingestor-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_ingestor-0.0.5.tar", last modified: Wed Apr 10 11:05:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
