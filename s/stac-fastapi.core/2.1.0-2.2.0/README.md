# Comparing `tmp/stac-fastapi.core-2.1.0.tar.gz` & `tmp/stac_fastapi.core-2.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.core-2.1.0.tar", last modified: Sun Mar  3 14:57:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

