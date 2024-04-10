# Comparing `tmp/interminal-0.3.7.tar.gz` & `tmp/interminal-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/interminal-0.3.7.tar", last modified: Tue Nov 27 01:32:07 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
