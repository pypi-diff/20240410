# Comparing `tmp/shipyard_http-0.1.0a1.tar.gz` & `tmp/shipyard_http-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_http-0.1.0a1.tar", max compression
+gzip compressed data, was "shipyard_http-0.1.1a0.tar", max compression
```

## Comparing `shipyard_http-0.1.0a1.tar` & `shipyard_http-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-12-27 14:59:12.923713 shipyard_http-0.1.0a1/README.md
--rw-r--r--   0        0        0      359 2023-12-29 19:54:23.875086 shipyard_http-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-27 14:59:12.923667 shipyard_http-0.1.0a1/shipyard_http/__init__.py
--rw-r--r--   0        0        0        0 2023-12-27 16:06:28.213777 shipyard_http-0.1.0a1/shipyard_http/cli/__init__.py
--rw-r--r--   0        0        0     4719 2023-12-27 16:08:14.682548 shipyard_http-0.1.0a1/shipyard_http/cli/download_file.py
--rw-r--r--   0        0        0     5727 2023-12-27 16:08:32.501134 shipyard_http-0.1.0a1/shipyard_http/cli/execute_request.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 shipyard_http-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.742554 shipyard_http-0.1.1a0/README.md
+-rw-r--r--   0        0        0      482 2024-04-09 22:36:52.664197 shipyard_http-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743381 shipyard_http-0.1.1a0/shipyard_http/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743456 shipyard_http-0.1.1a0/shipyard_http/cli/__init__.py
+-rw-r--r--   0        0        0     3694 2024-04-09 21:08:58.774558 shipyard_http-0.1.1a0/shipyard_http/cli/download_file.py
+-rw-r--r--   0        0        0     3568 2024-04-09 21:08:58.774913 shipyard_http-0.1.1a0/shipyard_http/cli/execute_request.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 shipyard_http-0.1.1a0/PKG-INFO
```

### Comparing `shipyard_http-0.1.0a1/shipyard_http/cli/download_file.py` & `shipyard_http-0.1.1a0/shipyard_http/cli/download_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,152 +1,115 @@
 import argparse
-import requests
+import json
 import os
 import sys
-import json
+
+import requests
+from shipyard_bp_utils import files as shipyard
+from shipyard_templates import ShipyardLogger
+
+logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--url', dest='url', required=True)
-    parser.add_argument('--custom-headers', dest='custom_headers',
-                        required=False, default='{}')
-    # authentication header is separated so it can be obfuscated
+    parser.add_argument("--url", dest="url", required=True)
+    parser.add_argument(
+        "--custom-headers", dest="custom_headers", required=False, default="{}"
+    )
+    # authentication header is separated, so it can be obfuscated
     # as a password type in the Blueprint.
     parser.add_argument(
-        '--authentication-headers',
-        dest='authentication_headers',
+        "--authentication-headers",
+        dest="authentication_headers",
         required=False,
-        default='{}')
+        default="{}",
+    )
     parser.add_argument(
-        '--destination-file-name',
-        dest='destination_file_name',
-        default='',
-        required=False)
+        "--destination-file-name",
+        dest="destination_file_name",
+        default="",
+        required=False,
+    )
     parser.add_argument(
-        '--destination-folder-name',
-        dest='destination_folder_name',
-        default='',
-        required=False)
-    args = parser.parse_args()
-    return args
-
-
-def combine_folder_and_file_name(folder_name, file_name):
-    """
-    Combine together the provided folder_name and file_name into one path variable.
-    """
-    combined_name = os.path.normpath(
-        f'{folder_name}{"/" if folder_name else ""}{file_name}')
-    combined_name = os.path.normpath(combined_name)
-
-    return combined_name
-
-
-def clean_folder_name(folder_name):
-    """
-    Cleans folders name by removing duplicate '/' as well as leading and trailing '/' characters.
-    """
-    folder_name = folder_name.strip('/')
-    if folder_name != '':
-        folder_name = os.path.normpath(folder_name)
-    return folder_name
-
-
-def convert_to_boolean(string):
-    """
-    Shipyard can't support passing Booleans to code, so we have to convert
-    string values to their boolean values.
-    """
-    if string in ['True', 'true', 'TRUE']:
-        value = True
-    else:
-        value = False
-    return value
+        "--destination-folder-name",
+        dest="destination_folder_name",
+        default="",
+        required=False,
+    )
+    return parser.parse_args()
 
 
 def extract_filename_from_url(url):
-    file_name = url.split('/')[-1]
-    return file_name
+    return url.split("/")[-1]
 
 
 def download_file(url, destination_name, headers=None, params=None):
-    print(f'Currently downloading the file from {url}...')
+    logger.info(f"Currently downloading the file from {url}...")
     try:
         with requests.get(url, headers=headers, stream=True, params=params) as r:
             r.raise_for_status()
-            with open(destination_name, 'wb') as f:
+            with open(destination_name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=(16 * 1024 * 1024)):
                     f.write(chunk)
 
-        print(f'Successfully downloaded {url} to {destination_name}.')
+        logger.info(f"Successfully downloaded {url} to {destination_name}.")
     except requests.exceptions.HTTPError as eh:
-        print(
-            'URL returned an HTTP Error.\n',
-            eh)
+        logger.error("URL returned an HTTP Error.\n", eh)
         sys.exit(1)
     except requests.exceptions.ConnectionError as ec:
-        print(
-            'Could not connect to the URL. Check to make sure that it was typed correctly.\n',
-            ec)
+        logger.error(
+            "Could not connect to the URL. Check to make sure that it was typed correctly.\n",
+            ec,
+        )
         sys.exit(2)
     except requests.exceptions.Timeout as et:
-        print('Timed out while connecting to the URL.\n', et)
+        logger.error("Timed out while connecting to the URL.\n", et)
         sys.exit(3)
     except requests.exceptions.RequestException as e:
-        print('Unexpected error occured. Please try again.\n', e)
+        logger.error("Unexpected error occurred. Please try again.\n", e)
         sys.exit(4)
     return
 
 
 def add_to_headers(headers, key, value):
     headers[key] = value
     return headers
 
 
-def create_folder_if_dne(destination_folder_name):
-    if not os.path.exists(destination_folder_name) and (
-            destination_folder_name != ''):
-        os.makedirs(destination_folder_name)
-
-
 def main():
     args = get_args()
     url = args.url
 
-    if args.custom_headers == '':
-        custom_headers = json.loads('{}')
+    if args.custom_headers == "":
+        custom_headers = json.loads("{}")
     else:
         custom_headers = json.loads(args.custom_headers)
 
-    if args.authentication_headers == '':
-        authentication_headers = json.loads('{}')
+    if args.authentication_headers == "":
+        authentication_headers = json.loads("{}")
     else:
         authentication_headers = json.loads(args.authentication_headers)
-    destination_file_name = args.destination_file_name
-    if not destination_file_name:
-        destination_file_name = extract_filename_from_url(url)
-    destination_folder_name = clean_folder_name(args.destination_folder_name)
-    destination_name = combine_folder_and_file_name(
-        destination_folder_name, destination_file_name)
+    destination_file_name = args.destination_file_name or extract_filename_from_url(url)
+    destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+    destination_name = shipyard.combine_folder_and_file_name(destination_folder_name, destination_file_name)
     headers = {}
     params = {}
 
-    create_folder_if_dne(destination_folder_name)
+    shipyard.create_folder_if_dne(destination_folder_name)
     if custom_headers:
         for key, value in custom_headers.items():
             headers = add_to_headers(headers, key, value)
     if authentication_headers:
         for key, value in custom_headers.items():
             headers = add_to_headers(headers, key, value)
 
     download_file(url, destination_name, headers, params)
     written_file_size = os.path.getsize(destination_name)
-    print(
-        f'The downloaded file contained {written_file_size/1000000}MB of data.')
+    logger.info(f"The downloaded file contained {written_file_size / 1000000}MB of data.")
     if written_file_size == 0:
-        print('File downloaded contained no data.')
+        logger.warning("File downloaded contained no data.")
         sys.exit(5)
 
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":
+    main()
```

