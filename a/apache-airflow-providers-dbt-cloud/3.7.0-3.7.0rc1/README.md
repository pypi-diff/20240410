# Comparing `tmp/apache_airflow_providers_dbt_cloud-3.7.0.tar.gz` & `tmp/apache_airflow_providers_dbt_cloud-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_dbt_cloud-3.7.0.tar", last modified: Mon Mar  4 12:28:48 2024, max compression
+gzip compressed data, was "apache_airflow_providers_dbt_cloud-3.7.0rc1.tar", last modified: Mon Mar  4 12:28:48 2024, max compression
```

## Comparing `apache_airflow_providers_dbt_cloud-3.7.0.tar` & `apache_airflow_providers_dbt_cloud-3.7.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4382 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/LICENSE
--rw-r--r--   0        0        0     1584 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0        0        0     3287 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0        0        0    26082 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/hooks/dbt.py
--rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0        0        0    15630 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/operators/dbt.py
--rw-r--r--   0        0        0      787 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0        0        0     6860 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/sensors/dbt.py
--rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0        0        0     4648 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/triggers/dbt.py
--rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/utils/__init__.py
--rw-r--r--   0        0        0     5644 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/utils/openlineage.py
--rw-r--r--   0        0        0     3129 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     6287 1970-01-01 00:00:00.000000 apache_airflow_providers_dbt_cloud-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4386 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/LICENSE
+-rw-r--r--   0        0        0     1584 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0        0        0     3287 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0        0        0    26082 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0        0        0    15630 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/operators/dbt.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0        0        0     6860 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0        0        0     4648 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/utils/__init__.py
+-rw-r--r--   0        0        0     5644 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/utils/openlineage.py
+-rw-r--r--   0        0        0     3138 2024-03-04 12:28:48.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 apache_airflow_providers_dbt_cloud-3.7.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/README.rst` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.7.0``
+Release: ``3.7.0.rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/dbt-cloud/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/LICENSE` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/get_provider_info.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/operators/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/operators/dbt.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/utils/__init__.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/airflow/providers/dbt/cloud/utils/openlineage.py` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/airflow/providers/dbt/cloud/utils/openlineage.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/pyproject.toml` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-dbt-cloud"
-version = "3.7.0"
+version = "3.7.0.rc1"
 description = "Provider package apache-airflow-providers-dbt-cloud for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -53,15 +53,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
     "aiohttp>=3.9.2",
     "apache-airflow-providers-http",
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0.dev0",
     "asgiref",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_dbt_cloud-3.7.0/PKG-INFO` & `apache_airflow_providers_dbt_cloud-3.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.7.0
+Version: 3.7.0rc1
 Summary: Provider package apache-airflow-providers-dbt-cloud for Apache Airflow
 Keywords: airflow-provider,dbt.cloud,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: aiohttp>=3.9.2
 Requires-Dist: apache-airflow-providers-http
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: asgiref
 Requires-Dist: apache-airflow-providers-http ; extra == "http"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -76,15 +76,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.7.0``
+Release: ``3.7.0.rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/dbt-cloud/>`__
 
 
 Provider package
 ----------------
```

