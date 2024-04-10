# Comparing `tmp/cmind-2.0.3.tar.gz` & `tmp/cmind-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.0.3.tar", last modified: Wed Mar 20 12:54:39 2024, max compression
+gzip compressed data, was "cmind-2.0.4.tar", last modified: Wed Apr 10 13:41:29 2024, max compression
```

## Comparing `cmind-2.0.3.tar` & `cmind-2.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.979287 cmind-2.0.3/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-03-10 19:31:48.000000 cmind-2.0.3/LICENSE.CK.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-03-10 19:31:48.000000 cmind-2.0.3/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10312 2024-03-20 12:54:39.969287 cmind-2.0.3/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9877 2024-03-10 19:31:48.000000 cmind-2.0.3/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-03-20 12:54:30.000000 cmind-2.0.3/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47667 2024-03-20 11:42:12.000000 cmind-2.0.3/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28064 2024-03-20 12:38:58.000000 cmind-2.0.3/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-03-20 12:38:58.000000 cmind-2.0.3/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    37831 2024-03-20 12:51:28.000000 cmind-2.0.3/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-03-20 11:59:46.000000 cmind-2.0.3/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    23188 2024-03-20 12:50:23.000000 cmind-2.0.3/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    42388 2024-03-10 19:31:48.000000 cmind-2.0.3/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-03-20 12:54:39.969287 cmind-2.0.3/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10312 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1290 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-03-10 19:31:59.000000 cmind-2.0.3/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-03-20 12:54:39.000000 cmind-2.0.3/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-03-20 12:54:39.979287 cmind-2.0.3/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2898 2024-03-10 19:31:48.000000 cmind-2.0.3/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.702234 cmind-2.0.4/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-10 13:40:53.000000 cmind-2.0.4/LICENSE.CK.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-10 13:40:53.000000 cmind-2.0.4/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10383 2024-04-10 13:41:29.702234 cmind-2.0.4/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9948 2024-04-10 13:40:53.000000 cmind-2.0.4/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.702234 cmind-2.0.4/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    37831 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    22835 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10383 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1290 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-10 13:41:29.702234 cmind-2.0.4/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2898 2024-04-10 13:40:53.000000 cmind-2.0.4/setup.py
```

### Comparing `cmind-2.0.3/LICENSE.CK.md` & `cmind-2.0.4/LICENSE.CK.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/LICENSE.md` & `cmind-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/PKG-INFO` & `cmind-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.0.3
+Version: 2.0.4
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
@@ -62,14 +62,17 @@
 
 ```bash
 
 pip install cmind -U
 
 cm pull repo mlcommons@ck
 
+cm checkout repo mlcommons@ck --branch=dev
+cm checkout repo mlcommons@ck --branch=master
+
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
 cm run script "get ml-model image-classification resnet50 raw _fp32 _onnx"
@@ -201,15 +204,15 @@
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
 
 cmr "get conda"
 
-cm pull repo ctuning@cm-reproduce-research-projects
+cm pull repo ctuning@cm4research
 cmr "reproduce paper micro-2023 victima _install_deps"
 cmr "reproduce paper micro-2023 victima _run" 
 
 ```
 
 
 See a few examples of modular containers and GitHub actions with CM commands:
```

### Comparing `cmind-2.0.3/README.md` & `cmind-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
 ```bash
 
 pip install cmind -U
 
 cm pull repo mlcommons@ck
 
+cm checkout repo mlcommons@ck --branch=dev
+cm checkout repo mlcommons@ck --branch=master
+
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
 cm run script "get ml-model image-classification resnet50 raw _fp32 _onnx"
@@ -187,15 +190,15 @@
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
 
 cmr "get conda"
 
-cm pull repo ctuning@cm-reproduce-research-projects
+cm pull repo ctuning@cm4research
 cmr "reproduce paper micro-2023 victima _install_deps"
 cmr "reproduce paper micro-2023 victima _run" 
 
 ```
 
 
 See a few examples of modular containers and GitHub actions with CM commands:
```

### Comparing `cmind-2.0.3/cmind/artifact.py` & `cmind-2.0.4/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/automation.py` & `cmind-2.0.4/cmind/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,15 +572,18 @@
 
         deleted_lst = []
 
         for artifact in lst:
             path_to_artifact = artifact.path
 
             if console:
-                print ('Deleting CM artifact in {} ...'.format(path_to_artifact))
+                tags = artifact.meta.get('tags',[])
+                x = '' if len(tags)=='' else ' with tags "{}"'.format(','.join(tags))
+                
+                print ('Deleting CM artifact in {}{} ...'.format(path_to_artifact, x))
 
                 if not force:
                     ask = input('  Are you sure you want to delete this artifact (y/N): ')
                     ask = ask.strip().lower()
 
                     if ask!='y':
                         print ('    Skipped!')
@@ -590,15 +593,16 @@
                 continue
 
             # Deleting artifact
             deleted_lst.append(artifact)
 
             if os.name == 'nt':
                 # To be able to remove .git files
-                shutil.rmtree(path_to_artifact, ignore_errors = False, onerror = delete_helper)
+                shutil.rmtree(path_to_artifact, onerror = utils.rm_read_only)
+#                shutil.rmtree(path_to_artifact, ignore_errors = False, onerror = delete_helper)
             else:
                 shutil.rmtree(path_to_artifact)
 
             # Index
             if self.cmind.use_index:
                 r=self.cmind.index.add(artifact.meta, artifact.path, 
                                        (artifact.repo_meta['alias'], artifact.repo_meta['uid']),
@@ -1250,19 +1254,19 @@
 
             r = utils.copy_to_clipboard({'string':clipboard, 'skip_fail':True})
             # Skip output
 
 
         return {'return':0, 'list': lst}
 
-############################################################
-def delete_helper(func, path, ret):
-    import stat, errno
-
-    if ret[1].errno != errno.EACCES:
-        raise
-    else:
-        clean_attr = stat.S_IRWXG | stat.S_IRWXO | stat.S_IRWXU
-        os.chmod(path, clean_attr)
-        func(path)
-
-    return
+#############################################################
+#def delete_helper(func, path, ret):
+#    import stat, errno
+#
+#    if ret[1].errno != errno.EACCES:
+#        raise
+#    else:
+#        clean_attr = stat.S_IRWXG | stat.S_IRWXO | stat.S_IRWXU
+#        os.chmod(path, clean_attr)
+#        func(path)
+#
+#    return
```

### Comparing `cmind-2.0.3/cmind/cli.py` & `cmind-2.0.4/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/config.py` & `cmind-2.0.4/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/core.py` & `cmind-2.0.4/cmind/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,15 @@
         if self.use_index and self.index.updated:
             rx = self.index.save()
             # Ignore output for now to continue working even if issues ...
 
             self.index.updated=False
 
         # If delayed help
-        if delayed_help:
+        if delayed_help and not r.get('skip_delayed_help', False):
             print ('')
             print (delayed_help_api_prefix_0)
             print ('')
             print (delayed_help_api_prefix)
             print ('')
             print (delayed_help_api)
```

### Comparing `cmind-2.0.3/cmind/index.py` & `cmind-2.0.4/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/net.py` & `cmind-2.0.4/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/automation/README.md` & `cmind-2.0.4/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/automation/module.py` & `cmind-2.0.4/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.0.4/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/automation/module_misc.py` & `cmind-2.0.4/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/ck/README.md` & `cmind-2.0.4/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/ck/module.py` & `cmind-2.0.4/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/core/README.md` & `cmind-2.0.4/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/core/module.py` & `cmind-2.0.4/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/repo/README.md` & `cmind-2.0.4/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo/automation/repo/module.py` & `cmind-2.0.4/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repo.py` & `cmind-2.0.4/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/cmind/repos.py` & `cmind-2.0.4/cmind/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
             x = input('Delete this repo (Y/n)? ')
             if x.strip().lower() not in ['n','no']:
                 import shutil
 
                 print ('')
                 print ('Deleting {} ...'.format(path_to_repo))
-                shutil.rmtree(path_to_repo, onerror=rm_read_only)
+                shutil.rmtree(path_to_repo, onerror=utils.rm_read_only)
                 print ('')
 
         cur_dir = os.getcwd()
 
         clone=False
 
         download=True if url.find('.zip')>0 else False
@@ -650,31 +650,13 @@
             # Check if remove all
             if remove_all:
                 import shutil
 
                 if console:
                     print ('  Deleting repository content ...')
 
-                shutil.rmtree(path_to_repo, onerror=rm_read_only)
+                shutil.rmtree(path_to_repo, onerror=utils.rm_read_only)
             else:
                 if console:
                     print ('  CM repository was unregistered from CM but its content was not deleted ...')
 
         return {'return':0}
-
-##############################################################################
-def rm_read_only(f, p, e):
-    """
-    Internal aux function to remove files and dirs even if read only
-    particularly on Windows
-    """
-
-    import os
-    import stat
-    import errno
-
-    ex = e[1]
-
-    os.chmod(p, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
-    f(p)
-
-    return
```

### Comparing `cmind-2.0.3/cmind/utils.py` & `cmind-2.0.4/cmind/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1609,7 +1609,25 @@
     if matched and len(no_tags)>0:
         for t in no_tags:
             if t in tags:
                 matched = False
                 break
 
     return matched
+
+##############################################################################
+def rm_read_only(f, p, e):
+    """
+    Internal aux function to remove files and dirs even if read only
+    particularly on Windows
+    """
+
+    import os
+    import stat
+    import errno
+
+    ex = e[1]
+
+    os.chmod(p, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+    f(p)
+
+    return
```

### Comparing `cmind-2.0.3/cmind.egg-info/PKG-INFO` & `cmind-2.0.4/cmind.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.0.3
+Version: 2.0.4
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
@@ -62,14 +62,17 @@
 
 ```bash
 
 pip install cmind -U
 
 cm pull repo mlcommons@ck
 
+cm checkout repo mlcommons@ck --branch=dev
+cm checkout repo mlcommons@ck --branch=master
+
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
 cm run script "get ml-model image-classification resnet50 raw _fp32 _onnx"
@@ -201,15 +204,15 @@
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
 
 cmr "get conda"
 
-cm pull repo ctuning@cm-reproduce-research-projects
+cm pull repo ctuning@cm4research
 cmr "reproduce paper micro-2023 victima _install_deps"
 cmr "reproduce paper micro-2023 victima _run" 
 
 ```
 
 
 See a few examples of modular containers and GitHub actions with CM commands:
```

### Comparing `cmind-2.0.3/cmind.egg-info/SOURCES.txt` & `cmind-2.0.4/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-2.0.3/setup.py` & `cmind-2.0.4/setup.py`

 * *Files identical despite different names*

