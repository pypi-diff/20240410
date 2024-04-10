# Comparing `tmp/xia-module-gcp-bigquery-0.0.8.tar.gz` & `tmp/xia-module-gcp-bigquery-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-gcp-bigquery-0.0.8.tar", last modified: Sat Apr  6 17:55:40 2024, max compression
+gzip compressed data, was "xia-module-gcp-bigquery-0.0.9.tar", last modified: Sat Apr  6 19:25:47 2024, max compression
```

## Comparing `xia-module-gcp-bigquery-0.0.8.tar` & `xia-module-gcp-bigquery-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/base/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.234328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 17:55:14.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:55:40.230328 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 17:55:40.000000 xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.642554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 19:25:21.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:47.638554 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 19:25:47.000000 xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/top_level.txt
```

### Comparing `xia-module-gcp-bigquery-0.0.8/LICENSE` & `xia-module-gcp-bigquery-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/setup.py` & `xia-module-gcp-bigquery-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml`

 * *Files 23% similar despite different names*

```diff
@@ -17,26 +17,26 @@
       name: Checkout code
       uses: actions/checkout@v4
 
     - id: prepare-modules
       name: Prepare modules
       run: |
         pip install xia-framework xia-module
-        python main.py prepare
+        python -m xia_framework.application prepare -e ${{ vars.env_name }}
 
     - id: auth-gcp-oidc
       name: Authenticate to Google Cloud
       uses: google-github-actions/auth@v2
       with:
         project_id: ${{ vars.PROJECT_ID }}
         workload_identity_provider: ${{ vars.SECRET_WIP_NAME }}
         service_account: ${{ vars.PROVIDER_SA_EMAIL }}
 
     - id: terraform-apply
       name: Apply Terraform
-      uses: ./.github/actions/gcp-module-dataset/gcs-terraform-apply
+      uses: x-i-a/action-gcs-terraform-apply@main
       with:
         cosmos_name: ${{ vars.cosmos_name }}
         realm_name: ${{ vars.realm_name }}
         foundation_name: ${{ vars.foundation_name }}
         app_name: ${{ vars.app_name }}
         env_name: ${{ vars.env_name }}
```

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.8/xia_module_gcp_bigquery.egg-info/SOURCES.txt` & `xia-module-gcp-bigquery-0.0.9/xia_module_gcp_bigquery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 xia_module_gcp_bigquery.egg-info/requires.txt
 xia_module_gcp_bigquery.egg-info/top_level.txt
 xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
-xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
 xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
```

