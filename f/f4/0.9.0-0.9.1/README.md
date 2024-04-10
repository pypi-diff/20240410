# Comparing `tmp/f4-0.9.0.tar.gz` & `tmp/f4-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.0.tar", last modified: Fri Mar  8 17:13:18 2024, max compression
+gzip compressed data, was "f4-0.9.1.tar", last modified: Wed Apr 10 20:31:51 2024, max compression
```

## Comparing `f4-0.9.0.tar` & `f4-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2024-03-08 17:13:18.461748 f4-0.9.0/
--rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.9.0/LICENSE
--rw-r--r--   0 srp33      (501) staff       (20)      711 2024-03-08 17:13:18.461624 f4-0.9.0/PKG-INFO
--rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.9.0/README.md
--rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.9.0/pyproject.toml
--rw-r--r--   0 srp33      (501) staff       (20)      733 2024-03-08 17:13:18.462288 f4-0.9.0/setup.cfg
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2024-03-08 17:13:18.449904 f4-0.9.0/src/
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2024-03-08 17:13:18.456643 f4-0.9.0/src/f4/
--rwxr-xr-x   0 srp33      (501) staff       (20)    53983 2024-03-08 16:47:13.000000 f4-0.9.0/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (501) staff       (20)    58076 2024-03-08 15:30:15.000000 f4-0.9.0/src/f4/Parser.py
--rwxr-xr-x   0 srp33      (501) staff       (20)     8144 2024-03-08 17:12:59.000000 f4-0.9.0/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (501) staff       (20)      368 2024-02-08 00:16:33.000000 f4-0.9.0/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2024-03-08 17:13:18.461079 f4-0.9.0/src/f4.egg-info/
--rw-r--r--   0 srp33      (501) staff       (20)      711 2024-03-08 17:13:18.000000 f4-0.9.0/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (501) staff       (20)      278 2024-03-08 17:13:18.000000 f4-0.9.0/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (501) staff       (20)        1 2024-03-08 17:13:18.000000 f4-0.9.0/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (501) staff       (20)       67 2024-03-08 17:13:18.000000 f4-0.9.0/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (501) staff       (20)        3 2024-03-08 17:13:18.000000 f4-0.9.0/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2024-03-08 17:13:18.459194 f4-0.9.0/test/
--rwxr-xr-x   0 srp33      (501) staff       (20)    56275 2024-03-08 16:47:23.000000 f4-0.9.0/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-10 20:31:51.466842 f4-0.9.1/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.1/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-10 20:31:51.466771 f4-0.9.1/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.1/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.1/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-10 20:31:51.467154 f4-0.9.1/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-10 20:31:51.460725 f4-0.9.1/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-10 20:31:51.464636 f4-0.9.1/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    47512 2024-04-08 23:50:37.000000 f4-0.9.1/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-05 19:33:49.000000 f4-0.9.1/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    10745 2024-04-09 17:49:11.000000 f4-0.9.1/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-09 20:02:03.000000 f4-0.9.1/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-03 21:29:18.000000 f4-0.9.1/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-10 20:31:51.466541 f4-0.9.1/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-10 20:31:51.000000 f4-0.9.1/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-10 20:31:51.000000 f4-0.9.1/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-10 20:31:51.000000 f4-0.9.1/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-10 20:31:51.000000 f4-0.9.1/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-10 20:31:51.000000 f4-0.9.1/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-10 20:31:51.465844 f4-0.9.1/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55966 2024-04-09 20:01:24.000000 f4-0.9.1/test/test.py
```

### Comparing `f4-0.9.0/LICENSE` & `f4-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.0/PKG-INFO` & `f4-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.0/setup.cfg` & `f4-0.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.0
+version = 0.9.1
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.0/src/f4/Builder.py` & `f4-0.9.1/src/f4/Builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,14 @@
 
     # Save and format data to a temp file for each column chunk.
     joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(save_formatted_data)(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, chunk_indices[0], chunk_indices[1], tmp_dir_path2, out_items_chunk_size, verbose) for chunk_number, chunk_indices in enumerate(column_chunk_indices))
 
     # Combine column databases across the chunks.
     combine_column_databases(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path2, verbose)
 
-#TODO: Compress all intermediate files
-
     # Create meta files for all columns.
     save_column_name_info(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
     save_column_types(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
     save_column_coordinates(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
 
     # Merge the saved/formatted data across the column chunks.
     # Get number of rows.
@@ -90,86 +88,14 @@
     combine_into_single_file(delimited_file_path, f4_file_path, tmp_dir_path2, file_read_chunk_size, verbose)
 
     rmtree(tmp_dir_path2)
 
     print_message(f"Done converting {delimited_file_path} to {f4_file_path}.", verbose)
 
 #TODO: Move to a different file so we don't need to import Parser?
-# def transpose(f4_src_file_path, f4_dest_file_path, num_parallel=1, tmp_dir_path=None, verbose=False):
-#     if num_parallel > 1:
-#         global joblib
-#         joblib = __import__('joblib', globals(), locals())
-#
-#     print_message(f"Transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
-#
-#     if tmp_dir_path:
-#         makedirs(tmp_dir_path, exist_ok=True)
-#     else:
-#         tmp_dir_path = mkdtemp()
-#
-#     tmp_dir_path = fix_dir_path_ending(tmp_dir_path)
-#     makedirs(tmp_dir_path, exist_ok=True)
-#     tmp_tsv_file_path = f"{tmp_dir_path}tmp.tsv.gz"
-#
-#     with initialize(f4_src_file_path) as src_file_data:
-#         column_names, column_type_dict, column_coords_dict, bigram_size_dict = get_column_meta(src_file_data, set(), [])
-#         column_coords = [column_coords_dict[name] for name in column_names]
-#         num_rows = src_file_data.stat_dict["num_rows"]
-#
-#     if num_parallel == 1:
-#         chunk_file_path = transpose_lines_to_temp(f4_src_file_path, tmp_dir_path, 0, num_rows, column_names, column_coords, bigram_size_dict, verbose)
-#
-#         print_message(f"Extracting transposed values from {chunk_file_path} for {f4_src_file_path}.", verbose)
-#         with gzip.open(tmp_tsv_file_path, "w", compresslevel=1) as tmp_tsv_file:
-#             with open(chunk_file_path, "rb") as chunk_file:
-#                 for column_index, column_name in enumerate(column_names):
-#                     tmp_tsv_file.write(column_name)
-#
-#                     column_size = column_coords[column_index][1] - column_coords[column_index][0]
-#                     for row_index in range(num_rows):
-#                         tmp_tsv_file.write(b"\t" + chunk_file.read(column_size))
-#
-#                     tmp_tsv_file.write(b"\n")
-#
-#             remove(chunk_file_path)
-#     else:
-#         row_index_chunks = list(split_integer_list_into_chunks(list(range(num_rows)), num_parallel))
-#
-#         chunk_file_paths = joblib.Parallel(n_jobs=num_parallel)(
-#              joblib.delayed(transpose_lines_to_temp)(f4_src_file_path, tmp_dir_path, row_index_chunk[0], row_index_chunk[-1] + 1, column_names, column_coords, bigram_size_dict, verbose) for row_index_chunk in row_index_chunks)
-#
-#         chunk_file_handles = {}
-#         for row_index_chunk in row_index_chunks:
-#             chunk_file_path = f"{tmp_dir_path}{row_index_chunk[0]}"
-#             chunk_file_handles[chunk_file_path] = open(chunk_file_path, "rb")
-#
-#         try:
-#             with gzip.open(tmp_tsv_file_path, "w", compresslevel=1) as tmp_tsv_file:
-#                 for column_index, column_name in enumerate(column_names):
-#                     tmp_tsv_file.write(column_name)
-#
-#                     column_size = column_coords[column_index][1] - column_coords[column_index][0]
-#
-#                     for row_index_chunk in row_index_chunks:
-#                         chunk_file_path = f"{tmp_dir_path}{row_index_chunk[0]}"
-#
-#                         for row_index in range(row_index_chunk[0], row_index_chunk[-1] + 1):
-#                             tmp_tsv_file.write(b"\t" + chunk_file_handles[chunk_file_path].read(column_size))
-#
-#                     tmp_tsv_file.write(b"\n")
-#         finally:
-#             for chunk_file_path in chunk_file_handles:
-#                 chunk_file_handles[chunk_file_path].close()
-#                 remove(chunk_file_path)
-#
-#     print_message(f"Converting temp file at {tmp_tsv_file_path} to {f4_dest_file_path}.", verbose)
-#     convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, compression_type=src_file_data.decompression_type, num_parallel=num_parallel, verbose=verbose)
-#     remove(tmp_tsv_file_path)
-
-#TODO: Move to a different file so we don't need to import Parser?
 # def inner_join(f4_left_src_file_path, f4_right_src_file_path, join_column, f4_dest_file_path, num_parallel=1, tmp_dir_path=None, verbose=False):
 #     print_message(f"Inner joining {f4_left_src_file_path} and {f4_right_src_file_path} based on the {join_column} column, saving to {f4_dest_file_path}.", verbose)
 #
 #     join_column = join_column.encode()
 #
 #     if tmp_dir_path:
 #         makedirs(tmp_dir_path, exist_ok=True)
@@ -258,15 +184,15 @@
                         max_column_name_length = len(column_name)
 
         for column_name in next_text[:newline_index].split(delimiter):
             current_column_index += 1
             if len(column_name) > max_column_name_length:
                 max_column_name_length = len(column_name)
 
-        in_file.seek(current_index + newline_index + 1)
+        # in_file.seek(current_index + newline_index + 1)
 
     num_cols = current_column_index + 1
 
     if num_cols == 0:
         raise Exception(f"No data was detected in {delimited_file_path}.")
 
     return num_cols, max_column_name_length
@@ -328,15 +254,15 @@
             if start_column_index <= current_column_index < end_column_index:
                 save_tuples.append((current_column_index, column_name,))
 
                 if len(save_tuples) == out_items_chunk_size:
                     cursor.executemany(sql, save_tuples)
                     save_tuples = []
 
-        in_file.seek(current_index + newline_index + 1)
+        # in_file.seek(current_index + newline_index + 1)
 
     if len(save_tuples) > 0:
         cursor.executemany(sql, save_tuples)
 
 # This function is executed in parallel.
 def parse_column_info(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, start_column_index, end_column_index, tmp_dir_path, out_items_chunk_size, verbose):
     print_message(f"Parsing column names, sizes, and types when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose)
@@ -354,15 +280,15 @@
                     WHERE column_index = ?'''
 
     num_rows = 0
 
     # We will find the max size for each column and count how many there are of each type.
     with get_delimited_file_handle(delimited_file_path) as in_file:
         skip_comments(in_file, comment_prefix)
-        skip_line(in_file)
+        skip_line(in_file) # Header line
 
         # Loop through the file for the specified columns and update the dictionaries.
         save_tuples = []
         for column_index, value in iterate_delimited_file_column_indices(in_file, delimiter, file_read_chunk_size, start_column_index, end_column_index):
             if column_index == start_column_index:
                 num_rows += 1
 
@@ -490,15 +416,14 @@
     cursor = conn.cursor()
 
     max_column_name_length = get_max_column_length(cursor, "column_name")
     max_column_index_length = get_max_column_length(cursor, "column_index")
 
     ##########################################################
     # cni = column name first, sorted by column name
-    # cin = column index first, sorted by column index
     ##########################################################
 
     cniccml = max(len(str(max_column_name_length)), len(str(max_column_name_length + max_column_index_length)))
     write_str_to_file(get_data_path(tmp_dir_path, "cniccml"), str(cniccml).encode())
 
     cnicc = format_string_as_fixed_width(b"0", cniccml)
     cnicc += format_string_as_fixed_width(str(max_column_name_length).encode(), cniccml)
@@ -1045,51 +970,60 @@
             with open_temp_file_compressed(file_path) as component_file:
                 while chunk := component_file.read(read_chunk_size):
                     f4_file.write(chunk)
 
             remove(file_path)
 
 def skip_comments(in_file, comment_prefix):
+    if comment_prefix is None:
+        return
+
     next_text = in_file.read(len(comment_prefix))
 
     while next_text == comment_prefix:
         skip_line(in_file)
         next_text = in_file.read(len(comment_prefix))
 
     in_file.seek(in_file.tell() - len(next_text))
 
-# This function is slow when working with gzipped files because of the backwards seek(). Only use it sparingly.
 def skip_line(in_file):
-    chunk_size = 100000
-    current_index = in_file.tell()
-
-    while (newline_index := (next_text := in_file.read(chunk_size)).find(b"\n")) == -1:
-        current_index += len(next_text)
-
-    in_file.seek(current_index + newline_index + 1)
-
-def skip_lines(in_file, num_lines_to_skip):
-    if num_lines_to_skip <= 0:
-        return
+    while True:
+        next_char = in_file.read(1)
+        if next_char == b"\n":
+            break
 
-    chunk_size = 100000
-    num_lines_skipped = 0
-
-    while next_text := in_file.read(chunk_size):
-        how_far_to_reverse = len(next_text)
-
-        while (newline_index := next_text.find(b"\n")) > -1:
-            num_lines_skipped += 1
-            how_far_to_reverse -= newline_index + 1
-
-            if num_lines_skipped == num_lines_to_skip:
-                in_file.seek(in_file.tell() - how_far_to_reverse)
-                return
-            else:
-                next_text = next_text[newline_index + 1:]
+# This function is slow when working with gzipped files because of the backwards seek(). Only use it sparingly.
+# def skip_line(in_file):
+#     chunk_size = 100000
+#     current_index = in_file.tell()
+#
+#     while (newline_index := (next_text := in_file.read(chunk_size)).find(b"\n")) == -1:
+#         current_index += len(next_text)
+#
+#     in_file.seek(current_index + newline_index + 1)
+
+# def skip_lines(in_file, num_lines_to_skip):
+#     if num_lines_to_skip <= 0:
+#         return
+#
+#     chunk_size = 100000
+#     num_lines_skipped = 0
+#
+#     while next_text := in_file.read(chunk_size):
+#         how_far_to_reverse = len(next_text)
+#
+#         while (newline_index := next_text.find(b"\n")) > -1:
+#             num_lines_skipped += 1
+#             how_far_to_reverse -= newline_index + 1
+#
+#             if num_lines_skipped == num_lines_to_skip:
+#                 in_file.seek(in_file.tell() - how_far_to_reverse)
+#                 return
+#             else:
+#                 next_text = next_text[newline_index + 1:]
 
 def iterate_delimited_file_column_indices(in_file, delimiter, file_read_chunk_size, start_column_index, end_column_index):
     previous_text = b""
     current_column_index = -1
 
     while next_text := in_file.read(file_read_chunk_size):
         next_text = previous_text + next_text
@@ -1151,61 +1085,7 @@
 #         if b' ' not in i.to_bytes(length = length, byteorder = "big"):
 #             ints.append(i)
 #
 #         i += 1
 #
 #     for i in ints:
 #         yield i, values.pop(0)
-
-def prepare_tmp_dir(tmp_dir_path):
-    # Figure out where temp files will be stored and create directory, if needed.
-    if tmp_dir_path:
-        makedirs(tmp_dir_path, exist_ok=True)
-        tmp_dir_path = tmp_dir_path
-    else:
-        tmp_dir_path = mkdtemp()
-
-    unique_id = uuid4()
-    tmp_dir_path = fix_dir_path_ending(tmp_dir_path) + f"f4_{unique_id}/"
-    makedirs(tmp_dir_path, exist_ok=True)
-
-    return tmp_dir_path
-
-#TODO: Move to a different file so we don't need to import Parser?
-# def transpose_lines_to_temp(data_file_path, tmp_dir_path, start_row_index, end_row_index, column_names, column_coords, bigram_size_dict, verbose):
-#     with initialize(data_file_path) as file_data:
-#         tmp_file_path = f"{tmp_dir_path}{start_row_index}"
-#         print_message(f"Transposing lines to {tmp_file_path} for {data_file_path} - start row {start_row_index}, end row {end_row_index}.", verbose)
-#
-#         with open(tmp_file_path, "wb+") as tmp_file:
-#             num_rows = end_row_index - start_row_index
-#
-#             for column_index in range(len(column_names)):
-#                 # Create placeholder space for column values in temp file
-#                 column_coord = column_coords[column_index]
-#                 tmp_file.write(b" " * (column_coord[1] - column_coord[0]) * num_rows)
-#
-#             tmp_file.flush()
-#
-#             with mmap(tmp_file.fileno(), 0, prot=PROT_WRITE) as mm_handle:
-#                 # Iterate through each row and save the values in the correct locations in the temp file
-#                 parse_function = get_parse_row_values_function(file_data)
-#
-#                 # Find the start position of each row
-#                 out_line_positions = [0]
-#                 for column_index in range(1, len(column_names)):
-#                     previous_column_size = column_coords[column_index - 1][1] - column_coords[column_index - 1][0]
-#                     this_line_position = out_line_positions[-1] + previous_column_size * num_rows
-#                     out_line_positions.append(this_line_position)
-#
-#                 # Iterate through each row and store the values in the respective column
-#                 for row_index in range(start_row_index, end_row_index):
-#                     row_values = parse_function(file_data, row_index, column_coords, bigram_size_dict=bigram_size_dict)
-#
-#                     for column_index, value in enumerate(row_values):
-#                         out_position = out_line_positions[column_index]
-#                         column_size = column_coords[column_index][1] - column_coords[column_index][0]
-#                         value = format_string_as_fixed_width(value, column_size)
-#                         mm_handle[out_position:(out_position + len(value))] = value
-#                         out_line_positions[column_index] += len(value)
-#
-#         return tmp_file_path
```

### Comparing `f4-0.9.0/src/f4/Parser.py` & `f4-0.9.1/src/f4/Parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -743,20 +743,27 @@
 
         if column_name in column_names_set:
             column_indices.append(column_index)
 
     return column_indices
 
 # def get_column_name_from_index(file_data, column_index):
-#     position = get_identifier_row_index(file_data, "cin", column_index, file_data.cache_dict["num_cols"])
+#     cn_start = file_data.file_map_dict["cn"][0]
+#     cn_end = file_data.file_map_dict["cn"][1]
 #
-#     if position < 0:
-#         raise Exception(f"Could not retrieve name because column index {column_index.decode()} was not found.")
-#
-#     return position
+#     cn_current = cn_start
+#     column_index_current = 0
+
+
+
+    # column_name = b""
+    # while cn_current < cn_end and (next_char := src_file_data.file_handle[cn_current:(cn_current + 1)]) != b"\n":
+    #     column_name += next_char
+    #     cn_current += 1
+    # cn_current += 1
 
 def get_column_type_from_index(file_data, column_index):
     return next(parse_data_values_from_file(file_data, "ct", column_index, 1, [[0, 1]])).decode()
 
 def get_value_from_single_column_file(file_handle, content_start_index, segment_length, row_index):
     start_search_position = content_start_index + row_index * segment_length
     return file_handle[start_search_position:(start_search_position + segment_length)].rstrip(b" ")
@@ -823,19 +830,16 @@
 
     for coords in data_coords:
         yield file_data.file_handle[(start_pos + coords[0]):(start_pos + coords[1])].rstrip(b" ")
 
 def get_parse_row_value_function(file_data):
     if not file_data.decompression_type:
         return parse_row_value
-    # elif file_data.decompression_type == "zstd":
     else:
         return parse_zstd_compressed_row_value
-    # else:
-    #     return parse_dictionary_compressed_row_value
 
 def parse_row_value(file_data, data_file_key, row_index, column_coords):
     return parse_data_value_from_file(file_data, data_file_key, row_index, file_data.cache_dict[data_file_key + "ll"], column_coords).rstrip(b" ")
 
 def parse_zstd_compressed_row_value(file_data, data_file_key, row_index, column_coords):
     line = get_zstd_compressed_row(file_data, row_index)
 
@@ -879,19 +883,16 @@
 # def parse_dictionary_compressed_row_value(file_data, data_file_key, row_index, column_coords, bigram_size_dict=None, column_name=None):
 #     value = parse_data_value_from_file(file_data, data_file_key, row_index, file_data.cache_dict["ll"], column_coords).rstrip(b" ")
 #     return decompress(value, file_data.decompressor[column_name], bigram_size_dict[column_name])
 
 def get_parse_row_values_function(file_data):
     if not file_data.decompression_type:
         return parse_row_values
-    # elif file_data.decompression_type == "zstd":
     else:
         return parse_zstd_compressed_row_values
-    # else:
-    #     return parse_dictionary_compressed_row_values
 
 def parse_row_values(file_data, data_file_key, row_index, column_coords):
     return list(parse_data_values_from_file(file_data, data_file_key, row_index, file_data.cache_dict[data_file_key + "ll"], column_coords))
 
 def parse_zstd_compressed_row_values(file_data, data_file_key, row_index, column_coords):
     line = get_zstd_compressed_row(file_data, row_index)
 
@@ -1232,8 +1233,8 @@
         upper_position = end_search_position
     else:
         upper_position = search_with_filter(file_data, data_file_key, coords[0], lower_range[0], lower_range[1], end_search_position, fltr)
 
     if retrieve_row_indices:
         return retrieve_matching_row_indices(file_data, data_file_key, coords[1], (lower_range[0], upper_position), num_parallel)
 
-    return (lower_range[0], upper_position)
+    return (lower_range[0], upper_position)
```

### Comparing `f4-0.9.0/src/f4/Utilities.py` & `f4-0.9.1/src/f4/Utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.0"
+    return "0.9.1"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
@@ -57,32 +57,36 @@
 
 def reverse_string(s):
     return s[::-1]
 
 def get_delimited_file_handle(file_path):
     if file_path.endswith(".gz"):
         return gzip.open(file_path)
+    elif file_path.endswith(".zstd"):
+        # FYI: This compression format is a hidden feature for input files.
+        # Skipping comments is not supported.
+        return open_temp_file_compressed(file_path)
     else:
         return open(file_path, "rb")
 
-def open_temp_file_to_compress(file_path):
-    fh = open(file_path, "wb")
-    return ZstdCompressor(level=1, write_content_size=True).stream_writer(fh)
-
 def write_temp_file_original_size(file_path, num_bytes):
     with open(get_temp_file_original_size_path(file_path), "wb") as size_file:
         size_file.write(str(num_bytes).encode())
 
 def get_temp_file_original_size(file_path):
     with open(get_temp_file_original_size_path(file_path), "rb") as size_file:
         return int(size_file.read().decode())
 
 def get_temp_file_original_size_path(file_path):
     return f"{file_path}__original_size"
 
+def open_temp_file_to_compress(file_path, mode="wb"):
+    fh = open(file_path, mode)
+    return ZstdCompressor(level=1, write_content_size=True).stream_writer(fh)
+
 def open_temp_file_compressed(file_path):
     fh = open(file_path, "rb")
     return ZstdDecompressor().stream_reader(fh)
 
 def read_compressed_file_line_by_line(compressed_file_path):
     with open(compressed_file_path, 'rb') as compressed_file:
         dctx = ZstdDecompressor()
@@ -164,14 +168,28 @@
 
 def deserialize(msg):
     return msgpack.decode(msg)
 
 def fix_dir_path_ending(dir_path):
     return dir_path if dir_path.endswith("/") else dir_path + "/"
 
+def prepare_tmp_dir(tmp_dir_path):
+    # Figure out where temp files will be stored and create directory, if needed.
+    if tmp_dir_path:
+        makedirs(tmp_dir_path, exist_ok=True)
+        tmp_dir_path = tmp_dir_path
+    else:
+        tmp_dir_path = mkdtemp()
+
+    unique_id = uuid4()
+    tmp_dir_path = fix_dir_path_ending(tmp_dir_path) + f"f4_{unique_id}/"
+    makedirs(tmp_dir_path, exist_ok=True)
+
+    return tmp_dir_path
+
 def remove_tmp_dir(tmp_dir_path, verbose):
     # Remove the temp directory if it was generated by the code (not the user).
     if tmp_dir_path:
         try:
             rmtree(tmp_dir_path)
             print_message(f"Removed {tmp_dir_path} directory", verbose)
         except:
@@ -182,29 +200,14 @@
     cursor = 0
     total_elements = len(my_list)
 
     while cursor < total_elements:
         yield my_list[cursor:(cursor + max_items_per_chunk)]
         cursor += max_items_per_chunk
 
-# def split_list_into_chunks(my_list, num_parallel):
-#     items_per_chunk = ceil(len(my_list) / num_parallel)
-#
-#     return_indices = list()
-#
-#     for an_int in my_list:
-#         return_indices.append(an_int)
-#
-#         if len(return_indices) == items_per_chunk:
-#             yield return_indices
-#             return_indices = list()
-#
-#     if len(return_indices) > 0:
-#         yield return_indices
-
 def iterate_single_value(value):
     yield value
 
 def generate_range_chunks(total_n, n_per_chunk):
     num_chunks = ceil(total_n / n_per_chunk)
     current_n = -n_per_chunk
 
@@ -261,8 +264,8 @@
 #         return ">="
 #     elif op == gt:
 #         return ">"
 #     elif op == le:
 #         return "<="
 #     elif op == lt:
 #         return "<"
-#     return "<>"
+#     return "<>"
```

### Comparing `f4-0.9.0/src/f4.egg-info/PKG-INFO` & `f4-0.9.1/src/f4.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.0/test/test.py` & `f4-0.9.1/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,33 +541,33 @@
 
     # Clean up data files
     for file_path in glob.glob(f"{f4_file_path}*"):
         os.unlink(file_path)
 
 def test_transpose(tsv_file_path, f4_file_path, out_file_path, num_parallel, compression_type):
     f4.convert_delimited_file(tsv_file_path, f4_file_path, num_parallel=num_parallel, compression_type=compression_type)
-    f4.transpose(f4_file_path, out_file_path, num_parallel=num_parallel)
+    f4.transpose(f4_file_path, out_file_path, src_column_for_names="ID", num_parallel=num_parallel)
 
-    check_result("Dimensions", "Number of rows", f4.get_num_rows(out_file_path), 8)
-    check_result("Dimensions", "Number of columns", f4.get_num_cols(out_file_path), 6)
+    check_result("Transpose - Dimensions", "Number of rows", f4.get_num_rows(out_file_path), 8)
+    check_result("Transpose - Dimensions", "Number of columns", f4.get_num_cols(out_file_path), 6)
 
-    check_result("Column types", "ID column", f4.get_column_type_from_name(out_file_path, "ID"), "s")
-    check_result("Column types", "E column", f4.get_column_type_from_name(out_file_path, "E"), "s")
-    check_result("Column types", "A column", f4.get_column_type_from_name(out_file_path, "A"), "s")
-    check_result("Column types", "B column", f4.get_column_type_from_name(out_file_path, "B"), "s")
-    check_result("Column types", "C column", f4.get_column_type_from_name(out_file_path, "C"), "s")
-    check_result("Column types", "D column", f4.get_column_type_from_name(out_file_path, "D"), "s")
+    check_result("Transpose - Column types", "ID column", f4.get_column_type_from_name(out_file_path, "ID"), "s")
+    check_result("Transpose - Column types", "E column", f4.get_column_type_from_name(out_file_path, "E"), "s")
+    check_result("Transpose - Column types", "A column", f4.get_column_type_from_name(out_file_path, "A"), "s")
+    check_result("Transpose - Column types", "B column", f4.get_column_type_from_name(out_file_path, "B"), "s")
+    check_result("Transpose - Column types", "C column", f4.get_column_type_from_name(out_file_path, "C"), "s")
+    check_result("Transpose - Column types", "D column", f4.get_column_type_from_name(out_file_path, "D"), "s")
 
     out_file_path_2 = out_file_path + "2"
     f4.query(out_file_path, f4.StringFilter("ID", operator.eq, "OrdinalA"), ["A"], out_file_path_2, num_parallel=num_parallel)
-    check_results("Filter by ID", read_file_into_lists(out_file_path_2), [[b"A"], [b"Low"]])
+    check_results("Transpose - Filter by ID", read_file_into_lists(out_file_path_2), [[b"A"], [b"Low"]])
     os.unlink(out_file_path_2)
 
     f4.query(out_file_path, f4.StringFilter("B", operator.eq, "High"), ["D"], out_file_path_2, num_parallel=num_parallel)
-    check_results("Filter by B", read_file_into_lists(out_file_path_2), [[b"D"], [b"Med"]])
+    check_results("Transpose - Filter by B", read_file_into_lists(out_file_path_2), [[b"D"], [b"Med"]])
     os.unlink(out_file_path_2)
 
 def test_inner_join(num_parallel, compression_type):
     data1 = read_file_into_lists("data/small.tsv")
     data2 = read_file_into_lists("data/small.tsv")
 
     # Manage header rows.
@@ -783,29 +783,23 @@
     run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = "zstd")
     run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = "zstd")
 
     # Small tests with z-standard compression (and indexing)
     run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = "zstd", index_columns = index_columns)
     run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = "zstd", index_columns = index_columns)
 
-    ## Small tests with dictionary-based compression
-    ##run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = "dictionary")
-    ##run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = "dictionary")
-
-    ## Small tests with dictionary-based compression (and indexing)
-    ##run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = "dictionary", index_columns = index_columns)
-    ##run_small_tests("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = "dictionary", index_columns = index_columns)
-
     # Transpose without compression
-    #test_transpose("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = None)
-    #test_transpose("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = None)
+    f4_transposed_file_path = "/tmp/small_transposed.f4"
+    test_transpose("data/small.tsv", f4_file_path, f4_transposed_file_path, num_parallel = 1, compression_type = None)
+    test_transpose("data/small.tsv", f4_file_path, f4_transposed_file_path, num_parallel = 2, compression_type = None)
 
     # Transpose with zstd compression
-    #test_transpose("data/small.tsv", f4_file_path, out_file_path, num_parallel = 1, compression_type = "zstd")
-    #test_transpose("data/small.tsv", f4_file_path, out_file_path, num_parallel = 2, compression_type = "zstd")
+    f4_transposed_file_path = "/tmp/small_transposed_zstd.f4"
+    test_transpose("data/small.tsv", f4_file_path, f4_transposed_file_path, num_parallel = 1, compression_type = "zstd")
+    test_transpose("data/small.tsv", f4_file_path, f4_transposed_file_path, num_parallel = 2, compression_type = "zstd")
 
     # Inner join without compression
     #test_inner_join(num_parallel = 1, compression_type = None)
 
     # Inner join with compression
     #test_inner_join(num_parallel = 1, compression_type = "zstd")
 
@@ -865,36 +859,36 @@
     num_lines = 0
     with open(out_file_path, "r", newline="\n") as out_file:
         for line in out_file:
             num_lines += 1
 
     print(f"  {elapsed_time:.2f} seconds, {num_lines} lines in output file")
 
-run_all_small_tests()
-sys.exit()
+#run_all_small_tests()
+#sys.exit()
 
 #for compression_type in [None]:
-#for compression_type in ["zstd"]:
-for compression_type in [None, "zstd"]:
+for compression_type in ["zstd"]:
+#for compression_type in [None, "zstd"]:
     # Medium tests
-    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
-    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
+#    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
+#    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 
     # Large tests
 #    num_parallel = 1
 #    num_parallel = 4
     num_parallel = 16
     build_outputs = True
     #build_outputs = False
     verbose = True
     #verbose = False
     check_outputs = True
     #check_outputs = False
 
-#    run_larger_tests(num_parallel=num_parallel, size="large_tall", extension="", discrete1_index=251, numeric1_index=501, build_outputs=build_outputs, compression_type=compression_type, verbose=verbose, check_outputs=check_outputs, tmp_dir_path="/tmp/large_tall")
+    run_larger_tests(num_parallel=num_parallel, size="large_tall", extension="", discrete1_index=251, numeric1_index=501, build_outputs=build_outputs, compression_type=compression_type, verbose=verbose, check_outputs=check_outputs, tmp_dir_path="/tmp/large_tall")
 #    run_larger_tests(num_parallel=num_parallel, size="large_wide", extension="", discrete1_index=250001, numeric1_index=500001, build_outputs=build_outputs, compression_type=compression_type, verbose=verbose, check_outputs=check_outputs, tmp_dir_path="/tmp/large_wide")
 #
 #    run_larger_tests(num_parallel=num_parallel, size="large_tall", extension=".gz", discrete1_index=251, numeric1_index=501, build_outputs=build_outputs, compression_type=compression_type, verbose=verbose, check_outputs=check_outputs, tmp_dir_path="/tmp/large_tall_gz")
 #    run_larger_tests(num_parallel=num_parallel, size="large_wide", extension=".gz", discrete1_index=250001, numeric1_index=500001, build_outputs=build_outputs, compression_type=compression_type, verbose=verbose, check_outputs=check_outputs, tmp_dir_path="/tmp/large_wide_gz")
 #
 #    run_super_tests(num_parallel=num_parallel, size="test_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/test_tall")
 #    run_super_tests(num_parallel=num_parallel, size="test_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/test_wide")
@@ -905,14 +899,14 @@
 #    run_super_tests(num_parallel=num_parallel, size="super_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_tall")
 #    run_super_tests(num_parallel=num_parallel, size="super_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_wide")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_tall")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_wide")
 
     #Attempt this? https://community.hpe.com/t5/servers-systems-the-right/cray-graph-engine-takes-on-a-trillion-triples/ba-p/7096770
 
-    ##f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", num_parallel=num_parallel, verbose=verbose)
-    ##f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", num_parallel=num_parallel, verbose=verbose)
+#    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
+    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 
     ##f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose)
     ##f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose)
 
 print("All tests passed!!")
```

