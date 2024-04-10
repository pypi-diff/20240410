# Comparing `tmp/sodata-0.0.3.tar.gz` & `tmp/sodata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sodata-0.0.3.tar", last modified: Wed Apr 10 06:38:07 2024, max compression
+gzip compressed data, was "sodata-0.0.4.tar", last modified: Wed Apr 10 06:53:42 2024, max compression
```

## Comparing `sodata-0.0.3.tar` & `sodata-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:38:07.780614 sodata-0.0.3/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.3/README.md
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-10 06:38:07.780614 sodata-0.0.3/setup.cfg
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      343 2024-04-10 06:38:05.000000 sodata-0.0.3/setup.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/sodata/
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.3/sodata/__init__.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.3/sodata/chunk_split.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1959 2024-04-10 05:11:02.000000 sodata-0.0.3/sodata/file_process.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      141 2024-04-09 12:56:22.000000 sodata-0.0.3/sodata/text_clean.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/sodata.egg-info/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/SOURCES.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/dependency_links.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       19 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/requires.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/top_level.txt
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:53:42.609323 sodata-0.0.4/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:53:42.609323 sodata-0.0.4/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.4/README.md
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-10 06:53:42.609323 sodata-0.0.4/setup.cfg
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      343 2024-04-10 06:53:41.000000 sodata-0.0.4/setup.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:53:42.609323 sodata-0.0.4/sodata/
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.4/sodata/__init__.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.4/sodata/chunk_split.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1822 2024-04-10 06:52:10.000000 sodata-0.0.4/sodata/file_process.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      141 2024-04-09 12:56:22.000000 sodata-0.0.4/sodata/text_clean.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:53:42.609323 sodata-0.0.4/sodata.egg-info/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:53:42.000000 sodata-0.0.4/sodata.egg-info/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-10 06:53:42.000000 sodata-0.0.4/sodata.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-10 06:53:42.000000 sodata-0.0.4/sodata.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       19 2024-04-10 06:53:42.000000 sodata-0.0.4/sodata.egg-info/requires.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-10 06:53:42.000000 sodata-0.0.4/sodata.egg-info/top_level.txt
```

### Comparing `sodata-0.0.3/sodata/file_process.py` & `sodata-0.0.4/sodata/file_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,10 +39,9 @@
                     text_data = process_txt_file(filepath)
                     with open(output_file, 'a', encoding='utf-8') as fp:
                         fp.write(json.dumps({"text": text_data}, ensure_ascii=False) + '\n')
                     print(f"Processed and saved {file} successfully.")
                 except UnicodeDecodeError as e:
                     print(e)
 
-process_folder_and_save_to_jsonl('/home/zhanghong/sodata/data/BL',  '/home/zhanghong/sodata/data/json_data/BL.jsonl')
-print("finished!")
+
```

