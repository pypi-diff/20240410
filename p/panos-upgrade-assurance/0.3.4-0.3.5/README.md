# Comparing `tmp/panos_upgrade_assurance-0.3.4.tar.gz` & `tmp/panos_upgrade_assurance-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.3.4.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.3.5.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.3.4.tar` & `panos_upgrade_assurance-0.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/LICENSE
--rw-r--r--   0        0        0     1679 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/README.md
--rw-r--r--   0        0        0       76 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    67339 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0     2869 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/exceptions.py
--rw-r--r--   0        0        0    60228 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    31975 2024-03-07 11:26:41.636117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    13150 2024-03-07 11:26:41.640117 panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0     1370 2024-03-07 11:26:41.640117 panos_upgrade_assurance-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1679 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/README.md
+-rw-r--r--   0        0        0       76 2024-04-10 01:28:02.984299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    67339 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2869 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    60521 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31975 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    13150 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1370 2024-04-10 01:28:02.988299 panos_upgrade_assurance-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.3.5/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.3.4/LICENSE` & `panos_upgrade_assurance-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/README.md` & `panos_upgrade_assurance-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/check_firewall.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/exceptions.py` & `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1389,19 +1389,24 @@
             'warnings': None}}
         ```
 
         """
         jobs = self.op_parser(cmd="show jobs all")
         results = dict()
 
-        if jobs:
-            for job in jobs["job"]:
+        job_results = jobs.get("job") if isinstance(jobs, dict) else None
+        if isinstance(job_results, list):
+            for job in job_results:
                 jid = job["id"]
                 job.pop("id")
                 results[jid] = job
+        elif isinstance(job_results, dict):  # single job entry - FW just started up
+            jid = job_results["id"]
+            job_results.pop("id")
+            results[jid] = job_results
 
         return results
 
     def get_user_id_service_status(self) -> dict:
         """Get the status of the User ID agent service.
 
         The user-id service is used to redistribute user-id information to other firewalls.
```

### Comparing `panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.3.5/panos_upgrade_assurance/utils.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.3.4/pyproject.toml` & `panos_upgrade_assurance-0.3.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
```

### Comparing `panos_upgrade_assurance-0.3.4/PKG-INFO` & `panos_upgrade_assurance-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

