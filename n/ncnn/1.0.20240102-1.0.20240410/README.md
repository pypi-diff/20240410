# Comparing `tmp/ncnn-1.0.20240102.tar.gz` & `tmp/ncnn-1.0.20240410-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncnn-1.0.20240102.tar", last modified: Tue Jan  2 02:35:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

