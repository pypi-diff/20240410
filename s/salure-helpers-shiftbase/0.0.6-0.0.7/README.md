# Comparing `tmp/salure_helpers_shiftbase-0.0.6.tar.gz` & `tmp/salure_helpers_shiftbase-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_shiftbase-0.0.6.tar", last modified: Wed Mar 20 13:22:19 2024, max compression
+gzip compressed data, was "dist/salure_helpers_shiftbase-0.0.7.tar", last modified: Wed Apr 10 10:09:45 2024, max compression
```

## Comparing `salure_helpers_shiftbase-0.0.6.tar` & `salure_helpers_shiftbase-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      271 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers/shiftbase/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-20 13:21:59.000000 salure_helpers_shiftbase-0.0.6/salure_helpers/shiftbase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5643 2024-03-20 13:21:59.000000 salure_helpers_shiftbase-0.0.6/salure_helpers/shiftbase/shiftbase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      271 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/salure_helpers_shiftbase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 13:22:19.000000 salure_helpers_shiftbase-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-20 13:21:59.000000 salure_helpers_shiftbase-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers/shiftbase/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-10 10:09:28.000000 salure_helpers_shiftbase-0.0.7/salure_helpers/shiftbase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6768 2024-04-10 10:09:28.000000 salure_helpers_shiftbase-0.0.7/salure_helpers/shiftbase/shiftbase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/salure_helpers_shiftbase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 10:09:45.000000 salure_helpers_shiftbase-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-10 10:09:28.000000 salure_helpers_shiftbase-0.0.7/setup.py
```

### Comparing `salure_helpers_shiftbase-0.0.6/salure_helpers/shiftbase/shiftbase.py` & `salure_helpers_shiftbase-0.0.7/salure_helpers/shiftbase/shiftbase.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,8 +117,38 @@
         response = requests.get(url=f"{self.url}contract_types",
                                 headers=self.headers,
                                 params=filters)
         response.raise_for_status()
         response_json = response.json()['data']
         contract_types = [contract_type.get("ContractType") for contract_type in response_json]
 
-        return pd.DataFrame(contract_types)
+        return pd.DataFrame(contract_types)
+
+    def get_absentees(self, filters: dict = None) -> pd.DataFrame:
+        """
+        This method retrieves the absentees from Shiftbase.
+        :return:
+        """
+        response = requests.get(url=f"{self.url}absentees",
+                                headers=self.headers,
+                                params=filters)
+        response.raise_for_status()
+        response_json = response.json()['data']
+        absentees = [contract_type.get("Absentee") for absentee in response_json]
+
+        return pd.DataFrame(absentees)
+
+    def get_absentee_options(self, filters: dict = None) -> pd.DataFrame:
+        """
+        This method retrieves the absentee options from Shiftbase.
+        :return:
+        """
+        response = requests.get(url=f"{self.url}absentee_options",
+                                headers=self.headers,
+                                params=filters)
+        response.raise_for_status()
+        response_json = response.json()['data']
+        absentee_options = [contract_type.get("AbsenteeOption") for absentee_option in response_json]
+
+        return pd.DataFrame(absentee_options)
+
+
```

