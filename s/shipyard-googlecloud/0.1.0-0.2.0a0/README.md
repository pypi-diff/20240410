# Comparing `tmp/shipyard_googlecloud-0.1.0.tar.gz` & `tmp/shipyard_googlecloud-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_googlecloud-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_googlecloud-0.2.0a0.tar", max compression
```

## Comparing `shipyard_googlecloud-0.1.0.tar` & `shipyard_googlecloud-0.2.0a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.831133 shipyard_googlecloud-0.1.0/README.md
--rw-r--r--   0        0        0      681 2024-03-20 03:57:58.685906 shipyard_googlecloud-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-12 18:48:21.831530 shipyard_googlecloud-0.1.0/shipyard_googlecloud/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436211 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/__init__.py
--rw-r--r--   0        0        0      454 2024-03-20 03:57:58.686610 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/authtest.py
--rw-r--r--   0        0        0     9276 2024-03-20 03:57:58.687372 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/download.py
--rw-r--r--   0        0        0       98 2024-03-20 03:57:58.687498 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/exit_codes.py
--rw-r--r--   0        0        0     7880 2024-03-20 03:57:58.688039 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/move.py
--rw-r--r--   0        0        0     5189 2024-03-20 03:57:58.688864 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/remove.py
--rw-r--r--   0        0        0     8773 2024-03-20 03:57:58.689656 shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/upload.py
--rw-r--r--   0        0        0     1097 2024-03-20 03:57:58.690702 shipyard_googlecloud-0.1.0/shipyard_googlecloud/googlecloud.py
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 shipyard_googlecloud-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.831133 shipyard_googlecloud-0.2.0a0/README.md
+-rw-r--r--   0        0        0      625 2024-04-10 16:50:44.088720 shipyard_googlecloud-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-12 18:48:21.831530 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436211 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-25 01:03:55.080367 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/authtest.py
+-rw-r--r--   0        0        0     5290 2024-04-01 15:54:40.971130 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/download.py
+-rw-r--r--   0        0        0     6224 2024-03-25 01:03:55.081223 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/move.py
+-rw-r--r--   0        0        0     3460 2024-03-25 01:03:55.081667 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/remove.py
+-rw-r--r--   0        0        0     4377 2024-03-25 01:03:55.082080 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/upload.py
+-rw-r--r--   0        0        0     1066 2024-03-25 01:03:55.082389 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/googlecloud.py
+-rw-r--r--   0        0        0     3262 2024-04-10 16:42:37.478377 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/utils.py
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 shipyard_googlecloud-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_googlecloud-0.1.0/shipyard_googlecloud/cli/download.py` & `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/move.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+import argparse
 import os
 import re
-import json
-import tempfile
-import argparse
+import sys
+
+from shipyard_bp_utils import files as shipyard
+from shipyard_templates import ShipyardLogger, ExitCodeException, CloudStorage
 
-from google.cloud import storage
-from google.cloud.exceptions import *
+from shipyard_googlecloud import utils
+
+logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--bucket-name", dest="bucket_name", required=True)
+    parser.add_argument(
+        "--source-bucket-name", dest="source_bucket_name", required=True
+    )
+    parser.add_argument(
+        "--destination-bucket-name", dest="destination_bucket_name", required=True
+    )
     parser.add_argument(
         "--source-file-name-match-type",
         dest="source_file_name_match_type",
         default="exact_match",
         choices={"exact_match", "regex_match"},
         required=False,
     )
@@ -39,255 +47,130 @@
         dest="gcp_application_credentials",
         default=None,
         required=True,
     )
     return parser.parse_args()
 
 
-def set_environment_variables(args):
-    """
-    Set GCP credentials as environment variables if they're provided via keyword
-    arguments rather than seeded as environment variables. This will override
-    system defaults.
-    """
-    credentials = args.gcp_application_credentials
-    try:
-        json_credentials = json.loads(credentials)
-        fd, path = tempfile.mkstemp()
-        print(f"Storing json credentials temporarily at {path}")
-        with os.fdopen(fd, "w") as tmp:
-            tmp.write(credentials)
-        os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = path
-        return path
-    except Exception:
-        print("Using specified json credentials file")
-        os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = credentials
-        return
-
-
-def extract_file_name_from_source_full_path(source_full_path):
-    """
-    Use the file name provided in the source_file_name variable. Should be run only
-    if a destination_file_name is not provided.
-    """
-    destination_file_name = os.path.basename(source_full_path)
-    return destination_file_name
-
-
-def enumerate_destination_file_name(destination_file_name, file_number=1):
-    """
-    Append a number to the end of the provided destination file name.
-    Only used when multiple files are matched to, preventing the destination file from being continuously overwritten.
-    """
-    if re.search(r"\.", destination_file_name):
-        destination_file_name = re.sub(
-            r"\.", f"_{file_number}.", destination_file_name, 1
-        )
-    else:
-        destination_file_name = f"{destination_file_name}_{file_number}"
-    return destination_file_name
-
-
-def determine_destination_file_name(
-    *, source_full_path, destination_file_name, file_number=None
-):
-    """
-    Determine if the destination_file_name was provided, or should be extracted from the source_file_name,
-    or should be enumerated for multiple file downloads.
-    """
-    if destination_file_name:
-        if file_number:
-            destination_file_name = enumerate_destination_file_name(
-                destination_file_name, file_number
-            )
-        else:
-            destination_file_name = destination_file_name
-    else:
-        destination_file_name = extract_file_name_from_source_full_path(
-            source_full_path
-        )
-
-    return destination_file_name
-
-
-def clean_folder_name(folder_name):
-    """
-    Cleans folders name by removing duplicate '/' as well as leading and trailing '/' characters.
-    """
-    folder_name = folder_name.strip("/")
-    if folder_name != "":
-        folder_name = os.path.normpath(folder_name)
-    return folder_name
-
-
-def combine_folder_and_file_name(folder_name, file_name):
-    """
-    Combine together the provided folder_name and file_name into one path variable.
-    """
-    combined_name = os.path.normpath(
-        f'{folder_name}{"/" if folder_name else ""}{file_name}'
-    )
-    combined_name = os.path.normpath(combined_name)
-
-    return combined_name
-
-
-def determine_destination_name(
-    destination_folder_name, destination_file_name, source_full_path, file_number=None
-):
-    """
-    Determine the final destination name of the file being downloaded.
-    """
-    destination_file_name = determine_destination_file_name(
-        destination_file_name=destination_file_name,
-        source_full_path=source_full_path,
-        file_number=file_number,
-    )
-    destination_name = combine_folder_and_file_name(
-        destination_folder_name, destination_file_name
-    )
-    return destination_name
-
-
-def find_google_cloud_storage_file_names(bucket, prefix=""):
-    """
-    Fetched all the files in the bucket which are returned in a list as
-    Google Blob objects
-    """
-    return list(bucket.list_blobs(prefix=prefix))
-
-
-def find_matching_files(file_blobs, file_name_re):
-    """
-    Return a list of all file_names that matched the regular expression.
-    """
-    matching_file_names = []
-    for blob in file_blobs:
-        if re.search(file_name_re, blob.name):
-            matching_file_names.append(blob)
-
-    return matching_file_names
-
-
 def download_google_cloud_storage_file(blob, destination_file_name=None):
     """
     Download a selected file from Google Cloud Storage to local storage in
     the current working directory.
     """
-    local_path = os.path.normpath(f"{os.getcwd()}/{destination_file_name}")
+    local_path = os.path.join(os.getcwd(), destination_file_name)
 
     blob.download_to_filename(local_path)
 
-    print(f"{blob.bucket.name}/{blob.name} successfully downloaded to {local_path}")
-
-    return
+    logger.info(
+        f"{blob.bucket.name}/{blob.name} successfully downloaded to {local_path}"
+    )
 
 
-def get_gclient(args):
+def move_google_cloud_storage_file(
+    source_bucket, source_blob_path, destination_bucket, destination_blob_path
+):
     """
-    Attempts to create the Google Cloud Storage Client with the associated
-    environment variables
+    Moves blobs between directories or buckets. First copies the
+    blob to destination then deletes the source blob from the old location.
     """
-    try:
-        gclient = storage.Client()
-    except Exception as e:
-        print(
-            f"Error accessing Google Cloud Storage with service account "
-            f"{args.gcp_application_credentials}"
-        )
-        raise (e)
-
-    return gclient
+    # get source blob
+    source_blob = source_bucket.blob(source_blob_path)
 
+    # copy to destination
+    dest_blob = source_bucket.copy_blob(
+        source_blob, destination_bucket, destination_blob_path
+    )
+    # delete in old destination
+    source_blob.delete()
 
-def get_bucket(*, gclient, bucket_name):
-    """
-    Fetches and returns the bucket from Google Cloud Storage
-    """
-    try:
-        bucket = gclient.get_bucket(bucket_name)
-    except NotFound as e:
-        print(f"Bucket {bucket_name} does not exist\n {e}")
-        raise (e)
-
-    return bucket
+    logger.info(f"File moved from {source_blob} to {dest_blob}")
 
 
-def get_storage_blob(bucket, source_folder_name, source_file_name):
-    """
-    Fetches and returns the single source file blob from the buck on
-    Google Cloud Storage
-    """
-    source_path = source_file_name
-    if source_folder_name != "":
-        source_path = f"{source_folder_name}/{source_file_name}"
-    blob = bucket.get_blob(source_path)
+def main():
+    tmp_file = None
     try:
-        blob.exists()
-        return blob
-    except Exception as e:
-        print(f"File {source_path} does not exist")
-        raise (e)
+        args = get_args()
+        source_bucket_name = args.source_bucket_name
+        destination_bucket_name = args.destination_bucket_name
+        source_file_name = args.source_file_name
+        source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
+        source_file_name_match_type = args.source_file_name_match_type
 
+        destination_folder_name = shipyard.clean_folder_name(
+            args.destination_folder_name
+        )
+        destination_file_name = args.destination_file_name
 
-def main():
-    args = get_args()
-    tmp_file = set_environment_variables(args)
-    bucket_name = args.bucket_name
-    source_file_name = args.source_file_name
-    source_folder_name = clean_folder_name(args.source_folder_name)
-    source_full_path = combine_folder_and_file_name(
-        folder_name=source_folder_name, file_name=source_file_name
-    )
-    source_file_name_match_type = args.source_file_name_match_type
-    gcp_application_credentials = args.gcp_application_credentials
+        tmp_file = utils.set_environment_variables(args.gcp_application_credentials)
+        gclient = utils.get_gclient(args.gcp_application_credentials)
 
-    destination_folder_name = clean_folder_name(args.destination_folder_name)
-    if not os.path.exists(destination_folder_name) and (destination_folder_name != ""):
-        os.makedirs(destination_folder_name)
-
-    gclient = get_gclient(args)
-    bucket = get_bucket(gclient=gclient, bucket_name=bucket_name)
-
-    if source_file_name_match_type == "regex_match":
-        file_names = find_google_cloud_storage_file_names(
-            bucket=bucket, prefix=source_folder_name
+        source_bucket = utils.get_bucket(
+            gclient=gclient, bucket_name=source_bucket_name
         )
-        matching_file_names = find_matching_files(
-            file_names, re.compile(source_file_name)
+        destination_bucket = utils.get_bucket(
+            gclient=gclient, bucket_name=destination_bucket_name
         )
-        print(f"{len(matching_file_names)} files found. Preparing to download...")
 
-        for index, blob in enumerate(matching_file_names):
-            destination_name = determine_destination_name(
+        if args.source_file_name_match_type == "exact_match":
+            blob = utils.get_storage_blob(
+                bucket=source_bucket,
+                source_folder_name=source_folder_name,
+                source_file_name=source_file_name,
+            )
+            dest_file = shipyard.determine_destination_file_name(
+                source_full_path=blob.name, destination_file_name=destination_file_name
+            )
+            destination_full_path = shipyard.determine_destination_full_path(
                 destination_folder_name=destination_folder_name,
-                destination_file_name=args.destination_file_name,
-                source_full_path=blob.name,
-                file_number=index + 1,
+                destination_file_name=dest_file,
+                source_full_path=blob,
             )
-
-            print(f"Downloading file {index+1} of {len(matching_file_names)}")
-            download_google_cloud_storage_file(
-                blob=blob, destination_file_name=destination_name
+            move_google_cloud_storage_file(
+                source_bucket=source_bucket,
+                source_blob_path=blob.name,
+                destination_bucket=destination_bucket,
+                destination_blob_path=destination_full_path,
+            )
+        elif source_file_name_match_type == "regex_match":
+            blobs = list(source_bucket.list_blobs(prefix=source_folder_name))
+            file_names = list(map(lambda x: x.name, blobs))
+            matching_file_names = shipyard.find_all_file_matches(
+                file_names, re.compile(source_file_name)
             )
-    else:
-        blob = get_storage_blob(
-            bucket=bucket,
-            source_folder_name=source_folder_name,
-            source_file_name=source_file_name,
-        )
-        destination_name = determine_destination_name(
-            destination_folder_name=destination_folder_name,
-            destination_file_name=args.destination_file_name,
-            source_full_path=source_full_path,
-        )
 
-        download_google_cloud_storage_file(
-            blob=blob, destination_file_name=destination_name
-        )
-    if tmp_file:
-        print(f"Removing temporary credentials file {tmp_file}")
-        os.remove(tmp_file)
+            if not matching_file_names:
+                raise FileNotFoundError(f"No files found matching {source_file_name}")
+            number_of_matches = len(matching_file_names)
+            logger.info(f"{number_of_matches} files found. Preparing to move...")
+
+            for index, blob in enumerate(matching_file_names, 1):
+                destination_full_path = shipyard.determine_destination_full_path(
+                    destination_folder_name=destination_folder_name,
+                    destination_file_name=destination_file_name,
+                    source_full_path=blob,
+                    file_number=None if number_of_matches == 1 else index,
+                )
+                logger.info(f"moving file {index} of {number_of_matches}")
+                move_google_cloud_storage_file(
+                    source_bucket=source_bucket,
+                    source_blob_path=blob,
+                    destination_bucket=destination_bucket,
+                    destination_blob_path=destination_full_path,
+                )
+    except ExitCodeException as e:
+        logger.error(e)
+        sys.exit(e.exit_code)
+
+    except FileNotFoundError as e:
+        logger.error(e)
+        sys.exit(CloudStorage.EXIT_CODE_FILE_NOT_FOUND)
+    except Exception as e:
+        logger.error(e)
+        sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
+    finally:
+        if tmp_file:
+            logger.info(f"Removing temporary credentials file {tmp_file}")
+            os.remove(tmp_file)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_googlecloud-0.1.0/shipyard_googlecloud/googlecloud.py` & `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/googlecloud.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from google.cloud import storage
-from shipyard_templates import CloudStorage
 import json
 import os
 import tempfile
 
+from google.cloud import storage
+from shipyard_templates import CloudStorage
+
 
 class GoogleCloudClient(CloudStorage):
     def __init__(self, service_account: str) -> None:
         self.service_account = service_account
-        super().__init__(service_account=self.service_account)
+        # super().__init__(service_account=self.service_account)
 
     def _set_env_vars(self):
         try:
             json_credentials = json.loads(self.service_account)
             fd, path = tempfile.mkstemp()
             print(f"Storing json credentials temporarily at {path}")
             with os.fdopen(fd, "w") as tmp:
@@ -22,18 +23,18 @@
         except Exception as e:
             os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = self.service_account
 
     def connect(self):
         fd = self._set_env_vars()
         return storage.Client()
 
-    def move_or_rename_files(self):
+    def move(self):
         pass
 
-    def upload_files(self):
+    def upload(self):
         pass
 
-    def download_files(self):
+    def download(self):
         pass
 
-    def remove_files(self):
+    def remove(self):
         pass
```

### Comparing `shipyard_googlecloud-0.1.0/PKG-INFO` & `shipyard_googlecloud-0.2.0a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: shipyard-googlecloud
-Version: 0.1.0
+Version: 0.2.0a0
 Summary: A local client for connecting and working with Google Cloud Service
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: google-cloud-storage (==2.7.0)
+Requires-Dist: google-cloud-storage (>=2.15.0,<3.0.0)
 Requires-Dist: httplib2 (==0.15.0)
-Requires-Dist: shipyard-templates (==0.5.0a0)
-Requires-Dist: shipyard-utils (>=0.1.4,<0.2.0)
+Requires-Dist: shipyard-bp-utils (>=1.1.1,<2.0.0)
 Description-Content-Type: text/markdown
```

