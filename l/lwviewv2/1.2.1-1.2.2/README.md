# Comparing `tmp/lwviewv2-1.2.1.tar.gz` & `tmp/lwviewv2-1.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lwviewv2-1.2.1.tar", last modified: Fri Apr  5 13:03:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

