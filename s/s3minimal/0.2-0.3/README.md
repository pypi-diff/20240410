# Comparing `tmp/s3minimal-0.2.tar.gz` & `tmp/s3minimal-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3minimal-0.2.tar", max compression
+gzip compressed data, was "s3minimal-0.3.tar", max compression
```

## Comparing `s3minimal-0.2.tar` & `s3minimal-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-10-11 01:55:34.013000 s3minimal-0.2/LICENSE
--rw-r--r--   0        0        0     2437 2023-10-11 02:43:51.988000 s3minimal-0.2/README.md
--rw-r--r--   0        0        0      639 2024-01-11 03:03:11.204224 s3minimal-0.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-10-11 01:55:34.014000 s3minimal-0.2/s3minimal/__init__.py
--rw-r--r--   0        0        0      304 2023-10-30 20:44:31.019501 s3minimal-0.2/s3minimal/errors.py
--rw-r--r--   0        0        0    10085 2024-01-11 02:59:01.892728 s3minimal-0.2/s3minimal/s3.py
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 s3minimal-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-11 01:55:34.013000 s3minimal-0.3/LICENSE
+-rw-r--r--   0        0        0     2437 2023-10-11 02:43:51.988000 s3minimal-0.3/README.md
+-rw-r--r--   0        0        0      639 2024-04-10 13:06:15.542532 s3minimal-0.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-10-11 01:55:34.014000 s3minimal-0.3/s3minimal/__init__.py
+-rw-r--r--   0        0        0      304 2023-10-30 20:44:31.019501 s3minimal-0.3/s3minimal/errors.py
+-rw-r--r--   0        0        0    10028 2024-04-10 13:05:52.426956 s3minimal-0.3/s3minimal/s3.py
+-rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 s3minimal-0.3/PKG-INFO
```

### Comparing `s3minimal-0.2/LICENSE` & `s3minimal-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3minimal-0.2/README.md` & `s3minimal-0.3/README.md`

 * *Files identical despite different names*

### Comparing `s3minimal-0.2/pyproject.toml` & `s3minimal-0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s3minimal"
-version = "0.2"
+version = "0.3"
 description = "A Python library designed to simplify interactions with Amazon S3 using the `aiobotocore` and `botocore` libraries. It provides asynchronous and synchronous classes for various S3 operations."
 authors = ["Jamal <jsaied99@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jsaied99/s3minimal/"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `s3minimal-0.2/s3minimal/s3.py` & `s3minimal-0.3/s3minimal/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         """
         Sets the bucket to be used for S3.
         # Example:
         >>> set_bucket("bucket_name")
         None
         """
         self.bucket = os.getenv("AWS_BUCKET", bucket)
-        print(f"Using bucket {self.bucket}")
 
     async def __get_client(self):
         """
         Gets a client for S3. This is a private method.
         """
         return self.session.create_client(
             "s3",
@@ -162,15 +161,15 @@
                     cors_configuration = kwargs.get("cors_configuration", {})
                     await client.put_bucket_cors(
                         Bucket=bucket_name,
                         CORSConfiguration=cors_configuration,
                     )
             except ClientError as e:
                 raise CreateBucketError(f"Failed to create bucket {bucket_name}: {e}")
-            
+
     def get_client(self):
         """
         Gets a client for S3. This is a private method.
         #Opening this for compatibility with other libraries
         """
         return self.__get_client()
```

### Comparing `s3minimal-0.2/PKG-INFO` & `s3minimal-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3minimal
-Version: 0.2
+Version: 0.3
 Summary: A Python library designed to simplify interactions with Amazon S3 using the `aiobotocore` and `botocore` libraries. It provides asynchronous and synchronous classes for various S3 operations.
 Home-page: https://github.com/jsaied99/s3minimal/
 License: MIT
 Author: Jamal
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

