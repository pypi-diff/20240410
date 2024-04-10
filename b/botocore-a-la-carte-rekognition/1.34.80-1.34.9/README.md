# Comparing `tmp/botocore-a-la-carte-rekognition-1.34.80.tar.gz` & `tmp/botocore-a-la-carte-rekognition-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-rekognition-1.34.80.tar", last modified: Tue Apr  9 01:00:56 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-rekognition-1.34.9.tar", last modified: Thu Dec 28 01:06:58 2023, max compression
```

## Comparing `botocore-a-la-carte-rekognition-1.34.80.tar` & `botocore-a-la-carte-rekognition-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.356228 botocore-a-la-carte-rekognition-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-09 01:00:56.356228 botocore-a-la-carte-rekognition-1.34.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.352228 botocore-a-la-carte-rekognition-1.34.80/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.352228 botocore-a-la-carte-rekognition-1.34.80/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.352228 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.356228 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-09 01:00:24.000000 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-09 01:00:24.000000 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-09 01:00:24.000000 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   451966 2024-04-09 01:00:24.000000 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 01:00:24.000000 botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:56.356228 botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:00:56.356228 botocore-a-la-carte-rekognition-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-09 01:00:56.000000 botocore-a-la-carte-rekognition-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.362410 botocore-a-la-carte-rekognition-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:58.362410 botocore-a-la-carte-rekognition-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.358410 botocore-a-la-carte-rekognition-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.358410 botocore-a-la-carte-rekognition-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.358410 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.358410 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2023-12-28 01:06:26.000000 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2023-12-28 01:06:26.000000 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-12-28 01:06:26.000000 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   449826 2023-12-28 01:06:26.000000 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-28 01:06:26.000000 botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:58.362410 botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:58.362410 botocore-a-la-carte-rekognition-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-28 01:06:58.000000 botocore-a-la-carte-rekognition-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-rekognition-1.34.80/LICENSE.txt` & `botocore-a-la-carte-rekognition-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/PKG-INFO` & `botocore-a-la-carte-rekognition-1.34.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rekognition
-Version: 1.34.80
+Version: 1.34.9
 Summary: rekognition data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/endpoint-rule-set-1.json` & `botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/examples-1.json` & `botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/paginators-1.json` & `botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/service-2.json` & `botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8993685211049037%*

 * *Differences: {"'documentation'": "'<p>This is the API Reference for <a "*

 * *                    'href="https://docs.aws.amazon.com/rekognition/latest/dg/images.html">Amazon '*

 * *                    'Rekognition Image</a>, <a '*

 * *                    'href="https://docs.aws.amazon.com/rekognition/latest/customlabels-dg/what-is.html">Amazon '*

 * *                    'Rekognition Custom Labels</a>, <a '*

 * *                    'href="https://docs.aws.amazon.com/rekognition/latest/dg/video.html">Amazon '*

 * *                    'Rekognition Sto […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>This is the API Reference for <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/images.html\">Amazon Rekognition Image</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/customlabels-dg/what-is.html\">Amazon Rekognition Custom Labels</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/video.html\">Amazon Rekognition Stored Video</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/streaming-video.html\">Amazon Rekognition Streaming Video</a>. It provides descriptions of actions, data types, common parameters, and common errors.</p> <p> <b>Amazon Rekognition Image</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_AssociateFaces.html\">AssociateFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CompareFaces.html\">CompareFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateCollection.html\">CreateCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateUser.html\">CreateUser</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteCollection.html\">DeleteCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteFaces.html\">DeleteFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteUser.html\">DeleteUser</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeCollection.html\">DescribeCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectFaces.html\">DetectFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectLabels.html\">DetectLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectModerationLabels.html\">DetectModerationLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectProtectiveEquipment.html\">DetectProtectiveEquipment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectText.html\">DetectText</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DisassociateFaces.html\">DisassociateFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetCelebrityInfo.html\">GetCelebrityInfo</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetMediaAnalysisJob.html\">GetMediaAnalysisJob</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_IndexFaces.html\">IndexFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListCollections.html\">ListCollections</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListMediaAnalysisJob.html\">ListMediaAnalysisJob</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListFaces.html\">ListFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListFaces.html\">ListUsers</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_RecognizeCelebrities.html\">RecognizeCelebrities</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchFaces.html\">SearchFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchFacesByImage.html\">SearchFacesByImage</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsers.html\">SearchUsers</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsersByImage.html\">SearchUsersByImage</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartMediaAnalysisJob.html\">StartMediaAnalysisJob</a> </p> </li> </ul> <p> <b>Amazon Rekognition Custom Labels</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CopyProjectVersion.html\">CopyProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateDataset.html\">CreateDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateProject.html\">CreateProject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateProjectVersion.html\">CreateProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteDataset.html\">DeleteDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProject.html\">DeleteProject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProjectPolicy.html\">DeleteProjectPolicy</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProjectVersion.html\">DeleteProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeDataset.html\">DescribeDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeProjects.html\">DescribeProjects</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeProjectVersions.html\">DescribeProjectVersions</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectCustomLabels.html\">DetectCustomLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DistributeDatasetEntries.html\">DistributeDatasetEntries</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListDatasetEntries.html\">ListDatasetEntries</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListDatasetLabels.html\">ListDatasetLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListProjectPolicies.html\">ListProjectPolicies</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_PutProjectPolicy.html\">PutProjectPolicy</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartProjectVersion.html\">StartProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StopProjectVersion.html\">StopProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_UpdateDatasetEntries.html\">UpdateDatasetEntries</a> </p> </li> </ul> <p> <b>Amazon Rekognition Video Stored Video</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetCelebrityRecognition.html\">GetCelebrityRecognition</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetContentModeration.html\">GetContentModeration</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetFaceDetection.html\">GetFaceDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetFaceSearch.html\">GetFaceSearch</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetLabelDetection.html\">GetLabelDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetPersonTracking.html\">GetPersonTracking</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetSegmentDetection.html\">GetSegmentDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetTextDetection.html\">GetTextDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartCelebrityRecognition.html\">StartCelebrityRecognition</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartContentModeration.html\">StartContentModeration</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartFaceDetection.html\">StartFaceDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartFaceSearch.html\">StartFaceSearch</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartLabelDetection.html\">StartLabelDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartPersonTracking.html\">StartPersonTracking</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartSegmentDetection.html\">StartSegmentDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartTextDetection.html\">StartTextDetection</a> </p> </li> </ul> <p> <b>Amazon Rekognition Video Streaming Video</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateStreamProcessor.html\">CreateStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteStreamProcessor.html\">DeleteStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeStreamProcessor.html\">DescribeStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListStreamProcessors.html\">ListStreamProcessors</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartStreamProcessor.html\">StartStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StopStreamProcessor.html\">StopStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_UpdateStreamProcessor.html\">UpdateStreamProcessor</a> </p> </li> </ul>",
+    "documentation": "<p>This is the API Reference for <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/images.html\">Amazon Rekognition Image</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/customlabels-dg/what-is.html\">Amazon Rekognition Custom Labels</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/video.html\">Amazon Rekognition Stored Video</a>, <a href=\"https://docs.aws.amazon.com/rekognition/latest/dg/streaming-video.html\">Amazon Rekognition Streaming Video</a>. It provides descriptions of actions, data types, common parameters, and common errors.</p> <p> <b>Amazon Rekognition Image</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_AssociateFaces.html\">AssociateFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CompareFaces.html\">CompareFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateCollection.html\">CreateCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateUser.html\">CreateUser</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteCollection.html\">DeleteCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteFaces.html\">DeleteFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteUser.html\">DeleteUser</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeCollection.html\">DescribeCollection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectFaces.html\">DetectFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectLabels.html\">DetectLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectModerationLabels.html\">DetectModerationLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectProtectiveEquipment.html\">DetectProtectiveEquipment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectText.html\">DetectText</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DisassociateFaces.html\">DisassociateFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetCelebrityInfo.html\">GetCelebrityInfo</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_IndexFaces.html\">IndexFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListCollections.html\">ListCollections</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListFaces.html\">ListFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListFaces.html\">ListUsers</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_RecognizeCelebrities.html\">RecognizeCelebrities</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchFaces.html\">SearchFaces</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchFacesByImage.html\">SearchFacesByImage</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsers.html\">SearchUsers</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsersByImage.html\">SearchUsersByImage</a> </p> </li> </ul> <p> <b>Amazon Rekognition Custom Labels</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CopyProjectVersion.html\">CopyProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateDataset.html\">CreateDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateProject.html\">CreateProject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateProjectVersion.html\">CreateProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteDataset.html\">DeleteDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProject.html\">DeleteProject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProjectPolicy.html\">DeleteProjectPolicy</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteProjectVersion.html\">DeleteProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeDataset.html\">DescribeDataset</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeProjects.html\">DescribeProjects</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeProjectVersions.html\">DescribeProjectVersions</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectCustomLabels.html\">DetectCustomLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DistributeDatasetEntries.html\">DistributeDatasetEntries</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListDatasetEntries.html\">ListDatasetEntries</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListDatasetLabels.html\">ListDatasetLabels</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListProjectPolicies.html\">ListProjectPolicies</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_PutProjectPolicy.html\">PutProjectPolicy</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartProjectVersion.html\">StartProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StopProjectVersion.html\">StopProjectVersion</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_UpdateDatasetEntries.html\">UpdateDatasetEntries</a> </p> </li> </ul> <p> <b>Amazon Rekognition Video Stored Video</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetCelebrityRecognition.html\">GetCelebrityRecognition</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetContentModeration.html\">GetContentModeration</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetFaceDetection.html\">GetFaceDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetFaceSearch.html\">GetFaceSearch</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetLabelDetection.html\">GetLabelDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetPersonTracking.html\">GetPersonTracking</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetSegmentDetection.html\">GetSegmentDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_GetTextDetection.html\">GetTextDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartCelebrityRecognition.html\">StartCelebrityRecognition</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartContentModeration.html\">StartContentModeration</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartFaceDetection.html\">StartFaceDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartFaceSearch.html\">StartFaceSearch</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartLabelDetection.html\">StartLabelDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartPersonTracking.html\">StartPersonTracking</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartSegmentDetection.html\">StartSegmentDetection</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartTextDetection.html\">StartTextDetection</a> </p> </li> </ul> <p> <b>Amazon Rekognition Video Streaming Video</b> </p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateStreamProcessor.html\">CreateStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteStreamProcessor.html\">DeleteStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DescribeStreamProcessor.html\">DescribeStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListStreamProcessors.html\">ListStreamProcessors</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StartStreamProcessor.html\">StartStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_StopStreamProcessor.html\">StopStreamProcessor</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/rekognition/latest/APIReference/API_UpdateStreamProcessor.html\">UpdateStreamProcessor</a> </p> </li> </ul>",
     "metadata": {
         "apiVersion": "2016-06-27",
         "endpointPrefix": "rekognition",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceFullName": "Amazon Rekognition",
         "serviceId": "Rekognition",
@@ -879,15 +879,15 @@
             },
             "name": "DescribeStreamProcessor",
             "output": {
                 "shape": "DescribeStreamProcessorResponse"
             }
         },
         "DetectCustomLabels": {
-            "documentation": "<note> <p>This operation applies only to Amazon Rekognition Custom Labels.</p> </note> <p>Detects custom labels in a supplied image by using an Amazon Rekognition Custom Labels model. </p> <p>You specify which version of a model version to use by using the <code>ProjectVersionArn</code> input parameter. </p> <p>You pass the input image as base64-encoded image bytes or as a reference to an image in an Amazon S3 bucket. If you use the AWS CLI to call Amazon Rekognition operations, passing image bytes is not supported. The image must be either a PNG or JPEG formatted file. </p> <p> For each object that the model version detects on an image, the API returns a (<code>CustomLabel</code>) object in an array (<code>CustomLabels</code>). Each <code>CustomLabel</code> object provides the label name (<code>Name</code>), the level of confidence that the image contains the object (<code>Confidence</code>), and object location information, if it exists, for the label on the image (<code>Geometry</code>). Note that for the <code>DetectCustomLabelsLabels</code> operation, <code>Polygons</code> are not returned in the <code>Geometry</code> section of the response.</p> <p>To filter labels that are returned, specify a value for <code>MinConfidence</code>. <code>DetectCustomLabelsLabels</code> only returns labels with a confidence that's higher than the specified value. The value of <code>MinConfidence</code> maps to the assumed threshold values created during training. For more information, see <i>Assumed threshold</i> in the Amazon Rekognition Custom Labels Developer Guide. Amazon Rekognition Custom Labels metrics expresses an assumed threshold as a floating point value between 0-1. The range of <code>MinConfidence</code> normalizes the threshold value to a percentage value (0-100). Confidence responses from <code>DetectCustomLabels</code> are also returned as a percentage. You can use <code>MinConfidence</code> to change the precision and recall or your model. For more information, see <i>Analyzing an image</i> in the Amazon Rekognition Custom Labels Developer Guide. </p> <p>If you don't specify a value for <code>MinConfidence</code>, <code>DetectCustomLabels</code> returns labels based on the assumed threshold of each label.</p> <p>This is a stateless API operation. That is, the operation does not persist any data.</p> <p>This operation requires permissions to perform the <code>rekognition:DetectCustomLabels</code> action. </p> <p>For more information, see <i>Analyzing an image</i> in the Amazon Rekognition Custom Labels Developer Guide. </p>",
+            "documentation": "<note> <p>This operation applies only to Amazon Rekognition Custom Labels.</p> </note> <p>Detects custom labels in a supplied image by using an Amazon Rekognition Custom Labels model. </p> <p>You specify which version of a model version to use by using the <code>ProjectVersionArn</code> input parameter. </p> <p>You pass the input image as base64-encoded image bytes or as a reference to an image in an Amazon S3 bucket. If you use the AWS CLI to call Amazon Rekognition operations, passing image bytes is not supported. The image must be either a PNG or JPEG formatted file. </p> <p> For each object that the model version detects on an image, the API returns a (<code>CustomLabel</code>) object in an array (<code>CustomLabels</code>). Each <code>CustomLabel</code> object provides the label name (<code>Name</code>), the level of confidence that the image contains the object (<code>Confidence</code>), and object location information, if it exists, for the label on the image (<code>Geometry</code>). </p> <p>To filter labels that are returned, specify a value for <code>MinConfidence</code>. <code>DetectCustomLabelsLabels</code> only returns labels with a confidence that's higher than the specified value. The value of <code>MinConfidence</code> maps to the assumed threshold values created during training. For more information, see <i>Assumed threshold</i> in the Amazon Rekognition Custom Labels Developer Guide. Amazon Rekognition Custom Labels metrics expresses an assumed threshold as a floating point value between 0-1. The range of <code>MinConfidence</code> normalizes the threshold value to a percentage value (0-100). Confidence responses from <code>DetectCustomLabels</code> are also returned as a percentage. You can use <code>MinConfidence</code> to change the precision and recall or your model. For more information, see <i>Analyzing an image</i> in the Amazon Rekognition Custom Labels Developer Guide. </p> <p>If you don't specify a value for <code>MinConfidence</code>, <code>DetectCustomLabels</code> returns labels based on the assumed threshold of each label.</p> <p>This is a stateless API operation. That is, the operation does not persist any data.</p> <p>This operation requires permissions to perform the <code>rekognition:DetectCustomLabels</code> action. </p> <p>For more information, see <i>Analyzing an image</i> in the Amazon Rekognition Custom Labels Developer Guide. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ResourceNotReadyException"
                 },
@@ -3014,15 +3014,15 @@
                 "FaceIds"
             ],
             "type": "structure"
         },
         "AssociateFacesResponse": {
             "members": {
                 "AssociatedFaces": {
-                    "documentation": "<p>An array of AssociatedFace objects containing FaceIDs that have been successfully associated with the UserID. Returned if the AssociateFaces action is successful.</p>",
+                    "documentation": "<p>An array of AssociatedFace objects containing FaceIDs that are successfully associated with the UserID is returned. Returned if the AssociateFaces action is successful.</p>",
                     "shape": "AssociatedFacesList"
                 },
                 "UnsuccessfulFaceAssociations": {
                     "documentation": "<p>An array of UnsuccessfulAssociation objects containing FaceIDs that are not successfully associated along with the reasons. Returned if the AssociateFaces action is successful.</p>",
                     "shape": "UnsuccessfulFaceAssociationList"
                 },
                 "UserStatus": {
@@ -3556,36 +3556,14 @@
         "ContentModerationSortBy": {
             "enum": [
                 "NAME",
                 "TIMESTAMP"
             ],
             "type": "string"
         },
-        "ContentType": {
-            "documentation": "<p>Contains information regarding the confidence and name of a detected content type.</p>",
-            "members": {
-                "Confidence": {
-                    "documentation": "<p>The confidence level of the label given</p>",
-                    "shape": "Percent"
-                },
-                "Name": {
-                    "documentation": "<p>The name of the label</p>",
-                    "shape": "String"
-                }
-            },
-            "type": "structure"
-        },
-        "ContentTypes": {
-            "max": 50,
-            "member": {
-                "shape": "ContentType"
-            },
-            "min": 0,
-            "type": "list"
-        },
         "CopyProjectVersionRequest": {
             "members": {
                 "DestinationProjectArn": {
                     "documentation": "<p>The ARN of the project in the trusted AWS account that you want to copy the model version to. </p>",
                     "shape": "ProjectArn"
                 },
                 "KmsKeyId": {
@@ -4817,18 +4795,14 @@
             "required": [
                 "Image"
             ],
             "type": "structure"
         },
         "DetectModerationLabelsResponse": {
             "members": {
-                "ContentTypes": {
-                    "documentation": "<p>A list of predicted results for the type of content an image contains. For example, the image content might be from animation, sports, or a video game.</p>",
-                    "shape": "ContentTypes"
-                },
                 "HumanLoopActivationOutput": {
                     "documentation": "<p>Shows the results of the human in the loop evaluation.</p>",
                     "shape": "HumanLoopActivationOutput"
                 },
                 "ModerationLabels": {
                     "documentation": "<p>Array of detected Moderation labels and the time, in milliseconds from the start of the video, they were detected.</p>",
                     "shape": "ModerationLabels"
@@ -7340,24 +7314,14 @@
             "members": {
                 "S3Object": {
                     "shape": "S3Object"
                 }
             },
             "type": "structure"
         },
-        "MediaAnalysisModelVersions": {
-            "documentation": "<p>Object containing information about the model versions of selected features in a given job.</p>",
-            "members": {
-                "Moderation": {
-                    "documentation": "<p>The Moderation base model version.</p>",
-                    "shape": "String"
-                }
-            },
-            "type": "structure"
-        },
         "MediaAnalysisOperationsConfig": {
             "documentation": "<p>Configuration options for a media analysis job. Configuration is operation-specific.</p>",
             "members": {
                 "DetectModerationLabels": {
                     "documentation": "<p>Contains configuration options for a DetectModerationLabels job.</p>",
                     "shape": "MediaAnalysisDetectModerationLabelsConfig"
                 }
@@ -7380,18 +7344,14 @@
                 "S3Bucket"
             ],
             "type": "structure"
         },
         "MediaAnalysisResults": {
             "documentation": "<p>Contains the results for a media analysis job created with StartMediaAnalysisJob.</p>",
             "members": {
-                "ModelVersions": {
-                    "documentation": "<p>Information about the model versions for the features selected in a given job.</p>",
-                    "shape": "MediaAnalysisModelVersions"
-                },
                 "S3Object": {
                     "shape": "S3Object"
                 }
             },
             "type": "structure"
         },
         "MediaAnalysisS3KeyPrefix": {
@@ -7414,18 +7374,14 @@
                 "Name": {
                     "documentation": "<p>The label name for the type of unsafe content detected in the image.</p>",
                     "shape": "String"
                 },
                 "ParentName": {
                     "documentation": "<p>The name for the parent label. Labels at the top level of the hierarchy have the parent label <code>\"\"</code>.</p>",
                     "shape": "String"
-                },
-                "TaxonomyLevel": {
-                    "documentation": "<p>The level of the moderation label with regard to its taxonomy, from 1 to 3.</p>",
-                    "shape": "UInteger"
                 }
             },
             "type": "structure"
         },
         "ModerationLabels": {
             "member": {
                 "shape": "ModerationLabel"
```

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore/data/rekognition/2016-06-27/waiters-2.json` & `botocore-a-la-carte-rekognition-1.34.9/botocore/data/rekognition/2016-06-27/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/PKG-INFO` & `botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rekognition
-Version: 1.34.80
+Version: 1.34.9
 Summary: rekognition data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rekognition-1.34.80/botocore_a_la_carte_rekognition.egg-info/SOURCES.txt` & `botocore-a-la-carte-rekognition-1.34.9/botocore_a_la_carte_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rekognition-1.34.80/setup.py` & `botocore-a-la-carte-rekognition-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-rekognition',
-    version="1.34.80",
+    version="1.34.9",
     description='rekognition data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/rekognition/*/*.json'],
```

