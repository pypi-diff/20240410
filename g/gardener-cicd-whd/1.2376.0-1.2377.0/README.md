# Comparing `tmp/gardener-cicd-whd-1.2376.0.tar.gz` & `tmp/gardener_cicd_whd-1.2377.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-whd-1.2376.0.tar", last modified: Wed Apr  3 15:05:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
