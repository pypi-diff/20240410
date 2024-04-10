# Comparing `tmp/fmake-0.1.4.tar.gz` & `tmp/fmake-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmake-0.1.4.tar", last modified: Thu Feb 22 10:14:17 2024, max compression
+gzip compressed data, was "fmake-0.1.5.tar", last modified: Fri Feb 23 03:56:03 2024, max compression
```

## Comparing `fmake-0.1.4.tar` & `fmake-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 10:14:17.211941 fmake-0.1.4/
--rw-rw-rw-   0        0        0      545 2024-02-22 10:14:17.209942 fmake-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-11-30 21:12:37.000000 fmake-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 10:14:17.126520 fmake-0.1.4/fmake/
--rw-rw-rw-   0        0        0     1886 2024-02-22 05:27:07.000000 fmake-0.1.4/fmake/Convert2CSV.py
--rw-rw-rw-   0        0        0      377 2024-02-22 02:06:00.000000 fmake-0.1.4/fmake/__init__.py
--rw-rw-rw-   0        0        0     8603 2023-03-12 23:40:03.000000 fmake-0.1.4/fmake/entity_to_data_frame.py
--rw-rw-rw-   0        0        0     1766 2024-02-22 05:27:48.000000 fmake-0.1.4/fmake/extract_files.py
--rw-rw-rw-   0        0        0     6350 2024-02-22 05:41:38.000000 fmake-0.1.4/fmake/generic_helper.py
--rw-rw-rw-   0        0        0      529 2023-03-12 23:40:03.000000 fmake-0.1.4/fmake/main_vhdl_make.py
--rw-rw-rw-   0        0        0     1182 2024-02-22 10:12:30.000000 fmake-0.1.4/fmake/make_build_system.py
--rw-rw-rw-   0        0        0     3873 2024-02-22 05:28:29.000000 fmake-0.1.4/fmake/make_test_bench_stimulus.py
-drwxrwxrwx   0        0        0        0 2024-02-22 10:14:17.171465 fmake-0.1.4/fmake/makeise/
--rw-rw-rw-   0        0        0        0 2023-03-27 03:53:04.000000 fmake-0.1.4/fmake/makeise/__init__.py
--rw-rw-rw-   0        0        0     4482 2022-03-23 02:23:21.000000 fmake-0.1.4/fmake/makeise/makePrj.py
--rw-rw-rw-   0        0        0    11352 2023-03-27 03:53:35.000000 fmake-0.1.4/fmake/makeise/makeise.py
--rw-rw-rw-   0        0        0     3817 2023-08-20 09:44:34.000000 fmake-0.1.4/fmake/run_ise.py
--rw-rw-rw-   0        0        0     4788 2023-03-27 02:30:03.000000 fmake-0.1.4/fmake/send_axi_stream_udp.py
--rw-rw-rw-   0        0        0     3309 2024-02-22 06:51:43.000000 fmake-0.1.4/fmake/text_io_query.py
-drwxrwxrwx   0        0        0        0 2024-02-22 10:14:17.205785 fmake-0.1.4/fmake/vhdl_csv_io/
--rw-rw-rw-   0        0        0     4814 2023-08-04 05:58:32.000000 fmake-0.1.4/fmake/vhdl_csv_io/CSV_UtilityPkg.py
--rw-rw-rw-   0        0        0      447 2023-08-04 05:57:35.000000 fmake-0.1.4/fmake/vhdl_csv_io/ClockGenerator.py
--rw-rw-rw-   0        0        0      392 2023-08-04 06:01:02.000000 fmake-0.1.4/fmake/vhdl_csv_io/__init__.py
--rw-rw-rw-   0        0        0     5188 2023-08-04 05:58:13.000000 fmake-0.1.4/fmake/vhdl_csv_io/csv_text_io_poll.py
--rw-rw-rw-   0        0        0     2031 2023-08-20 08:05:54.000000 fmake-0.1.4/fmake/vhdl_csv_io/e_csv_read_file.py
--rw-rw-rw-   0        0        0     2988 2023-08-20 08:05:33.000000 fmake-0.1.4/fmake/vhdl_csv_io/e_csv_write_file.py
--rw-rw-rw-   0        0        0     6973 2023-08-04 05:59:52.000000 fmake-0.1.4/fmake/vhdl_csv_io/type_conversions_helper.py
--rw-rw-rw-   0        0        0     5381 2024-02-22 05:29:30.000000 fmake-0.1.4/fmake/vhdl_dependency_db.py
--rw-rw-rw-   0        0        0     6310 2024-02-22 05:29:46.000000 fmake-0.1.4/fmake/vhdl_entity_class.py
--rw-rw-rw-   0        0        0     3203 2022-11-16 15:43:22.000000 fmake-0.1.4/fmake/vhdl_get_entity_def.py
--rw-rw-rw-   0        0        0     1221 2024-02-22 06:41:27.000000 fmake-0.1.4/fmake/vhdl_get_list_of_files.py
--rw-rw-rw-   0        0        0     3258 2024-02-22 05:30:19.000000 fmake-0.1.4/fmake/vhdl_get_type_def.py
--rw-rw-rw-   0        0        0      799 2022-11-16 15:43:22.000000 fmake-0.1.4/fmake/vhdl_load_file_without_comments.py
--rw-rw-rw-   0        0        0     6255 2024-02-22 05:31:04.000000 fmake-0.1.4/fmake/vhdl_make_implementation.py
--rw-rw-rw-   0        0        0     2240 2024-02-22 07:01:00.000000 fmake-0.1.4/fmake/vhdl_make_simulation.py
--rw-rw-rw-   0        0        0    14790 2024-02-22 05:31:58.000000 fmake-0.1.4/fmake/vhdl_make_test_bench.py
--rw-rw-rw-   0        0        0     1113 2022-11-16 15:43:22.000000 fmake-0.1.4/fmake/vhdl_make_test_bench_names.py
--rw-rw-rw-   0        0        0     3187 2023-03-12 23:40:03.000000 fmake-0.1.4/fmake/vhdl_merge_split_test_cases.py
--rw-rw-rw-   0        0        0     8036 2024-02-22 05:34:37.000000 fmake-0.1.4/fmake/vhdl_parser.py
--rw-rw-rw-   0        0        0      451 2022-12-07 23:12:58.000000 fmake-0.1.4/fmake/vhdl_programm_list.py
--rw-rw-rw-   0        0        0     2819 2024-02-22 10:11:21.000000 fmake-0.1.4/fmake/vhdl_run_vivado.py
-drwxrwxrwx   0        0        0        0 2024-02-22 10:14:17.207915 fmake-0.1.4/fmake.egg-info/
--rw-rw-rw-   0        0        0      545 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-22 10:14:16.000000 fmake-0.1.4/fmake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 10:14:17.211941 fmake-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-02-22 10:13:35.000000 fmake-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-23 03:56:03.466746 fmake-0.1.5/
+-rw-rw-rw-   0        0        0      545 2024-02-23 03:56:03.466746 fmake-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-11-30 21:12:37.000000 fmake-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-02-23 03:56:03.421967 fmake-0.1.5/fmake/
+-rw-rw-rw-   0        0        0     1886 2024-02-22 05:27:07.000000 fmake-0.1.5/fmake/Convert2CSV.py
+-rw-rw-rw-   0        0        0      377 2024-02-22 02:06:00.000000 fmake-0.1.5/fmake/__init__.py
+-rw-rw-rw-   0        0        0     8603 2023-03-12 23:40:03.000000 fmake-0.1.5/fmake/entity_to_data_frame.py
+-rw-rw-rw-   0        0        0     1766 2024-02-22 05:27:48.000000 fmake-0.1.5/fmake/extract_files.py
+-rw-rw-rw-   0        0        0     6350 2024-02-22 05:41:38.000000 fmake-0.1.5/fmake/generic_helper.py
+-rw-rw-rw-   0        0        0      529 2023-03-12 23:40:03.000000 fmake-0.1.5/fmake/main_vhdl_make.py
+-rw-rw-rw-   0        0        0     1182 2024-02-22 10:12:30.000000 fmake-0.1.5/fmake/make_build_system.py
+-rw-rw-rw-   0        0        0     3873 2024-02-22 05:28:29.000000 fmake-0.1.5/fmake/make_test_bench_stimulus.py
+drwxrwxrwx   0        0        0        0 2024-02-23 03:56:03.453510 fmake-0.1.5/fmake/makeise/
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:53:04.000000 fmake-0.1.5/fmake/makeise/__init__.py
+-rw-rw-rw-   0        0        0     4482 2022-03-23 02:23:21.000000 fmake-0.1.5/fmake/makeise/makePrj.py
+-rw-rw-rw-   0        0        0    11352 2023-03-27 03:53:35.000000 fmake-0.1.5/fmake/makeise/makeise.py
+-rw-rw-rw-   0        0        0     3817 2023-08-20 09:44:34.000000 fmake-0.1.5/fmake/run_ise.py
+-rw-rw-rw-   0        0        0     4788 2023-03-27 02:30:03.000000 fmake-0.1.5/fmake/send_axi_stream_udp.py
+-rw-rw-rw-   0        0        0     3309 2024-02-22 06:51:43.000000 fmake-0.1.5/fmake/text_io_query.py
+drwxrwxrwx   0        0        0        0 2024-02-23 03:56:03.466746 fmake-0.1.5/fmake/vhdl_csv_io/
+-rw-rw-rw-   0        0        0     4814 2023-08-04 05:58:32.000000 fmake-0.1.5/fmake/vhdl_csv_io/CSV_UtilityPkg.py
+-rw-rw-rw-   0        0        0      447 2023-08-04 05:57:35.000000 fmake-0.1.5/fmake/vhdl_csv_io/ClockGenerator.py
+-rw-rw-rw-   0        0        0      392 2023-08-04 06:01:02.000000 fmake-0.1.5/fmake/vhdl_csv_io/__init__.py
+-rw-rw-rw-   0        0        0     5188 2023-08-04 05:58:13.000000 fmake-0.1.5/fmake/vhdl_csv_io/csv_text_io_poll.py
+-rw-rw-rw-   0        0        0     2031 2023-08-20 08:05:54.000000 fmake-0.1.5/fmake/vhdl_csv_io/e_csv_read_file.py
+-rw-rw-rw-   0        0        0     2988 2023-08-20 08:05:33.000000 fmake-0.1.5/fmake/vhdl_csv_io/e_csv_write_file.py
+-rw-rw-rw-   0        0        0     6973 2023-08-04 05:59:52.000000 fmake-0.1.5/fmake/vhdl_csv_io/type_conversions_helper.py
+-rw-rw-rw-   0        0        0     5523 2024-02-23 03:55:02.000000 fmake-0.1.5/fmake/vhdl_dependency_db.py
+-rw-rw-rw-   0        0        0     6310 2024-02-22 05:29:46.000000 fmake-0.1.5/fmake/vhdl_entity_class.py
+-rw-rw-rw-   0        0        0     3203 2022-11-16 15:43:22.000000 fmake-0.1.5/fmake/vhdl_get_entity_def.py
+-rw-rw-rw-   0        0        0     1221 2024-02-22 06:41:27.000000 fmake-0.1.5/fmake/vhdl_get_list_of_files.py
+-rw-rw-rw-   0        0        0     3258 2024-02-22 05:30:19.000000 fmake-0.1.5/fmake/vhdl_get_type_def.py
+-rw-rw-rw-   0        0        0      799 2022-11-16 15:43:22.000000 fmake-0.1.5/fmake/vhdl_load_file_without_comments.py
+-rw-rw-rw-   0        0        0     6255 2024-02-22 05:31:04.000000 fmake-0.1.5/fmake/vhdl_make_implementation.py
+-rw-rw-rw-   0        0        0     2261 2024-02-23 03:55:15.000000 fmake-0.1.5/fmake/vhdl_make_simulation.py
+-rw-rw-rw-   0        0        0    14790 2024-02-22 05:31:58.000000 fmake-0.1.5/fmake/vhdl_make_test_bench.py
+-rw-rw-rw-   0        0        0     1113 2022-11-16 15:43:22.000000 fmake-0.1.5/fmake/vhdl_make_test_bench_names.py
+-rw-rw-rw-   0        0        0     3187 2023-03-12 23:40:03.000000 fmake-0.1.5/fmake/vhdl_merge_split_test_cases.py
+-rw-rw-rw-   0        0        0     8036 2024-02-22 05:34:37.000000 fmake-0.1.5/fmake/vhdl_parser.py
+-rw-rw-rw-   0        0        0      451 2022-12-07 23:12:58.000000 fmake-0.1.5/fmake/vhdl_programm_list.py
+-rw-rw-rw-   0        0        0     2819 2024-02-22 10:11:21.000000 fmake-0.1.5/fmake/vhdl_run_vivado.py
+drwxrwxrwx   0        0        0        0 2024-02-23 03:56:03.466746 fmake-0.1.5/fmake.egg-info/
+-rw-rw-rw-   0        0        0      545 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-23 03:56:03.000000 fmake-0.1.5/fmake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-23 03:56:03.466746 fmake-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-02-23 03:55:29.000000 fmake-0.1.5/setup.py
```

### Comparing `fmake-0.1.4/PKG-INFO` & `fmake-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmake
-Version: 0.1.4
+Version: 0.1.5
 Summary: build scripts for firmware projects
 Home-page: 
 Author: Richard Peschke
 Author-email: peschke@hawaii.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmake-0.1.4/fmake/Convert2CSV.py` & `fmake-0.1.5/fmake/Convert2CSV.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/entity_to_data_frame.py` & `fmake-0.1.5/fmake/entity_to_data_frame.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/extract_files.py` & `fmake-0.1.5/fmake/extract_files.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/generic_helper.py` & `fmake-0.1.5/fmake/generic_helper.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/main_vhdl_make.py` & `fmake-0.1.5/fmake/main_vhdl_make.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/make_build_system.py` & `fmake-0.1.5/fmake/make_build_system.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/make_test_bench_stimulus.py` & `fmake-0.1.5/fmake/make_test_bench_stimulus.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/makeise/makePrj.py` & `fmake-0.1.5/fmake/makeise/makePrj.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/makeise/makeise.py` & `fmake-0.1.5/fmake/makeise/makeise.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/run_ise.py` & `fmake-0.1.5/fmake/run_ise.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/send_axi_stream_udp.py` & `fmake-0.1.5/fmake/send_axi_stream_udp.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/text_io_query.py` & `fmake-0.1.5/fmake/text_io_query.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_csv_io/CSV_UtilityPkg.py` & `fmake-0.1.5/fmake/vhdl_csv_io/CSV_UtilityPkg.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_csv_io/csv_text_io_poll.py` & `fmake-0.1.5/fmake/vhdl_csv_io/csv_text_io_poll.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_csv_io/e_csv_read_file.py` & `fmake-0.1.5/fmake/vhdl_csv_io/e_csv_read_file.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_csv_io/e_csv_write_file.py` & `fmake-0.1.5/fmake/vhdl_csv_io/e_csv_write_file.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_csv_io/type_conversions_helper.py` & `fmake-0.1.5/fmake/vhdl_csv_io/type_conversions_helper.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_dependency_db.py` & `fmake-0.1.5/fmake/vhdl_dependency_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,27 +97,32 @@
         df_find_entity = get_dependencies_recursive_full(df_component_USED,   df_entity_def, df_find_entity)
         df_find_entity = get_dependencies_recursive_full(df_packageUSE,       df_packageDef, df_find_entity)
         
         self.filelist = df_find_entity["filename"].tolist()   
         return self.filelist
 
             
-    def get_dependencies_and_make_project_file(self,Entity):
+    def get_dependencies_and_make_project_file(self,Entity, IsSimulation = False):
         if not  self.IsInitilized:
             raise Exception("dependency_db_cl not initilized")
         fileList = self.get_dependencies(Entity)
         
         OutputFile =  "build/" +Entity+"/"+Entity+".prj"
         outPath = "build/" +Entity
         
         try_make_dir(outPath)
          
         lines = ""
         for k in fileList:
             lines += 'vhdl work "../../' + k + '"\n'
+        
+        
+        if IsSimulation:
+            lines = lines.replace("env_impl.vhd","env_sim.vhd")
+            
         save_file(OutputFile, lines)
         self.filelist  = fileList
         return fileList
```

### Comparing `fmake-0.1.4/fmake/vhdl_entity_class.py` & `fmake-0.1.5/fmake/vhdl_entity_class.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_get_entity_def.py` & `fmake-0.1.5/fmake/vhdl_get_entity_def.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_get_list_of_files.py` & `fmake-0.1.5/fmake/vhdl_get_list_of_files.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_get_type_def.py` & `fmake-0.1.5/fmake/vhdl_get_type_def.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_load_file_without_comments.py` & `fmake-0.1.5/fmake/vhdl_load_file_without_comments.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_make_implementation.py` & `fmake-0.1.5/fmake/vhdl_make_implementation.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_make_simulation.py` & `fmake-0.1.5/fmake/vhdl_make_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     save_file(BuildFolder+Entity+ "/"+ Entity +"_header.txt", Content)
     vprint(1)("=======Done Extracting Header From File====")
 
 
 def vhdl_make_simulation(Entity,BuildFolder = "build/"):
 
 
-    fileList = get_dependency_db().get_dependencies_and_make_project_file(Entity)
+    fileList = get_dependency_db().get_dependencies_and_make_project_file(Entity, IsSimulation = True)
     if len(fileList)==0:
         vprint(1)("unable to find entity: ", Entity)
         return 
     
     extract_header_from_top_file(Entity, fileList[0],BuildFolder)
```

### Comparing `fmake-0.1.4/fmake/vhdl_make_test_bench.py` & `fmake-0.1.5/fmake/vhdl_make_test_bench.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_make_test_bench_names.py` & `fmake-0.1.5/fmake/vhdl_make_test_bench_names.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_merge_split_test_cases.py` & `fmake-0.1.5/fmake/vhdl_merge_split_test_cases.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_parser.py` & `fmake-0.1.5/fmake/vhdl_parser.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake/vhdl_run_vivado.py` & `fmake-0.1.5/fmake/vhdl_run_vivado.py`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/fmake.egg-info/PKG-INFO` & `fmake-0.1.5/fmake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmake
-Version: 0.1.4
+Version: 0.1.5
 Summary: build scripts for firmware projects
 Home-page: 
 Author: Richard Peschke
 Author-email: peschke@hawaii.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmake-0.1.4/fmake.egg-info/SOURCES.txt` & `fmake-0.1.5/fmake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmake-0.1.4/setup.py` & `fmake-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fmake", 
-    version="0.1.4",
+    version="0.1.5",
     author="Richard Peschke",
     author_email="peschke@hawaii.edu",
     description="build scripts for firmware projects",
     long_description="long_description",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

