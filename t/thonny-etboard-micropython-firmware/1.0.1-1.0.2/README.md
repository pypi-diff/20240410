# Comparing `tmp/thonny-etboard-micropython-firmware-1.0.1.tar.gz` & `tmp/thonny_etboard_micropython_firmware-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-etboard-micropython-firmware-1.0.1.tar", last modified: Tue Aug 31 00:45:12 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

