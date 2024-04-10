# Comparing `tmp/rcsb.db-1.717.tar.gz` & `tmp/rcsb.db-1.718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.717.tar", last modified: Thu Apr  4 15:33:48 2024, max compression
+gzip compressed data, was "rcsb.db-1.718.tar", last modified: Wed Apr 10 21:05:38 2024, max compression
```

## Comparing `rcsb.db-1.717.tar` & `rcsb.db-1.718.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.966329 rcsb.db-1.717/
--rw-r--r--   0 vsts      (1001) docker     (127)    30462 2024-04-04 15:10:22.000000 rcsb.db-1.717/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-04 15:10:22.000000 rcsb.db-1.717/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-04 15:10:22.000000 rcsb.db-1.717/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-04-04 15:33:48.966329 rcsb.db-1.717/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    26823 2024-04-04 15:10:22.000000 rcsb.db-1.717/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.950329 rcsb.db-1.717/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7661 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24702 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8774 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15040 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54787 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)    11601 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 15:13:43.000000 rcsb.db-1.717/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-04 15:10:22.000000 rcsb.db-1.717/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-04 15:33:48.966329 rcsb.db-1.717/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-04-04 15:10:22.000000 rcsb.db-1.717/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/
+-rw-r--r--   0 vsts      (1001) docker     (127)    30577 2024-04-10 20:44:31.000000 rcsb.db-1.718/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-10 20:44:31.000000 rcsb.db-1.718/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-10 20:44:31.000000 rcsb.db-1.718/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-04-10 21:05:38.514944 rcsb.db-1.718/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    24032 2024-04-10 20:44:31.000000 rcsb.db-1.718/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.502943 rcsb.db-1.718/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13346 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8990 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.506943 rcsb.db-1.718/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15187 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    60384 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.510944 rcsb.db-1.718/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:31.000000 rcsb.db-1.718/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)    22136 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 20:44:32.000000 rcsb.db-1.718/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 21:05:38.514944 rcsb.db-1.718/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    25578 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 20:48:40.000000 rcsb.db-1.718/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-10 21:05:38.000000 rcsb.db-1.718/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-10 20:44:32.000000 rcsb.db-1.718/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-10 21:05:38.514944 rcsb.db-1.718/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-04-10 20:44:32.000000 rcsb.db-1.718/setup.py
```

### Comparing `rcsb.db-1.717/HISTORY.txt` & `rcsb.db-1.718/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -349,7 +349,8 @@
  23-Sep-2023  V1.712 Add support for pdb_id_u cifType in DataTypeApplicationInfo
   6-Nov-2023  V1.713 Add maxStepLength argument to RepoLoadWorkflow
  21-Nov-2023  V1.714 Add support in json schema for min and unique items for sub-categories and iterable attributes
  15-Dec-2023  V1.715 Revert setting for mergeValidationReports
  19-Mar-2024  V1.716 Add quality check to PdbxLoader to ensure validation report data are loaded along with the primary data;
                      Begin updating PdbxLoader and RepoLoadEx to support weekly update workflow CLI requirements
  03-Apr-2024  V1.717 Add int_list cifType to DataTypeApplicationInfo
+ 09-Apr-2024  V1.718 Update RepoLoadExec CLI and RepoLoadWorkflow to support CLI usage from weekly-update workflow
```

### Comparing `rcsb.db-1.717/LICENSE` & `rcsb.db-1.718/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/PKG-INFO` & `rcsb.db-1.718/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.717
+Version: 1.718
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -104,16 +104,27 @@
 Follow the instructions provided by at the [HomeBrew](https://brew.sh/) site to
 install this system.   Once HomeBrew is installed, you can further install the
 [MariaDB](https://mariadb.com/kb/en/library/installing-mariadb-on-macos-using-homebrew/) and
 [MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/) packages which
 are required to support the ExDB  tools.  HomeBrew also provides a variety of options for
 managing a [Python virtual environments](https://gist.github.com/Geoyi/f55ed54d24cc9ff1c14bd95fac21c042).
 
+### Configuration File
+
+RCSB/PDB repository path details are stored as configuration options.
+An example configuration file included in this package is viewable under `rcsb/db/config`: [exdb-config-example.yml](https://github.com/rcsb/py-rcsb_db/blob/master/rcsb/db/config/exdb-config-example.yml). This example references dictionary resources and mock repository data
+provided in the package in `rcsb/mock-data/*`. The `site_info_configuration` section
+in this file provides database server connection details and common path details.
+This is followed by sections specifying the dictionaries, helper functions, and
+configuration used to define the schema for the each supported content type
+(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
+
 ### Command Line Interfaces
 
+#### Schema File Generation
 A convenience CLI `schema_update_cli` is provided for generating operational schema from
 PDBx/mmCIF dictionary metadata.  Schema are encoded for the ExDB  API (rcsb), and
 for the document schema encoded in JSON and BSON formats.  The latter schema can be used to
 validate the loadable document objects produced for the collections served by MongoDB.
 
 ```bash
  => schema_update_cli  --help
@@ -182,129 +193,205 @@
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for dependencies and
                         testing
 ________________________________________________________________________________
 
 ```
 
+##### Example Usage
+
 For example, the following command will generate the JSON and BSON schema for the collections in the
 pdbx_core schema.
 
 ```bash
 schema_update_cli  --mock --schema_types json,bson \
                    --schema_level full  \
                    --update_pdbx_core   \
                    --cache_path . \
                    --config_path ./rcsb/db/config/exdb-config-example.yml  \
                    --config_name site_info_configuration
 ```
 
+#### ExDB Loading
+
 A convenience CLI `exdb_repo_load_cli` is provided to support loading PDB repositories
 containing entry and chemical reference data content types in the form of document collections
 compatible with MongoDB.
 
 ```bash
 exdb_repo_load_cli --help
 
-usage: exdb_repo_load_cli [-h] [--full] [--replace] [--load_chem_comp_ref]
-                          [--load_chem_comp_core_ref]
-                          [--load_bird_chem_comp_ref]
-                          [--load_bird_chem_comp_core_ref] [--load_bird_ref]
-                          [--load_bird_family_ref] [--load_entry_data]
-                          [--load_pdbx_core] [--load_pdbx_core_merge]
-                          [--load_pdbx_core_entry] [--load_pdbx_core_entity]
-                          [--load_pdbx_core_entity_monomer]
-                          [--load_pdbx_core_assembly] [--load_ihm_dev]
+usage: exdb_repo_load_cli [-h] [--op OP_TYPE] [--load_type LOAD_TYPE]
+                          [--database DATABASE_NAME]
                           [--config_path CONFIG_PATH]
                           [--config_name CONFIG_NAME] [--db_type DB_TYPE]
+                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--document_style DOCUMENT_STYLE]
-                          [--read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--disable_read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--load_id_list_path LOAD_ID_LIST_PATH]
                           [--load_file_list_path LOAD_FILE_LIST_PATH]
                           [--fail_file_list_path FAIL_FILE_LIST_PATH]
                           [--save_file_list_path SAVE_FILE_LIST_PATH]
-                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--file_limit FILE_LIMIT]
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --full                Fresh full load in a new tables/collections
-  --replace             Load with replacement in an existing table/collection
-                        (default)
-  --load_chem_comp_ref  Load Chemical Component reference definitions (public
-                        subset)
-  --load_chem_comp_core_ref
-                        Load Chemical Component Core reference definitions
-                        (public subset)
-  --load_bird_chem_comp_ref
-                        Load Bird Chemical Component reference definitions
-                        (public subset)
-  --load_bird_chem_comp_core_ref
-                        Load Bird Chemical Component Core reference
-                        definitions (public subset)
-  --load_bird_ref       Load Bird reference definitions (public subset)
-  --load_bird_family_ref
-                        Load Bird Family reference definitions (public subset)
-  --load_entry_data     Load PDBx entry data (current released subset)
-  --load_pdbx_core      Load all PDBx core collections (current released
-                        subset)
-  --load_pdbx_core_merge
-                        Load all PDBx core collections with merged content
-                        (current released subset)
-  --load_pdbx_core_entry
-                        Load PDBx core entry (current released subset)
-  --load_pdbx_core_entity
-                        Load PDBx core entity (current released subset)
-  --load_pdbx_core_entity_monomer
-                        Load PDBx core entity monomer (current released
-                        subset)
-  --load_pdbx_core_assembly
-                        Load PDBx core assembly (current released subset)
-  --load_ihm_dev        Load I/HM DEV model data (current released subset)
+  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+                        Loading operation to perform
+  --load_type {replace,full}
+                        Type of load ('replace' for incremental and
+                        multi-worker load, 'full' for complete and
+                        fresh single-worker load)
+  --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
+                        Database to load (most common choices are:
+                        'pdbx_core', 'pdbx_comp_model_core', or
+                        'bird_chem_comp_core')
   --config_path CONFIG_PATH
                         Path to configuration options file
   --config_name CONFIG_NAME
                         Configuration section name
-  --db_type DB_TYPE     Database server type (default=mongo)
   --document_style DOCUMENT_STYLE
-                        Document organization (rowwise_by_name_with_cardinalit
-                        y|rowwise_by_name|columnwise_by_name|rowwise_by_id|row
-                        wise_no_name
-  --read_back_check     Perform read back check on all documents
+                        Document organization (rowwise_by_name_with_c
+                        ardinality|rowwise_by_name|columnwise_by_name
+                        |rowwise_by_id|rowwise_no_name)
+  --cache_path CACHE_PATH
+                        Cache path for resource files
+  --num_proc NUM_PROC   Number of processes to execute (default=2)
+  --chunk_size CHUNK_SIZE
+                        Number of files loaded per process
+  --max_step_length MAX_STEP_LENGTH
+                        Maximum subList size (default=500)
   --schema_level SCHEMA_LEVEL
-                        Schema validation level (full|min default=None)
+                        Schema validation level (full|min)
+  --collection_list COLLECTION_LIST
+                        Specific collections to load
+  --load_id_list_path LOAD_ID_LIST_PATH
+                        Input file containing the list of IDs to load
+                        in the current iteration by a single worker
+  --holdings_file_path HOLDINGS_FILE_PATH
+                        File containing the complete list of all IDs
+                        (or holdings files) that will be loaded
   --load_file_list_path LOAD_FILE_LIST_PATH
-                        Input file containing load file path list (override
-                        automatic repository scan)
+                        Input file containing load file path list
+                        (override automatic repository scan)
   --fail_file_list_path FAIL_FILE_LIST_PATH
-                        Output file containing file paths that fail to load
+                        Output file containing file paths that fail
+                        to load
   --save_file_list_path SAVE_FILE_LIST_PATH
-                        Save repo file paths from automatic file system scan
-                        in this path
-  --num_proc NUM_PROC   Number of processes to execute (default=2)
-  --chunk_size CHUNK_SIZE
-                        Number of files loaded per process
+                        Save repo file paths from automatic file
+                        system scan in this path
+  --load_file_list_dir LOAD_FILE_LIST_DIR
+                        Directory path for storing load file lists
+  --num_sublists NUM_SUBLISTS
+                        Number of sublists to create/load for the
+                        associated database
+  --force_reload        Force re-load of provided ID list (i.e.,
+                        don't just load delta; useful for manual/test
+                        runs).
+  --provider_type_exclude PROVIDER_TYPE_EXCLUDE
+                        Resource provider types to exclude
+  --db_type DB_TYPE     Database server type (default=mongo)
   --file_limit FILE_LIMIT
                         Load file limit for testing
   --prune_document_size PRUNE_DOCUMENT_SIZE
                         Prune large documents to this size limit (MB)
+  --regex_purge         Perform additional regex-based purge of all
+                        pre-existing documents for loadType != 'full'
+  --data_selectors  [ ...]
+                        Data selectors, space-separated.
+  --disable_read_back_check
+                        Disable read back check on all documents
+  --disable_merge_validation_reports
+                        Disable merging of validation report data
+                        with the primary content type
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for testing
-  --cache_path CACHE_PATH
-                        Cache path for resource files
   --rebuild_cache       Rebuild cached resource files
   --rebuild_schema      Rebuild schema on-the-fly if not cached
   --vrpt_repo_path VRPT_REPO_PATH
                         Path to validation report repository
 ________________________________________________________________________________
 ```
 
+##### Example Usage
+The following commands demonstrate how each type of operation (`--op`) is used for loading of PDB repository data to ExDB. For all commands, the following environmental variables must first be set:
+
+```bash
+export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
+export OE_LICENSE=/path/to/oe_license.txt
+export NLTK_DATA=/path/to/nltk_data
+```
+
+`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+```bash
+exdb_repo_load_cli --op "build-resource-cache" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--num_proc 6  \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+```bash
+exdb_repo_load_cli --op "pdbx-db-wiper" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+```bash
+exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+```bash
+exdb_repo_load_cli --op "pdbx-loader" \
+--database "pdbx_core" \
+--load_type replace  \
+--config_path /opt/etl-scratch/config/exdb-loader-config.yml \
+--config_name site_info_remote_configuration \
+--num_proc 8  \
+--chunk_size 5  \
+--max_step_length 500 \
+--load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+```bash
+exdb_repo_load_cli --op "pdbx-loader-check" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+#### Repository Scanning
+
 Part of the schema definition process supported by this module involves refining
 the dictionary metadata with more specific data typing and coverage details.
 A scanning tools is provided to collect and organize these details for the
 other ETL tools in this package.  The following convenience CLI, `repo_scan_cli`,
 is provided to scan supported PDB repository content and update data type and coverage details.
 
 ```bash
@@ -367,14 +454,15 @@
   --mock                Use MOCK repository configuration for testing
   --working_path WORKING_PATH
                         Working path for temporary files
 ________________________________________________________________________________
 
 ```
 
+#### ETL Processing
 The following CLI provides a preliminary access to ETL functions for processing
 derived content types such as sequence comparative data.
 
 ```bash
 etl_exec_cli --help
 usage: etl_exec_cli [-h] [--full] [--etl_entity_sequence_clusters]
                     [--etl_repository_holdings] [--data_set_id DATA_SET_ID]
@@ -421,170 +509,48 @@
   --cache_path CACHE_PATH
                         Path containing cache directories
   --rebuild_cache       Rebuild cached resource files
 ________________________________________________________________________________
 
 ```
 
-### Examples
+### Additional Examples
+
+(*Note: The examples below are outdated and may not function as described. They are only kept here for historical reference.*)
 
 If you are working in the source repository, then you can run the CLI commands in the following manner.
 The following examples load data in the mock repositories in source distribution assuming you have a local
 default installation of MongoDb (no user/pw assigned).
 
 To run the command-line interface `exdb_repo_load_cli` outside of the source distribution, you will need to
 create a configuration file with the appropriate path details and authentication credentials.
 
 For instance, to perform a fresh/full load of all of the chemical component definitions in the mock repository:
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py --full  --load_chem_comp_ref  \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --fail_file_list_path failed-cc-path-list.txt \
                       --read_back_check
 ```
 
 The following illustrates, a full load of the mock structure data repository followed by a reload with replacement of
 this same data.
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py  --mock --full  --load_entry_data \
                      --config_path ../config/exdb-config-example.yml \
                      --config_name site_info_configuration \
                      --save_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                      --fail_file_list_path failed-entry-path-list.txt
 
 python RepoLoadExec.py --mock --replace  --load_entry_data \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --load_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                       --fail_file_list_path failed-entry-path-list.txt
 ```
-
-### Configuration Example
-
-RCSB/PDB repository path details are stored as configuration options.
-An example configuration file included in this package is shown below.
-This example is references dictionary resources and mock repository data
-provided in the package in `rcsb/mock-data/*`. Example configuration details are
-stored in rcsb/db/config/exdb-config-example.yml.The `site_info_configuration` section
-in this file provides database server connection details and common path details.
-This is followed by sections specifying the dictionaries, helper functions, and
-configuration used to define the schema for the each supported content type
-(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
-
-```yaml
-site_info_configuration:
-  # Site specific path and server configuration options - (REFERENCING DEVELOPMENT RESOURCES)
-  #
-  CONFIG_SUPPORT_TOKEN: CONFIG_SUPPORT_TOKEN_ENV
-  #
-  # Database server connection details
-  #
-  MONGO_DB_HOST: localhost
-  MONGO_DB_PORT: "27017"
-  _MONGO_DB_USER_NAME: ""
-  _MONGO_DB_PASSWORD: ""
-  MYSQL_DB_HOST_NAME: localhost
-  MYSQL_DB_PORT_NUMBER: "3306"
-  _MYSQL_DB_USER_NAME: wrIzBGtCsQmkjc7tbEPQ3oEaOnpvivXaKcQsvXD6kn4KHMvA7LCL4O9GlAI=
-  _MYSQL_DB_PASSWORD: qXPp32Z6DhNVMwo9fQIK5+KB13c1Jd43E3Bn6LmJcSyXc0NAt4H/hwo/xglYpmELV5Vqaw==
-  _MYSQL_DB_PASSWORD_ALT: s6mNxq3FIwZLrLiIeHpDZQcuVxfQqrR3gA+dEMOGgHwsjrJV5da08H74RmnNRus74Q==
-  MYSQL_DB_DATABASE_NAME: mysql
-  CRATE_DB_HOST: localhost
-  CRATE_DB_PORT: "4200"
-  COCKROACH_DB_HOST: localhost
-  COCKROACH_DB_PORT: "26257"
-  COCKROACH_DB_NAME: system
-  _COCKROACH_DB_USER_NAME: HR2ez8iLbEpvN+hXKIQS3qa6/QpiFRpf/WvrfHiwfjcL09E+iWTQJhsxTsw=
-  #
-  # Primary repository data and related computed repository data paths
-  #
-  BIRD_REPO_PATH: MOCK_BIRD_REPO
-  BIRD_FAMILY_REPO_PATH: MOCK_BIRD_FAMILY_REPO
-  BIRD_CHEM_COMP_REPO_PATH: MOCK_BIRD_CC_REPO
-  CHEM_COMP_REPO_PATH: MOCK_CHEM_COMP_REPO
-  PDBX_REPO_PATH: MOCK_PDBX_SANDBOX
-  RCSB_EXCHANGE_SANDBOX_PATH: MOCK_EXCHANGE_SANDBOX
-  IHM_DEV_REPO_PATH: MOCK_IHM_REPO
-  VRPT_REPO_PATH: MOCK_VALIDATION_REPORTS
-  VRPT_REPO_PATH_ENV: VRPT_REPO_PATH_ALT
-  #
-  RCSB_EDMAP_LIST_PATH: MOCK_EXCHANGE_SANDBOX/status/edmaps.json
-  #
-  RCSB_SEQUENCE_CLUSTER_DATA_PATH: cluster_data/mmseqs_clusters_current
-  SIFTS_SUMMARY_DATA_PATH: sifts-summary
-  # -------------------------------------------------------------------------------------------
-  #   -- Below are common across current deployments -
-  #
-  # Supporting and integrated resource data cache directory names
-  #
-  #DRUGBANK_CACHE_DIR: DrugBank
-  _DRUGBANK_AUTH_USERNAME: 0qrpNd4OhGuVsJqEpcsAVEovZ0hl6QkgxmbTy3bPssd06Z9tuM6bJqgsWwmFCd0JnjIMIEWyKPMmF1pI5g==
-  _DRUGBANK_AUTH_PASSWORD: lA/K132i8DOtLdMHfm3gpNqprZ6ABKjsCRxfcXIMnxpKQzBv/B6dmC7x1vRO86JhqdT0b84=
-  DRUGBANK_MOCK_URL_TARGET: DrugBank/full_database.zip
-  #
-  #ATC_CACHE_DIR: atc
-  #CHEM_COMP_CACHE_DIR: chem_comp
-  NCBI_TAXONOMY_CACHE_DIR: NCBI
-  ENZYME_CLASSIFICATION_CACHE_DIR: ec
-  STRUCT_DOMAIN_CLASSIFICATION_CACHE_DIR: domains_struct
-  SIFTS_SUMMARY_CACHE_DIR: sifts_summary
-  DICTIONARY_CACHE_DIR: dictionaries
-  DATA_TYPE_INFO_CACHE_DIR: data_type_and_coverage
-  REPO_UTIL_CACHE_DIR: repo_util
-  EXDB_CACHE_DIR: exdb
-  CITATION_REFERENCE_CACHE_DIR: cit_ref
-  #
-  #
-  PROVENANCE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/provenance/rcsb_extend_provenance_info.json
-  PROVENANCE_INFO_CACHE_DIR: provenance
-  #
-  SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/schema_definitions
-  SCHEMA_DEFINITION_CACHE_DIR: schema_definitions
-  JSON_SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/json_schema_definitions
-  JSON_SCHEMA_DEFINITION_CACHE_DIR: json_schema_definitions
-  #
-  # Helper class binding and mappings
-  #
-  DICT_METHOD_HELPER_MODULE_PATH_MAP:
-    rcsb.utils.dictionary.DictMethodEntryHelper: rcsb.utils.dictionary.DictMethodEntryHelper
-    rcsb.utils.dictionary.DictMethodChemRefHelper: rcsb.utils.dictionary.DictMethodChemRefHelper
-    rcsb.utils.dictionary.DictMethodEntityHelper: rcsb.utils.dictionary.DictMethodEntityHelper
-    rcsb.utils.dictionary.DictMethodAssemblyHelper: rcsb.utils.dictionary.DictMethodAssemblyHelper
-    rcsb.utils.dictionary.DictMethodEntityInstanceHelper: rcsb.utils.dictionary.DictMethodEntityInstanceHelper
-  # ------ ------ ------ ------ ------ ------ ------ -------
-  # ADDED rcsb.db V0.966 Source dictionary locators -
-  #
-  PDBX_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/mmcif_pdbx_v5_next.dic
-  RCSB_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/dist/rcsb_mmcif_ext.dic
-  IHMDEV_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/ihm-extension.dic
-  FLR_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/flr-extension.dic
-  VRPT_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_mmcif_ext.dic
-  VRPT_DICT_MAPPING_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_dictmap.json
-  # ------ ------ ------ ------ ------ ------ ------ ------ ------
-  # Added in rcsb.db V0.966 - Data type details and type mapping
-  APP_DATA_TYPE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage/app_data_type_mapping.cif
-  INSTANCE_DATA_TYPE_INFO_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage
-  #
-  CONTENT_DEF_HELPER_MODULE: rcsb.db.helpers.ContentDefinitionHelper
-  DOCUMENT_DEF_HELPER_MODULE: rcsb.db.helpers.DocumentDefinitionHelper
-  CONFIG_APPEND_LOCATOR_PATHS:
-    - https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/config/exdb-config-schema.yml
-# ------ ------ ------ ------ ------ ------ ------ ------ ------
-#  Added V1.001 for stash storage server
-#  -- This is a placeholder configuration to support remote testing --
-#  local|server
-  STASH_MODE: local
-  STASH_LOCAL_BASE_PATH: stash-storage
-  #
-  STASH_SERVER_URL: https://raw.githubusercontent.com
-  STASH_SERVER_FALLBACK_URL: https://raw.githubusercontent.com
-  _STASH_SERVER_BASE_PATH: bIo7kGc2w6Oel0QNr7Pc/4bFfDQayhPxddnGHynP6yudxc44QYuAFoTFdOqY2ZzsM2DEk56r26MfG66bEQ42lp38guy837xwzN1Vgu+r9zvAm11HXEA=
-  REFERENCE_SEQUENCE_ALIGNMETS: PDB
-##
-```
```

### Comparing `rcsb.db-1.717/README.md` & `rcsb.db-1.718/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -60,16 +60,27 @@
 Follow the instructions provided by at the [HomeBrew](https://brew.sh/) site to
 install this system.   Once HomeBrew is installed, you can further install the
 [MariaDB](https://mariadb.com/kb/en/library/installing-mariadb-on-macos-using-homebrew/) and
 [MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/) packages which
 are required to support the ExDB  tools.  HomeBrew also provides a variety of options for
 managing a [Python virtual environments](https://gist.github.com/Geoyi/f55ed54d24cc9ff1c14bd95fac21c042).
 
+### Configuration File
+
+RCSB/PDB repository path details are stored as configuration options.
+An example configuration file included in this package is viewable under `rcsb/db/config`: [exdb-config-example.yml](https://github.com/rcsb/py-rcsb_db/blob/master/rcsb/db/config/exdb-config-example.yml). This example references dictionary resources and mock repository data
+provided in the package in `rcsb/mock-data/*`. The `site_info_configuration` section
+in this file provides database server connection details and common path details.
+This is followed by sections specifying the dictionaries, helper functions, and
+configuration used to define the schema for the each supported content type
+(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
+
 ### Command Line Interfaces
 
+#### Schema File Generation
 A convenience CLI `schema_update_cli` is provided for generating operational schema from
 PDBx/mmCIF dictionary metadata.  Schema are encoded for the ExDB  API (rcsb), and
 for the document schema encoded in JSON and BSON formats.  The latter schema can be used to
 validate the loadable document objects produced for the collections served by MongoDB.
 
 ```bash
  => schema_update_cli  --help
@@ -138,129 +149,205 @@
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for dependencies and
                         testing
 ________________________________________________________________________________
 
 ```
 
+##### Example Usage
+
 For example, the following command will generate the JSON and BSON schema for the collections in the
 pdbx_core schema.
 
 ```bash
 schema_update_cli  --mock --schema_types json,bson \
                    --schema_level full  \
                    --update_pdbx_core   \
                    --cache_path . \
                    --config_path ./rcsb/db/config/exdb-config-example.yml  \
                    --config_name site_info_configuration
 ```
 
+#### ExDB Loading
+
 A convenience CLI `exdb_repo_load_cli` is provided to support loading PDB repositories
 containing entry and chemical reference data content types in the form of document collections
 compatible with MongoDB.
 
 ```bash
 exdb_repo_load_cli --help
 
-usage: exdb_repo_load_cli [-h] [--full] [--replace] [--load_chem_comp_ref]
-                          [--load_chem_comp_core_ref]
-                          [--load_bird_chem_comp_ref]
-                          [--load_bird_chem_comp_core_ref] [--load_bird_ref]
-                          [--load_bird_family_ref] [--load_entry_data]
-                          [--load_pdbx_core] [--load_pdbx_core_merge]
-                          [--load_pdbx_core_entry] [--load_pdbx_core_entity]
-                          [--load_pdbx_core_entity_monomer]
-                          [--load_pdbx_core_assembly] [--load_ihm_dev]
+usage: exdb_repo_load_cli [-h] [--op OP_TYPE] [--load_type LOAD_TYPE]
+                          [--database DATABASE_NAME]
                           [--config_path CONFIG_PATH]
                           [--config_name CONFIG_NAME] [--db_type DB_TYPE]
+                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--document_style DOCUMENT_STYLE]
-                          [--read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--disable_read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--load_id_list_path LOAD_ID_LIST_PATH]
                           [--load_file_list_path LOAD_FILE_LIST_PATH]
                           [--fail_file_list_path FAIL_FILE_LIST_PATH]
                           [--save_file_list_path SAVE_FILE_LIST_PATH]
-                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--file_limit FILE_LIMIT]
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --full                Fresh full load in a new tables/collections
-  --replace             Load with replacement in an existing table/collection
-                        (default)
-  --load_chem_comp_ref  Load Chemical Component reference definitions (public
-                        subset)
-  --load_chem_comp_core_ref
-                        Load Chemical Component Core reference definitions
-                        (public subset)
-  --load_bird_chem_comp_ref
-                        Load Bird Chemical Component reference definitions
-                        (public subset)
-  --load_bird_chem_comp_core_ref
-                        Load Bird Chemical Component Core reference
-                        definitions (public subset)
-  --load_bird_ref       Load Bird reference definitions (public subset)
-  --load_bird_family_ref
-                        Load Bird Family reference definitions (public subset)
-  --load_entry_data     Load PDBx entry data (current released subset)
-  --load_pdbx_core      Load all PDBx core collections (current released
-                        subset)
-  --load_pdbx_core_merge
-                        Load all PDBx core collections with merged content
-                        (current released subset)
-  --load_pdbx_core_entry
-                        Load PDBx core entry (current released subset)
-  --load_pdbx_core_entity
-                        Load PDBx core entity (current released subset)
-  --load_pdbx_core_entity_monomer
-                        Load PDBx core entity monomer (current released
-                        subset)
-  --load_pdbx_core_assembly
-                        Load PDBx core assembly (current released subset)
-  --load_ihm_dev        Load I/HM DEV model data (current released subset)
+  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+                        Loading operation to perform
+  --load_type {replace,full}
+                        Type of load ('replace' for incremental and
+                        multi-worker load, 'full' for complete and
+                        fresh single-worker load)
+  --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
+                        Database to load (most common choices are:
+                        'pdbx_core', 'pdbx_comp_model_core', or
+                        'bird_chem_comp_core')
   --config_path CONFIG_PATH
                         Path to configuration options file
   --config_name CONFIG_NAME
                         Configuration section name
-  --db_type DB_TYPE     Database server type (default=mongo)
   --document_style DOCUMENT_STYLE
-                        Document organization (rowwise_by_name_with_cardinalit
-                        y|rowwise_by_name|columnwise_by_name|rowwise_by_id|row
-                        wise_no_name
-  --read_back_check     Perform read back check on all documents
+                        Document organization (rowwise_by_name_with_c
+                        ardinality|rowwise_by_name|columnwise_by_name
+                        |rowwise_by_id|rowwise_no_name)
+  --cache_path CACHE_PATH
+                        Cache path for resource files
+  --num_proc NUM_PROC   Number of processes to execute (default=2)
+  --chunk_size CHUNK_SIZE
+                        Number of files loaded per process
+  --max_step_length MAX_STEP_LENGTH
+                        Maximum subList size (default=500)
   --schema_level SCHEMA_LEVEL
-                        Schema validation level (full|min default=None)
+                        Schema validation level (full|min)
+  --collection_list COLLECTION_LIST
+                        Specific collections to load
+  --load_id_list_path LOAD_ID_LIST_PATH
+                        Input file containing the list of IDs to load
+                        in the current iteration by a single worker
+  --holdings_file_path HOLDINGS_FILE_PATH
+                        File containing the complete list of all IDs
+                        (or holdings files) that will be loaded
   --load_file_list_path LOAD_FILE_LIST_PATH
-                        Input file containing load file path list (override
-                        automatic repository scan)
+                        Input file containing load file path list
+                        (override automatic repository scan)
   --fail_file_list_path FAIL_FILE_LIST_PATH
-                        Output file containing file paths that fail to load
+                        Output file containing file paths that fail
+                        to load
   --save_file_list_path SAVE_FILE_LIST_PATH
-                        Save repo file paths from automatic file system scan
-                        in this path
-  --num_proc NUM_PROC   Number of processes to execute (default=2)
-  --chunk_size CHUNK_SIZE
-                        Number of files loaded per process
+                        Save repo file paths from automatic file
+                        system scan in this path
+  --load_file_list_dir LOAD_FILE_LIST_DIR
+                        Directory path for storing load file lists
+  --num_sublists NUM_SUBLISTS
+                        Number of sublists to create/load for the
+                        associated database
+  --force_reload        Force re-load of provided ID list (i.e.,
+                        don't just load delta; useful for manual/test
+                        runs).
+  --provider_type_exclude PROVIDER_TYPE_EXCLUDE
+                        Resource provider types to exclude
+  --db_type DB_TYPE     Database server type (default=mongo)
   --file_limit FILE_LIMIT
                         Load file limit for testing
   --prune_document_size PRUNE_DOCUMENT_SIZE
                         Prune large documents to this size limit (MB)
+  --regex_purge         Perform additional regex-based purge of all
+                        pre-existing documents for loadType != 'full'
+  --data_selectors  [ ...]
+                        Data selectors, space-separated.
+  --disable_read_back_check
+                        Disable read back check on all documents
+  --disable_merge_validation_reports
+                        Disable merging of validation report data
+                        with the primary content type
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for testing
-  --cache_path CACHE_PATH
-                        Cache path for resource files
   --rebuild_cache       Rebuild cached resource files
   --rebuild_schema      Rebuild schema on-the-fly if not cached
   --vrpt_repo_path VRPT_REPO_PATH
                         Path to validation report repository
 ________________________________________________________________________________
 ```
 
+##### Example Usage
+The following commands demonstrate how each type of operation (`--op`) is used for loading of PDB repository data to ExDB. For all commands, the following environmental variables must first be set:
+
+```bash
+export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
+export OE_LICENSE=/path/to/oe_license.txt
+export NLTK_DATA=/path/to/nltk_data
+```
+
+`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+```bash
+exdb_repo_load_cli --op "build-resource-cache" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--num_proc 6  \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+```bash
+exdb_repo_load_cli --op "pdbx-db-wiper" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+```bash
+exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+```bash
+exdb_repo_load_cli --op "pdbx-loader" \
+--database "pdbx_core" \
+--load_type replace  \
+--config_path /opt/etl-scratch/config/exdb-loader-config.yml \
+--config_name site_info_remote_configuration \
+--num_proc 8  \
+--chunk_size 5  \
+--max_step_length 500 \
+--load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+```bash
+exdb_repo_load_cli --op "pdbx-loader-check" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+#### Repository Scanning
+
 Part of the schema definition process supported by this module involves refining
 the dictionary metadata with more specific data typing and coverage details.
 A scanning tools is provided to collect and organize these details for the
 other ETL tools in this package.  The following convenience CLI, `repo_scan_cli`,
 is provided to scan supported PDB repository content and update data type and coverage details.
 
 ```bash
@@ -323,14 +410,15 @@
   --mock                Use MOCK repository configuration for testing
   --working_path WORKING_PATH
                         Working path for temporary files
 ________________________________________________________________________________
 
 ```
 
+#### ETL Processing
 The following CLI provides a preliminary access to ETL functions for processing
 derived content types such as sequence comparative data.
 
 ```bash
 etl_exec_cli --help
 usage: etl_exec_cli [-h] [--full] [--etl_entity_sequence_clusters]
                     [--etl_repository_holdings] [--data_set_id DATA_SET_ID]
@@ -377,170 +465,48 @@
   --cache_path CACHE_PATH
                         Path containing cache directories
   --rebuild_cache       Rebuild cached resource files
 ________________________________________________________________________________
 
 ```
 
-### Examples
+### Additional Examples
+
+(*Note: The examples below are outdated and may not function as described. They are only kept here for historical reference.*)
 
 If you are working in the source repository, then you can run the CLI commands in the following manner.
 The following examples load data in the mock repositories in source distribution assuming you have a local
 default installation of MongoDb (no user/pw assigned).
 
 To run the command-line interface `exdb_repo_load_cli` outside of the source distribution, you will need to
 create a configuration file with the appropriate path details and authentication credentials.
 
 For instance, to perform a fresh/full load of all of the chemical component definitions in the mock repository:
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py --full  --load_chem_comp_ref  \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --fail_file_list_path failed-cc-path-list.txt \
                       --read_back_check
 ```
 
 The following illustrates, a full load of the mock structure data repository followed by a reload with replacement of
 this same data.
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py  --mock --full  --load_entry_data \
                      --config_path ../config/exdb-config-example.yml \
                      --config_name site_info_configuration \
                      --save_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                      --fail_file_list_path failed-entry-path-list.txt
 
 python RepoLoadExec.py --mock --replace  --load_entry_data \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --load_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                       --fail_file_list_path failed-entry-path-list.txt
 ```
-
-### Configuration Example
-
-RCSB/PDB repository path details are stored as configuration options.
-An example configuration file included in this package is shown below.
-This example is references dictionary resources and mock repository data
-provided in the package in `rcsb/mock-data/*`. Example configuration details are
-stored in rcsb/db/config/exdb-config-example.yml.The `site_info_configuration` section
-in this file provides database server connection details and common path details.
-This is followed by sections specifying the dictionaries, helper functions, and
-configuration used to define the schema for the each supported content type
-(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
-
-```yaml
-site_info_configuration:
-  # Site specific path and server configuration options - (REFERENCING DEVELOPMENT RESOURCES)
-  #
-  CONFIG_SUPPORT_TOKEN: CONFIG_SUPPORT_TOKEN_ENV
-  #
-  # Database server connection details
-  #
-  MONGO_DB_HOST: localhost
-  MONGO_DB_PORT: "27017"
-  _MONGO_DB_USER_NAME: ""
-  _MONGO_DB_PASSWORD: ""
-  MYSQL_DB_HOST_NAME: localhost
-  MYSQL_DB_PORT_NUMBER: "3306"
-  _MYSQL_DB_USER_NAME: wrIzBGtCsQmkjc7tbEPQ3oEaOnpvivXaKcQsvXD6kn4KHMvA7LCL4O9GlAI=
-  _MYSQL_DB_PASSWORD: qXPp32Z6DhNVMwo9fQIK5+KB13c1Jd43E3Bn6LmJcSyXc0NAt4H/hwo/xglYpmELV5Vqaw==
-  _MYSQL_DB_PASSWORD_ALT: s6mNxq3FIwZLrLiIeHpDZQcuVxfQqrR3gA+dEMOGgHwsjrJV5da08H74RmnNRus74Q==
-  MYSQL_DB_DATABASE_NAME: mysql
-  CRATE_DB_HOST: localhost
-  CRATE_DB_PORT: "4200"
-  COCKROACH_DB_HOST: localhost
-  COCKROACH_DB_PORT: "26257"
-  COCKROACH_DB_NAME: system
-  _COCKROACH_DB_USER_NAME: HR2ez8iLbEpvN+hXKIQS3qa6/QpiFRpf/WvrfHiwfjcL09E+iWTQJhsxTsw=
-  #
-  # Primary repository data and related computed repository data paths
-  #
-  BIRD_REPO_PATH: MOCK_BIRD_REPO
-  BIRD_FAMILY_REPO_PATH: MOCK_BIRD_FAMILY_REPO
-  BIRD_CHEM_COMP_REPO_PATH: MOCK_BIRD_CC_REPO
-  CHEM_COMP_REPO_PATH: MOCK_CHEM_COMP_REPO
-  PDBX_REPO_PATH: MOCK_PDBX_SANDBOX
-  RCSB_EXCHANGE_SANDBOX_PATH: MOCK_EXCHANGE_SANDBOX
-  IHM_DEV_REPO_PATH: MOCK_IHM_REPO
-  VRPT_REPO_PATH: MOCK_VALIDATION_REPORTS
-  VRPT_REPO_PATH_ENV: VRPT_REPO_PATH_ALT
-  #
-  RCSB_EDMAP_LIST_PATH: MOCK_EXCHANGE_SANDBOX/status/edmaps.json
-  #
-  RCSB_SEQUENCE_CLUSTER_DATA_PATH: cluster_data/mmseqs_clusters_current
-  SIFTS_SUMMARY_DATA_PATH: sifts-summary
-  # -------------------------------------------------------------------------------------------
-  #   -- Below are common across current deployments -
-  #
-  # Supporting and integrated resource data cache directory names
-  #
-  #DRUGBANK_CACHE_DIR: DrugBank
-  _DRUGBANK_AUTH_USERNAME: 0qrpNd4OhGuVsJqEpcsAVEovZ0hl6QkgxmbTy3bPssd06Z9tuM6bJqgsWwmFCd0JnjIMIEWyKPMmF1pI5g==
-  _DRUGBANK_AUTH_PASSWORD: lA/K132i8DOtLdMHfm3gpNqprZ6ABKjsCRxfcXIMnxpKQzBv/B6dmC7x1vRO86JhqdT0b84=
-  DRUGBANK_MOCK_URL_TARGET: DrugBank/full_database.zip
-  #
-  #ATC_CACHE_DIR: atc
-  #CHEM_COMP_CACHE_DIR: chem_comp
-  NCBI_TAXONOMY_CACHE_DIR: NCBI
-  ENZYME_CLASSIFICATION_CACHE_DIR: ec
-  STRUCT_DOMAIN_CLASSIFICATION_CACHE_DIR: domains_struct
-  SIFTS_SUMMARY_CACHE_DIR: sifts_summary
-  DICTIONARY_CACHE_DIR: dictionaries
-  DATA_TYPE_INFO_CACHE_DIR: data_type_and_coverage
-  REPO_UTIL_CACHE_DIR: repo_util
-  EXDB_CACHE_DIR: exdb
-  CITATION_REFERENCE_CACHE_DIR: cit_ref
-  #
-  #
-  PROVENANCE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/provenance/rcsb_extend_provenance_info.json
-  PROVENANCE_INFO_CACHE_DIR: provenance
-  #
-  SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/schema_definitions
-  SCHEMA_DEFINITION_CACHE_DIR: schema_definitions
-  JSON_SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/json_schema_definitions
-  JSON_SCHEMA_DEFINITION_CACHE_DIR: json_schema_definitions
-  #
-  # Helper class binding and mappings
-  #
-  DICT_METHOD_HELPER_MODULE_PATH_MAP:
-    rcsb.utils.dictionary.DictMethodEntryHelper: rcsb.utils.dictionary.DictMethodEntryHelper
-    rcsb.utils.dictionary.DictMethodChemRefHelper: rcsb.utils.dictionary.DictMethodChemRefHelper
-    rcsb.utils.dictionary.DictMethodEntityHelper: rcsb.utils.dictionary.DictMethodEntityHelper
-    rcsb.utils.dictionary.DictMethodAssemblyHelper: rcsb.utils.dictionary.DictMethodAssemblyHelper
-    rcsb.utils.dictionary.DictMethodEntityInstanceHelper: rcsb.utils.dictionary.DictMethodEntityInstanceHelper
-  # ------ ------ ------ ------ ------ ------ ------ -------
-  # ADDED rcsb.db V0.966 Source dictionary locators -
-  #
-  PDBX_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/mmcif_pdbx_v5_next.dic
-  RCSB_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/dist/rcsb_mmcif_ext.dic
-  IHMDEV_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/ihm-extension.dic
-  FLR_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/flr-extension.dic
-  VRPT_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_mmcif_ext.dic
-  VRPT_DICT_MAPPING_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_dictmap.json
-  # ------ ------ ------ ------ ------ ------ ------ ------ ------
-  # Added in rcsb.db V0.966 - Data type details and type mapping
-  APP_DATA_TYPE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage/app_data_type_mapping.cif
-  INSTANCE_DATA_TYPE_INFO_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage
-  #
-  CONTENT_DEF_HELPER_MODULE: rcsb.db.helpers.ContentDefinitionHelper
-  DOCUMENT_DEF_HELPER_MODULE: rcsb.db.helpers.DocumentDefinitionHelper
-  CONFIG_APPEND_LOCATOR_PATHS:
-    - https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/config/exdb-config-schema.yml
-# ------ ------ ------ ------ ------ ------ ------ ------ ------
-#  Added V1.001 for stash storage server
-#  -- This is a placeholder configuration to support remote testing --
-#  local|server
-  STASH_MODE: local
-  STASH_LOCAL_BASE_PATH: stash-storage
-  #
-  STASH_SERVER_URL: https://raw.githubusercontent.com
-  STASH_SERVER_FALLBACK_URL: https://raw.githubusercontent.com
-  _STASH_SERVER_BASE_PATH: bIo7kGc2w6Oel0QNr7Pc/4bFfDQayhPxddnGHynP6yudxc44QYuAFoTFdOqY2ZzsM2DEk56r26MfG66bEQ42lp38guy837xwzN1Vgu+r9zvAm11HXEA=
-  REFERENCE_SEQUENCE_ALIGNMETS: PDB
-##
-```
```

### Comparing `rcsb.db-1.717/rcsb/db/cli/ETLExec.py` & `rcsb.db-1.718/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb.db-1.718/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,98 @@
 ##
-# File: RepoHoldingsEtlWorker.py
+# File: SequenceClustersEtlWorker.py
 # Date: 2-Jul-2018  jdw
 #
-# ETL utilities for processing repository holding data.
+# ETL utilities for sequence cluster data
+#
 # Updates:
 #  15-Jul-2018 jdw split out to separate module and add status tracking
-#  26-Nov-2018 jdw add COLLECTION_HOLDINGS_PRERELEASE
-#  14-Dec-2019 jdw reorganize and consolidate repository_holdings collections
-#  25-Sep-2021 jdw substitute RepoHoldingsRemoteDataPrep() for data processing
+#  28-Oct-2018 jdw adjustments for new configuration organization
+#   4-Jan-2019 jdw differentiate site and application config sections for provenance.
+#   1-Jun-2022 dwp Add clusterFileNameTemplate input argument
+#   4-Apr-2023 dwp Add maxStepLength input argument (the larger the length, the faster the load)
 #
 ##
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
-import os
 
 from rcsb.db.mongo.DocumentLoader import DocumentLoader
+from rcsb.db.processors.ClusterDataPrep import ClusterDataPrep
 from rcsb.db.processors.DataExchangeStatus import DataExchangeStatus
-from rcsb.db.processors.RepoHoldingsDataPrep import RepoHoldingsDataPrep
-from rcsb.db.processors.RepoHoldingsRemoteDataPrep import RepoHoldingsRemoteDataPrep
+from rcsb.db.utils.ProvenanceProvider import ProvenanceProvider
 
 logger = logging.getLogger(__name__)
 
 
-class RepoHoldingsEtlWorker(object):
-    """Prepare and load repository holdings and repository update data."""
+class SequenceClustersEtlWorker(object):
+    """Prepare and load sequence cluster data.
+
+     Note: relevant configuration options -
+
+    site_info:
+     'RCSB_SEQUENCE_CLUSTER_DATA_PATH': ...
+
+    entity_sequence_clusters:
+     DATABASE_NAME: sequence_clusters
+     DATABASE_VERSION_STRING: v5
+     COLLECTION_ENTITY_MEMBERS: entity_members
+     COLLECTION_ENTITY_MEMBERS_INDEX: data_set_id,entry_id,entity_id
+     COLLECTION_CLUSTER_MEMBERS: cluster_members
+     COLLECTION_CLUSTER_MEMBERS_INDEX: data_set_id,identity,cluster_id
+     COLLECTION_VERSION_STRING: v0_1
+     ENTITY_SCHEMA_NAME: rcsb_entity_sequence_cluster_entity_list
+     CLUSTER_SCHEMA_NAME: rcsb_entity_sequence_cluster_identifer_list
+     SEQUENCE_IDENTITY_LEVELS: 100,95,90,70,50,30
+     COLLECTION_CLUSTER_PROVENANCE: cluster_provenance
+     PROVENANCE_KEY_NAME: rcsb_entity_sequence_cluster_prov
+     PROVENANCE_INFO_LOCATOR: provenance/rcsb_extend_provenance_info.json
+
+
+    """
 
-    def __init__(self, cfgOb, sandboxPath, cachePath, numProc=2, chunkSize=10, readBackCheck=False, documentLimit=None, verbose=False):
+    def __init__(self, cfgOb, workPath=None, numProc=2, chunkSize=100, maxStepLength=40000, readBackCheck=False, documentLimit=None, verbose=False, clusterFileNameTemplate=None):
         self.__cfgOb = cfgOb
-        self.__cfgSectionName = self.__cfgOb.getDefaultSectionName()
-        self.__sandboxPath = sandboxPath
-        self.__cachePath = cachePath
+        self.__cachePath = workPath
         self.__readBackCheck = readBackCheck
         self.__numProc = numProc
         self.__chunkSize = chunkSize
+        self.__maxStepLength = maxStepLength
         self.__documentLimit = documentLimit
         self.__resourceName = "MONGO_DB"
-        self.__filterType = "assign-dates"
         self.__verbose = verbose
+        self.__clusterFileNameTemplate = clusterFileNameTemplate
+        #
+        self.__sectionCluster = "entity_sequence_clusters_configuration"
+        self.__clusterDataPath = self.__cfgOb.getPath("RCSB_SEQUENCE_CLUSTER_DATA_PATH", sectionName=self.__cfgOb.getDefaultSectionName())
+        self.__databaseName = self.__cfgOb.get("DATABASE_NAME", sectionName=self.__sectionCluster, default="sequence_clusters")
+        self.__databaseVersion = self.__cfgOb.get("DATABASE_VERSION_STRING", sectionName=self.__sectionCluster, default="v5")
+        #
+        self.__entityMemberCollection = self.__cfgOb.get("COLLECTION_ENTITY_MEMBERS", sectionName=self.__sectionCluster, default="entity_members")
+        self.__clusterMembersCollection = self.__cfgOb.get("COLLECTION_CLUSTER_MEMBERS", sectionName=self.__sectionCluster, default="cluster_members")
+        self.__clusterProvenanceCollection = self.__cfgOb.get("COLLECTION_CLUSTER_PROVENANCE", sectionName=self.__sectionCluster, default="cluster_provenance")
+        # self.__collectionVersion = self.__cfgOb.get("COLLECTION_VERSION_STRING", sectionName=self.__sectionCluster, default="v0_1")
+        #
+        self.__entitySchemaName = self.__cfgOb.get("ENTITY_SCHEMA_NAME", sectionName=self.__sectionCluster, default="rcsb_entity_sequence_cluster_entity_list")
+        self.__clusterSchemaName = self.__cfgOb.get("CLUSTER_SCHEMA_NAME", sectionName=self.__sectionCluster, default="rcsb_entity_sequence_cluster_identifer_list")
+        #
+        tS = self.__cfgOb.get("COLLECTION_ENTITY_MEMBERS_INDEX", sectionName=self.__sectionCluster, default=None)
+        self.__entityMemberCollectionIndexL = tS.split(",") if tS else None
+        tS = self.__cfgOb.get("COLLECTION_CLUSTER_MEMBERS_INDEX", sectionName=self.__sectionCluster, default=None)
+        self.__clusterMembersCollectionIndexL = tS.split(",") if tS else None
+        # sample data set
+        #
+        tS = self.__cfgOb.get("SEQUENCE_IDENTITY_LEVELS", sectionName=self.__sectionCluster, default=None)
+        self.__identityLevels = tS.split(",") if tS else ["100", "95", "90", "70", "50", "30"]
+        #
         self.__statusList = []
+        #
 
     def __updateStatus(self, updateId, databaseName, collectionName, status, startTimestamp):
         try:
             sFlag = "Y" if status else "N"
             desp = DataExchangeStatus()
             desp.setStartTime(tS=startTimestamp)
             desp.setObject(databaseName, collectionName)
@@ -53,99 +100,85 @@
             desp.setEndTime()
             self.__statusList.append(desp.getStatus())
             return True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
-    def load(self, updateId, loadType="full"):
-        """Load legacy repository holdings and status data -
-
-        Relevant configuration options:
+    def __extract(self, dataSetId, dataLocator, levels):
+        """Extract sequence cluster data set  (mmseq2 or blastclust organization)"""
+        try:
+            cdp = ClusterDataPrep(
+                workPath=self.__cachePath,
+                entitySchemaName=self.__entitySchemaName,
+                clusterSchemaName=self.__clusterSchemaName,
+                clusterFileNameTemplate=self.__clusterFileNameTemplate,
+            )
+            _, docBySequenceD, docByClusterD = cdp.extract(dataSetId, clusterSetLocator=dataLocator, levels=levels, clusterType="entity")
+            return docBySequenceD, docByClusterD
+        except Exception as e:
+            logger.exception("Failing with %s", str(e))
 
-        [DEFAULT]
-        RCSB_EXCHANGE_SANDBOX_PATH=MOCK_EXCHANGE_SANDBOX
+        return {}, {}
 
-        [repository_holdings_configuration]
-        DATABASE_NAME=repository_holdings
-        DATABASE_VERSION_STRING=v5
-        COLLECTION_HOLDINGS_UPDATE=rcsb_repository_holdings_update_entry
-        COLLECTION_HOLDINGS_CURRENT=rcsb_repository_holdings_current_entry
-        COLLECTION_HOLDINGS_UNRELEASED=rcsb_repository_holdings_unreleased_entry
-        COLLECTION_HOLDINGS_REMOVED=rcsb_repository_holdings_removed_entry
-        COLLECTION_VERSION_STRING=v0_1
+    def __fetchProvenance(self):
+        """Fetching a provenance dictionary content."""
+        try:
+            provKeyName = self.__cfgOb.get("PROVENANCE_KEY_NAME", sectionName=self.__sectionCluster, default="rcsb_entity_sequence_cluster_prov")
+            provU = ProvenanceProvider(self.__cfgOb, self.__cachePath, useCache=True)
+            pD = provU.fetch()
+            return pD[provKeyName] if provKeyName in pD else {}
+        except Exception as e:
+            logger.exception("Failing with %s", str(e))
+        return {}
 
-        """
+    def etl(self, dataSetId, dataLocator=None, loadType="full"):
+        """Prepare and load sequence cluster data by entity and by cluster identifer."""
         try:
             self.__statusList = []
             desp = DataExchangeStatus()
             statusStartTimestamp = desp.setStartTime()
-
-            discoveryMode = self.__cfgOb.get("DISCOVERY_MODE", sectionName=self.__cfgSectionName, default="local")
-            # ---
-            baseUrlPDB = self.__cfgOb.getPath("PDB_REPO_URL", sectionName=self.__cfgSectionName, default="https://files.wwpdb.org/pub")
-            fallbackUrlPDB = self.__cfgOb.getPath("PDB_REPO_FALLBACK_URL", sectionName=self.__cfgSectionName, default="https://files.wwpdb.org/pub")
-            edMapUrl = self.__cfgOb.getPath("RCSB_EDMAP_LIST_PATH", sectionName=self.__cfgSectionName, default=None)
-            #
-            kwD = {
-                "holdingsTargetUrl": os.path.join(baseUrlPDB, "pdb", "holdings"),
-                "holdingsFallbackUrl": os.path.join(fallbackUrlPDB, "pdb", "holdings"),
-                "edmapsLocator": edMapUrl,
-                "updateTargetUrl": os.path.join(baseUrlPDB, "pdb", "data", "status", "latest"),
-                "updateFallbackUrl": os.path.join(fallbackUrlPDB, "pdb", "data", "status", "latest"),
-                "filterType": self.__filterType,
-            }
-            # ---
-            if discoveryMode == "local":
-                rhdp = RepoHoldingsDataPrep(cfgOb=self.__cfgOb, sandboxPath=self.__sandboxPath, cachePath=self.__cachePath, filterType=self.__filterType)
-            else:
-                rhdp = RepoHoldingsRemoteDataPrep(cachePath=self.__cachePath, **kwD)
+            #
+            docBySequenceD, docByClusterD = self.__extract(dataSetId=dataSetId, dataLocator=dataLocator, levels=self.__identityLevels)
             #
             dl = DocumentLoader(
                 self.__cfgOb,
                 self.__cachePath,
                 self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
+                maxStepLength=self.__maxStepLength,
                 documentLimit=self.__documentLimit,
                 verbose=self.__verbose,
                 readBackCheck=self.__readBackCheck,
             )
             #
-            sectionName = "repository_holdings_configuration"
-            databaseName = self.__cfgOb.get("DATABASE_NAME", sectionName=sectionName)
-            # collectionVersion = self.__cfgOb.get("COLLECTION_VERSION_STRING", sectionName=sectionName)
-            # addValues = {"_schema_version": collectionVersion}
+            databaseName = self.__databaseName
+            # addValues = {"_schema_version": self.__collectionVersion}
             addValues = None
             #
-            dList = rhdp.getHoldingsUpdateEntry(updateId=updateId)
-            collectionName = self.__cfgOb.get("COLLECTION_HOLDINGS_UPDATE", sectionName=sectionName)
-            ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=["update_id", "entry_id"], keyNames=None, addValues=addValues)
-            self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
-            #
-            dList = rhdp.getHoldingsCurrentEntry(updateId=updateId)
-            collectionName = self.__cfgOb.get("COLLECTION_HOLDINGS_CURRENT", sectionName=sectionName)
-            ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=["update_id", "entry_id"], keyNames=None, addValues=addValues)
-            self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
-
-            dList = rhdp.getHoldingsUnreleasedEntry(updateId=updateId)
-            collectionName = self.__cfgOb.get("COLLECTION_HOLDINGS_UNRELEASED", sectionName=sectionName)
-            ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=["update_id", "entry_id"], keyNames=None, addValues=addValues)
-            self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
-            #
-            dList = rhdp.getHoldingsRemovedEntry(updateId=updateId)
-            collectionName = self.__cfgOb.get("COLLECTION_HOLDINGS_REMOVED", sectionName=sectionName)
-            ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=["update_id", "entry_id"], keyNames=None, addValues=addValues)
-            self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
-            #
-            dList = rhdp.getHoldingsCombinedEntry(updateId=updateId)
-            collectionName = self.__cfgOb.get("COLLECTION_HOLDINGS_COMBINED", sectionName=sectionName)
-            ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=["update_id", "entry_id"], keyNames=None, addValues=addValues)
-            self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
+            collectionName = self.__entityMemberCollection
+            dList = docBySequenceD[self.__entitySchemaName]
+            ok1 = dl.load(
+                databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=self.__entityMemberCollectionIndexL, keyNames=None, addValues=addValues
+            )
+            self.__updateStatus(dataSetId, databaseName, collectionName, ok1, statusStartTimestamp)
             #
-            return True
+            collectionName = self.__clusterMembersCollection
+            dList = docByClusterD[self.__clusterSchemaName]
+            ok2 = dl.load(
+                databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=self.__clusterMembersCollectionIndexL, keyNames=None, addValues=addValues
+            )
+            self.__updateStatus(dataSetId, databaseName, collectionName, ok2, statusStartTimestamp)
+            #
+            pD = self.__fetchProvenance()
+            collectionName = self.__clusterProvenanceCollection
+            ok3 = dl.load(databaseName, collectionName, loadType=loadType, documentList=[pD], indexAttributeList=None, keyNames=None, addValues=addValues)
+            self.__updateStatus(dataSetId, databaseName, collectionName, ok3, statusStartTimestamp)
+            #
+            return ok1 and ok2 and ok3
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
     def getLoadStatus(self):
         return self.__statusList
```

### Comparing `rcsb.db-1.717/rcsb/db/cli/RepoScanExec.py` & `rcsb.db-1.718/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb.db-1.718/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb.db-1.718/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb.db-1.718/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/cockroach/Connection.py` & `rcsb.db-1.718/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/crate/Connection.py` & `rcsb.db-1.718/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/crate/CrateDbLoader.py` & `rcsb.db-1.718/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/crate/CrateDbUtil.py` & `rcsb.db-1.718/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/ContentDefinition.py` & `rcsb.db-1.718/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/DataTypeApiProvider.py` & `rcsb.db-1.718/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb.db-1.718/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb.db-1.718/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/SchemaDefAccess.py` & `rcsb.db-1.718/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/define/SchemaDefBuild.py` & `rcsb.db-1.718/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb.db-1.718/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb.db-1.718/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/helpers/r.py` & `rcsb.db-1.718/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mongo/Connection.py` & `rcsb.db-1.718/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mongo/ConnectionBase.py` & `rcsb.db-1.718/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mongo/DocumentLoader.py` & `rcsb.db-1.718/rcsb/db/mongo/DocumentLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
             optionsD["readBackCheck"] = self.__readBackCheck
             optionsD["loadType"] = loadType
             optionsD["keyNames"] = keyNames
             # ---------------- - ---------------- - ---------------- - ---------------- - ---------------- -
             #
             docList = documentList[: self.__documentLimit] if self.__documentLimit else documentList
             logger.debug("Full document list length %d limit %r", len(documentList), self.__documentLimit)
+            logger.info("Loading documents with numProc %r chunkSize %r maxStepLength %r", self.__numProc, self.__chunkSize, self.__maxStepLength)
             numProc = self.__numProc
             chunkSize = self.__chunkSize if docList and self.__chunkSize < len(docList) else 0
             #
             if addValues:
                 try:
                     for doc in docList:
                         for k, v in addValues.items():
```

### Comparing `rcsb.db-1.717/rcsb/db/mongo/MongoDbUtil.py` & `rcsb.db-1.718/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mongo/PdbxLoader.py` & `rcsb.db-1.718/rcsb/db/mongo/PdbxLoader.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 #     22-Feb-2023 dwp  Use case-sensitivity for brute force document purge
 #     26-Apr-2023 dwp  Fix regex document purge, and add regexPurge flag to control running that step (with default set to skip it)
 #      8-May-2023 dwp  Fix error handling in PdbxLoader to cause failure when documents fail to load
 #      7-Nov-2023 dwp  Remove unused redundant PdbxLoaderWorker code (already present in PdbxLoader)
 #     19-Mar-2024 dwp  Add additional quality assurance measure to catch and cleanup pre-loaded documents in which one or more related
 #                      containers fails to be read properly (incl. validation reports);
 #                      Begin adding code to support weekly update workflow CLI requirements
+#     26-Mar-2024 dwp  Add arguments and logic to support CLI usage from weekly-update workflow
 #
 ##
 """
 Worker methods for loading primary data content following mapping conventions in external schema definitions.
 
 """
 
@@ -152,18 +153,20 @@
         regexPurge=False,
         logSize=False,
         validationLevel="min",
         mergeContentTypes=None,
         useNameFlag=True,
         updateSchemaOnReplace=True,
         validateFailures=True,
+        rebuildCache=False,
         reloadPartial=True,
         providerTypeExclude=None,
         restoreUseGit=True,
         restoreUseStash=True,
+        forceReload=False,
     ):
         """Driver method for loading PDBx/mmCIF content into the Mongo document store.
 
         Args:
             databaseName (str): A content datbase schema (e.g. 'bird','bird_family','bird_chem_comp', chem_comp', 'pdbx', 'pdbx_core')
             collectionLoadList (list, optional): list of collection names in this schema to load (default is load all collections)
             loadType (str, optional): mode of loading 'full' (bulk delete then bulk insert) or 'replace'
@@ -177,45 +180,63 @@
             regexPurge (bool, optional): perform an additional regex-based round of purging of all pre-existing documents for loadType != "full" (default False)
             logSize (bool, optional): Compute and log bson serialized object size
             validationLevel (str, optional): Completeness of json/bson metadata schema bound to each collection (e.g. 'min', 'full' or None)
             mergeContentTypes (list, optional): repository content types to combined with the primary content type (e.g., ["vrpt"])
             useNameFlag (bool, optional): Use container name as unique identifier otherwise use UID property.
             updateSchemaOnReplace (bool, optional): Update validation schema for loadType == 'replace'
             validateFailures (bool, optional): output validation report on load failures
+            rebuildCache (bool, optional): whether to force rebuild of all cache resources (default is False, to just check them)
             reloadPartial (bool, optional): on load failures attempt reload of partial objects.
             providerTypeExclude (str, optional): exclude dictionary method provider by type name. Defaults to None.
             restoreUseStash (bool, optional): restore cache resources using stash storage.  Defaults to True.
             restoreUseGit (bool, optional): restore cache resources using git storage.  Defaults to True.
+            forceReload (bool, optional): Force re-load of provided ID list (i.e., don't just load delta; useful for manual/test runs)
         Returns:
             bool: True on success or False otherwise
 
         """
         try:
             #
             self.__statusList = []
             desp = DataExchangeStatus()
             statusStartTimestamp = desp.setStartTime()
             #
             logger.info("Beginning load operation (%r) for database %s", loadType, databaseName)
             startTime = self.__begin(message="loading operation")
             #
             # -- Check database to see if any entries have already been loaded, and determine the delta for the current load
-            # if databaseName in ["pdbx_core", "pdbx_comp_model_core"]:
-            #     totalIdsAlreadyLoaded = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=databaseName + "_entry")
-            #     subsetIdsAlreadyLoaded = list(set(totalIdsAlreadyLoaded).intersection(set(inputIdCodeList)))  # Get the list of IDs from only the given sublist that are already loaded
-            #     idCodesToLoadL = list(set(inputIdCodeList) ^ set(subsetIdsAlreadyLoaded))  # Get a list of the delta between the two lists—-i.e., the entry IDs needed to be loaded
-            #     logger.info(
-            #         "Total # IDs already loaded %d, # IDs provided as input %d (of which %d are already loaded), # IDs to load for current iteration %d",
-            #         len(totalIdsAlreadyLoaded),
-            #         len(inputIdCodeList),
-            #         len(subsetIdsAlreadyLoaded),
-            #         len(idCodesToLoadL)
-            #     )
+            inputIdCodeList = inputIdCodeList if inputIdCodeList else []
+            if databaseName in ["pdbx_core", "pdbx_comp_model_core"]:
+                totalIdsAlreadyLoaded = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=databaseName + "_entry")
+                # Get the list of IDs from only the given sublist that are already loaded
+                subsetIdsAlreadyLoaded = list(set(totalIdsAlreadyLoaded).intersection(set(inputIdCodeList)))
+                if not forceReload:
+                    # Get a list of the delta between the two lists—-i.e., the entry IDs needed to be loaded
+                    idCodesToLoadL = list(set(inputIdCodeList) ^ set(subsetIdsAlreadyLoaded))
+                else:
+                    idCodesToLoadL = inputIdCodeList
+                logger.info(
+                    "Total # IDs already loaded %d, # IDs provided as input %d (of which %d are already loaded), # IDs to load for current iteration %d",
+                    len(totalIdsAlreadyLoaded),
+                    len(inputIdCodeList),
+                    len(subsetIdsAlreadyLoaded),
+                    len(idCodesToLoadL)
+                )
+                # Check if all entries are already loaded, and if so, exit here.
+                if len(idCodesToLoadL) == 0:
+                    logger.info("All entries for current iteration already loaded. Skipping re-load.")
+                    return True
+                #
+                if len(idCodesToLoadL) < 100:
+                    logger.info("List of entries to load: %r", idCodesToLoadL)
             #
-            locatorObjList = self.__rpP.getLocatorObjList(contentType=databaseName, inputPathList=inputPathList, inputIdCodeList=inputIdCodeList, mergeContentTypes=mergeContentTypes)
+            else:
+                # For "bird_chem_comp_core":
+                idCodesToLoadL = inputIdCodeList
+            locatorObjList = self.__rpP.getLocatorObjList(contentType=databaseName, inputPathList=inputPathList, inputIdCodeList=idCodesToLoadL, mergeContentTypes=mergeContentTypes)
             logger.info("Loading database %s (%r) with path length %d", databaseName, loadType, len(locatorObjList))
             #
             if saveInputFileListPath:
                 self.__writePathList(saveInputFileListPath, self.__rpP.getLocatorPaths(locatorObjList))
                 logger.info("Saving %d paths in %s", len(locatorObjList), saveInputFileListPath)
             # ---
             # Don't load resource providers which are irrelevant to 'pdbx_core' or 'pdbx_comp_model_core'
@@ -229,15 +250,16 @@
             dP = DictionaryApiProviderWrapper(self.__cachePath, cfgOb=self.__cfgOb, useCache=True)
             dictApi = dP.getApiByName(databaseName)
             # ---
             dmrP = DictMethodResourceProvider(
                 self.__cfgOb, cachePath=self.__cachePath, restoreUseStash=restoreUseStash, restoreUseGit=restoreUseGit, providerTypeExclude=providerTypeExclude
             )
             # Cache dependencies in serial mode.
-            ok = dmrP.cacheResources(useCache=True)
+            useCacheInCheck = not rebuildCache
+            ok = dmrP.cacheResources(useCache=useCacheInCheck)
             if not ok:
                 logger.error("Checking cached resource dependencies failed - %s load (%r) aborted", databaseName, loadType)
                 return ok
             # ---
             self.__dmh = DictMethodRunner(dictApi, modulePathMap=modulePathMap, resourceProvider=dmrP)
             #
             filterType = "drop-empty-attributes|drop-empty-tables|skip-max-width|assign-dates|convert-iterables|normalize-enums|translateXMLCharRefs"
@@ -347,35 +369,52 @@
             if failedFilePath and failedPathList:
                 wOk = self.__writePathList(failedFilePath, failedPathList)
                 logger.info("Writing failure path %s length %d status %r", failedFilePath, len(failList), wOk)
             #
             ok = len(failList) == 0
             self.__end(startTime, "Loading operation completed with status " + str(ok))
             #
+            # -- Check database to see if any entries have already been loaded, and determine the delta for the current load
+            if databaseName in ["pdbx_core", "pdbx_comp_model_core"]:
+                totalIdsAlreadyLoaded = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=databaseName + "_entry")
+                # Get the list of IDs from only the given sublist that are already loaded
+                subsetIdsAlreadyLoaded = list(set(totalIdsAlreadyLoaded).intersection(set(inputIdCodeList)))
+                idCodesNotLoadedL = list(set(inputIdCodeList) ^ set(subsetIdsAlreadyLoaded))
+                ok2 = len(idCodesNotLoadedL) == 0
+                if not ok2:
+                    logger.error(
+                        "%d entries were NOT loaded in current iteration (%d out of input %d were loaded)",
+                        len(idCodesNotLoadedL),
+                        len(subsetIdsAlreadyLoaded),
+                        len(inputIdCodeList),
+                    )
+                ok = ok2 and ok
+
             # Create the status objects for the current operations
             # ----
             sFlag = "Y" if ok else "N"
             for collectionName in collectionNameList:
                 desp.setStartTime(tS=statusStartTimestamp)
                 desp.setObject(databaseName, collectionName)
                 desp.setStatus(updateId=None, successFlag=sFlag)
                 desp.setEndTime()
                 self.__statusList.append(desp.getStatus())
             #
             if ok:
                 logger.info("Completed loading %s with status %r loaded %d paths", databaseName, ok, numPaths)
             else:
-                logger.info(
+                logger.error(
                     "Completed loading %s with status %r failure count %d of %d paths: %r",
                     databaseName,
                     ok,
                     len(failList),
                     numPaths,
                     [os.path.basename(pth) for pth in failedPathList],
                 )
+                # raise ValueError("Failed loading %s - Check log for more details" % databaseName)
             #
             return ok
         except Exception as e:
             logger.exception("Failing with %s", str(e))
 
         return False
 
@@ -1031,13 +1070,69 @@
                 self.__removeCollection(databaseName, collectionName)
                 indexDL = docIndexD[collectionName] if collectionName in docIndexD else []
                 bsonSchema = None
                 if validationLevel and validationLevel in ["min", "full"]:
                     bsonSchema = self.__schP.getJsonSchema(databaseName, collectionName, encodingType="BSON", level=validationLevel)
                 ok = self.__createCollection(databaseName, collectionName, indexDL=indexDL, bsonSchema=bsonSchema)
                 logger.debug("Collection create return status %r", ok)
+                colIdL = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=collectionName)
+                ok = len(colIdL) == 0 and ok
+                logger.info("Collection wipe and create return status %r", ok)
             #
             return ok
         except Exception as e:
             logger.exception("Failing with %s", str(e))
 
         return False
+
+    def loadCompleteCheck(
+        self,
+        databaseName,
+        completeIdCodeList=None,
+        completeIdCodeCount=None,
+    ):
+        """Driver method for checking if DB loading is complete (following the execution of the individual sublist tasks).
+
+        Args:
+            databaseName (str): A content datbase schema (e.g. 'pdbx_core', 'pdbx_comp_model_core)
+            completeIdCodeList (list, optional): Complete list of ID codes that should be loaded by the end of all sublist loader tasks
+            completeIdCodeCount (int, optional): Number of total ID codes that should be loaded by the end of all sublist loader tasks
+        Returns:
+            bool: True on success or False otherwise
+        """
+        try:
+            logger.info("Beginning load completeness check for database %s", databaseName)
+            if databaseName not in ["pdbx_core", "pdbx_comp_model_core"]:
+                logger.error("Unsupported database for completed load checking %s", databaseName)
+                return False
+            # -- Check database to see if any entries have already been loaded, and determine the delta for the current load
+            totalIdsAlreadyLoaded = self.__getLoadedRcsbIdList(databaseName=databaseName, collectionName=databaseName + "_entry")
+            if completeIdCodeList:
+                # Get the list of IDs from only the given sublist that are already loaded
+                subsetIdsAlreadyLoaded = list(set(totalIdsAlreadyLoaded).intersection(set(completeIdCodeList)))
+                # Get a list of the delta between the two lists—-i.e., the entry IDs needed to be loaded
+                idsNotLoaded = list(set(completeIdCodeList) ^ set(subsetIdsAlreadyLoaded))
+                logger.info(
+                    "Total # IDs already loaded %d, total # IDs for complete load %d (of which %d are already loaded), # IDs to load for current iteration %d",
+                    len(totalIdsAlreadyLoaded),
+                    len(completeIdCodeList),
+                    len(subsetIdsAlreadyLoaded),
+                    len(idsNotLoaded)
+                )
+                # Check if all entries are already loaded, and if so, exit here.
+                if len(idsNotLoaded) == 0:
+                    logger.info("All entries have been loaded (%r entries)", len(completeIdCodeList))
+                    return True
+                else:
+                    logger.error("Not all entries have been loaded (missing %r entries)", len(idsNotLoaded))
+            elif completeIdCodeCount:
+                numIdsNotLoaded = completeIdCodeCount - len(totalIdsAlreadyLoaded)
+                if numIdsNotLoaded == 0:
+                    logger.info("All entries have been loaded (%r entries)", completeIdCodeCount)
+                    return True
+                else:
+                    logger.error("Not all entries have been loaded (missing %r entries)", numIdsNotLoaded)
+
+        except Exception as e:
+            logger.exception("Failing with %s", str(e))
+
+        return False
```

### Comparing `rcsb.db-1.717/rcsb/db/mysql/Connection.py` & `rcsb.db-1.718/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mysql/ConnectionBase.py` & `rcsb.db-1.718/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mysql/MyDbAdapter.py` & `rcsb.db-1.718/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mysql/MyDbUtil.py` & `rcsb.db-1.718/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb.db-1.718/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb.db-1.718/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/ClusterDataPrep.py` & `rcsb.db-1.718/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/DataExchangeStatus.py` & `rcsb.db-1.718/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/DataTransformFactory.py` & `rcsb.db-1.718/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb.db-1.718/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb.db-1.718/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb.db-1.718/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/processors/SchemaDefReShape.py` & `rcsb.db-1.718/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/sql/QueryDirectives.py` & `rcsb.db-1.718/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/sql/SqlGen.py` & `rcsb.db-1.718/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb.db-1.718/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb.db-1.718/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/ProvenanceProvider.py` & `rcsb.db-1.718/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/SchemaProvider.py` & `rcsb.db-1.718/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/TextUtil.py` & `rcsb.db-1.718/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/TimeUtil.py` & `rcsb.db-1.718/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/makePathList.py` & `rcsb.db-1.718/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb/db/utils/unescape.py` & `rcsb.db-1.718/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/rcsb.db.egg-info/PKG-INFO` & `rcsb.db-1.718/rcsb.db.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.717
+Version: 1.718
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -104,16 +104,27 @@
 Follow the instructions provided by at the [HomeBrew](https://brew.sh/) site to
 install this system.   Once HomeBrew is installed, you can further install the
 [MariaDB](https://mariadb.com/kb/en/library/installing-mariadb-on-macos-using-homebrew/) and
 [MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/) packages which
 are required to support the ExDB  tools.  HomeBrew also provides a variety of options for
 managing a [Python virtual environments](https://gist.github.com/Geoyi/f55ed54d24cc9ff1c14bd95fac21c042).
 
+### Configuration File
+
+RCSB/PDB repository path details are stored as configuration options.
+An example configuration file included in this package is viewable under `rcsb/db/config`: [exdb-config-example.yml](https://github.com/rcsb/py-rcsb_db/blob/master/rcsb/db/config/exdb-config-example.yml). This example references dictionary resources and mock repository data
+provided in the package in `rcsb/mock-data/*`. The `site_info_configuration` section
+in this file provides database server connection details and common path details.
+This is followed by sections specifying the dictionaries, helper functions, and
+configuration used to define the schema for the each supported content type
+(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
+
 ### Command Line Interfaces
 
+#### Schema File Generation
 A convenience CLI `schema_update_cli` is provided for generating operational schema from
 PDBx/mmCIF dictionary metadata.  Schema are encoded for the ExDB  API (rcsb), and
 for the document schema encoded in JSON and BSON formats.  The latter schema can be used to
 validate the loadable document objects produced for the collections served by MongoDB.
 
 ```bash
  => schema_update_cli  --help
@@ -182,129 +193,205 @@
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for dependencies and
                         testing
 ________________________________________________________________________________
 
 ```
 
+##### Example Usage
+
 For example, the following command will generate the JSON and BSON schema for the collections in the
 pdbx_core schema.
 
 ```bash
 schema_update_cli  --mock --schema_types json,bson \
                    --schema_level full  \
                    --update_pdbx_core   \
                    --cache_path . \
                    --config_path ./rcsb/db/config/exdb-config-example.yml  \
                    --config_name site_info_configuration
 ```
 
+#### ExDB Loading
+
 A convenience CLI `exdb_repo_load_cli` is provided to support loading PDB repositories
 containing entry and chemical reference data content types in the form of document collections
 compatible with MongoDB.
 
 ```bash
 exdb_repo_load_cli --help
 
-usage: exdb_repo_load_cli [-h] [--full] [--replace] [--load_chem_comp_ref]
-                          [--load_chem_comp_core_ref]
-                          [--load_bird_chem_comp_ref]
-                          [--load_bird_chem_comp_core_ref] [--load_bird_ref]
-                          [--load_bird_family_ref] [--load_entry_data]
-                          [--load_pdbx_core] [--load_pdbx_core_merge]
-                          [--load_pdbx_core_entry] [--load_pdbx_core_entity]
-                          [--load_pdbx_core_entity_monomer]
-                          [--load_pdbx_core_assembly] [--load_ihm_dev]
+usage: exdb_repo_load_cli [-h] [--op OP_TYPE] [--load_type LOAD_TYPE]
+                          [--database DATABASE_NAME]
                           [--config_path CONFIG_PATH]
                           [--config_name CONFIG_NAME] [--db_type DB_TYPE]
+                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--document_style DOCUMENT_STYLE]
-                          [--read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--disable_read_back_check] [--schema_level SCHEMA_LEVEL]
+                          [--load_id_list_path LOAD_ID_LIST_PATH]
                           [--load_file_list_path LOAD_FILE_LIST_PATH]
                           [--fail_file_list_path FAIL_FILE_LIST_PATH]
                           [--save_file_list_path SAVE_FILE_LIST_PATH]
-                          [--num_proc NUM_PROC] [--chunk_size CHUNK_SIZE]
                           [--file_limit FILE_LIMIT]
                           [--prune_document_size PRUNE_DOCUMENT_SIZE]
                           [--debug] [--mock] [--cache_path CACHE_PATH]
                           [--rebuild_cache] [--rebuild_schema]
                           [--vrpt_repo_path VRPT_REPO_PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
-  --full                Fresh full load in a new tables/collections
-  --replace             Load with replacement in an existing table/collection
-                        (default)
-  --load_chem_comp_ref  Load Chemical Component reference definitions (public
-                        subset)
-  --load_chem_comp_core_ref
-                        Load Chemical Component Core reference definitions
-                        (public subset)
-  --load_bird_chem_comp_ref
-                        Load Bird Chemical Component reference definitions
-                        (public subset)
-  --load_bird_chem_comp_core_ref
-                        Load Bird Chemical Component Core reference
-                        definitions (public subset)
-  --load_bird_ref       Load Bird reference definitions (public subset)
-  --load_bird_family_ref
-                        Load Bird Family reference definitions (public subset)
-  --load_entry_data     Load PDBx entry data (current released subset)
-  --load_pdbx_core      Load all PDBx core collections (current released
-                        subset)
-  --load_pdbx_core_merge
-                        Load all PDBx core collections with merged content
-                        (current released subset)
-  --load_pdbx_core_entry
-                        Load PDBx core entry (current released subset)
-  --load_pdbx_core_entity
-                        Load PDBx core entity (current released subset)
-  --load_pdbx_core_entity_monomer
-                        Load PDBx core entity monomer (current released
-                        subset)
-  --load_pdbx_core_assembly
-                        Load PDBx core assembly (current released subset)
-  --load_ihm_dev        Load I/HM DEV model data (current released subset)
+  --op {pdbx-loader,build-resource-cache,pdbx-db-wiper,pdbx-id-list-splitter,pdbx-loader-check,etl-entity-sequence-clusters,etl-repository-holdings}
+                        Loading operation to perform
+  --load_type {replace,full}
+                        Type of load ('replace' for incremental and
+                        multi-worker load, 'full' for complete and
+                        fresh single-worker load)
+  --database {pdbx_core,pdbx_comp_model_core,bird_chem_comp_core,chem_comp,chem_comp_core,bird_chem_comp,bird,bird_family,ihm_dev}
+                        Database to load (most common choices are:
+                        'pdbx_core', 'pdbx_comp_model_core', or
+                        'bird_chem_comp_core')
   --config_path CONFIG_PATH
                         Path to configuration options file
   --config_name CONFIG_NAME
                         Configuration section name
-  --db_type DB_TYPE     Database server type (default=mongo)
   --document_style DOCUMENT_STYLE
-                        Document organization (rowwise_by_name_with_cardinalit
-                        y|rowwise_by_name|columnwise_by_name|rowwise_by_id|row
-                        wise_no_name
-  --read_back_check     Perform read back check on all documents
+                        Document organization (rowwise_by_name_with_c
+                        ardinality|rowwise_by_name|columnwise_by_name
+                        |rowwise_by_id|rowwise_no_name)
+  --cache_path CACHE_PATH
+                        Cache path for resource files
+  --num_proc NUM_PROC   Number of processes to execute (default=2)
+  --chunk_size CHUNK_SIZE
+                        Number of files loaded per process
+  --max_step_length MAX_STEP_LENGTH
+                        Maximum subList size (default=500)
   --schema_level SCHEMA_LEVEL
-                        Schema validation level (full|min default=None)
+                        Schema validation level (full|min)
+  --collection_list COLLECTION_LIST
+                        Specific collections to load
+  --load_id_list_path LOAD_ID_LIST_PATH
+                        Input file containing the list of IDs to load
+                        in the current iteration by a single worker
+  --holdings_file_path HOLDINGS_FILE_PATH
+                        File containing the complete list of all IDs
+                        (or holdings files) that will be loaded
   --load_file_list_path LOAD_FILE_LIST_PATH
-                        Input file containing load file path list (override
-                        automatic repository scan)
+                        Input file containing load file path list
+                        (override automatic repository scan)
   --fail_file_list_path FAIL_FILE_LIST_PATH
-                        Output file containing file paths that fail to load
+                        Output file containing file paths that fail
+                        to load
   --save_file_list_path SAVE_FILE_LIST_PATH
-                        Save repo file paths from automatic file system scan
-                        in this path
-  --num_proc NUM_PROC   Number of processes to execute (default=2)
-  --chunk_size CHUNK_SIZE
-                        Number of files loaded per process
+                        Save repo file paths from automatic file
+                        system scan in this path
+  --load_file_list_dir LOAD_FILE_LIST_DIR
+                        Directory path for storing load file lists
+  --num_sublists NUM_SUBLISTS
+                        Number of sublists to create/load for the
+                        associated database
+  --force_reload        Force re-load of provided ID list (i.e.,
+                        don't just load delta; useful for manual/test
+                        runs).
+  --provider_type_exclude PROVIDER_TYPE_EXCLUDE
+                        Resource provider types to exclude
+  --db_type DB_TYPE     Database server type (default=mongo)
   --file_limit FILE_LIMIT
                         Load file limit for testing
   --prune_document_size PRUNE_DOCUMENT_SIZE
                         Prune large documents to this size limit (MB)
+  --regex_purge         Perform additional regex-based purge of all
+                        pre-existing documents for loadType != 'full'
+  --data_selectors  [ ...]
+                        Data selectors, space-separated.
+  --disable_read_back_check
+                        Disable read back check on all documents
+  --disable_merge_validation_reports
+                        Disable merging of validation report data
+                        with the primary content type
   --debug               Turn on verbose logging
   --mock                Use MOCK repository configuration for testing
-  --cache_path CACHE_PATH
-                        Cache path for resource files
   --rebuild_cache       Rebuild cached resource files
   --rebuild_schema      Rebuild schema on-the-fly if not cached
   --vrpt_repo_path VRPT_REPO_PATH
                         Path to validation report repository
 ________________________________________________________________________________
 ```
 
+##### Example Usage
+The following commands demonstrate how each type of operation (`--op`) is used for loading of PDB repository data to ExDB. For all commands, the following environmental variables must first be set:
+
+```bash
+export CONFIG_SUPPORT_TOKEN_ENV=personal_token_used_for_decrypting_config_variables
+export OE_LICENSE=/path/to/oe_license.txt
+export NLTK_DATA=/path/to/nltk_data
+```
+
+`--op build-resource-cache` - Build the external resource cache that will be used for and integrated with the loading of PDB structure data.
+```bash
+exdb_repo_load_cli --op "build-resource-cache" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--num_proc 6  \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-db-wiper` - Wipe the pre-existing database (and all of its collections).
+```bash
+exdb_repo_load_cli --op "pdbx-db-wiper" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-id-list-splitter` - Split the full list of input IDs into smaller, equally-sized sublists.
+```bash
+exdb_repo_load_cli --op "pdbx-id-list-splitter" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+`--op pdbx-loader` - Load a list of entry IDs to ExDB.
+```bash
+exdb_repo_load_cli --op "pdbx-loader" \
+--database "pdbx_core" \
+--load_type replace  \
+--config_path /opt/etl-scratch/config/exdb-loader-config.yml \
+--config_name site_info_remote_configuration \
+--num_proc 8  \
+--chunk_size 5  \
+--max_step_length 500 \
+--load_id_list_path "/opt/etl-scratch/work-dir/load_file_lists/pdbx_core_ids-1.txt" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+
+```
+
+`--op pdbx-loader-check` - Check the resulting ExDB database to confirm that all expected documents were loaded.
+```bash
+exdb_repo_load_cli --op "pdbx-loader-check" \
+--database "pdbx_core" \
+--config_path "/opt/etl-scratch/config/exdb-loader-config.yml" \
+--config_name "site_info_remote_configuration" \
+--cache_path "/opt/etl-scratch/data/CACHE" \
+--load_file_list_dir "/opt/etl-scratch/work-dir/load_file_lists" \
+--holdings_file_path "https://files.wwpdb.org/pub/pdb/holdings/released_structures_last_modified_dates.json.gz" \
+--num_sublists 10 \
+
+```
+
+#### Repository Scanning
+
 Part of the schema definition process supported by this module involves refining
 the dictionary metadata with more specific data typing and coverage details.
 A scanning tools is provided to collect and organize these details for the
 other ETL tools in this package.  The following convenience CLI, `repo_scan_cli`,
 is provided to scan supported PDB repository content and update data type and coverage details.
 
 ```bash
@@ -367,14 +454,15 @@
   --mock                Use MOCK repository configuration for testing
   --working_path WORKING_PATH
                         Working path for temporary files
 ________________________________________________________________________________
 
 ```
 
+#### ETL Processing
 The following CLI provides a preliminary access to ETL functions for processing
 derived content types such as sequence comparative data.
 
 ```bash
 etl_exec_cli --help
 usage: etl_exec_cli [-h] [--full] [--etl_entity_sequence_clusters]
                     [--etl_repository_holdings] [--data_set_id DATA_SET_ID]
@@ -421,170 +509,48 @@
   --cache_path CACHE_PATH
                         Path containing cache directories
   --rebuild_cache       Rebuild cached resource files
 ________________________________________________________________________________
 
 ```
 
-### Examples
+### Additional Examples
+
+(*Note: The examples below are outdated and may not function as described. They are only kept here for historical reference.*)
 
 If you are working in the source repository, then you can run the CLI commands in the following manner.
 The following examples load data in the mock repositories in source distribution assuming you have a local
 default installation of MongoDb (no user/pw assigned).
 
 To run the command-line interface `exdb_repo_load_cli` outside of the source distribution, you will need to
 create a configuration file with the appropriate path details and authentication credentials.
 
 For instance, to perform a fresh/full load of all of the chemical component definitions in the mock repository:
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py --full  --load_chem_comp_ref  \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --fail_file_list_path failed-cc-path-list.txt \
                       --read_back_check
 ```
 
 The following illustrates, a full load of the mock structure data repository followed by a reload with replacement of
 this same data.
 
 ```bash
 
-cd rcsb/db/scripts
+cd rcsb/db/cli
 python RepoLoadExec.py  --mock --full  --load_entry_data \
                      --config_path ../config/exdb-config-example.yml \
                      --config_name site_info_configuration \
                      --save_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                      --fail_file_list_path failed-entry-path-list.txt
 
 python RepoLoadExec.py --mock --replace  --load_entry_data \
                       --config_path ../config/exdb-config-example.yml \
                       --config_name site_info_configuration \
                       --load_file_list_path  LATEST_PDBX_LOAD_LIST.txt \
                       --fail_file_list_path failed-entry-path-list.txt
 ```
-
-### Configuration Example
-
-RCSB/PDB repository path details are stored as configuration options.
-An example configuration file included in this package is shown below.
-This example is references dictionary resources and mock repository data
-provided in the package in `rcsb/mock-data/*`. Example configuration details are
-stored in rcsb/db/config/exdb-config-example.yml.The `site_info_configuration` section
-in this file provides database server connection details and common path details.
-This is followed by sections specifying the dictionaries, helper functions, and
-configuration used to define the schema for the each supported content type
-(e.g., pdbx_core, chem_comp_core, bird_chem_comp_core,.. ).
-
-```yaml
-site_info_configuration:
-  # Site specific path and server configuration options - (REFERENCING DEVELOPMENT RESOURCES)
-  #
-  CONFIG_SUPPORT_TOKEN: CONFIG_SUPPORT_TOKEN_ENV
-  #
-  # Database server connection details
-  #
-  MONGO_DB_HOST: localhost
-  MONGO_DB_PORT: "27017"
-  _MONGO_DB_USER_NAME: ""
-  _MONGO_DB_PASSWORD: ""
-  MYSQL_DB_HOST_NAME: localhost
-  MYSQL_DB_PORT_NUMBER: "3306"
-  _MYSQL_DB_USER_NAME: wrIzBGtCsQmkjc7tbEPQ3oEaOnpvivXaKcQsvXD6kn4KHMvA7LCL4O9GlAI=
-  _MYSQL_DB_PASSWORD: qXPp32Z6DhNVMwo9fQIK5+KB13c1Jd43E3Bn6LmJcSyXc0NAt4H/hwo/xglYpmELV5Vqaw==
-  _MYSQL_DB_PASSWORD_ALT: s6mNxq3FIwZLrLiIeHpDZQcuVxfQqrR3gA+dEMOGgHwsjrJV5da08H74RmnNRus74Q==
-  MYSQL_DB_DATABASE_NAME: mysql
-  CRATE_DB_HOST: localhost
-  CRATE_DB_PORT: "4200"
-  COCKROACH_DB_HOST: localhost
-  COCKROACH_DB_PORT: "26257"
-  COCKROACH_DB_NAME: system
-  _COCKROACH_DB_USER_NAME: HR2ez8iLbEpvN+hXKIQS3qa6/QpiFRpf/WvrfHiwfjcL09E+iWTQJhsxTsw=
-  #
-  # Primary repository data and related computed repository data paths
-  #
-  BIRD_REPO_PATH: MOCK_BIRD_REPO
-  BIRD_FAMILY_REPO_PATH: MOCK_BIRD_FAMILY_REPO
-  BIRD_CHEM_COMP_REPO_PATH: MOCK_BIRD_CC_REPO
-  CHEM_COMP_REPO_PATH: MOCK_CHEM_COMP_REPO
-  PDBX_REPO_PATH: MOCK_PDBX_SANDBOX
-  RCSB_EXCHANGE_SANDBOX_PATH: MOCK_EXCHANGE_SANDBOX
-  IHM_DEV_REPO_PATH: MOCK_IHM_REPO
-  VRPT_REPO_PATH: MOCK_VALIDATION_REPORTS
-  VRPT_REPO_PATH_ENV: VRPT_REPO_PATH_ALT
-  #
-  RCSB_EDMAP_LIST_PATH: MOCK_EXCHANGE_SANDBOX/status/edmaps.json
-  #
-  RCSB_SEQUENCE_CLUSTER_DATA_PATH: cluster_data/mmseqs_clusters_current
-  SIFTS_SUMMARY_DATA_PATH: sifts-summary
-  # -------------------------------------------------------------------------------------------
-  #   -- Below are common across current deployments -
-  #
-  # Supporting and integrated resource data cache directory names
-  #
-  #DRUGBANK_CACHE_DIR: DrugBank
-  _DRUGBANK_AUTH_USERNAME: 0qrpNd4OhGuVsJqEpcsAVEovZ0hl6QkgxmbTy3bPssd06Z9tuM6bJqgsWwmFCd0JnjIMIEWyKPMmF1pI5g==
-  _DRUGBANK_AUTH_PASSWORD: lA/K132i8DOtLdMHfm3gpNqprZ6ABKjsCRxfcXIMnxpKQzBv/B6dmC7x1vRO86JhqdT0b84=
-  DRUGBANK_MOCK_URL_TARGET: DrugBank/full_database.zip
-  #
-  #ATC_CACHE_DIR: atc
-  #CHEM_COMP_CACHE_DIR: chem_comp
-  NCBI_TAXONOMY_CACHE_DIR: NCBI
-  ENZYME_CLASSIFICATION_CACHE_DIR: ec
-  STRUCT_DOMAIN_CLASSIFICATION_CACHE_DIR: domains_struct
-  SIFTS_SUMMARY_CACHE_DIR: sifts_summary
-  DICTIONARY_CACHE_DIR: dictionaries
-  DATA_TYPE_INFO_CACHE_DIR: data_type_and_coverage
-  REPO_UTIL_CACHE_DIR: repo_util
-  EXDB_CACHE_DIR: exdb
-  CITATION_REFERENCE_CACHE_DIR: cit_ref
-  #
-  #
-  PROVENANCE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/provenance/rcsb_extend_provenance_info.json
-  PROVENANCE_INFO_CACHE_DIR: provenance
-  #
-  SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/schema_definitions
-  SCHEMA_DEFINITION_CACHE_DIR: schema_definitions
-  JSON_SCHEMA_DEFINITION_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/json_schema_definitions
-  JSON_SCHEMA_DEFINITION_CACHE_DIR: json_schema_definitions
-  #
-  # Helper class binding and mappings
-  #
-  DICT_METHOD_HELPER_MODULE_PATH_MAP:
-    rcsb.utils.dictionary.DictMethodEntryHelper: rcsb.utils.dictionary.DictMethodEntryHelper
-    rcsb.utils.dictionary.DictMethodChemRefHelper: rcsb.utils.dictionary.DictMethodChemRefHelper
-    rcsb.utils.dictionary.DictMethodEntityHelper: rcsb.utils.dictionary.DictMethodEntityHelper
-    rcsb.utils.dictionary.DictMethodAssemblyHelper: rcsb.utils.dictionary.DictMethodAssemblyHelper
-    rcsb.utils.dictionary.DictMethodEntityInstanceHelper: rcsb.utils.dictionary.DictMethodEntityInstanceHelper
-  # ------ ------ ------ ------ ------ ------ ------ -------
-  # ADDED rcsb.db V0.966 Source dictionary locators -
-  #
-  PDBX_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/mmcif_pdbx_v5_next.dic
-  RCSB_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/dist/rcsb_mmcif_ext.dic
-  IHMDEV_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/ihm-extension.dic
-  FLR_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/flr-extension.dic
-  VRPT_DICT_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_mmcif_ext.dic
-  VRPT_DICT_MAPPING_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/dictionary_files/reference/vrpt_dictmap.json
-  # ------ ------ ------ ------ ------ ------ ------ ------ ------
-  # Added in rcsb.db V0.966 - Data type details and type mapping
-  APP_DATA_TYPE_INFO_LOCATOR: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage/app_data_type_mapping.cif
-  INSTANCE_DATA_TYPE_INFO_LOCATOR_PATH: https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/data_type_and_coverage
-  #
-  CONTENT_DEF_HELPER_MODULE: rcsb.db.helpers.ContentDefinitionHelper
-  DOCUMENT_DEF_HELPER_MODULE: rcsb.db.helpers.DocumentDefinitionHelper
-  CONFIG_APPEND_LOCATOR_PATHS:
-    - https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/config/exdb-config-schema.yml
-# ------ ------ ------ ------ ------ ------ ------ ------ ------
-#  Added V1.001 for stash storage server
-#  -- This is a placeholder configuration to support remote testing --
-#  local|server
-  STASH_MODE: local
-  STASH_LOCAL_BASE_PATH: stash-storage
-  #
-  STASH_SERVER_URL: https://raw.githubusercontent.com
-  STASH_SERVER_FALLBACK_URL: https://raw.githubusercontent.com
-  _STASH_SERVER_BASE_PATH: bIo7kGc2w6Oel0QNr7Pc/4bFfDQayhPxddnGHynP6yudxc44QYuAFoTFdOqY2ZzsM2DEk56r26MfG66bEQ42lp38guy837xwzN1Vgu+r9zvAm11HXEA=
-  REFERENCE_SEQUENCE_ALIGNMETS: PDB
-##
-```
```

### Comparing `rcsb.db-1.717/rcsb.db.egg-info/SOURCES.txt` & `rcsb.db-1.718/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/requirements.txt` & `rcsb.db-1.718/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.717/setup.py` & `rcsb.db-1.718/setup.py`

 * *Files identical despite different names*

