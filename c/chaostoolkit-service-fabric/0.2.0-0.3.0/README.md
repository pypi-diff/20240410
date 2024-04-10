# Comparing `tmp/chaostoolkit-service-fabric-0.2.0.tar.gz` & `tmp/chaostoolkit_service_fabric-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chaostoolkit-service-fabric/chaostoolkit-service-fabric/dist/.tmp-1gious07/chaostoolkit-service-fabric-0.2.0.", last modified: Mon Feb 27 09:50:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

