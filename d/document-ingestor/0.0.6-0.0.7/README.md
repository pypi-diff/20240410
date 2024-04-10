# Comparing `tmp/document_ingestor-0.0.6-py3-none-any.whl.zip` & `tmp/document_ingestor-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2999 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-10 11:42 document_ingestor-0.0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2434 b- defN 24-Apr-10 11:42 document_ingestor-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 11:42 document_ingestor-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-10 11:42 document_ingestor-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      439 b- defN 24-Apr-10 11:42 document_ingestor-0.0.6.dist-info/RECORD
-5 files, 4057 bytes uncompressed, 2171 bytes compressed:  46.5%
+Zip file size: 2997 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-10 11:44 document_ingestor-0.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2413 b- defN 24-Apr-10 11:44 document_ingestor-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 11:44 document_ingestor-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-10 11:44 document_ingestor-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      439 b- defN 24-Apr-10 11:44 document_ingestor-0.0.7.dist-info/RECORD
+5 files, 4036 bytes uncompressed, 2169 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: document_ingestor-0.0.6.dist-info/LICENSE.txt
+Filename: document_ingestor-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: document_ingestor-0.0.6.dist-info/METADATA
+Filename: document_ingestor-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: document_ingestor-0.0.6.dist-info/WHEEL
+Filename: document_ingestor-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: document_ingestor-0.0.6.dist-info/top_level.txt
+Filename: document_ingestor-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: document_ingestor-0.0.6.dist-info/RECORD
+Filename: document_ingestor-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `document_ingestor-0.0.6.dist-info/LICENSE.txt` & `document_ingestor-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `document_ingestor-0.0.6.dist-info/METADATA` & `document_ingestor-0.0.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-ingestor
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 Author: Milan Anand Raj
 Author-email: Milan Anand Raj <manandraj20@iitk.ac.in>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,14 +32,13 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pymupdf <=1.23.11
 Requires-Dist: openai
 Requires-Dist: pinecone-client
 Requires-Dist: numpy
 Requires-Dist: tiktoken
-Requires-Dist: time
 
 # Document ingestor
 This package consumes one or more spanish constitution pdf and then processes it to generate the embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 
 # Requirements
 pymupdf==1.23.8
```

