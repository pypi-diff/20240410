# Comparing `tmp/document_ingestor-0.0.4.tar.gz` & `tmp/document_ingestor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_ingestor-0.0.4.tar", last modified: Mon Mar 25 11:41:56 2024, max compression
+gzip compressed data, was "document_ingestor-0.0.5.tar", last modified: Wed Apr 10 11:05:39 2024, max compression
```

## Comparing `document_ingestor-0.0.4.tar` & `document_ingestor-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 11:41:56.281332 document_ingestor-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1007 2024-03-25 11:41:56.273624 document_ingestor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.0.4/README.md
--rw-rw-rw-   0        0        0      706 2024-03-25 11:39:30.000000 document_ingestor-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-25 11:41:56.281332 document_ingestor-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-25 11:41:56.185982 document_ingestor-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-25 11:41:56.238832 document_ingestor-0.0.4/src/document_ingestor/
--rw-rw-rw-   0        0        0        0 2024-03-24 16:55:37.000000 document_ingestor-0.0.4/src/document_ingestor/__init__.py
--rw-rw-rw-   0        0        0     5779 2024-03-25 11:38:33.000000 document_ingestor-0.0.4/src/document_ingestor/embedding_process.py
--rw-rw-rw-   0        0        0     6093 2024-03-24 16:55:37.000000 document_ingestor-0.0.4/src/document_ingestor/pdf_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-25 11:41:56.273624 document_ingestor-0.0.4/src/document_ingestor.egg-info/
--rw-rw-rw-   0        0        0     1007 2024-03-25 11:41:56.000000 document_ingestor-0.0.4/src/document_ingestor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-03-25 11:41:56.000000 document_ingestor-0.0.4/src/document_ingestor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 11:41:56.000000 document_ingestor-0.0.4/src/document_ingestor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-25 11:41:56.000000 document_ingestor-0.0.4/src/document_ingestor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 11:05:39.625039 document_ingestor-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2434 2024-04-10 11:05:39.625039 document_ingestor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 11:05:39.622310 document_ingestor-0.0.5/document_ingestor.egg-info/
+-rw-rw-rw-   0        0        0     2434 2024-04-10 11:05:39.000000 document_ingestor-0.0.5/document_ingestor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-10 11:05:39.000000 document_ingestor-0.0.5/document_ingestor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:05:39.000000 document_ingestor-0.0.5/document_ingestor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-10 11:05:39.000000 document_ingestor-0.0.5/document_ingestor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:05:39.000000 document_ingestor-0.0.5/document_ingestor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      968 2024-04-10 11:05:27.000000 document_ingestor-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      818 2024-04-10 11:05:39.625039 document_ingestor-0.0.5/setup.cfg
```

### Comparing `document_ingestor-0.0.4/LICENSE.txt` & `document_ingestor-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.0.4/pyproject.toml` & `document_ingestor-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 [project]
 name = "document_ingestor"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
-  { name="Milan Anand Raj", email="manandraj20@iitk.ac.in" },
+  { name = "Milan Anand Raj", email = "manandraj20@iitk.ac.in" },
 ]
-description = "This package consumes one or more spanish constitution pdf and then processes it to generate the embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors."
+description = "This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pymupdf<=1.23.11",
+    "openai",
+    "pinecone-client",
+    "numpy",
+    "tikitoken",
+    "time",
+]
+license = {file = "LICENSE.txt"} 
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
+Issues = "https://github.com/pypa/sampleproject/issues"
+
+
+
```

