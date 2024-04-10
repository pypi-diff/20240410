# Comparing `tmp/gardener-cicd-dso-1.2377.0.tar.gz` & `tmp/gardener-cicd-dso-1.2378.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2377.0.tar", last modified: Wed Apr 10 11:55:27 2024, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2378.0.tar", last modified: Wed Apr 10 13:21:10 2024, max compression
```

## Comparing `gardener-cicd-dso-1.2377.0.tar` & `gardener-cicd-dso-1.2378.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:27.794517 gardener-cicd-dso-1.2377.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 11:55:27.794517 gardener-cicd-dso-1.2377.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:27.790517 gardener-cicd-dso-1.2377.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:27.790517 gardener-cicd-dso-1.2377.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8345 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:27.794517 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 11:55:27.000000 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-04-10 11:55:27.000000 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:55:27.000000 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-04-10 11:55:27.000000 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-10 11:55:27.000000 gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:27.794517 gardener-cicd-dso-1.2377.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10627 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29194 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     9129 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 11:55:27.794517 gardener-cicd-dso-1.2377.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-10 11:54:39.000000 gardener-cicd-dso-1.2377.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:10.485696 gardener-cicd-dso-1.2378.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 13:21:10.485696 gardener-cicd-dso-1.2378.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:10.481696 gardener-cicd-dso-1.2378.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:10.481696 gardener-cicd-dso-1.2378.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8345 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:10.485696 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 13:21:10.000000 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-10 13:21:10.000000 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:21:10.000000 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-10 13:21:10.000000 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-10 13:21:10.000000 gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:10.485696 gardener-cicd-dso-1.2378.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10627 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    29221 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     9129 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 13:21:10.485696 gardener-cicd-dso-1.2378.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-10 13:20:09.000000 gardener-cicd-dso-1.2378.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2377.0/LICENSE` & `gardener-cicd-dso-1.2378.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/README.md` & `gardener-cicd-dso-1.2378.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/checkmarx/client.py` & `gardener-cicd-dso-1.2378.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/checkmarx/model.py` & `gardener-cicd-dso-1.2378.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/checkmarx/project.py` & `gardener-cicd-dso-1.2378.0/checkmarx/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             scan_id=scan_id,
             timeout_seconds=timeout_seconds,
         )
 
         return model.ScanResult(
             state=scan_state,
             scanned_element=cnudie.iter.SourceNode(
-                path=(component,),
+                path=(cnudie.iter.NodePathEntry(component),),
                 source=source,
             ),
             project_id=self.project_details.id,
             artifact_name=self.artifact_name,
             scan_response=scan_response,
             scan_statistic=statistics,
             report_url=report_url,
```

### Comparing `gardener-cicd-dso-1.2377.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2378.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/checkmarx/util.py` & `gardener-cicd-dso-1.2378.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/client.py` & `gardener-cicd-dso-1.2378.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2378.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/model.py` & `gardener-cicd-dso-1.2378.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/report.py` & `gardener-cicd-dso-1.2378.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/routes.py` & `gardener-cicd-dso-1.2378.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/scan.py` & `gardener-cicd-dso-1.2378.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/clamav/util.py` & `gardener-cicd-dso-1.2378.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2378.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/protecode/assessments.py` & `gardener-cicd-dso-1.2378.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/protecode/client.py` & `gardener-cicd-dso-1.2378.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/protecode/model.py` & `gardener-cicd-dso-1.2378.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/protecode/rescore.py` & `gardener-cicd-dso-1.2378.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/protecode/scanning.py` & `gardener-cicd-dso-1.2378.0/protecode/scanning.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
                 scan_result = bse
                 scan_failed = True
                 logger.warning(bse.print_stacktrace())
 
             c = scan_request.component
             r = scan_request.artefact
             scanned_element = cnudie.iter.ResourceNode(
-                path=(c,),
+                path=(cnudie.iter.NodePathEntry(c),),
                 resource=r,
             )
 
             if scan_failed:
                 logger.error(f'scan of {scanned_element=} failed; {scan_result=}')
                 return
```

### Comparing `gardener-cicd-dso-1.2377.0/protecode/util.py` & `gardener-cicd-dso-1.2378.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/setup.dso.py` & `gardener-cicd-dso-1.2378.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2377.0/setup.py` & `gardener-cicd-dso-1.2378.0/setup.py`

 * *Files identical despite different names*

