# Comparing `tmp/benvy-1.4.6-py3-none-any.whl.zip` & `tmp/benvy-1.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 78114 bytes, number of entries: 54
+Zip file size: 78172 bytes, number of entries: 54
 -rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 benvy/BenvyConfig.py
 -rw-r--r--  2.0 unx     7757 b- defN 80-Jan-01 00:00 benvy/container/dicontainer.py
 -rw-r--r--  2.0 unx     2187 b- defN 80-Jan-01 00:00 benvy/databricks/BinExecutableFlagSetter.py
 -rw-r--r--  2.0 unx     1020 b- defN 80-Jan-01 00:00 benvy/databricks/DatabricksConnectConfigCreator.py
 -rw-r--r--  2.0 unx      807 b- defN 80-Jan-01 00:00 benvy/databricks/DatabricksConnectDetector.py
 -rw-r--r--  2.0 unx      416 b- defN 80-Jan-01 00:00 benvy/databricks/DatabricksContext.py
 -rw-r--r--  2.0 unx      454 b- defN 80-Jan-01 00:00 benvy/databricks/api/WorkspaceApiFactory.py
 -rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 benvy/databricks/dbutils/DBUtilsResolver.py
 -rw-r--r--  2.0 unx      198 b- defN 80-Jan-01 00:00 benvy/databricks/detector.py
 -rw-r--r--  2.0 unx     1007 b- defN 80-Jan-01 00:00 benvy/databricks/notebook/CommandConverter.py
 -rw-r--r--  2.0 unx      876 b- defN 80-Jan-01 00:00 benvy/databricks/notebook/CommandsConverter.py
 -rw-r--r--  2.0 unx      499 b- defN 80-Jan-01 00:00 benvy/databricks/notebook/NotebookConverter.py
 -rw-r--r--  2.0 unx      861 b- defN 80-Jan-01 00:00 benvy/databricks/repos/bootstrap.py
--rw-r--r--  2.0 unx     1404 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/BootstrapConfig.py
+-rw-r--r--  2.0 unx     1505 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/BootstrapConfig.py
 -rw-r--r--  2.0 unx      581 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/BootstrapInstallConfig.py
 -rw-r--r--  2.0 unx      478 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/BootstrapInstallDevConfig.py
 -rw-r--r--  2.0 unx      416 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/BootstrapSetupEnvConfig.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 benvy/databricks/repos/config/PoetrySetupConfig.py
 -rw-r--r--  2.0 unx     1035 b- defN 80-Jan-01 00:00 benvy/databricks/repos/export/ExportObject.py
 -rw-r--r--  2.0 unx     4167 b- defN 80-Jan-01 00:00 benvy/databricks/repos/export/NotebooksAndFilesExporter.py
 -rw-r--r--  2.0 unx     2514 b- defN 80-Jan-01 00:00 benvy/databricks/repos/install/DbrDependenciesChecker.py
@@ -45,12 +45,12 @@
 -rw-r--r--  2.0 unx      286 b- defN 80-Jan-01 00:00 benvy/databricks/repos/uploader/get_uploader.py
 -rw-r--r--  2.0 unx      946 b- defN 80-Jan-01 00:00 benvy/hadoop/WinutilsDownloader.py
 -rw-r--r--  2.0 unx      371 b- defN 80-Jan-01 00:00 benvy/init.py
 -rw-r--r--  2.0 unx     3599 b- defN 80-Jan-01 00:00 benvy/java/JavaSetup.py
 -rw-r--r--  2.0 unx      537 b- defN 80-Jan-01 00:00 benvy/java/JavaVersion.py
 -rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 benvy/libroot.py
 -rw-r--r--  2.0 unx     1292 b- defN 80-Jan-01 00:00 benvy/mutex/Mutex.py
--rw-r--r--  2.0 unx     1704 b- defN 80-Jan-01 00:00 benvy-1.4.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 benvy-1.4.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 benvy-1.4.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     5329 b- defN 16-Jan-01 00:00 benvy-1.4.6.dist-info/RECORD
-54 files, 130791 bytes uncompressed, 69322 bytes compressed:  47.0%
+-rw-r--r--  2.0 unx     1704 b- defN 80-Jan-01 00:00 benvy-1.4.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 benvy-1.4.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 benvy-1.4.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     5329 b- defN 16-Jan-01 00:00 benvy-1.4.7.dist-info/RECORD
+54 files, 130892 bytes uncompressed, 69380 bytes compressed:  47.0%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: benvy/libroot.py
 Comment: 
 
 Filename: benvy/mutex/Mutex.py
 Comment: 
 
-Filename: benvy-1.4.6.dist-info/METADATA
+Filename: benvy-1.4.7.dist-info/METADATA
 Comment: 
 
-Filename: benvy-1.4.6.dist-info/WHEEL
+Filename: benvy-1.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: benvy-1.4.6.dist-info/entry_points.txt
+Filename: benvy-1.4.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: benvy-1.4.6.dist-info/RECORD
+Filename: benvy-1.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benvy/databricks/repos/config/BootstrapConfig.py

```diff
@@ -1,25 +1,27 @@
+import os
 import logging
 from penvy.env.EnvConfig import EnvConfig
 from penvy.PenvyConfig import PenvyConfig
 from benvy.databricks.repos.project_root_resolver import resolve_project_root
 
 
 class BootstrapConfig(EnvConfig):
     def get_parameters(self) -> dict:
         poetry_version = PenvyConfig().get_parameters()["poetry"]["install_version"]
+        poetry_executable = os.getenv("DAIPE_POETRY_EXECUTABLE_PATH") or "/root/.poetry/bin/poetry"
 
         return {
             "project": {
                 "dir": resolve_project_root(),
             },
             "poetry": {
                 "version": poetry_version,
                 "home": "/root/.poetry",
-                "executable": "/root/.poetry/bin/poetry",
+                "executable": poetry_executable,
                 "archive_url": f"https://github.com/python-poetry/poetry/releases/download/{poetry_version}/{self.__get_archive_filename(poetry_version)}",
                 "install_script_url": f"https://raw.githubusercontent.com/python-poetry/poetry/{poetry_version}/get-poetry.py",
                 "archive_path": f"/dbfs/FileStore/jars/daipe/poetry/{self.__get_archive_filename(poetry_version)}",
                 "install_script_path": "/dbfs/FileStore/jars/daipe/poetry/get-poetry.py",
             },
             "logger": {
                 "name": "daipe-bootstrap",
```

## Comparing `benvy-1.4.6.dist-info/METADATA` & `benvy-1.4.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benvy
-Version: 1.4.6
+Version: 1.4.7
 Summary: Daipe framework development environment initializer
 Home-page: https://github.com/daipe-ai/benvy
 License: MIT
 Author: Jiri Koutny
 Author-email: jiri.koutny@datasentics.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `benvy-1.4.6.dist-info/RECORD` & `benvy-1.4.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 benvy/databricks/api/WorkspaceApiFactory.py,sha256=5XbTRplyGkfzaxGYJoCHcdn9SaZaV5IMHI9Yb1Mvij8,454
 benvy/databricks/dbutils/DBUtilsResolver.py,sha256=57MBScznFm1pNfihXOtDyRjS6Q_JLkCKCqqQciif-dA,249
 benvy/databricks/detector.py,sha256=MzZbkvlYuLAVisdjhzXD0CjBl5xeljp8ZfiUIT9ghyw,198
 benvy/databricks/notebook/CommandConverter.py,sha256=AQFpOxKIlJlX_Ar3teJohwGHDDvHKv4JnB3rk5sc-0Y,1007
 benvy/databricks/notebook/CommandsConverter.py,sha256=_iIKgIzljK5wlb0qr5HJ_RgaVPfOvl-t3v_EcLOKxUg,876
 benvy/databricks/notebook/NotebookConverter.py,sha256=G49bIR654lIkuiMz-pr_spp-8d0C5xTlj0ibBNwXqW8,499
 benvy/databricks/repos/bootstrap.py,sha256=3xmcXF0rhpk2UyAhgC6oHj-vyLQ8vfiJmi-n5zianQ4,861
-benvy/databricks/repos/config/BootstrapConfig.py,sha256=Y9B7wV8zfpEEIz88yfJ8klWWWKHaZkRmONOcWJMAXDc,1404
+benvy/databricks/repos/config/BootstrapConfig.py,sha256=RDmAx3X1bgX6JSVZMPE-niMY5uAjkE0ohPVDr7I9veE,1505
 benvy/databricks/repos/config/BootstrapInstallConfig.py,sha256=vpJb19WiGw3judRTdGqBTl7DC6X_Rstn2PfjlqAzYfE,581
 benvy/databricks/repos/config/BootstrapInstallDevConfig.py,sha256=k0-vWKY-90bcXIivsDIVFfVYlPb0yPxtfJWnmnjlKQ4,478
 benvy/databricks/repos/config/BootstrapSetupEnvConfig.py,sha256=nIO1I33Op9iam5d1tb65UnYAv-WClxIKUf3TywwkjzU,416
 benvy/databricks/repos/config/PoetrySetupConfig.py,sha256=pQAaC5ZlBNmQN5qULRsonG23OKj5DbBN3kCFMKd7cZQ,415
 benvy/databricks/repos/export/ExportObject.py,sha256=ON3GwY5WzbMuFx1anaxSQXoP5gw4mKeX3kcEyn4nHtE,1035
 benvy/databricks/repos/export/NotebooksAndFilesExporter.py,sha256=xfNdemrd2JmYW_lu2Zg7ObO6wNqTLuGCXOs7tGqZWmI,4167
 benvy/databricks/repos/install/DbrDependenciesChecker.py,sha256=gc_eXa8zmugd7Y9E1SEOPWe6PFrZwp6bNb1FBoqEAhU,2514
@@ -44,11 +44,11 @@
 benvy/databricks/repos/uploader/get_uploader.py,sha256=De0YLAH5stjJa289G5P83m7761LCWymfv1i1VUAxY78,286
 benvy/hadoop/WinutilsDownloader.py,sha256=AP5jbW5JlSZb_eWAJmNnrS5Q-nJQFRpAvtQQfg4giX0,946
 benvy/init.py,sha256=ZYDtP6jahWBPKgY9zZl9y78V5nF3iLMQ53fjR1QcSRQ,371
 benvy/java/JavaSetup.py,sha256=0IOM6Kgj4f42_Bj0b7nYdHPjLX66Yrc4OGiatzWXXz4,3599
 benvy/java/JavaVersion.py,sha256=DkVaMxi5rWIOR5BviIG4W7h1IxkpDTD2h2tR-9SNOpg,537
 benvy/libroot.py,sha256=fMY1E2FjAl7mjwlG5ANA5PSb6iaV4ngvHR5nJCA4spE,85
 benvy/mutex/Mutex.py,sha256=0yO0VIOCgZ4bZ4-bRe4UQMCM9tp34EItfp-vJ4jE1D8,1292
-benvy-1.4.6.dist-info/METADATA,sha256=VVpheaELfGiqRt4p6Z9x-fdyWSqEGmDMUK2PPHJy2FU,1704
-benvy-1.4.6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-benvy-1.4.6.dist-info/entry_points.txt,sha256=A4hn6nYD2GsWzefFDnoxMy5i28WYpi7R1MM_OmX25i4,46
-benvy-1.4.6.dist-info/RECORD,,
+benvy-1.4.7.dist-info/METADATA,sha256=ddWJTTGN5i6UwrTAWKbAdyfjJCeakzZ-CZdtx3vrRFs,1704
+benvy-1.4.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+benvy-1.4.7.dist-info/entry_points.txt,sha256=A4hn6nYD2GsWzefFDnoxMy5i28WYpi7R1MM_OmX25i4,46
+benvy-1.4.7.dist-info/RECORD,,
```

