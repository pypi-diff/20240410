# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.0.1rc1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.1.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.0.1rc1.tar", last modified: Mon Mar  4 12:26:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

