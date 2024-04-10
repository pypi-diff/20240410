# Comparing `tmp/python-mecab-ko-1.3.3.tar.gz` & `tmp/python_mecab_ko-1.3.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mecab-ko-1.3.3.tar", last modified: Fri Dec 30 07:19:48 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

