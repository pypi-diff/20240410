# Comparing `tmp/pyaogmaneo-2.4.4.tar.gz` & `tmp/pyaogmaneo-2.4.5-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.4.tar", last modified: Tue Apr  9 00:50:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

