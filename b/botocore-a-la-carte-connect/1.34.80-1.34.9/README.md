# Comparing `tmp/botocore-a-la-carte-connect-1.34.80.tar.gz` & `tmp/botocore-a-la-carte-connect-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-connect-1.34.80.tar", last modified: Tue Apr  9 01:00:34 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-connect-1.34.9.tar", last modified: Thu Dec 28 01:06:37 2023, max compression
```

## Comparing `botocore-a-la-carte-connect-1.34.80.tar` & `botocore-a-la-carte-connect-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.748043 botocore-a-la-carte-connect-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-09 01:00:34.748043 botocore-a-la-carte-connect-1.34.80/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.744043 botocore-a-la-carte-connect-1.34.80/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.744043 botocore-a-la-carte-connect-1.34.80/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.744043 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.744043 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/
--rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-04-09 01:00:23.000000 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 01:00:23.000000 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-04-09 01:00:23.000000 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   938892 2024-04-09 01:00:23.000000 botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:00:34.748043 botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:00:34.748043 botocore-a-la-carte-connect-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 01:00:34.000000 botocore-a-la-carte-connect-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.518246 botocore-a-la-carte-connect-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:06:37.518246 botocore-a-la-carte-connect-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.514246 botocore-a-la-carte-connect-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.514246 botocore-a-la-carte-connect-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.514246 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.514246 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/
+-rw-r--r--   0 runner    (1001) docker     (127)    15297 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10783 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   910649 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.518246 botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:37.518246 botocore-a-la-carte-connect-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-connect-1.34.80/LICENSE.txt` & `botocore-a-la-carte-connect-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-1.34.80/PKG-INFO` & `botocore-a-la-carte-connect-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connect
-Version: 1.34.80
+Version: 1.34.9
 Summary: connect data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/endpoint-rule-set-1.json` & `botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/paginators-1.json` & `botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-1.34.80/botocore/data/connect/2017-08-08/service-2.json` & `botocore-a-la-carte-connect-1.34.9/botocore/data/connect/2017-08-08/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992369557819633%*

 * *Differences: {"'operations'": "{'DeleteQuickConnect': {'documentation': '<p>Deletes a quick connect.</p>'}, "*

 * *                 "'DeleteUser': {'documentation': '<p>Deletes a user account from the specified "*

 * *                 "Amazon Connect instance.</p> <p>For information about what happens to a user\\'s "*

 * *                 'data when their account is deleted, see <a '*

 * *                 'href="https://docs.aws.amazon.com/connect/latest/adminguide/delete-users.html">Delete '*

 * *                 'Users from Your Amazon Connec […]*

```diff
@@ -1858,15 +1858,15 @@
             },
             "input": {
                 "shape": "DeleteQueueRequest"
             },
             "name": "DeleteQueue"
         },
         "DeleteQuickConnect": {
-            "documentation": "<p>Deletes a quick connect. </p> <important> <p>After calling <a href=\"https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteUser.html\">DeleteUser</a>, it's important to call <code>DeleteQuickConnect</code> to delete any records related to the deleted users. This will help you:</p> <ul> <li> <p>Avoid dangling resources that impact your service quotas.</p> </li> <li> <p>Remove deleted users so they don't appear to agents as transfer options.</p> </li> <li> <p>Avoid the disruption of other Amazon Connect processes, such as instance replication and syncing if you're using <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/setup-connect-global-resiliency.html\">Amazon Connect Global Resiliency</a>. </p> </li> </ul> </important>",
+            "documentation": "<p>Deletes a quick connect.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InvalidParameterException"
                 },
@@ -2066,15 +2066,15 @@
             },
             "input": {
                 "shape": "DeleteUseCaseRequest"
             },
             "name": "DeleteUseCase"
         },
         "DeleteUser": {
-            "documentation": "<p>Deletes a user account from the specified Amazon Connect instance.</p> <p>For information about what happens to a user's data when their account is deleted, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/delete-users.html\">Delete Users from Your Amazon Connect Instance</a> in the <i>Amazon Connect Administrator Guide</i>.</p> <important> <p>After calling DeleteUser, call <a href=\"https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteQuickConnect.html\">DeleteQuickConnect</a> to delete any records related to the deleted users. This will help you:</p> <ul> <li> <p>Avoid dangling resources that impact your service quotas.</p> </li> <li> <p>Remove deleted users so they don't appear to agents as transfer options.</p> </li> <li> <p>Avoid the disruption of other Amazon Connect processes, such as instance replication and syncing if you're using <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/setup-connect-global-resiliency.html\">Amazon Connect Global Resiliency</a>. </p> </li> </ul> </important>",
+            "documentation": "<p>Deletes a user account from the specified Amazon Connect instance.</p> <p>For information about what happens to a user's data when their account is deleted, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/delete-users.html\">Delete Users from Your Amazon Connect Instance</a> in the <i>Amazon Connect Administrator Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InvalidParameterException"
                 },
@@ -3940,15 +3940,15 @@
             },
             "name": "ListContactFlows",
             "output": {
                 "shape": "ListContactFlowsResponse"
             }
         },
         "ListContactReferences": {
-            "documentation": "<p>This API is in preview release for Amazon Connect and is subject to change.</p> <p>For the specified <code>referenceTypes</code>, returns a list of references associated with the contact. <i>References</i> are links to documents that are related to a contact, such as emails, attachments, or URLs.</p>",
+            "documentation": "<p>This API is in preview release for Amazon Connect and is subject to change.</p> <p>For the specified <code>referenceTypes</code>, returns a list of references associated with the contact. </p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InvalidParameterException"
                 },
@@ -5946,15 +5946,15 @@
             },
             "name": "StartWebRTCContact",
             "output": {
                 "shape": "StartWebRTCContactResponse"
             }
         },
         "StopContact": {
-            "documentation": "<p>Ends the specified contact. Use this API to stop queued callbacks. It does not work for voice contacts that use the following initiation methods:</p> <ul> <li> <p>DISCONNECT</p> </li> <li> <p>TRANSFER</p> </li> <li> <p>QUEUE_TRANSFER</p> </li> </ul> <p>Chat and task contacts can be terminated in any state, regardless of initiation method.</p>",
+            "documentation": "<p>Ends the specified contact. This call does not work for voice contacts that use the following initiation methods:</p> <ul> <li> <p>DISCONNECT</p> </li> <li> <p>TRANSFER</p> </li> <li> <p>QUEUE_TRANSFER</p> </li> </ul> <p>Chat and task contacts, however, can be terminated in any state, regardless of initiation method.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "ContactNotFoundException"
                 },
@@ -7800,15 +7800,15 @@
             ],
             "type": "structure"
         },
         "AgentContactReference": {
             "documentation": "<p>Information about the <a href=\"https://docs.aws.amazon.com/connect/latest/APIReference/API_Contact.html\">contact</a> associated to the user.</p>",
             "members": {
                 "AgentContactState": {
-                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/about-contact-states.html\">state of the contact</a>.</p> <note> <p>When <code>AgentContactState</code> is set to <code>CONNECTED_ONHOLD</code>, <code>StateStartTimestamp</code> is not changed. Instead, <code>StateStartTimestamp</code> reflects the time the contact was <code>CONNECTED</code> to the agent.</p> </note>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/about-contact-states.html\">state of the contact</a>.</p>",
                     "shape": "ContactState"
                 },
                 "Channel": {
                     "documentation": "<p>The channel of the contact.</p>",
                     "shape": "Channel"
                 },
                 "ConnectedToAgentTimestamp": {
@@ -7838,19 +7838,18 @@
                 "shape": "AgentContactReference"
             },
             "type": "list"
         },
         "AgentFirstName": {
             "max": 100,
             "min": 1,
-            "sensitive": true,
             "type": "string"
         },
         "AgentHierarchyGroups": {
-            "documentation": "<p>A structure that defines search criteria for contacts using agent hierarchy group levels. For more information about agent hierarchies, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/agent-hierarchy.html\">Set Up Agent Hierarchies</a> in the <i>Amazon Connect Administrator Guide</i>.</p>",
+            "documentation": "<p>A structure that defines agent hierarchy group levels which can be used to filter search results. Important: Agent hierarchy group level information in search result is a snapshot, it does not represent current agent hierarchy who handled the contact.</p>",
             "members": {
                 "L1Ids": {
                     "documentation": "<p>The identifiers for level 1 hierarchy groups.</p>",
                     "shape": "HierarchyGroupIdList"
                 },
                 "L2Ids": {
                     "documentation": "<p>The identifiers for level 2 hierarchy groups.</p>",
@@ -7888,15 +7887,14 @@
                 }
             },
             "type": "structure"
         },
         "AgentLastName": {
             "max": 100,
             "min": 1,
-            "sensitive": true,
             "type": "string"
         },
         "AgentPauseDurationInSeconds": {
             "min": 0,
             "type": "integer"
         },
         "AgentResourceId": {
@@ -8344,15 +8342,15 @@
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "location": "uri",
                     "locationName": "InstanceId",
                     "shape": "InstanceId"
                 },
                 "ResourceType": {
-                    "documentation": "<p>A valid resource type. To <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/enable-contact-analysis-segment-streams.html\">enable streaming for real-time analysis of contacts</a>, use the following types:</p> <ul> <li> <p>For chat contacts, use <code>REAL_TIME_CONTACT_ANALYSIS_CHAT_SEGMENTS</code>.</p> </li> <li> <p>For voice contacts, use <code>REAL_TIME_CONTACT_ANALYSIS_VOICE_SEGMENTS</code>.</p> </li> </ul> <note> <p> <code>REAL_TIME_CONTACT_ANALYSIS_SEGMENTS</code> is deprecated, but it is still supported and will apply only to VOICE channel contacts. Use <code>REAL_TIME_CONTACT_ANALYSIS_VOICE_SEGMENTS</code> for voice contacts moving forward.</p> <p>If you have previously associated a stream with <code>REAL_TIME_CONTACT_ANALYSIS_SEGMENTS</code>, no action is needed to update the stream to <code>REAL_TIME_CONTACT_ANALYSIS_VOICE_SEGMENTS</code>.</p> </note>",
+                    "documentation": "<p>A valid resource type.</p>",
                     "shape": "InstanceStorageResourceType"
                 },
                 "StorageConfig": {
                     "documentation": "<p>A valid storage type.</p>",
                     "shape": "InstanceStorageConfig"
                 }
             },
@@ -8623,38 +8621,19 @@
                 "Value": {
                     "documentation": "<p>The value of the attribute.</p>",
                     "shape": "InstanceAttributeValue"
                 }
             },
             "type": "structure"
         },
-        "AttributeAndCondition": {
-            "documentation": "<p>A list of conditions which would be applied together with an <code>AND</code> condition.</p>",
-            "members": {
-                "HierarchyGroupCondition": {
-                    "shape": "HierarchyGroupCondition"
-                },
-                "TagConditions": {
-                    "documentation": "<p>A leaf node condition which can be used to specify a tag condition.</p>",
-                    "shape": "TagAndConditionList"
-                }
-            },
-            "type": "structure"
-        },
         "AttributeName": {
             "max": 32767,
             "min": 1,
             "type": "string"
         },
-        "AttributeOrConditionList": {
-            "member": {
-                "shape": "AttributeAndCondition"
-            },
-            "type": "list"
-        },
         "AttributeValue": {
             "max": 32767,
             "min": 0,
             "type": "string"
         },
         "Attributes": {
             "key": {
@@ -9253,18 +9232,18 @@
                     "documentation": "<p>Information about Amazon Connect Wisdom.</p>",
                     "shape": "WisdomInfo"
                 }
             },
             "type": "structure"
         },
         "ContactAnalysis": {
-            "documentation": "<p>A structure that defines search criteria for contacts using analysis outputs from Amazon Connect Contact Lens.</p>",
+            "documentation": "<p>A structure that defines filters can be used to search within outputs analyzed by Amazon Connect Contact Lens in a contact.</p>",
             "members": {
                 "Transcript": {
-                    "documentation": "<p>Search criteria based on transcript analyzed by Amazon Connect Contact Lens.</p>",
+                    "documentation": "<p>A structure that defines filters can be used to search with text within an Amazon Connect Contact Lens analyzed transcript.</p>",
                     "shape": "Transcript"
                 }
             },
             "type": "structure"
         },
         "ContactDataRequest": {
             "documentation": "<p>Request object with information to create a contact.</p>",
@@ -9587,15 +9566,15 @@
             "documentation": "<p>Information of returned contact.</p>",
             "members": {
                 "AgentInfo": {
                     "documentation": "<p>Information about the agent who accepted the contact.</p>",
                     "shape": "ContactSearchSummaryAgentInfo"
                 },
                 "Arn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the contact.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the contact</p>",
                     "shape": "ARN"
                 },
                 "Channel": {
                     "documentation": "<p>How the contact reached your contact center.</p>",
                     "shape": "Channel"
                 },
                 "DisconnectTimestamp": {
@@ -9611,15 +9590,15 @@
                     "shape": "ContactId"
                 },
                 "InitiationMethod": {
                     "documentation": "<p>Indicates how the contact was initiated.</p>",
                     "shape": "ContactInitiationMethod"
                 },
                 "InitiationTimestamp": {
-                    "documentation": "<p>The date and time this contact was initiated, in UTC time. For <code>INBOUND</code>, this is when the contact arrived. For <code>OUTBOUND</code>, this is when the agent began dialing. For <code>CALLBACK</code>, this is when the callback contact was created. For <code>TRANSFER</code> and <code>QUEUE_TRANSFER</code>, this is when the transfer was initiated. For API, this is when the request arrived. For <code>EXTERNAL_OUTBOUND</code>, this is when the agent started dialing the external participant. For <code>MONITOR</code>, this is when the supervisor started listening to a contact.</p>",
+                    "documentation": "<p>The date and time this contact was initiated, in UTC time. For INBOUND, this is when the contact arrived. For OUTBOUND, this is when the agent began dialing. For CALLBACK, this is when the callback contact was created. For TRANSFER and QUEUE_TRANSFER, this is when the transfer was initiated. For API, this is when the request arrived. For EXTERNAL_OUTBOUND, this is when the agent started dialing the external participant. For MONITOR, this is when the supervisor started listening to a contact.</p>",
                     "shape": "timestamp"
                 },
                 "PreviousContactId": {
                     "documentation": "<p>If this contact is not the first contact, this is the ID of the previous contact.</p>",
                     "shape": "ContactId"
                 },
                 "QueueInfo": {
@@ -9741,34 +9720,14 @@
                 "TagCondition": {
                     "documentation": "<p>A leaf node condition which can be used to specify a tag condition. </p>",
                     "shape": "TagCondition"
                 }
             },
             "type": "structure"
         },
-        "ControlPlaneUserAttributeFilter": {
-            "documentation": "<p>An object that can be used to specify Tag conditions or Hierarchy Group conditions inside the <code>SearchFilter</code>.</p> <p>This accepts an <code>OR</code> of <code>AND</code> (List of List) input where:</p> <ul> <li> <p>The top level list specifies conditions that need to be applied with <code>OR</code> operator</p> </li> <li> <p>The inner list specifies conditions that need to be applied with <code>AND</code> operator.</p> </li> </ul> <note> <p>Only one field can be populated. Maximum number of allowed Tag conditions is 25. Maximum number of allowed Hierarchy Group conditions is 20. </p> </note>",
-            "members": {
-                "AndCondition": {
-                    "documentation": "<p>A list of conditions which would be applied together with an <code>AND</code> condition.</p>",
-                    "shape": "AttributeAndCondition"
-                },
-                "HierarchyGroupCondition": {
-                    "shape": "HierarchyGroupCondition"
-                },
-                "OrConditions": {
-                    "documentation": "<p>A list of conditions which would be applied together with an <code>OR</code> condition.</p>",
-                    "shape": "AttributeOrConditionList"
-                },
-                "TagCondition": {
-                    "shape": "TagCondition"
-                }
-            },
-            "type": "structure"
-        },
         "CreateAgentStatusRequest": {
             "members": {
                 "Description": {
                     "documentation": "<p>The description of the status.</p>",
                     "shape": "AgentStatusDescription"
                 },
                 "DisplayOrder": {
@@ -10521,34 +10480,26 @@
             "max": 127,
             "min": 1,
             "pattern": "^[ a-zA-Z0-9_@-]+$",
             "type": "string"
         },
         "CreateSecurityProfileRequest": {
             "members": {
-                "AllowedAccessControlHierarchyGroupId": {
-                    "documentation": "<p>The identifier of the hierarchy group that a security profile uses to restrict access to resources in Amazon Connect.</p>",
-                    "shape": "HierarchyGroupId"
-                },
                 "AllowedAccessControlTags": {
                     "documentation": "<p>The list of tags that a security profile uses to restrict access to resources in Amazon Connect.</p>",
                     "shape": "AllowedAccessControlTags"
                 },
                 "Applications": {
                     "documentation": "<p>This API is in preview release for Amazon Connect and is subject to change.</p> <p>A list of third-party applications that the security profile will give access to.</p>",
                     "shape": "Applications"
                 },
                 "Description": {
                     "documentation": "<p>The description of the security profile.</p>",
                     "shape": "SecurityProfileDescription"
                 },
-                "HierarchyRestrictedResources": {
-                    "documentation": "<p>The list of resources that a security profile applies hierarchy restrictions to in Amazon Connect. Following are acceptable ResourceNames: <code>User</code>.</p>",
-                    "shape": "HierarchyRestrictedResourceList"
-                },
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "location": "uri",
                     "locationName": "InstanceId",
                     "shape": "InstanceId"
                 },
                 "Permissions": {
@@ -10816,15 +10767,15 @@
                     "shape": "SecurityProfileIds"
                 },
                 "Tags": {
                     "documentation": "<p>The tags used to organize, track, or control access for this resource. For example, { \"Tags\": {\"key1\":\"value1\", \"key2\":\"value2\"} }.</p>",
                     "shape": "TagMap"
                 },
                 "Username": {
-                    "documentation": "<p>The user name for the account. For instances not using SAML for identity management, the user name can include up to 20 characters. If you are using SAML for identity management, the user name can include up to 64 characters from [a-zA-Z0-9_-.\\@]+.</p> <p>Username can include @ only if used in an email format. For example:</p> <ul> <li> <p>Correct: testuser</p> </li> <li> <p>Correct: testuser@example.com</p> </li> <li> <p>Incorrect: testuser@example</p> </li> </ul>",
+                    "documentation": "<p>The user name for the account. For instances not using SAML for identity management, the user name can include up to 20 characters. If you are using SAML for identity management, the user name can include up to 64 characters from [a-zA-Z0-9_-.\\@]+.</p>",
                     "shape": "AgentUsername"
                 }
             },
             "required": [
                 "Username",
                 "PhoneConfig",
                 "SecurityProfileIds",
@@ -11010,15 +10961,14 @@
                     "shape": "SecurityToken"
                 },
                 "RefreshTokenExpiration": {
                     "documentation": "<p>Renews the expiration timer for a generated token.</p>",
                     "shape": "timestamp"
                 }
             },
-            "sensitive": true,
             "type": "structure"
         },
         "CrossChannelBehavior": {
             "documentation": "<p>Defines the cross-channel routing behavior that allows an agent working on a contact in one channel to be offered a contact from a different channel.</p>",
             "members": {
                 "BehaviorType": {
                     "documentation": "<p>Specifies the other channels that can be routed to an agent handling their current channel.</p>",
@@ -12480,15 +12430,14 @@
                 "Vocabulary"
             ],
             "type": "structure"
         },
         "Description": {
             "max": 4096,
             "min": 0,
-            "sensitive": true,
             "type": "string"
         },
         "Description250": {
             "max": 250,
             "min": 1,
             "pattern": "(^[\\S].*[\\S]$)|(^[\\S]$)",
             "type": "string"
@@ -12983,15 +12932,14 @@
                 "Message": {
                     "shape": "Message"
                 }
             },
             "type": "structure"
         },
         "Email": {
-            "sensitive": true,
             "type": "string"
         },
         "EmailReference": {
             "documentation": "<p>Information about a reference when the <code>referenceType</code> is <code>EMAIL</code>. Otherwise, null.</p>",
             "members": {
                 "Name": {
                     "documentation": "<p>Identifier of the email reference.</p>",
@@ -13847,22 +13795,22 @@
             ],
             "type": "structure"
         },
         "EvaluationNote": {
             "documentation": "<p>Information about notes for a contact evaluation.</p>",
             "members": {
                 "Value": {
-                    "documentation": "<p>The note for an item (section or question) in a contact evaluation.</p> <note> <p>Even though a note in an evaluation can have up to 3072 chars, there is also a limit on the total number of chars for all the notes in the evaluation combined. Assuming there are N questions in the evaluation being submitted, then the max char limit for all notes combined is N x 1024.</p> </note>",
+                    "documentation": "<p>The note for an item (section or question) in a contact evaluation.</p>",
                     "shape": "EvaluationNoteString"
                 }
             },
             "type": "structure"
         },
         "EvaluationNoteString": {
-            "max": 3072,
+            "max": 1024,
             "min": 0,
             "type": "string"
         },
         "EvaluationNotesMap": {
             "key": {
                 "shape": "ResourceId"
             },
@@ -14221,23 +14169,23 @@
                 }
             },
             "type": "structure"
         },
         "GetCurrentMetricDataRequest": {
             "members": {
                 "CurrentMetrics": {
-                    "documentation": "<p>The metrics to retrieve. Specify the name and unit for each metric. The following metrics are available. For a description of all the metrics, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html\">Real-time Metrics Definitions</a> in the <i>Amazon Connect Administrator Guide</i>.</p> <dl> <dt>AGENTS_AFTER_CONTACT_WORK</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#aftercallwork-real-time\">ACW</a> </p> </dd> <dt>AGENTS_AVAILABLE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#available-real-time\">Available</a> </p> </dd> <dt>AGENTS_ERROR</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#error-real-time\">Error</a> </p> </dd> <dt>AGENTS_NON_PRODUCTIVE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#non-productive-time-real-time\">NPT (Non-Productive Time)</a> </p> </dd> <dt>AGENTS_ON_CALL</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#on-call-real-time\">On contact</a> </p> </dd> <dt>AGENTS_ON_CONTACT</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#on-call-real-time\">On contact</a> </p> </dd> <dt>AGENTS_ONLINE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#online-real-time\">Online</a> </p> </dd> <dt>AGENTS_STAFFED</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#staffed-real-time\">Staffed</a> </p> </dd> <dt>CONTACTS_IN_QUEUE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#in-queue-real-time\">In queue</a> </p> </dd> <dt>CONTACTS_SCHEDULED</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#scheduled-real-time\">Scheduled</a> </p> </dd> <dt>OLDEST_CONTACT_AGE</dt> <dd> <p>Unit: SECONDS</p> <p>When you use groupings, Unit says SECONDS and the Value is returned in SECONDS. </p> <p>When you do not use groupings, Unit says SECONDS but the Value is returned in MILLISECONDS. For example, if you get a response like this:</p> <p> <code>{ \"Metric\": { \"Name\": \"OLDEST_CONTACT_AGE\", \"Unit\": \"SECONDS\" }, \"Value\": 24113.0 </code>}</p> <p>The actual OLDEST_CONTACT_AGE is 24 seconds.</p> <p>When the filter <code>RoutingStepExpression</code> is used, this metric is still calculated from enqueue time. For example, if a contact that has been queued under <code>&lt;Expression 1&gt;</code> for 10 seconds has expired and <code>&lt;Expression 2&gt;</code> becomes active, then <code>OLDEST_CONTACT_AGE</code> for this queue will be counted starting from 10, not 0.</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#oldest-real-time\">Oldest</a> </p> </dd> <dt>SLOTS_ACTIVE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#active-real-time\">Active</a> </p> </dd> <dt>SLOTS_AVAILABLE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#availability-real-time\">Availability</a> </p> </dd> </dl>",
+                    "documentation": "<p>The metrics to retrieve. Specify the name and unit for each metric. The following metrics are available. For a description of all the metrics, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html\">Real-time Metrics Definitions</a> in the <i>Amazon Connect Administrator Guide</i>.</p> <dl> <dt>AGENTS_AFTER_CONTACT_WORK</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#aftercallwork-real-time\">ACW</a> </p> </dd> <dt>AGENTS_AVAILABLE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#available-real-time\">Available</a> </p> </dd> <dt>AGENTS_ERROR</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#error-real-time\">Error</a> </p> </dd> <dt>AGENTS_NON_PRODUCTIVE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#non-productive-time-real-time\">NPT (Non-Productive Time)</a> </p> </dd> <dt>AGENTS_ON_CALL</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#on-call-real-time\">On contact</a> </p> </dd> <dt>AGENTS_ON_CONTACT</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#on-call-real-time\">On contact</a> </p> </dd> <dt>AGENTS_ONLINE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#online-real-time\">Online</a> </p> </dd> <dt>AGENTS_STAFFED</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#staffed-real-time\">Staffed</a> </p> </dd> <dt>CONTACTS_IN_QUEUE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#in-queue-real-time\">In queue</a> </p> </dd> <dt>CONTACTS_SCHEDULED</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#scheduled-real-time\">Scheduled</a> </p> </dd> <dt>OLDEST_CONTACT_AGE</dt> <dd> <p>Unit: SECONDS</p> <p>When you use groupings, Unit says SECONDS and the Value is returned in SECONDS. </p> <p>When you do not use groupings, Unit says SECONDS but the Value is returned in MILLISECONDS. For example, if you get a response like this:</p> <p> <code>{ \"Metric\": { \"Name\": \"OLDEST_CONTACT_AGE\", \"Unit\": \"SECONDS\" }, \"Value\": 24113.0 </code>}</p> <p>The actual OLDEST_CONTACT_AGE is 24 seconds.</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#oldest-real-time\">Oldest</a> </p> </dd> <dt>SLOTS_ACTIVE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#active-real-time\">Active</a> </p> </dd> <dt>SLOTS_AVAILABLE</dt> <dd> <p>Unit: COUNT</p> <p>Name in real-time metrics report: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/real-time-metrics-definitions.html#availability-real-time\">Availability</a> </p> </dd> </dl>",
                     "shape": "CurrentMetrics"
                 },
                 "Filters": {
-                    "documentation": "<p>The filters to apply to returned metrics. You can filter up to the following limits:</p> <ul> <li> <p>Queues: 100</p> </li> <li> <p>Routing profiles: 100</p> </li> <li> <p>Channels: 3 (VOICE, CHAT, and TASK channels are supported.)</p> </li> <li> <p>RoutingStepExpressions: 50</p> </li> </ul> <p>Metric data is retrieved only for the resources associated with the queues or routing profiles, and by any channels included in the filter. (You cannot filter by both queue AND routing profile.) You can include both resource IDs and resource ARNs in the same request.</p> <p>When using the <code>RoutingStepExpression</code> filter, you need to pass exactly one <code>QueueId</code>. The filter is also case sensitive so when using the <code>RoutingStepExpression</code> filter, grouping by <code>ROUTING_STEP_EXPRESSION</code> is required.</p> <p>Currently tagging is only supported on the resources that are passed in the filter.</p>",
+                    "documentation": "<p>The filters to apply to returned metrics. You can filter up to the following limits:</p> <ul> <li> <p>Queues: 100</p> </li> <li> <p>Routing profiles: 100</p> </li> <li> <p>Channels: 3 (VOICE, CHAT, and TASK channels are supported.)</p> </li> </ul> <p>Metric data is retrieved only for the resources associated with the queues or routing profiles, and by any channels included in the filter. (You cannot filter by both queue AND routing profile.) You can include both resource IDs and resource ARNs in the same request. </p> <p>Currently tagging is only supported on the resources that are passed in the filter.</p>",
                     "shape": "Filters"
                 },
                 "Groupings": {
-                    "documentation": "<p>The grouping applied to the metrics returned. For example, when grouped by <code>QUEUE</code>, the metrics returned apply to each queue rather than aggregated for all queues. </p> <ul> <li> <p>If you group by <code>CHANNEL</code>, you should include a Channels filter. VOICE, CHAT, and TASK channels are supported.</p> </li> <li> <p>If you group by <code>ROUTING_PROFILE</code>, you must include either a queue or routing profile filter. In addition, a routing profile filter is required for metrics <code>CONTACTS_SCHEDULED</code>, <code>CONTACTS_IN_QUEUE</code>, and <code> OLDEST_CONTACT_AGE</code>.</p> </li> <li> <p>If no <code>Grouping</code> is included in the request, a summary of metrics is returned.</p> </li> <li> <p>When using the <code>RoutingStepExpression</code> filter, group by <code>ROUTING_STEP_EXPRESSION</code> is required.</p> </li> </ul>",
+                    "documentation": "<p>The grouping applied to the metrics returned. For example, when grouped by <code>QUEUE</code>, the metrics returned apply to each queue rather than aggregated for all queues. </p> <ul> <li> <p>If you group by <code>CHANNEL</code>, you should include a Channels filter. VOICE, CHAT, and TASK channels are supported.</p> </li> <li> <p>If you group by <code>ROUTING_PROFILE</code>, you must include either a queue or routing profile filter. In addition, a routing profile filter is required for metrics <code>CONTACTS_SCHEDULED</code>, <code>CONTACTS_IN_QUEUE</code>, and <code> OLDEST_CONTACT_AGE</code>.</p> </li> <li> <p>If no <code>Grouping</code> is included in the request, a summary of metrics is returned.</p> </li> </ul>",
                     "shape": "Groupings"
                 },
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "location": "uri",
                     "locationName": "InstanceId",
                     "shape": "InstanceId"
@@ -14412,19 +14360,19 @@
         "GetMetricDataRequest": {
             "members": {
                 "EndTime": {
                     "documentation": "<p>The timestamp, in UNIX Epoch time format, at which to end the reporting interval for the retrieval of historical metrics data. The time must be specified using an interval of 5 minutes, such as 11:00, 11:05, 11:10, and must be later than the start time timestamp.</p> <p>The time range between the start and end time must be less than 24 hours.</p>",
                     "shape": "timestamp"
                 },
                 "Filters": {
-                    "documentation": "<p>The queues, up to 100, or channels, to use to filter the metrics returned. Metric data is retrieved only for the resources associated with the queues or channels included in the filter. You can include both queue IDs and queue ARNs in the same request. VOICE, CHAT, and TASK channels are supported.</p> <p>RoutingStepExpression is not a valid filter for GetMetricData and we recommend switching to GetMetricDataV2 for more up-to-date features.</p> <note> <p>To filter by <code>Queues</code>, enter the queue ID/ARN, not the name of the queue.</p> </note>",
+                    "documentation": "<p>The queues, up to 100, or channels, to use to filter the metrics returned. Metric data is retrieved only for the resources associated with the queues or channels included in the filter. You can include both queue IDs and queue ARNs in the same request. VOICE, CHAT, and TASK channels are supported.</p> <note> <p>To filter by <code>Queues</code>, enter the queue ID/ARN, not the name of the queue.</p> </note>",
                     "shape": "Filters"
                 },
                 "Groupings": {
-                    "documentation": "<p>The grouping applied to the metrics returned. For example, when results are grouped by queue, the metrics returned are grouped by queue. The values returned apply to the metrics for each queue rather than aggregated for all queues.</p> <p>If no grouping is specified, a summary of metrics for all queues is returned.</p> <p>RoutingStepExpression is not a valid filter for GetMetricData and we recommend switching to GetMetricDataV2 for more up-to-date features.</p>",
+                    "documentation": "<p>The grouping applied to the metrics returned. For example, when results are grouped by queue, the metrics returned are grouped by queue. The values returned apply to the metrics for each queue rather than aggregated for all queues.</p> <p>If no grouping is specified, a summary of metrics for all queues is returned.</p>",
                     "shape": "Groupings"
                 },
                 "HistoricalMetrics": {
                     "documentation": "<p>The metrics to retrieve. Specify the name, unit, and statistic for each metric. The following historical metrics are available. For a description of each metric, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html\">Historical Metrics Definitions</a> in the <i>Amazon Connect Administrator Guide</i>.</p> <note> <p>This API does not support a contacts incoming metric (there's no CONTACTS_INCOMING metric missing from the documented list). </p> </note> <dl> <dt>ABANDON_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>AFTER_CONTACT_WORK_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>API_CONTACTS_HANDLED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CALLBACK_CONTACTS_HANDLED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_ABANDONED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_AGENT_HUNG_UP_FIRST</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_CONSULTED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_HANDLED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_HANDLED_INCOMING</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_HANDLED_OUTBOUND</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_HOLD_ABANDONS</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_MISSED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_QUEUED</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_TRANSFERRED_IN</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_TRANSFERRED_IN_FROM_QUEUE</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_FROM_QUEUE</dt> <dd> <p>Unit: COUNT</p> <p>Statistic: SUM</p> </dd> <dt>HANDLE_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>HOLD_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>INTERACTION_AND_HOLD_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>INTERACTION_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>OCCUPANCY</dt> <dd> <p>Unit: PERCENT</p> <p>Statistic: AVG</p> </dd> <dt>QUEUE_ANSWER_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: AVG</p> </dd> <dt>QUEUED_TIME</dt> <dd> <p>Unit: SECONDS</p> <p>Statistic: MAX</p> </dd> <dt>SERVICE_LEVEL</dt> <dd> <p>You can include up to 20 SERVICE_LEVEL metrics in a request.</p> <p>Unit: PERCENT</p> <p>Statistic: AVG</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> </dd> </dl>",
                     "shape": "HistoricalMetrics"
                 },
                 "InstanceId": {
@@ -14472,32 +14420,32 @@
         "GetMetricDataV2Request": {
             "members": {
                 "EndTime": {
                     "documentation": "<p>The timestamp, in UNIX Epoch time format, at which to end the reporting interval for the retrieval of historical metrics data. The time must be later than the start time timestamp. It cannot be later than the current timestamp.</p>",
                     "shape": "Timestamp"
                 },
                 "Filters": {
-                    "documentation": "<p>The filters to apply to returned metrics. You can filter on the following resources:</p> <ul> <li> <p>Queues</p> </li> <li> <p>Routing profiles</p> </li> <li> <p>Agents</p> </li> <li> <p>Channels</p> </li> <li> <p>User hierarchy groups</p> </li> <li> <p>Feature</p> </li> <li> <p>Routing step expression</p> </li> </ul> <p>At least one filter must be passed from queues, routing profiles, agents, or user hierarchy groups.</p> <p>To filter by phone number, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/create-historical-metrics-report.html\">Create a historical metrics report</a> in the <i>Amazon Connect Administrator's Guide</i>.</p> <p>Note the following limits:</p> <ul> <li> <p> <b>Filter keys</b>: A maximum of 5 filter keys are supported in a single request. Valid filter keys: <code>QUEUE</code> | <code>ROUTING_PROFILE</code> | <code>AGENT</code> | <code>CHANNEL</code> | <code>AGENT_HIERARCHY_LEVEL_ONE</code> | <code>AGENT_HIERARCHY_LEVEL_TWO</code> | <code>AGENT_HIERARCHY_LEVEL_THREE</code> | <code>AGENT_HIERARCHY_LEVEL_FOUR</code> | <code>AGENT_HIERARCHY_LEVEL_FIVE</code> | <code>FEATURE</code> | <code>CASE_TEMPLATE_ARN</code> | <code>CASE_STATUS</code> | <code>contact/segmentAttributes/connect:Subtype</code> | <code>ROUTING_STEP_EXPRESSION</code> </p> </li> <li> <p> <b>Filter values</b>: A maximum of 100 filter values are supported in a single request. VOICE, CHAT, and TASK are valid <code>filterValue</code> for the CHANNEL filter key. They do not count towards limitation of 100 filter values. For example, a GetMetricDataV2 request can filter by 50 queues, 35 agents, and 15 routing profiles for a total of 100 filter values, along with 3 channel filters. </p> <p> <code>contact_lens_conversational_analytics</code> is a valid filterValue for the <code>FEATURE</code> filter key. It is available only to contacts analyzed by Contact Lens conversational analytics.</p> <p> <code>connect:Chat</code>, <code>connect:SMS</code>, <code>connect:Telephony</code>, and <code>connect:WebRTC</code> are valid <code>filterValue</code> examples (not exhaustive) for the <code>contact/segmentAttributes/connect:Subtype filter</code> key.</p> <p> <code>ROUTING_STEP_EXPRESSION</code> is a valid filter key with a filter value up to 3000 length. This filter is case and order sensitive. JSON string fields must be sorted in ascending order and JSON array order should be kept as is.</p> </li> </ul>",
+                    "documentation": "<p>The filters to apply to returned metrics. You can filter on the following resources:</p> <ul> <li> <p>Queues</p> </li> <li> <p>Routing profiles</p> </li> <li> <p>Agents</p> </li> <li> <p>Channels</p> </li> <li> <p>User hierarchy groups</p> </li> <li> <p>Feature</p> </li> </ul> <p>At least one filter must be passed from queues, routing profiles, agents, or user hierarchy groups.</p> <p>To filter by phone number, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/create-historical-metrics-report.html\">Create a historical metrics report</a> in the <i>Amazon Connect Administrator's Guide</i>.</p> <p>Note the following limits:</p> <ul> <li> <p> <b>Filter keys</b>: A maximum of 5 filter keys are supported in a single request. Valid filter keys: <code>QUEUE</code> | <code>ROUTING_PROFILE</code> | <code>AGENT</code> | <code>CHANNEL</code> | <code>AGENT_HIERARCHY_LEVEL_ONE</code> | <code>AGENT_HIERARCHY_LEVEL_TWO</code> | <code>AGENT_HIERARCHY_LEVEL_THREE</code> | <code>AGENT_HIERARCHY_LEVEL_FOUR</code> | <code>AGENT_HIERARCHY_LEVEL_FIVE</code> | <code>FEATURE</code> | <code>contact/segmentAttributes/connect:Subtype</code> </p> </li> <li> <p> <b>Filter values</b>: A maximum of 100 filter values are supported in a single request. VOICE, CHAT, and TASK are valid <code>filterValue</code> for the CHANNEL filter key. They do not count towards limitation of 100 filter values. For example, a GetMetricDataV2 request can filter by 50 queues, 35 agents, and 15 routing profiles for a total of 100 filter values, along with 3 channel filters. </p> <p> <code>contact_lens_conversational_analytics</code> is a valid filterValue for the <code>FEATURE</code> filter key. It is available only to contacts analyzed by Contact Lens conversational analytics.</p> <p> <code>connect:Chat</code>, <code>connect:SMS</code>, <code>connect:Telephony</code>, and <code>connect:WebRTC</code> are valid <code>filterValue</code> examples (not exhaustive) for the <code>contact/segmentAttributes/connect:Subtype filter</code> key.</p> </li> </ul>",
                     "shape": "FiltersV2List"
                 },
                 "Groupings": {
-                    "documentation": "<p>The grouping applied to the metrics that are returned. For example, when results are grouped by queue, the metrics returned are grouped by queue. The values that are returned apply to the metrics for each queue. They are not aggregated for all queues.</p> <p>If no grouping is specified, a summary of all metrics is returned.</p> <p>Valid grouping keys: <code>QUEUE</code> | <code>ROUTING_PROFILE</code> | <code>AGENT</code> | <code>CHANNEL</code> | <code>AGENT_HIERARCHY_LEVEL_ONE</code> | <code>AGENT_HIERARCHY_LEVEL_TWO</code> | <code>AGENT_HIERARCHY_LEVEL_THREE</code> | <code>AGENT_HIERARCHY_LEVEL_FOUR</code> | <code>AGENT_HIERARCHY_LEVEL_FIVE</code> | <code>CASE_TEMPLATE_ARN</code> | <code>CASE_STATUS</code> | <code>contact/segmentAttributes/connect:Subtype</code> | <code>ROUTING_STEP_EXPRESSION</code> </p>",
+                    "documentation": "<p>The grouping applied to the metrics that are returned. For example, when results are grouped by queue, the metrics returned are grouped by queue. The values that are returned apply to the metrics for each queue. They are not aggregated for all queues.</p> <p>If no grouping is specified, a summary of all metrics is returned.</p> <p>Valid grouping keys: <code>QUEUE</code> | <code>ROUTING_PROFILE</code> | <code>AGENT</code> | <code>CHANNEL</code> | <code>AGENT_HIERARCHY_LEVEL_ONE</code> | <code>AGENT_HIERARCHY_LEVEL_TWO</code> | <code>AGENT_HIERARCHY_LEVEL_THREE</code> | <code>AGENT_HIERARCHY_LEVEL_FOUR</code> | <code>AGENT_HIERARCHY_LEVEL_FIVE</code>, <code>contact/segmentAttributes/connect:Subtype</code> </p>",
                     "shape": "GroupingsV2"
                 },
                 "Interval": {
                     "documentation": "<p>The interval period and timezone to apply to returned metrics.</p> <ul> <li> <p> <code>IntervalPeriod</code>: An aggregated grouping applied to request metrics. Valid <code>IntervalPeriod</code> values are: <code>FIFTEEN_MIN</code> | <code>THIRTY_MIN</code> | <code>HOUR</code> | <code>DAY</code> | <code>WEEK</code> | <code>TOTAL</code>. </p> <p>For example, if <code>IntervalPeriod</code> is selected <code>THIRTY_MIN</code>, <code>StartTime</code> and <code>EndTime</code> differs by 1 day, then Amazon Connect returns 48 results in the response. Each result is aggregated by the THIRTY_MIN period. By default Amazon Connect aggregates results based on the <code>TOTAL</code> interval period. </p> <p>The following list describes restrictions on <code>StartTime</code> and <code>EndTime</code> based on which <code>IntervalPeriod</code> is requested. </p> <ul> <li> <p> <code>FIFTEEN_MIN</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 3 days.</p> </li> <li> <p> <code>THIRTY_MIN</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 3 days.</p> </li> <li> <p> <code>HOUR</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 3 days.</p> </li> <li> <p> <code>DAY</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 35 days.</p> </li> <li> <p> <code>WEEK</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 35 days.</p> </li> <li> <p> <code>TOTAL</code>: The difference between <code>StartTime</code> and <code>EndTime</code> must be less than 35 days.</p> </li> </ul> </li> <li> <p> <code>TimeZone</code>: The timezone applied to requested metrics.</p> </li> </ul>",
                     "shape": "IntervalDetails"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return per page.</p>",
                     "shape": "MaxResult100"
                 },
                 "Metrics": {
-                    "documentation": "<p>The metrics to retrieve. Specify the name, groupings, and filters for each metric. The following historical metrics are available. For a description of each metric, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html\">Historical metrics definitions</a> in the <i>Amazon Connect Administrator's Guide</i>.</p> <dl> <dt>ABANDONMENT_RATE</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#abandonment-rate-historical\">Abandonment rate</a> </p> </dd> <dt>AGENT_ADHERENT_TIME</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#adherent-time-historical\">Adherent time</a> </p> </dd> <dt>AGENT_ANSWER_RATE</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-answer-rate-historical\">Agent answer rate</a> </p> </dd> <dt>AGENT_NON_ADHERENT_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#non-adherent-time\">Non-adherent time</a> </p> </dd> <dt>AGENT_NON_RESPONSE</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-non-response\">Agent non-response</a> </p> </dd> <dt>AGENT_NON_RESPONSE_WITHOUT_CUSTOMER_ABANDONS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>Data for this metric is available starting from October 1, 2023 0:00:00 GMT.</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-nonresponse-no-abandon-historical\">Agent non-response without customer abandons</a> </p> </dd> <dt>AGENT_OCCUPANCY</dt> <dd> <p>Unit: Percentage</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#occupancy-historical\">Occupancy</a> </p> </dd> <dt>AGENT_SCHEDULE_ADHERENCE</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#adherence-historical\">Adherence</a> </p> </dd> <dt>AGENT_SCHEDULED_TIME</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#scheduled-time-historical\">Scheduled time</a> </p> </dd> <dt>AVG_ABANDON_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-queue-abandon-time-historical\">Average queue abandon time</a> </p> </dd> <dt>AVG_ACTIVE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-active-time-historical\">Average active time</a> </p> </dd> <dt>AVG_AFTER_CONTACT_WORK_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-acw-time-historical\">Average after contact work time</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_AGENT_CONNECTING_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>. For now, this metric only supports the following as <code>INITIATION_METHOD</code>: <code>INBOUND</code> | <code>OUTBOUND</code> | <code>CALLBACK</code> | <code>API</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#htm-avg-agent-api-connecting-time\">Average agent API connecting time</a> </p> <note> <p>The <code>Negate</code> key in Metric Level Filters is not applicable for this metric.</p> </note> </dd> <dt>AVG_AGENT_PAUSE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-agent-pause-time-historical\">Average agent pause time</a> </p> </dd> <dt>AVG_CASE_RELATED_CONTACTS</dt> <dd> <p>Unit: Count</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-contacts-case-historical\">Average contacts per case</a> </p> </dd> <dt>AVG_CASE_RESOLUTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-case-resolution-time-historical\">Average case resolution time</a> </p> </dd> <dt>AVG_CONTACT_DURATION</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-contact-duration-historical\">Average contact duration</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_CONVERSATION_DURATION</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-conversation-duration-historical\">Average conversation duration</a> </p> </dd> <dt>AVG_GREETING_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-greeting-time-agent-historical\">Average greeting time agent </a> </p> </dd> <dt>AVG_HANDLE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype, RoutingStepExpression</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-handle-time-historical\">Average handle time</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-customer-hold-time-historical\">Average customer hold time</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_HOLD_TIME_ALL_CONTACTS</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#avg-customer-hold-time-all-contacts-historical\">Average customer hold time all contacts</a> </p> </dd> <dt>AVG_HOLDS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-holds-historical\">Average holds</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_INTERACTION_AND_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-agent-interaction-customer-hold-time-historical\">Average agent interaction and customer hold time</a> </p> </dd> <dt>AVG_INTERACTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-agent-interaction-time-historical\">Average agent interaction time</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_INTERRUPTIONS_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-interruptions-agent-historical\">Average interruptions agent </a> </p> </dd> <dt>AVG_INTERRUPTION_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-interruptions-time-agent-historical\">Average interruption time agent</a> </p> </dd> <dt>AVG_NON_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html##average-non-talk-time-historical\">Average non-talk time</a> </p> </dd> <dt>AVG_QUEUE_ANSWER_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-queue-answer-time-historical\">Average queue answer time</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_RESOLUTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-resolution-time-historical\">Average resolution time</a> </p> </dd> <dt>AVG_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-talk-time-historical\">Average talk time</a> </p> </dd> <dt>AVG_TALK_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-talk-time-agent-historical\">Average talk time agent</a> </p> </dd> <dt>AVG_TALK_TIME_CUSTOMER</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#average-talk-time-customer-historical\">Average talk time customer</a> </p> </dd> <dt>CASES_CREATED</dt> <dd> <p>Unit: Count</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html##cases-created-historical\">Cases created</a> </p> </dd> <dt>CONTACTS_ABANDONED</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype, RoutingStepExpression</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-abandoned-historical\">Contact abandoned</a> </p> </dd> <dt>CONTACTS_CREATED</dt> <dd> <p>Unit: Count</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-created-historical\">Contacts created</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_HANDLED</dt> <dd> <p>Unit: Count</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>, <code>DISCONNECT_REASON</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype, RoutingStepExpression</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#api-contacts-handled-historical\">API contacts handled</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_HANDLED_BY_CONNECTED_TO_AGENT</dt> <dd> <p>Unit: Count</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-handled-by-connected-to-agent-historical\">Contacts handled by Connected to agent</a> </p> </dd> <dt>CONTACTS_HOLD_ABANDONS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-handled-by-connected-to-agent-historical\">Contacts hold disconnect</a> </p> </dd> <dt>CONTACTS_ON_HOLD_AGENT_DISCONNECT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-hold-agent-disconnect-historical\">Contacts hold agent disconnect</a> </p> </dd> <dt>CONTACTS_ON_HOLD_CUSTOMER_DISCONNECT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-hold-customer-disconnect-historical\">Contacts hold customer disconnect</a> </p> </dd> <dt>CONTACTS_PUT_ON_HOLD</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-hold-customer-disconnect-historical\">Contacts put on hold</a> </p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_EXTERNAL</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-transferred-out-external-historical\">Contacts transferred out external</a> </p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_INTERNAL</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-transferred-out-internal-historical\">Contacts transferred out internal</a> </p> </dd> <dt>CONTACTS_QUEUED</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-queued-historical\">Contacts queued</a> </p> </dd> <dt>CONTACTS_QUEUED_BY_ENQUEUE</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-queued-by-enqueue-historical\">Contacts queued by Enqueue</a> </p> </dd> <dt>CONTACTS_RESOLVED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code> enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\").</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-resolved-historical\">Contacts resolved in X</a> </p> </dd> <dt>CONTACTS_TRANSFERRED_OUT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-transferred-out-historical\">Contacts transferred out</a> </p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_TRANSFERRED_OUT_BY_AGENT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-transferred-out-by-agent-historical\">Contacts transferred out by agent</a> </p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_FROM_QUEUE</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-transferred-out-by-agent-historical\">Contacts transferred out queue</a> </p> </dd> <dt>CURRENT_CASES</dt> <dd> <p>Unit: Count</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#current-cases-historical\">Current cases</a> </p> </dd> <dt>MAX_QUEUED_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#maximum-queued-time-historical\">Maximum queued time</a> </p> </dd> <dt>PERCENT_CASES_FIRST_CONTACT_RESOLVED</dt> <dd> <p>Unit: Percent</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#cases-resolved-first-contact-historical\">Cases resolved on first contact</a> </p> </dd> <dt>PERCENT_CONTACTS_STEP_EXPIRED</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, RoutingStepExpression</p> <p>UI name: Not available </p> </dd> <dt>PERCENT_CONTACTS_STEP_JOINED</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, RoutingStepExpression</p> <p>UI name: Not available </p> </dd> <dt>PERCENT_NON_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#ntt-historical\">Non-talk time percent</a> </p> </dd> <dt>PERCENT_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#tt-historical\">Talk time percent</a> </p> </dd> <dt>PERCENT_TALK_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#ttagent-historical\">Talk time agent percent</a> </p> </dd> <dt>PERCENT_TALK_TIME_CUSTOMER</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#ttcustomer-historical\">Talk time customer percent</a> </p> </dd> <dt>REOPENED_CASE_ACTIONS</dt> <dd> <p>Unit: Count</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#cases-reopened-historical\">Cases reopened</a> </p> </dd> <dt>RESOLVED_CASE_ACTIONS</dt> <dd> <p>Unit: Count</p> <p>Required filter key: CASE_TEMPLATE_ARN</p> <p>Valid groupings and filters: CASE_TEMPLATE_ARN, CASE_STATUS</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#cases-resolved-historicall\">Cases resolved</a> </p> </dd> <dt>SERVICE_LEVEL</dt> <dd> <p>You can include up to 20 SERVICE_LEVEL metrics in a request.</p> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#service-level-historical\">Service level X</a> </p> </dd> <dt>STEP_CONTACTS_QUEUED</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, RoutingStepExpression</p> <p>UI name: Not available</p> </dd> <dt>SUM_AFTER_CONTACT_WORK_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#acw-historical\">After contact work time</a> </p> </dd> <dt>SUM_CONNECTING_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>. This metric only supports the following filter keys as <code>INITIATION_METHOD</code>: <code>INBOUND</code> | <code>OUTBOUND</code> | <code>CALLBACK</code> | <code>API</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#htm-agent-api-connecting-time\">Agent API connecting time</a> </p> <note> <p>The <code>Negate</code> key in Metric Level Filters is not applicable for this metric.</p> </note> </dd> <dt>SUM_CONTACT_FLOW_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contact-flow-time-historical\">Contact flow time</a> </p> </dd> <dt>SUM_CONTACT_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-on-contact-time-historical\">Agent on contact time</a> </p> </dd> <dt>SUM_CONTACTS_ANSWERED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-answered-x-historical\">Contacts answered in X seconds</a> </p> </dd> <dt>SUM_CONTACTS_ABANDONED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contacts-abandoned-x-historical\">Contacts abandoned in X seconds</a> </p> </dd> <dt>SUM_CONTACTS_DISCONNECTED </dt> <dd> <p>Valid metric filter key: <code>DISCONNECT_REASON</code> </p> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contact-disconnected-historical\">Contact disconnected</a> </p> </dd> <dt>SUM_ERROR_STATUS_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#error-status-time-historical\">Error status time</a> </p> </dd> <dt>SUM_HANDLE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#contact-handle-time-historical\">Contact handle time</a> </p> </dd> <dt>SUM_HOLD_TIME</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#customer-hold-time-historical\">Customer hold time</a> </p> </dd> <dt>SUM_IDLE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-idle-time-historica\">Agent idle time</a> </p> </dd> <dt>SUM_INTERACTION_AND_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-interaction-hold-time-historical\">Agent interaction and hold time</a> </p> </dd> <dt>SUM_INTERACTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#agent-interaction-time-historical\">Agent interaction time</a> </p> </dd> <dt>SUM_NON_PRODUCTIVE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#npt-historical\">Non-Productive Time</a> </p> </dd> <dt>SUM_ONLINE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#online-time-historical\">Online time</a> </p> </dd> <dt>SUM_RETRY_CALLBACK_ATTEMPTS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>UI name: <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html#callback-attempts-historical\">Callback attempts</a> </p> </dd> </dl>",
+                    "documentation": "<p>The metrics to retrieve. Specify the name, groupings, and filters for each metric. The following historical metrics are available. For a description of each metric, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/historical-metrics-definitions.html\">Historical metrics definitions</a> in the <i>Amazon Connect Administrator's Guide</i>.</p> <dl> <dt>ABANDONMENT_RATE</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AGENT_ADHERENT_TIME</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy </p> </dd> <dt>AGENT_ANSWER_RATE</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AGENT_NON_ADHERENT_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AGENT_NON_RESPONSE</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy </p> </dd> <dt>AGENT_NON_RESPONSE_WITHOUT_CUSTOMER_ABANDONS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <p>Data for this metric is available starting from October 1, 2023 0:00:00 GMT.</p> </dd> <dt>AGENT_OCCUPANCY</dt> <dd> <p>Unit: Percentage</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy </p> </dd> <dt>AGENT_SCHEDULE_ADHERENCE</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AGENT_SCHEDULED_TIME</dt> <dd> <p>This metric is available only in Amazon Web Services Regions where <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/regions.html#optimization_region\">Forecasting, capacity planning, and scheduling</a> is available.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AVG_ABANDON_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_ACTIVE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AVG_AFTER_CONTACT_WORK_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_AGENT_CONNECTING_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>. For now, this metric only supports the following as <code>INITIATION_METHOD</code>: <code>INBOUND</code> | <code>OUTBOUND</code> | <code>CALLBACK</code> | <code>API</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <note> <p>The <code>Negate</code> key in Metric Level Filters is not applicable for this metric.</p> </note> </dd> <dt>AVG_AGENT_PAUSE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>AVG_CONTACT_DURATION</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_CONVERSATION_DURATION</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_GREETING_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_HANDLE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_HOLD_TIME_ALL_CONTACTS</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_HOLDS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_INTERACTION_AND_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_INTERACTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_INTERRUPTIONS_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_INTERRUPTION_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_NON_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_QUEUE_ANSWER_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>AVG_RESOLUTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_TALK_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>AVG_TALK_TIME_CUSTOMER</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>CONTACTS_ABANDONED</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>CONTACTS_CREATED</dt> <dd> <p>Unit: Count</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_HANDLED</dt> <dd> <p>Unit: Count</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>, <code>DISCONNECT_REASON</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_HOLD_ABANDONS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>CONTACTS_ON_HOLD_AGENT_DISCONNECT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>CONTACTS_ON_HOLD_CUSTOMER_DISCONNECT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>CONTACTS_PUT_ON_HOLD</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_EXTERNAL</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_INTERNAL</dt> <dd> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>CONTACTS_QUEUED</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>CONTACTS_RESOLVED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code> enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\").</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, Feature, contact/segmentAttributes/connect:Subtype</p> <note> <p>Feature is a valid filter but not a valid grouping.</p> </note> </dd> <dt>CONTACTS_TRANSFERRED_OUT_BY_AGENT</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>CONTACTS_TRANSFERRED_OUT_FROM_QUEUE</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>MAX_QUEUED_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>PERCENT_NON_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>PERCENT_TALK_TIME</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>PERCENT_TALK_TIME_AGENT</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>PERCENT_TALK_TIME_CUSTOMER</dt> <dd> <p>This metric is available only for contacts analyzed by Contact Lens conversational analytics.</p> <p>Unit: Percentage</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>SERVICE_LEVEL</dt> <dd> <p>You can include up to 20 SERVICE_LEVEL metrics in a request.</p> <p>Unit: Percent</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> </dd> <dt>SUM_AFTER_CONTACT_WORK_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_CONNECTING_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid metric filter key: <code>INITIATION_METHOD</code>. This metric only supports the following filter keys as <code>INITIATION_METHOD</code>: <code>INBOUND</code> | <code>OUTBOUND</code> | <code>CALLBACK</code> | <code>API</code> </p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> <note> <p>The <code>Negate</code> key in Metric Level Filters is not applicable for this metric.</p> </note> </dd> <dt>SUM_CONTACT_FLOW_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_CONTACT_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_CONTACTS_ANSWERED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> </dd> <dt>SUM_CONTACTS_ABANDONED_IN_X</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> <p>Threshold: For <code>ThresholdValue</code>, enter any whole number from 1 to 604800 (inclusive), in seconds. For <code>Comparison</code>, you must enter <code>LT</code> (for \"Less than\"). </p> </dd> <dt>SUM_CONTACTS_DISCONNECTED </dt> <dd> <p>Valid metric filter key: <code>DISCONNECT_REASON</code> </p> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy, contact/segmentAttributes/connect:Subtype</p> </dd> <dt>SUM_ERROR_STATUS_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_HANDLE_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_HOLD_TIME</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_IDLE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_INTERACTION_AND_HOLD_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_INTERACTION_TIME</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_NON_PRODUCTIVE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_ONLINE_TIME_AGENT</dt> <dd> <p>Unit: Seconds</p> <p>Valid groupings and filters: Routing Profile, Agent, Agent Hierarchy</p> </dd> <dt>SUM_RETRY_CALLBACK_ATTEMPTS</dt> <dd> <p>Unit: Count</p> <p>Valid groupings and filters: Queue, Channel, Routing Profile, contact/segmentAttributes/connect:Subtype</p> </dd> </dl>",
                     "shape": "MetricsV2"
                 },
                 "NextToken": {
                     "documentation": "<p>The token for the next set of results. Use the value returned in the previous response in the next request to retrieve the next set of results.</p>",
                     "shape": "NextToken2500"
                 },
                 "ResourceArn": {
@@ -14657,15 +14605,15 @@
                 "Name"
             ],
             "type": "structure"
         },
         "GetTrafficDistributionRequest": {
             "members": {
                 "Id": {
-                    "documentation": "<p>The identifier of the traffic distribution group. This can be the ID or the ARN if the API is being called in the Region where the traffic distribution group was created. The ARN must be provided if the call is from the replicated Region.</p>",
+                    "documentation": "<p>The identifier of the traffic distribution group.</p>",
                     "location": "uri",
                     "locationName": "Id",
                     "shape": "TrafficDistributionGroupIdOrArn"
                 }
             },
             "required": [
                 "Id"
@@ -14713,15 +14661,15 @@
             "max": 2,
             "member": {
                 "shape": "Grouping"
             },
             "type": "list"
         },
         "GroupingsV2": {
-            "max": 3,
+            "max": 2,
             "member": {
                 "shape": "GroupingV2"
             },
             "type": "list"
         },
         "HierarchyGroup": {
             "documentation": "<p>Contains information about a hierarchy group.</p>",
@@ -14935,25 +14883,14 @@
                 "LevelTwo": {
                     "documentation": "<p>Information about level two.</p>",
                     "shape": "HierarchyGroupSummaryReference"
                 }
             },
             "type": "structure"
         },
-        "HierarchyRestrictedResourceList": {
-            "member": {
-                "shape": "HierarchyRestrictedResourceName"
-            },
-            "type": "list"
-        },
-        "HierarchyRestrictedResourceName": {
-            "max": 128,
-            "min": 1,
-            "type": "string"
-        },
         "HierarchyStructure": {
             "documentation": "<p>Contains information about a hierarchy structure.</p>",
             "members": {
                 "LevelFive": {
                     "documentation": "<p>Information about level five.</p>",
                     "shape": "HierarchyLevel"
                 },
@@ -15433,16 +15370,15 @@
                 "CONTACTFLOW_LOGS",
                 "CONTACT_LENS",
                 "AUTO_RESOLVE_BEST_VOICES",
                 "USE_CUSTOM_TTS_VOICES",
                 "EARLY_MEDIA",
                 "MULTI_PARTY_CONFERENCE",
                 "HIGH_VOLUME_OUTBOUND",
-                "ENHANCED_CONTACT_MONITORING",
-                "ENHANCED_CHAT_MONITORING"
+                "ENHANCED_CONTACT_MONITORING"
             ],
             "type": "string"
         },
         "InstanceAttributeValue": {
             "max": 100,
             "min": 1,
             "type": "string"
@@ -15522,17 +15458,15 @@
                 "SCHEDULED_REPORTS",
                 "MEDIA_STREAMS",
                 "CONTACT_TRACE_RECORDS",
                 "AGENT_EVENTS",
                 "REAL_TIME_CONTACT_ANALYSIS_SEGMENTS",
                 "ATTACHMENTS",
                 "CONTACT_EVALUATIONS",
-                "SCREEN_RECORDINGS",
-                "REAL_TIME_CONTACT_ANALYSIS_CHAT_SEGMENTS",
-                "REAL_TIME_CONTACT_ANALYSIS_VOICE_SEGMENTS"
+                "SCREEN_RECORDINGS"
             ],
             "type": "string"
         },
         "InstanceSummary": {
             "documentation": "<p>Information about the instance.</p>",
             "members": {
                 "Arn": {
@@ -17972,20 +17906,14 @@
             "type": "integer"
         },
         "MaxResult25": {
             "max": 25,
             "min": 1,
             "type": "integer"
         },
-        "MaxResult500": {
-            "box": true,
-            "max": 500,
-            "min": 1,
-            "type": "integer"
-        },
         "MaxResult7": {
             "max": 7,
             "min": 1,
             "type": "integer"
         },
         "MaxResults": {
             "max": 100,
@@ -18241,15 +18169,15 @@
                 "BARGE"
             ],
             "type": "string"
         },
         "MonitorContactRequest": {
             "members": {
                 "AllowedMonitorCapabilities": {
-                    "documentation": "<p>Specify which monitoring actions the user is allowed to take. For example, whether the user is allowed to escalate from silent monitoring to barge. AllowedMonitorCapabilities is required if barge is enabled.</p>",
+                    "documentation": "<p>Specify which monitoring actions the user is allowed to take. For example, whether the user is allowed to escalate from silent monitoring to barge.</p>",
                     "shape": "AllowedMonitorCapabilities"
                 },
                 "ClientToken": {
                     "documentation": "<p>A unique, case-sensitive identifier that you provide to ensure the idempotency of the request. If not provided, the Amazon Web Services SDK populates this field. For more information about idempotency, see <a href=\"https://aws.amazon.com/builders-library/making-retries-safe-with-idempotent-APIs/\">Making retries safe with idempotent APIs</a>.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
@@ -18285,15 +18213,14 @@
                 }
             },
             "type": "structure"
         },
         "Name": {
             "max": 512,
             "min": 0,
-            "sensitive": true,
             "type": "string"
         },
         "Name128": {
             "max": 128,
             "min": 1,
             "pattern": "(^[\\S].*[\\S]$)|(^[\\S]$)",
             "type": "string"
@@ -18511,16 +18438,15 @@
             "type": "string"
         },
         "ParticipantRole": {
             "enum": [
                 "AGENT",
                 "CUSTOMER",
                 "SYSTEM",
-                "CUSTOM_BOT",
-                "SUPERVISOR"
+                "CUSTOM_BOT"
             ],
             "type": "string"
         },
         "ParticipantTimerAction": {
             "enum": [
                 "Unset"
             ],
@@ -18601,15 +18527,14 @@
                     "shape": "ParticipantToken"
                 }
             },
             "type": "structure"
         },
         "Password": {
             "pattern": "/^(?=.*[a-z])(?=.*[A-Z])(?=.*\\d)[a-zA-Z\\d\\S]{8,64}$/",
-            "sensitive": true,
             "type": "string"
         },
         "PauseContactRequest": {
             "members": {
                 "ContactFlowId": {
                     "documentation": "<p>The identifier of the flow.</p>",
                     "shape": "ContactFlowId"
@@ -19048,15 +18973,15 @@
                     "documentation": "<p>The values of the predefined attribute.</p>",
                     "shape": "PredefinedAttributeValues"
                 }
             },
             "type": "structure"
         },
         "PredefinedAttributeName": {
-            "max": 64,
+            "max": 128,
             "min": 1,
             "type": "string"
         },
         "PredefinedAttributeSearchConditionList": {
             "member": {
                 "shape": "PredefinedAttributeSearchCriteria"
             },
@@ -19082,20 +19007,20 @@
         "PredefinedAttributeSearchSummaryList": {
             "member": {
                 "shape": "PredefinedAttribute"
             },
             "type": "list"
         },
         "PredefinedAttributeStringValue": {
-            "max": 64,
+            "max": 128,
             "min": 1,
             "type": "string"
         },
         "PredefinedAttributeStringValuesList": {
-            "max": 128,
+            "max": 75,
             "member": {
                 "shape": "PredefinedAttributeStringValue"
             },
             "min": 1,
             "type": "list"
         },
         "PredefinedAttributeSummary": {
@@ -21167,15 +21092,15 @@
                 "MATCH_ANY"
             ],
             "type": "string"
         },
         "SearchContactsRequest": {
             "members": {
                 "InstanceId": {
-                    "documentation": "<p>The identifier of Amazon Connect instance. You can find the instance ID in the Amazon Resource Name (ARN) of the instance.</p>",
+                    "documentation": "<p>The identifier of Amazon Connect instance. You can find the instance ID in the Amazon Resource Name (ARN) of the instance</p>",
                     "shape": "InstanceId"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return per page.</p>",
                     "shape": "MaxResult100"
                 },
@@ -21184,19 +21109,19 @@
                     "shape": "LargeNextToken"
                 },
                 "SearchCriteria": {
                     "documentation": "<p>The search criteria to be used to return contacts.</p>",
                     "shape": "SearchCriteria"
                 },
                 "Sort": {
-                    "documentation": "<p>Specifies a field to sort by and a sort order.</p>",
+                    "documentation": "<p>Specifies a field to sort by and a sort order</p>",
                     "shape": "Sort"
                 },
                 "TimeRange": {
-                    "documentation": "<p>Time range that you want to search results.</p>",
+                    "documentation": "<p>Time range that you want to search results</p>",
                     "shape": "SearchContactsTimeRange"
                 }
             },
             "required": [
                 "InstanceId",
                 "TimeRange"
             ],
@@ -21219,26 +21144,26 @@
             },
             "required": [
                 "Contacts"
             ],
             "type": "structure"
         },
         "SearchContactsTimeRange": {
-            "documentation": "<p>A structure of time range that you want to search results.</p>",
+            "documentation": "<p>A structure of time range that you want to search results</p>",
             "members": {
                 "EndTime": {
                     "documentation": "<p>The end time of the time range.</p>",
                     "shape": "Timestamp"
                 },
                 "StartTime": {
                     "documentation": "<p>The start time of the time range.</p>",
                     "shape": "Timestamp"
                 },
                 "Type": {
-                    "documentation": "<p>The type of timestamp to search.</p>",
+                    "documentation": "<p>The type of timestamp to search</p>",
                     "shape": "SearchContactsTimeRangeType"
                 }
             },
             "required": [
                 "Type",
                 "StartTime",
                 "EndTime"
@@ -21251,42 +21176,42 @@
                 "SCHEDULED_TIMESTAMP",
                 "CONNECTED_TO_AGENT_TIMESTAMP",
                 "DISCONNECT_TIMESTAMP"
             ],
             "type": "string"
         },
         "SearchCriteria": {
-            "documentation": "<p>A structure of search criteria to be used to return contacts.</p>",
+            "documentation": "<p>A structure of search criteria to be used to return contacts</p>",
             "members": {
                 "AgentHierarchyGroups": {
-                    "documentation": "<p>The agent hierarchy groups of the agent at the time of handling the contact.</p>",
+                    "documentation": "<p>The agent hierarchy groups</p>",
                     "shape": "AgentHierarchyGroups"
                 },
                 "AgentIds": {
-                    "documentation": "<p>The identifiers of agents who handled the contacts.</p>",
+                    "documentation": "<p>The array of agent ids</p>",
                     "shape": "AgentResourceIdList"
                 },
                 "Channels": {
-                    "documentation": "<p>The list of channels associated with contacts.</p>",
+                    "documentation": "<p>The array of channels</p>",
                     "shape": "ChannelList"
                 },
                 "ContactAnalysis": {
-                    "documentation": "<p>Search criteria based on analysis outputs from Amazon Connect Contact Lens.</p>",
+                    "documentation": "<p>The ContactAnalysis object used in search criteria</p>",
                     "shape": "ContactAnalysis"
                 },
                 "InitiationMethods": {
-                    "documentation": "<p>The list of initiation methods associated with contacts.</p>",
+                    "documentation": "<p>The array of initiaton methods</p>",
                     "shape": "InitiationMethodList"
                 },
                 "QueueIds": {
-                    "documentation": "<p>The list of queue IDs associated with contacts.</p>",
+                    "documentation": "<p>The array of queue ids.</p>",
                     "shape": "QueueIdList"
                 },
                 "SearchableContactAttributes": {
-                    "documentation": "<p>The search criteria based on user-defined contact attributes that have been configured for contact search. For more information, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/search-custom-attributes.html\">Search by customer contact attributes</a> in the <i>Amazon Connect Administrator Guide</i>.</p> <important> <p>To use <code>SearchableContactAttributes</code> in a search request, the <code>GetContactAttributes</code> action is required to perform an API request. For more information, see <a href=\"https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonconnect.html#amazonconnect-actions-as-permissions\">https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonconnect.html#amazonconnect-actions-as-permissions</a>Actions defined by Amazon Connect.</p> </important>",
+                    "documentation": "<p>The SearchableContactAttributes object used in search criteria</p>",
                     "shape": "SearchableContactAttributes"
                 }
             },
             "type": "structure"
         },
         "SearchHoursOfOperationsRequest": {
             "members": {
@@ -21427,15 +21352,15 @@
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "shape": "InstanceId"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return per page.</p>",
-                    "shape": "MaxResult500"
+                    "shape": "MaxResult100"
                 },
                 "NextToken": {
                     "documentation": "<p>The token for the next set of results. Use the value returned in the previous response in the next request to retrieve the next set of results.</p>",
                     "shape": "NextToken2500"
                 },
                 "SearchCriteria": {
                     "documentation": "<p>The search criteria to be used to return queues.</p> <note> <p>The <code>name</code> and <code>description</code> fields support \"contains\" queries with a minimum of 2 characters and a maximum of 25 characters. Any queries with character lengths outside of this range will throw invalid results. </p> </note>",
@@ -21561,15 +21486,15 @@
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "shape": "InstanceId"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return per page.</p>",
-                    "shape": "MaxResult500"
+                    "shape": "MaxResult100"
                 },
                 "NextToken": {
                     "documentation": "<p>The token for the next set of results. Use the value returned in the previous response in the next request to retrieve the next set of results.</p>",
                     "shape": "NextToken2500"
                 },
                 "SearchCriteria": {
                     "documentation": "<p>The search criteria to be used to return routing profiles.</p> <note> <p>The <code>name</code> and <code>description</code> fields support \"contains\" queries with a minimum of 2 characters and a maximum of 25 characters. Any queries with character lengths outside of this range will throw invalid results. </p> </note>",
@@ -21666,15 +21591,15 @@
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p> <note> <p>InstanceID is a required field. The \"Required: No\" below is incorrect.</p> </note>",
                     "shape": "InstanceId"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return per page.</p>",
-                    "shape": "MaxResult500"
+                    "shape": "MaxResult100"
                 },
                 "NextToken": {
                     "documentation": "<p>The token for the next set of results. Use the value returned in the previous response in the next request to retrieve the next set of results.</p>",
                     "shape": "NextToken2500"
                 },
                 "SearchCriteria": {
                     "shape": "UserSearchCriteria"
@@ -21770,39 +21695,39 @@
             "member": {
                 "shape": "SearchableContactAttributeValue"
             },
             "min": 0,
             "type": "list"
         },
         "SearchableContactAttributes": {
-            "documentation": "<p>A structure that defines search criteria based on user-defined contact attributes that are configured for contact search.</p>",
+            "documentation": "<p>A structure that defines searchable contact attributes which can be used to filter search results. </p>",
             "members": {
                 "Criteria": {
-                    "documentation": "<p>The list of criteria based on user-defined contact attributes that are configured for contact search.</p>",
+                    "documentation": "<p>The array of searhale contact attribute criteria</p>",
                     "shape": "SearchableContactAttributesCriteriaList"
                 },
                 "MatchType": {
-                    "documentation": "<p>The match type combining search criteria using multiple searchable contact attributes.</p>",
+                    "documentation": "<p>The match type of multiple searchable contact attributes criteria.</p>",
                     "shape": "SearchContactsMatchType"
                 }
             },
             "required": [
                 "Criteria"
             ],
             "type": "structure"
         },
         "SearchableContactAttributesCriteria": {
-            "documentation": "<p>The search criteria based on user-defned contact attribute key and values to search on.</p>",
+            "documentation": "<p>The criteria of searchable contact attributes.</p>",
             "members": {
                 "Key": {
-                    "documentation": "<p>The key containing a searchable user-defined contact attribute.</p>",
+                    "documentation": "<p>The searchable contact attribute key</p>",
                     "shape": "SearchableContactAttributeKey"
                 },
                 "Values": {
-                    "documentation": "<p>The list of values to search for within a user-defined contact attribute.</p>",
+                    "documentation": "<p>The array of contact attribute values used to filter search results.</p>",
                     "shape": "SearchableContactAttributeValueList"
                 }
             },
             "required": [
                 "Key",
                 "Values"
             ],
@@ -21845,34 +21770,26 @@
                 "shape": "SecurityKey"
             },
             "type": "list"
         },
         "SecurityProfile": {
             "documentation": "<p>Contains information about a security profile.</p>",
             "members": {
-                "AllowedAccessControlHierarchyGroupId": {
-                    "documentation": "<p>The identifier of the hierarchy group that a security profile uses to restrict access to resources in Amazon Connect.</p>",
-                    "shape": "HierarchyGroupId"
-                },
                 "AllowedAccessControlTags": {
                     "documentation": "<p>The list of tags that a security profile uses to restrict access to resources in Amazon Connect.</p>",
                     "shape": "AllowedAccessControlTags"
                 },
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the secruity profile.</p>",
                     "shape": "ARN"
                 },
                 "Description": {
                     "documentation": "<p>The description of the security profile.</p>",
                     "shape": "SecurityProfileDescription"
                 },
-                "HierarchyRestrictedResources": {
-                    "documentation": "<p>The list of resources that a security profile applies hierarchy restrictions to in Amazon Connect. Following are acceptable ResourceNames: <code>User</code>.</p>",
-                    "shape": "HierarchyRestrictedResourceList"
-                },
                 "Id": {
                     "documentation": "<p>The identifier for the security profile.</p>",
                     "shape": "SecurityProfileId"
                 },
                 "LastModifiedRegion": {
                     "documentation": "<p>The Amazon Web Services Region where this resource was last modified.</p>",
                     "shape": "RegionName"
@@ -22231,15 +22148,15 @@
             "min": 1,
             "type": "string"
         },
         "SnapshotVersion": {
             "type": "string"
         },
         "Sort": {
-            "documentation": "<p>A structure that defineds the field name to sort by and a sort order.</p>",
+            "documentation": "<p>A structure that defines the sort by and a sort order</p>",
             "members": {
                 "FieldName": {
                     "documentation": "<p>The name of the field on which to sort.</p>",
                     "shape": "SortableFieldName"
                 },
                 "Order": {
                     "documentation": "<p>An ascending or descending sort.</p>",
@@ -22305,15 +22222,15 @@
                     "shape": "ClientToken"
                 },
                 "ContactFlowId": {
                     "documentation": "<p>The identifier of the flow for initiating the chat. To see the ContactFlowId in the Amazon Connect admin website, on the navigation menu go to <b>Routing</b>, <b>Contact Flows</b>. Choose the flow. On the flow page, under the name of the flow, choose <b>Show additional flow information</b>. The ContactFlowId is the last part of the ARN, shown here in bold: </p> <p>arn:aws:connect:us-west-2:xxxxxxxxxxxx:instance/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/contact-flow/<b>846ec553-a005-41c0-8341-xxxxxxxxxxxx</b> </p>",
                     "shape": "ContactFlowId"
                 },
                 "InitialMessage": {
-                    "documentation": "<p>The initial message to be sent to the newly created chat. If you have a Lex bot in your flow, the initial message is not delivered to the Lex bot.</p>",
+                    "documentation": "<p>The initial message to be sent to the newly created chat.</p>",
                     "shape": "ChatMessage"
                 },
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "shape": "InstanceId"
                 },
                 "ParticipantDetails": {
@@ -23568,35 +23485,35 @@
             "enum": [
                 "GENERAL",
                 "CAMPAIGN"
             ],
             "type": "string"
         },
         "Transcript": {
-            "documentation": "<p>A structure that defines search criteria and matching logic to search for contacts by matching text with transcripts analyzed by Amazon Connect Contact Lens.</p>",
+            "documentation": "<p>The transcript object used to search results.</p>",
             "members": {
                 "Criteria": {
-                    "documentation": "<p>The list of search criteria based on Contact Lens conversational analytics transcript.</p>",
+                    "documentation": "<p>The array of transcript search criteria</p>",
                     "shape": "TranscriptCriteriaList"
                 },
                 "MatchType": {
-                    "documentation": "<p>The match type combining search criteria using multiple transcript criteria.</p>",
+                    "documentation": "<p>The match type of multiple transcript criteira</p>",
                     "shape": "SearchContactsMatchType"
                 }
             },
             "required": [
                 "Criteria"
             ],
             "type": "structure"
         },
         "TranscriptCriteria": {
-            "documentation": "<p>A structure that defines search criteria base on words or phrases, participants in the Contact Lens conversational analytics transcript.</p>",
+            "documentation": "<p>The transcript criteria used to search</p>",
             "members": {
                 "MatchType": {
-                    "documentation": "<p>The match type combining search criteria using multiple search texts in a transcript criteria.</p>",
+                    "documentation": "<p>The match type of search texts in a transcript criteria.</p>",
                     "shape": "SearchContactsMatchType"
                 },
                 "ParticipantRole": {
                     "documentation": "<p>The participant role in a transcript</p>",
                     "shape": "ParticipantRole"
                 },
                 "SearchText": {
@@ -24844,34 +24761,26 @@
                 "Actions",
                 "PublishStatus"
             ],
             "type": "structure"
         },
         "UpdateSecurityProfileRequest": {
             "members": {
-                "AllowedAccessControlHierarchyGroupId": {
-                    "documentation": "<p>The identifier of the hierarchy group that a security profile uses to restrict access to resources in Amazon Connect.</p>",
-                    "shape": "HierarchyGroupId"
-                },
                 "AllowedAccessControlTags": {
                     "documentation": "<p>The list of tags that a security profile uses to restrict access to resources in Amazon Connect.</p>",
                     "shape": "AllowedAccessControlTags"
                 },
                 "Applications": {
                     "documentation": "<p>This API is in preview release for Amazon Connect and is subject to change.</p> <p>A list of the third-party application's metadata.</p>",
                     "shape": "Applications"
                 },
                 "Description": {
                     "documentation": "<p>The description of the security profile.</p>",
                     "shape": "SecurityProfileDescription"
                 },
-                "HierarchyRestrictedResources": {
-                    "documentation": "<p>The list of resources that a security profile applies hierarchy restrictions to in Amazon Connect. Following are acceptable ResourceNames: <code>User</code>.</p>",
-                    "shape": "HierarchyRestrictedResourceList"
-                },
                 "InstanceId": {
                     "documentation": "<p>The identifier of the Amazon Connect instance. You can <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/find-instance-arn.html\">find the instance ID</a> in the Amazon Resource Name (ARN) of the instance.</p>",
                     "location": "uri",
                     "locationName": "InstanceId",
                     "shape": "InstanceId"
                 },
                 "Permissions": {
@@ -25000,15 +24909,15 @@
         "UpdateTrafficDistributionRequest": {
             "members": {
                 "AgentConfig": {
                     "documentation": "<p>The distribution of agents between the instance and its replica(s).</p>",
                     "shape": "AgentConfig"
                 },
                 "Id": {
-                    "documentation": "<p>The identifier of the traffic distribution group. This can be the ID or the ARN if the API is being called in the Region where the traffic distribution group was created. The ARN must be provided if the call is from the replicated Region. </p>",
+                    "documentation": "<p>The identifier of the traffic distribution group. This can be the ID or the ARN if the API is being called in the Region where the traffic distribution group was created. The ARN must be provided if the call is from the replicated Region.</p>",
                     "location": "uri",
                     "locationName": "Id",
                     "shape": "TrafficDistributionGroupIdOrArn"
                 },
                 "SignInConfig": {
                     "documentation": "<p>The distribution that determines which Amazon Web Services Regions should be used to sign in agents in to both the instance and its replica(s).</p>",
                     "shape": "SignInConfig"
@@ -25495,15 +25404,15 @@
         "UserIdList": {
             "member": {
                 "shape": "UserId"
             },
             "type": "list"
         },
         "UserIdentityInfo": {
-            "documentation": "<p>Contains information about the identity of a user.</p> <note> <p>For Amazon Connect instances that are created with the <code>EXISTING_DIRECTORY</code> identity management type, <code>FirstName</code>, <code>LastName</code>, and <code>Email</code> cannot be updated from within Amazon Connect because they are managed by the directory.</p> </note>",
+            "documentation": "<p>Contains information about the identity of a user.</p>",
             "members": {
                 "Email": {
                     "documentation": "<p>The email address. If you are using SAML for identity management and include this parameter, an error is returned.</p>",
                     "shape": "Email"
                 },
                 "FirstName": {
                     "documentation": "<p>The first name. This is required if you are using Amazon Connect or SAML for identity management.</p>",
@@ -25551,15 +25460,15 @@
             },
             "type": "structure"
         },
         "UserPhoneConfig": {
             "documentation": "<p>Contains information about the phone configuration settings for a user.</p>",
             "members": {
                 "AfterContactWorkTimeLimit": {
-                    "documentation": "<p>The After Call Work (ACW) timeout setting, in seconds. This parameter has a minimum value of 0 and a maximum value of 2,000,000 seconds (24 days). Enter 0 if you don't want to allocate a specific amount of ACW time. It essentially means an indefinite amount of time. When the conversation ends, ACW starts; the agent must choose Close contact to end ACW. </p> <note> <p>When returned by a <code>SearchUsers</code> call, <code>AfterContactWorkTimeLimit</code> is returned in milliseconds. </p> </note>",
+                    "documentation": "<p>The After Call Work (ACW) timeout setting, in seconds.</p> <note> <p>When returned by a <code>SearchUsers</code> call, <code>AfterContactWorkTimeLimit</code> is returned in milliseconds. </p> </note>",
                     "shape": "AfterContactWorkTimeLimit"
                 },
                 "AutoAccept": {
                     "documentation": "<p>The Auto accept setting.</p>",
                     "shape": "AutoAccept"
                 },
                 "DeskPhoneNumber": {
@@ -25679,29 +25588,25 @@
                     "shape": "HierarchyGroupCondition"
                 },
                 "OrConditions": {
                     "documentation": "<p>A list of conditions which would be applied together with an <code>OR</code> condition.</p>",
                     "shape": "UserSearchConditionList"
                 },
                 "StringCondition": {
-                    "documentation": "<p>A leaf node condition which can be used to specify a string condition.</p> <p>The currently supported values for <code>FieldName</code> are <code>Username</code>, <code>FirstName</code>, <code>LastName</code>, <code>RoutingProfileId</code>, <code>SecurityProfileId</code>, <code>ResourceId</code>.</p>",
+                    "documentation": "<p>A leaf node condition which can be used to specify a string condition.</p> <note> <p>The currently supported values for <code>FieldName</code> are <code>name</code>, <code>description</code>, and <code>resourceID</code>.</p> </note>",
                     "shape": "StringCondition"
                 }
             },
             "type": "structure"
         },
         "UserSearchFilter": {
             "documentation": "<p>Filters to be applied to search results.</p>",
             "members": {
                 "TagFilter": {
                     "shape": "ControlPlaneTagFilter"
-                },
-                "UserAttributeFilter": {
-                    "documentation": "<p>An object that can be used to specify Tag conditions or Hierarchy Group conditions inside the SearchFilter.</p> <p>This accepts an <code>OR</code> of <code>AND</code> (List of List) input where:</p> <ul> <li> <p>The top level list specifies conditions that need to be applied with <code>OR</code> operator.</p> </li> <li> <p>The inner list specifies conditions that need to be applied with <code>AND</code> operator.</p> </li> </ul> <note> <p>Only one field can be populated. This object can\u2019t be used along with TagFilter. Request can either contain TagFilter or UserAttributeFilter if SearchFilter is specified, combination of both is not supported and such request will throw AccessDeniedException.</p> </note>",
-                    "shape": "ControlPlaneUserAttributeFilter"
                 }
             },
             "type": "structure"
         },
         "UserSearchSummary": {
             "documentation": "<p>Information about the returned users.</p>",
             "members": {
```

### Comparing `botocore-a-la-carte-connect-1.34.80/botocore_a_la_carte_connect.egg-info/PKG-INFO` & `botocore-a-la-carte-connect-1.34.9/botocore_a_la_carte_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connect
-Version: 1.34.80
+Version: 1.34.9
 Summary: connect data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connect-1.34.80/setup.py` & `botocore-a-la-carte-connect-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-connect',
-    version="1.34.80",
+    version="1.34.9",
     description='connect data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/connect/*/*.json'],
```

