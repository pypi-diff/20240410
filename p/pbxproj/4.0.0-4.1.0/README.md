# Comparing `tmp/pbxproj-4.0.0.tar.gz` & `tmp/pbxproj-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbxproj-4.0.0.tar", last modified: Wed Oct 11 20:06:52 2023, max compression
+gzip compressed data, was "pbxproj-4.1.0.tar", last modified: Wed Apr 10 08:27:20 2024, max compression
```

## Comparing `pbxproj-4.0.0.tar` & `pbxproj-4.1.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.999942 pbxproj-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2023-10-11 20:06:51.999942 pbxproj-4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.995942 pbxproj-4.0.0/pbxproj/
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/PBXGenericObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/PBXKey.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/PBXList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/PBXObjects.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/PBXRootObject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/XcodeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.995942 pbxproj-4.0.0/pbxproj/pbxcli/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.995942 pbxproj-4.0.0/pbxproj/pbxextensions/
--rw-r--r--   0 runner    (1001) docker     (127)    30920 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxextensions/ProjectFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    16333 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxextensions/ProjectFlags.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxextensions/ProjectGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxextensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.999942 pbxproj-4.0.0/pbxproj/pbxsections/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXAggregateTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXBuildFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXContainerItemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXCopyFilesBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXFileReference.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXFrameworksBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXGenericBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXGenericTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXHeadersBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXLegacyTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXNativeTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXReferenceProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXResourcesBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXShellScriptBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXSourcesBuildPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/PBXTargetDependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/XCBuildConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/XCConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/XCRemoteSwiftPackageReference.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/XCSwiftPackageProductDependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-11 20:06:34.000000 pbxproj-4.0.0/pbxproj/pbxsections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 20:06:51.995942 pbxproj-4.0.0/pbxproj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-11 20:06:51.000000 pbxproj-4.0.0/pbxproj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 20:06:51.999942 pbxproj-4.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1502 2023-10-11 20:06:34.000000 pbxproj-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.591495 pbxproj-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-10 08:27:20.591495 pbxproj-4.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.583495 pbxproj-4.1.0/pbxproj/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/PBXGenericObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/PBXKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/PBXList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/PBXObjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/PBXRootObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/XcodeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.587495 pbxproj-4.1.0/pbxproj/pbxcli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.587495 pbxproj-4.1.0/pbxproj/pbxextensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    30988 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxextensions/ProjectFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16333 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxextensions/ProjectFlags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxextensions/ProjectGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxextensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.591495 pbxproj-4.1.0/pbxproj/pbxsections/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXAggregateTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXBuildFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXContainerItemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXCopyFilesBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXFileReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXFrameworksBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXGenericBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXGenericTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXHeadersBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXLegacyTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXNativeTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXReferenceProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXResourcesBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXShellScriptBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXSourcesBuildPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/PBXTargetDependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/XCBuildConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/XCConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/XCLocalSwiftPackageReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/XCRemoteSwiftPackageReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/XCSwiftPackageProductDependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 08:26:57.000000 pbxproj-4.1.0/pbxproj/pbxsections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:27:20.591495 pbxproj-4.1.0/pbxproj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 08:27:20.000000 pbxproj-4.1.0/pbxproj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:27:20.591495 pbxproj-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1502 2024-04-10 08:26:57.000000 pbxproj-4.1.0/setup.py
```

### Comparing `pbxproj-4.0.0/PKG-INFO` & `pbxproj-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pbxproj
-Version: 4.0.0
+Version: 4.1.0
 Summary: XCode Project manipulation library for Python
 Home-page: http://github.com/kronenthaler/mod-pbxproj
 Author: Ignacio Calderon
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: openstep_parser>=1.5.1
+Requires-Dist: docopt
 
 
-.. image:: https://img.shields.io/github/workflow/status/kronenthaler/mod-pbxproj/branch-check/master?logo=github&style=flat-square
+.. image:: https://img.shields.io/github/actions/workflow/status/kronenthaler/mod-pbxproj/branch-check.yml?event=push&style=flat&logo=github&color=4da533
    :target: https://github.com/kronenthaler/mod-pbxproj/actions?query=workflow%3Abranch-check
    :alt: GitHub Workflow Status (branch)
 
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=kronenthaler_mod-pbxproj&metric=alert_status
    :target: https://sonarcloud.io/summary/new_code?id=kronenthaler_mod-pbxproj
    :alt: Sonar Quality Gate status
 
@@ -21,23 +23,23 @@
    :target: https://sonarcloud.io/component_measures?metric=coverage&id=kronenthaler_mod-pbxproj
    :alt: Sonar branch coverage
 
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=kronenthaler_mod-pbxproj&metric=reliability_rating
    :target: https://sonarcloud.io/summary/new_code?id=kronenthaler_mod-pbxproj
    :alt: Sonar reliability grade
 
-.. image:: https://img.shields.io/pypi/v/pbxproj?color=97cb02&logo=python&logoColor=ffffff&style=flat-square
+.. image:: https://img.shields.io/pypi/v/pbxproj?logo=python&logoColor=ffffff&style=flat&color=4da533
    :target: https://pypi.python.org/pypi/pbxproj
    :alt: PyPI
 
-.. image:: https://img.shields.io/pypi/dm/pbxproj?color=97cb02&logo=python&logoColor=ffffff&style=flat-square
+.. image:: https://img.shields.io/pypi/dm/pbxproj?logo=python&logoColor=ffffff&style=flat&color=4da533
    :target: https://pypi.python.org/pypi/pbxproj/
    :alt: PyPI - Downloads
 
-.. image:: https://img.shields.io/pypi/l/pbxproj?color=97cb02&style=flat-square
+.. image:: https://img.shields.io/pypi/l/pbxproj?style=flat&color=4da533
    :target: license.txt
    :alt: PyPI - License
 
 pbxproj
 =======
 
 This module can read, modify, and write a .pbxproj file from an Xcode 4+ projects. The file is usually called project.pbxproj and can be found inside the .xcodeproj bundle. Because some task cannot be done by clicking on an UI or opening Xcode to do it for you, this python module lets you automate the modification process.
```

### Comparing `pbxproj-4.0.0/pbxproj/PBXGenericObject.py` & `pbxproj-4.1.0/pbxproj/PBXGenericObject.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 
 class PBXGenericObject(object):
     """
     Generic class that creates internal attributes to match the structure of the tree used to create the element.
     Also, prints itself using the openstep format. Extensions might be required to insert comments on right places.
     """
-    _VALID_KEY_REGEX = re.compile(r'^[a-zA-Z0-9\\._/]*$')
+    # use negative look-ahead to avoid matching the newline character in multiline strings
+    _VALID_KEY_REGEX = re.compile(r'^[a-zA-Z0-9\\._/]*(?!\n)$')
     _ESCAPE_REPLACEMENTS = [
         ('\\', '\\\\'),
         ('\n', '\\n'),
         ('\"', '\\"'),
         ('\0', '\\0'),
         ('\t', '\\\t'),
         ('\'', '\\\''),
```

### Comparing `pbxproj-4.0.0/pbxproj/PBXObjects.py` & `pbxproj-4.1.0/pbxproj/PBXObjects.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/XcodeProject.py` & `pbxproj-4.1.0/pbxproj/XcodeProject.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/__init__.py` & `pbxproj-4.1.0/pbxproj/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from pbxproj.PBXList import PBXList
 from pbxproj.PBXGenericObject import PBXGenericObject
 from pbxproj.PBXObjects import objects
 from pbxproj.PBXRootObject import rootObject
 from pbxproj.XcodeProject import XcodeProject
 from pbxproj.pbxsections import *
 
-__version__ = '4.0.0'
+__version__ = '4.1.0'
```

### Comparing `pbxproj-4.0.0/pbxproj/__main__.py` & `pbxproj-4.1.0/pbxproj/__main__.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxcli/__init__.py` & `pbxproj-4.1.0/pbxproj/pbxcli/__init__.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_file.py` & `pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_file.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_flag.py` & `pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_flag.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_folder.py` & `pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_folder.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxcli/pbxproj_show.py` & `pbxproj-4.1.0/pbxproj/pbxcli/pbxproj_show.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxextensions/ProjectFiles.py` & `pbxproj-4.1.0/pbxproj/pbxextensions/ProjectFiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,16 @@
         '.xcdatamodeld': ('wrapper.xcdatamodel', 'PBXSourcesBuildPhase'),
         '.xcassets': ('folder.assetcatalog', 'PBXResourcesBuildPhase'),
         '.xcconfig': ('sourcecode.xcconfig', 'PBXSourcesBuildPhase'),
         '.tbd': ('sourcecode.text-based-dylib-definition', 'PBXFrameworksBuildPhase'),
         '.bin': ('archive.macbinary', 'PBXResourcesBuildPhase'),
         '.mlmodel':('file.mlmodel', 'PBXSourcesBuildPhase'),
         '.html':('text.html', 'PBXResourcesBuildPhase'),
-        '.entitlements': ('text.plist.entitlements', 'PBXResourcesBuildPhase')
+        '.entitlements': ('text.plist.entitlements', 'PBXResourcesBuildPhase'),
+        '.xcprivacy': ('text.plist.xml', 'PBXResourcesBuildPhase')
     }
     _SPECIAL_FOLDERS = [
         '.bundle',
         '.framework',
         '.xcodeproj',
         '.xcassets',
         '.xcdatamodeld',
```

### Comparing `pbxproj-4.0.0/pbxproj/pbxextensions/ProjectFlags.py` & `pbxproj-4.1.0/pbxproj/pbxextensions/ProjectFlags.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxextensions/ProjectGroups.py` & `pbxproj-4.1.0/pbxproj/pbxextensions/ProjectGroups.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXBuildFile.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXBuildFile.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXContainerItemProxy.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXContainerItemProxy.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXCopyFilesBuildPhase.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXCopyFilesBuildPhase.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXFileReference.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXFileReference.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXGenericBuildPhase.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXGenericBuildPhase.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXGenericTarget.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXGenericTarget.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXGroup.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXGroup.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXProject.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXProject.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXReferenceProxy.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXReferenceProxy.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/PBXShellScriptBuildPhase.py` & `pbxproj-4.1.0/pbxproj/pbxsections/PBXShellScriptBuildPhase.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/XCBuildConfiguration.py` & `pbxproj-4.1.0/pbxproj/pbxsections/XCBuildConfiguration.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/XCConfigurationList.py` & `pbxproj-4.1.0/pbxproj/pbxsections/XCConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/XCRemoteSwiftPackageReference.py` & `pbxproj-4.1.0/pbxproj/pbxsections/XCRemoteSwiftPackageReference.py`

 * *Files identical despite different names*

### Comparing `pbxproj-4.0.0/pbxproj/pbxsections/__init__.py` & `pbxproj-4.1.0/pbxproj/pbxsections/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 from pbxproj.pbxsections.PBXAggregateTarget import *
 from pbxproj.pbxsections.PBXNativeTarget import *
 from pbxproj.pbxsections.PBXLegacyTarget import *
 from pbxproj.pbxsections.PBXReferenceProxy import *
 from pbxproj.pbxsections.PBXGroup import *
 from pbxproj.pbxsections.XCSwiftPackageProductDependency import *
 from pbxproj.pbxsections.XCRemoteSwiftPackageReference import *
+from pbxproj.pbxsections.XCLocalSwiftPackageReference import *
```

### Comparing `pbxproj-4.0.0/pbxproj.egg-info/PKG-INFO` & `pbxproj-4.1.0/pbxproj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pbxproj
-Version: 4.0.0
+Version: 4.1.0
 Summary: XCode Project manipulation library for Python
 Home-page: http://github.com/kronenthaler/mod-pbxproj
 Author: Ignacio Calderon
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: openstep_parser>=1.5.1
+Requires-Dist: docopt
 
 
-.. image:: https://img.shields.io/github/workflow/status/kronenthaler/mod-pbxproj/branch-check/master?logo=github&style=flat-square
+.. image:: https://img.shields.io/github/actions/workflow/status/kronenthaler/mod-pbxproj/branch-check.yml?event=push&style=flat&logo=github&color=4da533
    :target: https://github.com/kronenthaler/mod-pbxproj/actions?query=workflow%3Abranch-check
    :alt: GitHub Workflow Status (branch)
 
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=kronenthaler_mod-pbxproj&metric=alert_status
    :target: https://sonarcloud.io/summary/new_code?id=kronenthaler_mod-pbxproj
    :alt: Sonar Quality Gate status
 
@@ -21,23 +23,23 @@
    :target: https://sonarcloud.io/component_measures?metric=coverage&id=kronenthaler_mod-pbxproj
    :alt: Sonar branch coverage
 
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=kronenthaler_mod-pbxproj&metric=reliability_rating
    :target: https://sonarcloud.io/summary/new_code?id=kronenthaler_mod-pbxproj
    :alt: Sonar reliability grade
 
-.. image:: https://img.shields.io/pypi/v/pbxproj?color=97cb02&logo=python&logoColor=ffffff&style=flat-square
+.. image:: https://img.shields.io/pypi/v/pbxproj?logo=python&logoColor=ffffff&style=flat&color=4da533
    :target: https://pypi.python.org/pypi/pbxproj
    :alt: PyPI
 
-.. image:: https://img.shields.io/pypi/dm/pbxproj?color=97cb02&logo=python&logoColor=ffffff&style=flat-square
+.. image:: https://img.shields.io/pypi/dm/pbxproj?logo=python&logoColor=ffffff&style=flat&color=4da533
    :target: https://pypi.python.org/pypi/pbxproj/
    :alt: PyPI - Downloads
 
-.. image:: https://img.shields.io/pypi/l/pbxproj?color=97cb02&style=flat-square
+.. image:: https://img.shields.io/pypi/l/pbxproj?style=flat&color=4da533
    :target: license.txt
    :alt: PyPI - License
 
 pbxproj
 =======
 
 This module can read, modify, and write a .pbxproj file from an Xcode 4+ projects. The file is usually called project.pbxproj and can be found inside the .xcodeproj bundle. Because some task cannot be done by clicking on an UI or opening Xcode to do it for you, this python module lets you automate the modification process.
```

### Comparing `pbxproj-4.0.0/pbxproj.egg-info/SOURCES.txt` & `pbxproj-4.1.0/pbxproj.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,10 +38,11 @@
 pbxproj/pbxsections/PBXReferenceProxy.py
 pbxproj/pbxsections/PBXResourcesBuildPhase.py
 pbxproj/pbxsections/PBXShellScriptBuildPhase.py
 pbxproj/pbxsections/PBXSourcesBuildPhase.py
 pbxproj/pbxsections/PBXTargetDependency.py
 pbxproj/pbxsections/XCBuildConfiguration.py
 pbxproj/pbxsections/XCConfigurationList.py
+pbxproj/pbxsections/XCLocalSwiftPackageReference.py
 pbxproj/pbxsections/XCRemoteSwiftPackageReference.py
 pbxproj/pbxsections/XCSwiftPackageProductDependency.py
 pbxproj/pbxsections/__init__.py
```

### Comparing `pbxproj-4.0.0/setup.py` & `pbxproj-4.1.0/setup.py`

 * *Files identical despite different names*

