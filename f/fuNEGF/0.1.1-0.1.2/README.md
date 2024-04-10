# Comparing `tmp/fuNEGF-0.1.1.tar.gz` & `tmp/fuNEGF-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuNEGF-0.1.1.tar", last modified: Tue Apr  9 07:01:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

