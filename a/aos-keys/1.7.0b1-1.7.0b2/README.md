# Comparing `tmp/aos_keys-1.7.0b1-py3-none-any.whl.zip` & `tmp/aos_keys-1.7.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 17738 bytes, number of entries: 16
+Zip file size: 17740 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      117 b- defN 22-Jun-30 08:41 aos_keys/__init__.py
 -rw-rw-r--  2.0 unx     6720 b- defN 24-Feb-02 11:35 aos_keys/actions.py
 -rw-rw-r--  2.0 unx    11336 b- defN 24-Feb-02 11:35 aos_keys/certificate_manager.py
 -rw-rw-r--  2.0 unx     3239 b- defN 24-Feb-02 11:35 aos_keys/cloud_api.py
 -rw-rw-r--  2.0 unx     4323 b- defN 24-Feb-02 11:35 aos_keys/common.py
 -rw-rw-r--  2.0 unx     4959 b- defN 24-Mar-05 13:59 aos_keys/crypto_container.py
--rw-rw-r--  2.0 unx     6186 b- defN 24-Feb-02 11:35 aos_keys/key_manager.py
+-rw-rw-r--  2.0 unx     6194 b- defN 24-Mar-08 10:19 aos_keys/key_manager.py
 -rw-rw-r--  2.0 unx     8451 b- defN 24-Feb-02 11:35 aos_keys/main.py
 -rw-rw-r--  2.0 unx     1452 b- defN 22-Sep-23 09:10 aos_keys/files/1rootCA.crt
 -rw-rw-r--  2.0 unx      113 b- defN 22-Jun-30 08:41 aos_keys/files/__init__.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Mar-08 09:39 aos_keys-1.7.0b1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-08 09:39 aos_keys-1.7.0b1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 24-Mar-08 09:39 aos_keys-1.7.0b1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 24-Mar-08 09:39 aos_keys-1.7.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-23 08:16 aos_keys-1.7.0b1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1293 b- defN 24-Mar-08 09:39 aos_keys-1.7.0b1.dist-info/RECORD
-16 files, 50936 bytes uncompressed, 15608 bytes compressed:  69.4%
+-rw-rw-r--  2.0 unx     2597 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-23 08:16 aos_keys-1.7.0b2.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     1293 b- defN 24-Mar-08 10:24 aos_keys-1.7.0b2.dist-info/RECORD
+16 files, 50944 bytes uncompressed, 15610 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: aos_keys/files/1rootCA.crt
 Comment: 
 
 Filename: aos_keys/files/__init__.py
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/METADATA
+Filename: aos_keys-1.7.0b2.dist-info/METADATA
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/WHEEL
+Filename: aos_keys-1.7.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/entry_points.txt
+Filename: aos_keys-1.7.0b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/top_level.txt
+Filename: aos_keys-1.7.0b2.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/zip-safe
+Filename: aos_keys-1.7.0b2.dist-info/zip-safe
 Comment: 
 
-Filename: aos_keys-1.7.0b1.dist-info/RECORD
+Filename: aos_keys-1.7.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_keys/key_manager.py

```diff
@@ -131,16 +131,16 @@
     table.add_column('', style='bold')
     table.add_row('File: ', cert_file_path)
     _print_cert_field(table, 'Aos base domain: ', certificate, NameOID.ORGANIZATION_NAME)
     table.add_row('Serial number: ', f'{certificate.serial_number:X}')
     _print_cert_field(table, 'User: ', certificate, NameOID.COMMON_NAME)
     _print_cert_field(table, 'e-mail: ', certificate, NameOID.EMAIL_ADDRESS)
     _print_cert_field(table, 'Company name: ', certificate, NameOID.ORGANIZATIONAL_UNIT_NAME)
-    table.add_row('Valid not before: ', str(datetime_from_utc_to_local(certificate.not_valid_before)))
-    table.add_row('Valid not after: ', str(datetime_from_utc_to_local(certificate.not_valid_after)))
+    table.add_row('Valid not before: ', str(datetime_from_utc_to_local(certificate.not_valid_before_utc)))
+    table.add_row('Valid not after: ', str(datetime_from_utc_to_local(certificate.not_valid_after_utc)))
     console.print(table)
 
 
 def pem_to_pkcs12_bytes(private_key_pem: bytes, certificate_pem: bytes, friendly_name: str) -> bytes:
     """
     Create pkcs12 container from private key and certificate.
```

## Comparing `aos_keys-1.7.0b1.dist-info/METADATA` & `aos_keys-1.7.0b2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-keys
-Version: 1.7.0b1
+Version: 1.7.0b2
 Summary: AosEdge private keys and certificate manager
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `aos_keys-1.7.0b1.dist-info/RECORD` & `aos_keys-1.7.0b2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 aos_keys/__init__.py,sha256=uvRZHZ9NW2hkD1OdQb_DWAxB-NpqhCYWJyMKF3XP1Xg,117
 aos_keys/actions.py,sha256=fiUcpGgLQ8IBpNzW1zAsXNYJBNf3_kAYPvaSIpkmVIs,6720
 aos_keys/certificate_manager.py,sha256=M2UzrKUF7MXtGKhug84SESmwuqrEDKM-7gN9yxAGm9E,11336
 aos_keys/cloud_api.py,sha256=OrkbpciDzZXVn592HIWsHQ9GcBkyFRB6Qapi63stzj4,3239
 aos_keys/common.py,sha256=IU6JpwEWXvv-Qz49O0sRjbEKGtx9J-Y8z0nUYqOq-1M,4323
 aos_keys/crypto_container.py,sha256=8EvPQ1Vaom_0GfKn0Dw88AWtfzSeDAdxWrSF07DRmKg,4959
-aos_keys/key_manager.py,sha256=J52PSyc8CvjaOwn0S9AAwoVYMmm5gG-AsTp60046MjE,6186
+aos_keys/key_manager.py,sha256=nnPtsFgCCVoXEAHZJ61X23Cn8zfv4R5_UpEZl7-x6GI,6194
 aos_keys/main.py,sha256=v7OLfFPzjj_-1qWTxFZRjgN0BP_WlcDtXE5RNyG2lFg,8451
 aos_keys/files/1rootCA.crt,sha256=F1BzQ7LOEmNEi2Nl-QJ7s8xRIFLxWlFypOtRSwr84Yg,1452
 aos_keys/files/__init__.py,sha256=RugobKGxKbmCthe2-PYP85pYv7Gfzikpl_SQZ0vFfw8,113
-aos_keys-1.7.0b1.dist-info/METADATA,sha256=XCFtHpEkw4wrkaGb-1KS4lX03F6WF1qHO536enNQ1aA,2597
-aos_keys-1.7.0b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_keys-1.7.0b1.dist-info/entry_points.txt,sha256=sDI5cvPlgS-4UUF6Kc7ke2gk8wYpeyfr8SbVuNQvG-g,48
-aos_keys-1.7.0b1.dist-info/top_level.txt,sha256=IoCBFe4GEf-X3P8RfB0WvObZxCVLDWbTjgIKMaLo1jY,9
-aos_keys-1.7.0b1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-aos_keys-1.7.0b1.dist-info/RECORD,,
+aos_keys-1.7.0b2.dist-info/METADATA,sha256=DKORRYYmUmmEQ3Mr2YMnKA9dSPhTIRksiIQbOz8mhTc,2597
+aos_keys-1.7.0b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_keys-1.7.0b2.dist-info/entry_points.txt,sha256=sDI5cvPlgS-4UUF6Kc7ke2gk8wYpeyfr8SbVuNQvG-g,48
+aos_keys-1.7.0b2.dist-info/top_level.txt,sha256=IoCBFe4GEf-X3P8RfB0WvObZxCVLDWbTjgIKMaLo1jY,9
+aos_keys-1.7.0b2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+aos_keys-1.7.0b2.dist-info/RECORD,,
```

