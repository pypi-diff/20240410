# Comparing `tmp/dbstream-0.1.8.tar.gz` & `tmp/dbstream-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbstream-0.1.8.tar", last modified: Wed Oct 20 13:49:46 2021, max compression
+gzip compressed data, was "dist/dbstream-0.1.9.tar", last modified: Tue Oct 26 13:01:17 2021, max compression
```

## Comparing `dbstream-0.1.8.tar` & `dbstream-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:49:46.892335 dbstream-0.1.8/
--rw-r--r--   0 geoffrey   (501) staff       (20)      518 2021-10-20 13:49:46.892069 dbstream-0.1.8/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)       29 2021-10-20 13:46:01.000000 dbstream-0.1.8/README.md
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:49:46.887867 dbstream-0.1.8/dbstream/
--rw-r--r--   0 geoffrey   (501) staff       (20)     8709 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/DBStream.py
--rw-r--r--   0 geoffrey   (501) staff       (20)       39 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/__init__.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:49:46.891718 dbstream-0.1.8/dbstream/tools/
--rw-r--r--   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tools/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      369 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tools/dck_infos.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2991 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tools/parse_data.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      198 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tools/print_colors.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      572 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tools/regex.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1460 2021-10-20 13:46:01.000000 dbstream-0.1.8/dbstream/tunnel.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:49:46.890054 dbstream-0.1.8/dbstream.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)      518 2021-10-20 13:49:46.000000 dbstream-0.1.8/dbstream.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)      377 2021-10-20 13:49:46.000000 dbstream-0.1.8/dbstream.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2021-10-20 13:49:46.000000 dbstream-0.1.8/dbstream.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       50 2021-10-20 13:49:46.000000 dbstream-0.1.8/dbstream.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        9 2021-10-20 13:49:46.000000 dbstream-0.1.8/dbstream.egg-info/top_level.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2021-10-20 13:49:46.892422 dbstream-0.1.8/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)      767 2021-10-20 13:46:01.000000 dbstream-0.1.8/setup.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-26 13:01:17.561812 dbstream-0.1.9/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1063 2021-10-20 13:46:01.000000 dbstream-0.1.9/LICENSE
+-rw-r--r--   0 geoffrey   (501) staff       (20)      505 2021-10-26 13:01:17.560140 dbstream-0.1.9/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)       29 2021-10-20 13:46:01.000000 dbstream-0.1.9/README.md
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-26 13:01:17.542460 dbstream-0.1.9/dbstream/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     8982 2021-10-26 12:50:42.000000 dbstream-0.1.9/dbstream/DBStream.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)       39 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/__init__.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-26 13:01:17.554821 dbstream-0.1.9/dbstream/tools/
+-rw-r--r--   0 geoffrey   (501) staff       (20)        0 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tools/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      369 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tools/dck_infos.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2991 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tools/parse_data.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      198 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tools/print_colors.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      572 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tools/regex.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1460 2021-10-20 13:46:01.000000 dbstream-0.1.9/dbstream/tunnel.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2021-10-26 13:01:17.549115 dbstream-0.1.9/dbstream.egg-info/
+-rw-r--r--   0 geoffrey   (501) staff       (20)      505 2021-10-26 13:01:17.000000 dbstream-0.1.9/dbstream.egg-info/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)      385 2021-10-26 13:01:17.000000 dbstream-0.1.9/dbstream.egg-info/SOURCES.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)        1 2021-10-26 13:01:17.000000 dbstream-0.1.9/dbstream.egg-info/dependency_links.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       73 2021-10-26 13:01:17.000000 dbstream-0.1.9/dbstream.egg-info/requires.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)        9 2021-10-26 13:01:17.000000 dbstream-0.1.9/dbstream.egg-info/top_level.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       38 2021-10-26 13:01:17.562134 dbstream-0.1.9/setup.cfg
+-rw-r--r--   0 geoffrey   (501) staff       (20)      801 2021-10-26 12:50:42.000000 dbstream-0.1.9/setup.py
```

### Comparing `dbstream-0.1.8/dbstream/DBStream.py` & `dbstream-0.1.9/dbstream/DBStream.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import requests
 
 from dbstream.tools.parse_data import treat_json_data
 from dbstream.tools.regex import replace_query_details
 from dbstream.tunnel import create_ssh_tunnel
 
+from google.api_core.exceptions import Forbidden
 
 class DBStream:
 
     def __init__(self, instance_name, client_id, special_env=None):
         self.instance_name = instance_name
         self.instance_type_prefix = ""
         self.ssh_init_port = ""
@@ -136,15 +137,15 @@
                     "ssh_tunnel": True if self.ssh_tunnel else False,
                     "local_absolute_path": os.getcwd(),
                     "replace": replace
                 }
                 r = requests.post(url=url, data=json.dumps(body))
                 print(r.status_code)
 
-    def send(self, data, replace=False, apply_special_env=True, **kwargs):
+    def send(self, data, replace=False, apply_special_env=True, delay=5, **kwargs):
         # data['data'] = generate_dck_info(data['data'])
         list_of_tables_to_send, list_of_pop_fields = treat_json_data(data)
         for d in list_of_tables_to_send:
             # if d.get('table_name') == 'test.test_orders_fulfillments_line_items':
             #     print(d.get('data'))
             # else:
             #     print('OK')
@@ -157,15 +158,19 @@
                         column_names.append(k)
             data_to_send = {
                 "columns_name": column_names,
                 "rows": [[r.get(c) for c in column_names] for r in d['data']],
                 "table_name": d.get('table_name')
             }
             if len(data_to_send['columns_name']) > 0:
-                self.send_data(data=data_to_send, replace=replace, apply_special_env=apply_special_env, **kwargs)
+                try:
+                    self.send_data(data=data_to_send, replace=replace, apply_special_env=apply_special_env, **kwargs)
+                except Forbidden:
+                    time.sleep(delay)
+                    self.send_data(data=data_to_send, replace=replace, apply_special_env=apply_special_env, **kwargs)
 
     def send_temp_data(self, data, schema_prefix, table, column_names, apply_special_env=True):
         data_to_send = {
             "columns_name": column_names,
             "rows": [[r.get(c) for c in column_names] for r in data],
             "table_name": schema_prefix + '.' + table + '_temp'}
         self.send_data(
```

### Comparing `dbstream-0.1.8/dbstream/tools/parse_data.py` & `dbstream-0.1.9/dbstream/tools/parse_data.py`

 * *Files identical despite different names*

### Comparing `dbstream-0.1.8/dbstream/tools/regex.py` & `dbstream-0.1.9/dbstream/tools/regex.py`

 * *Files identical despite different names*

### Comparing `dbstream-0.1.8/dbstream/tunnel.py` & `dbstream-0.1.9/dbstream/tunnel.py`

 * *Files identical despite different names*

### Comparing `dbstream-0.1.8/setup.py` & `dbstream-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dbstream",
-    version="0.1.8",
+    version="0.1.9",
     author="Dacker",
     author_email="hello@dacker.co",
     description="A meta package to be connected to several databases",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dacker-team/dbstream",
     packages=setuptools.find_packages(),
@@ -18,10 +18,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
     install_requires=[
         "sshtunnel==0.1.5",
         "dacktool>=0.0.7",
-        "requests>=2.22.0"
+        "requests>=2.22.0",
+        "google-api-core==2.1.1"
     ],
 )
```

