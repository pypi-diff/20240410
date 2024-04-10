# Comparing `tmp/althaia-3.20.1.tar.gz` & `tmp/althaia-3.21.1-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "althaia-3.20.1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

