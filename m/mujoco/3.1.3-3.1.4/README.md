# Comparing `tmp/mujoco-3.1.3.tar.gz` & `tmp/mujoco-3.1.4-cp311-cp311-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-3.1.3.tar", last modified: Tue Mar  5 21:05:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

