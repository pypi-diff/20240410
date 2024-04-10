# Comparing `tmp/docprompt-0.2.4.tar.gz` & `tmp/docprompt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.4.tar", max compression
+gzip compressed data, was "docprompt-0.2.5.tar", max compression
```

## Comparing `docprompt-0.2.4.tar` & `docprompt-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.4/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.4/README.md
--rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.4/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.4/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.4/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.4/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.4/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.4/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.4/docprompt/provenance/util.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.4/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9472 2024-04-09 01:41:32.425414 docprompt-0.2.4/docprompt/schema/document.py
--rw-r--r--   0        0        0     6362 2024-04-05 21:39:49.476813 docprompt-0.2.4/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.4/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.4/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.4/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.4/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.4/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.4/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18333 2024-04-05 21:53:48.708070 docprompt-0.2.4/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.4/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.4/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.4/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.4/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.4/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.4/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.4/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.4/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.4/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.4/docprompt/utils/raster.py
--rw-r--r--   0        0        0     3655 2024-04-05 21:23:49.921077 docprompt-0.2.4/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.4/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-09 01:47:50.624269 docprompt-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.4/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.4/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.4/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.4/tests/test_date_extraction.py
--rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.4/tests/test_document.py
--rw-r--r--   0        0        0     1240 2024-04-09 01:41:32.425414 docprompt-0.2.4/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.4/tests/test_search.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.4/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.5/README.md
+-rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.5/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.5/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.5/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.5/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.5/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.5/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.5/docprompt/provenance/util.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.5/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9472 2024-04-09 01:41:32.425414 docprompt-0.2.5/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6362 2024-04-05 21:39:49.476813 docprompt-0.2.5/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.5/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.5/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.5/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.5/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.5/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.5/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18333 2024-04-05 21:53:48.708070 docprompt-0.2.5/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.5/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.5/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.5/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.5/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.5/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.5/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.5/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.5/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.5/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.5/docprompt/utils/raster.py
+-rw-r--r--   0        0        0     4015 2024-04-10 19:57:12.041828 docprompt-0.2.5/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.5/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-10 19:57:24.297921 docprompt-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.5/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.5/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.5/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.5/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.5/tests/test_document.py
+-rw-r--r--   0        0        0     1240 2024-04-09 01:41:32.425414 docprompt-0.2.5/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.5/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.5/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.5/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.5/PKG-INFO
```

### Comparing `docprompt-0.2.4/LICENSE` & `docprompt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/README.md` & `docprompt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/__init__.py` & `docprompt-0.2.5/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/_exec/ghostscript.py` & `docprompt-0.2.5/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/provenance/search.py` & `docprompt-0.2.5/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/provenance/source.py` & `docprompt-0.2.5/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/provenance/util.py` & `docprompt-0.2.5/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/schema/document.py` & `docprompt-0.2.5/docprompt/schema/document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/schema/layout.py` & `docprompt-0.2.5/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/schema/pipeline.py` & `docprompt-0.2.5/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/base.py` & `docprompt-0.2.5/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/message.py` & `docprompt-0.2.5/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/ocr/gcp.py` & `docprompt-0.2.5/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/ocr/result.py` & `docprompt-0.2.5/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/table_extraction/base.py` & `docprompt-0.2.5/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.2.5/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/tasks/table_extraction/result.py` & `docprompt-0.2.5/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/utils/date_extraction.py` & `docprompt-0.2.5/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/docprompt/utils/splitter.py` & `docprompt-0.2.5/docprompt/utils/splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,47 @@
 from typing import Iterator, Optional
 
 import pypdfium2 as pdfium
 
 from docprompt._exec.ghostscript import compress_pdf_to_bytes
 from docprompt.utils import get_page_count
 from threading import Lock
-import time
+import contextlib
+
 
 logger = logging.getLogger(__name__)
 
-PDFIUM_SPLIT_LOCK = Lock()
+PDFIUM_WRITE_LOCK = Lock()  # Deadlocks occur in threaded environments without this lock
 
 
 class UnsupportedDocumentType(ValueError):
     pass
 
 
+@contextlib.contextmanager
+def load_pdf_from_bytes(file_bytes: bytes):
+    pdf = pdfium.PdfDocument(file_bytes)
+
+    try:
+        yield pdf
+    finally:
+        pdf.close()
+
+
+@contextlib.contextmanager
+def writable_temp_pdf():
+    with PDFIUM_WRITE_LOCK:
+        pdf = pdfium.PdfDocument.new()
+
+        try:
+            yield pdf
+        finally:
+            pdf.close()
+
+
 def split_pdf_to_bytes(
     file_bytes: bytes,
     *,
     start_page: Optional[int] = None,
     stop_page: Optional[int] = None,
 ):
     """
@@ -33,68 +55,57 @@
     if stop_page is None:
         stop_page = get_page_count(file_bytes)
 
     if stop_page <= start_page:
         raise ValueError("stop_page must be greater than start_page")
 
     # Load the PDF from bytes
-    src_pdf = pdfium.PdfDocument(io.BytesIO(file_bytes))
-
-    # Create a new PDF for the current batch
-    dst_pdf = pdfium.PdfDocument.new()
+    with load_pdf_from_bytes(file_bytes) as src_pdf:
+        # Create a new PDF for the current batch
+        dst_pdf = pdfium.PdfDocument.new()
+
+        # Append pages to the batch
+        dst_pdf.import_pages(src_pdf, list(range(start_page, stop_page)))
+
+        # Save the batch PDF to a bytes buffer
+        pdf_bytes_buffer = io.BytesIO()
+        dst_pdf.save(pdf_bytes_buffer)
+        pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
 
-    # Append pages to the batch
-    dst_pdf.import_pages(src_pdf, list(range(start_page, stop_page)))
-
-    # Save the batch PDF to a bytes buffer
-    pdf_bytes_buffer = io.BytesIO()
-    dst_pdf.save(pdf_bytes_buffer)
-    pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
-
-    # Yield the bytes of the batch PDF
-    return pdf_bytes_buffer.getvalue()
+        # Yield the bytes of the batch PDF
+        return pdf_bytes_buffer.getvalue()
 
 
 def pdf_split_iter_fast(file_bytes: bytes, max_page_count: int) -> Iterator[bytes]:
     """
     Splits a PDF into batches of pages up to `max_page_count` pages quickly.
     """
-    # Load the PDF from bytes
-    with PDFIUM_SPLIT_LOCK:
-        src_pdf = pdfium.PdfDocument(io.BytesIO(file_bytes))
-
+    with load_pdf_from_bytes(file_bytes) as src_pdf:
         current_page = 0
         total_pages = len(src_pdf)
 
         while current_page < total_pages:
             # Determine the last page for the current batch
             last_page = min(current_page + max_page_count, total_pages)
 
-            dst_pdf = pdfium.PdfDocument.new()
-
-            # Append pages to the batch
-            dst_pdf.import_pages(src_pdf, list(range(current_page, last_page)))
-
-            # Save the batch PDF to a bytes buffer
-            pdf_bytes_buffer = io.BytesIO()
-            dst_pdf.save(pdf_bytes_buffer)
-            pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
-
-            dst_pdf.close()
+            with writable_temp_pdf() as dst_pdf:
+                # Append pages to the batch
+                dst_pdf.import_pages(src_pdf, list(range(current_page, last_page)))
+
+                # Save the batch PDF to a bytes buffer
+                pdf_bytes_buffer = io.BytesIO()
+                dst_pdf.save(pdf_bytes_buffer)
+                pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
 
             # Yield the bytes of the batch PDF
             yield pdf_bytes_buffer.getvalue()
 
             # Update the current page for the next batch
             current_page += max_page_count
 
-        src_pdf.close()
-
-    time.sleep(0.1)
-
 
 def pdf_split_iter_with_max_bytes(
     file_bytes: bytes, max_page_count: int, max_bytes: int
 ) -> Iterator[bytes]:
     """
     Splits a PDF into batches of pages up to `max_page_count` pages and `max_bytes` bytes.
     """
```

### Comparing `docprompt-0.2.4/docprompt/utils/util.py` & `docprompt-0.2.5/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/pyproject.toml` & `docprompt-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.4"
+version = "0.2.5"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.4/tests/fixtures/1.pdf` & `docprompt-0.2.5/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/fixtures/1_ocr.json` & `docprompt-0.2.5/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/test_date_extraction.py` & `docprompt-0.2.5/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/test_document.py` & `docprompt-0.2.5/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/test_layout_models.py` & `docprompt-0.2.5/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/test_search.py` & `docprompt-0.2.5/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/tests/util.py` & `docprompt-0.2.5/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.4/PKG-INFO` & `docprompt-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.4
+Version: 0.2.5
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.4 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.2.5 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

