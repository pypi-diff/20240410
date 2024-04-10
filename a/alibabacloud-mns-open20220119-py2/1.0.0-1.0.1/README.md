# Comparing `tmp/alibabacloud_mns-open20220119_py2-1.0.0.tar.gz` & `tmp/alibabacloud_mns-open20220119_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mns-open20220119_py2-1.0.0.tar", last modified: Fri May 20 06:07:51 2022, max compression
+gzip compressed data, was "dist/alibabacloud_mns-open20220119_py2-1.0.1.tar", last modified: Wed Apr 10 10:14:22 2024, max compression
```

## Comparing `alibabacloud_mns-open20220119_py2-1.0.0.tar` & `alibabacloud_mns-open20220119_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20154 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/client.py
--rw-r--r--   0 root         (0) root         (0)   101894 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      467 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2930 2022-05-20 06:07:51.000000 alibabacloud_mns-open20220119_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20154 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/client.py
+-rw-r--r--   0 root         (0) root         (0)    96492 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 10:14:22.000000 alibabacloud_mns-open20220119_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-10 10:14:21.000000 alibabacloud_mns-open20220119_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/LICENSE` & `alibabacloud_mns-open20220119_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/PKG-INFO` & `alibabacloud_mns-open20220119_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mns-open20220119_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/README-CN.md` & `alibabacloud_mns-open20220119_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/README.md` & `alibabacloud_mns-open20220119_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/client.py` & `alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119/models.py` & `alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,14 @@
 class CreateQueueResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateQueueResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateQueueResponse, self).to_map()
         if _map is not None:
             return _map
@@ -304,17 +301,14 @@
 class CreateTopicResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateTopicResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateTopicResponse, self).to_map()
         if _map is not None:
             return _map
@@ -452,17 +446,14 @@
 class DeleteQueueResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteQueueResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteQueueResponse, self).to_map()
         if _map is not None:
             return _map
@@ -564,17 +555,14 @@
 class DeleteTopicResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteTopicResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteTopicResponse, self).to_map()
         if _map is not None:
             return _map
@@ -623,29 +611,26 @@
             self.queue_name = m.get('QueueName')
         return self
 
 
 class GetQueueAttributesResponseBodyData(TeaModel):
     def __init__(self, active_messages=None, create_time=None, delay_messages=None, delay_seconds=None,
                  inactive_messages=None, last_modify_time=None, logging_enabled=None, maximum_message_size=None,
-                 message_retention_period=None, polling_wait_seconds=None, queue_internal_url=None, queue_name=None, queue_url=None,
-                 visibility_timeout=None):
+                 message_retention_period=None, polling_wait_seconds=None, queue_name=None, visibility_timeout=None):
         self.active_messages = active_messages  # type: long
         self.create_time = create_time  # type: long
         self.delay_messages = delay_messages  # type: long
         self.delay_seconds = delay_seconds  # type: long
         self.inactive_messages = inactive_messages  # type: long
         self.last_modify_time = last_modify_time  # type: long
         self.logging_enabled = logging_enabled  # type: bool
         self.maximum_message_size = maximum_message_size  # type: long
         self.message_retention_period = message_retention_period  # type: long
         self.polling_wait_seconds = polling_wait_seconds  # type: long
-        self.queue_internal_url = queue_internal_url  # type: str
         self.queue_name = queue_name  # type: str
-        self.queue_url = queue_url  # type: str
         self.visibility_timeout = visibility_timeout  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetQueueAttributesResponseBodyData, self).to_map()
@@ -669,20 +654,16 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.maximum_message_size is not None:
             result['MaximumMessageSize'] = self.maximum_message_size
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
         if self.polling_wait_seconds is not None:
             result['PollingWaitSeconds'] = self.polling_wait_seconds
-        if self.queue_internal_url is not None:
-            result['QueueInternalUrl'] = self.queue_internal_url
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
-        if self.queue_url is not None:
-            result['QueueUrl'] = self.queue_url
         if self.visibility_timeout is not None:
             result['VisibilityTimeout'] = self.visibility_timeout
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -701,20 +682,16 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaximumMessageSize') is not None:
             self.maximum_message_size = m.get('MaximumMessageSize')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
         if m.get('PollingWaitSeconds') is not None:
             self.polling_wait_seconds = m.get('PollingWaitSeconds')
-        if m.get('QueueInternalUrl') is not None:
-            self.queue_internal_url = m.get('QueueInternalUrl')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
-        if m.get('QueueUrl') is not None:
-            self.queue_url = m.get('QueueUrl')
         if m.get('VisibilityTimeout') is not None:
             self.visibility_timeout = m.get('VisibilityTimeout')
         return self
 
 
 class GetQueueAttributesResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None, status=None, success=None):
@@ -770,17 +747,14 @@
 class GetQueueAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetQueueAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetQueueAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -833,24 +807,22 @@
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class GetSubscriptionAttributesResponseBodyData(TeaModel):
     def __init__(self, create_time=None, endpoint=None, filter_tag=None, last_modify_time=None,
-                 notify_content_format=None, notify_strategy=None, subscription_name=None, subscription_url=None, topic_name=None,
-                 topic_owner=None):
+                 notify_content_format=None, notify_strategy=None, subscription_name=None, topic_name=None, topic_owner=None):
         self.create_time = create_time  # type: long
         self.endpoint = endpoint  # type: str
         self.filter_tag = filter_tag  # type: str
         self.last_modify_time = last_modify_time  # type: long
         self.notify_content_format = notify_content_format  # type: str
         self.notify_strategy = notify_strategy  # type: str
         self.subscription_name = subscription_name  # type: str
-        self.subscription_url = subscription_url  # type: str
         self.topic_name = topic_name  # type: str
         self.topic_owner = topic_owner  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -869,16 +841,14 @@
             result['LastModifyTime'] = self.last_modify_time
         if self.notify_content_format is not None:
             result['NotifyContentFormat'] = self.notify_content_format
         if self.notify_strategy is not None:
             result['NotifyStrategy'] = self.notify_strategy
         if self.subscription_name is not None:
             result['SubscriptionName'] = self.subscription_name
-        if self.subscription_url is not None:
-            result['SubscriptionURL'] = self.subscription_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         if self.topic_owner is not None:
             result['TopicOwner'] = self.topic_owner
         return result
 
     def from_map(self, m=None):
@@ -893,16 +863,14 @@
             self.last_modify_time = m.get('LastModifyTime')
         if m.get('NotifyContentFormat') is not None:
             self.notify_content_format = m.get('NotifyContentFormat')
         if m.get('NotifyStrategy') is not None:
             self.notify_strategy = m.get('NotifyStrategy')
         if m.get('SubscriptionName') is not None:
             self.subscription_name = m.get('SubscriptionName')
-        if m.get('SubscriptionURL') is not None:
-            self.subscription_url = m.get('SubscriptionURL')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         if m.get('TopicOwner') is not None:
             self.topic_owner = m.get('TopicOwner')
         return self
 
 
@@ -960,17 +928,14 @@
 class GetSubscriptionAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetSubscriptionAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetSubscriptionAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1018,24 +983,22 @@
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class GetTopicAttributesResponseBodyData(TeaModel):
     def __init__(self, create_time=None, last_modify_time=None, logging_enabled=None, max_message_size=None,
-                 message_count=None, message_retention_period=None, topic_inner_url=None, topic_name=None, topic_url=None):
+                 message_count=None, message_retention_period=None, topic_name=None):
         self.create_time = create_time  # type: long
         self.last_modify_time = last_modify_time  # type: long
         self.logging_enabled = logging_enabled  # type: bool
         self.max_message_size = max_message_size  # type: long
         self.message_count = message_count  # type: long
         self.message_retention_period = message_retention_period  # type: long
-        self.topic_inner_url = topic_inner_url  # type: str
         self.topic_name = topic_name  # type: str
-        self.topic_url = topic_url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTopicAttributesResponseBodyData, self).to_map()
         if _map is not None:
@@ -1050,20 +1013,16 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
         if self.message_count is not None:
             result['MessageCount'] = self.message_count
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
-        if self.topic_inner_url is not None:
-            result['TopicInnerUrl'] = self.topic_inner_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
-        if self.topic_url is not None:
-            result['TopicUrl'] = self.topic_url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('LastModifyTime') is not None:
@@ -1072,20 +1031,16 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
         if m.get('MessageCount') is not None:
             self.message_count = m.get('MessageCount')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
-        if m.get('TopicInnerUrl') is not None:
-            self.topic_inner_url = m.get('TopicInnerUrl')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
-        if m.get('TopicUrl') is not None:
-            self.topic_url = m.get('TopicUrl')
         return self
 
 
 class GetTopicAttributesResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None, status=None, success=None):
         self.code = code  # type: long
         self.data = data  # type: GetTopicAttributesResponseBodyData
@@ -1139,17 +1094,14 @@
 class GetTopicAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetTopicAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetTopicAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1208,29 +1160,26 @@
             self.queue_name = m.get('QueueName')
         return self
 
 
 class ListQueueResponseBodyDataPageData(TeaModel):
     def __init__(self, active_messages=None, create_time=None, delay_messages=None, delay_seconds=None,
                  inactive_messages=None, last_modify_time=None, logging_enabled=None, maximum_message_size=None,
-                 message_retention_period=None, polling_wait_seconds=None, queue_internal_url=None, queue_name=None, queue_url=None,
-                 visibility_timeout=None):
+                 message_retention_period=None, polling_wait_seconds=None, queue_name=None, visibility_timeout=None):
         self.active_messages = active_messages  # type: long
         self.create_time = create_time  # type: long
         self.delay_messages = delay_messages  # type: long
         self.delay_seconds = delay_seconds  # type: long
         self.inactive_messages = inactive_messages  # type: long
         self.last_modify_time = last_modify_time  # type: long
         self.logging_enabled = logging_enabled  # type: bool
         self.maximum_message_size = maximum_message_size  # type: long
         self.message_retention_period = message_retention_period  # type: long
         self.polling_wait_seconds = polling_wait_seconds  # type: long
-        self.queue_internal_url = queue_internal_url  # type: str
         self.queue_name = queue_name  # type: str
-        self.queue_url = queue_url  # type: str
         self.visibility_timeout = visibility_timeout  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListQueueResponseBodyDataPageData, self).to_map()
@@ -1254,20 +1203,16 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.maximum_message_size is not None:
             result['MaximumMessageSize'] = self.maximum_message_size
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
         if self.polling_wait_seconds is not None:
             result['PollingWaitSeconds'] = self.polling_wait_seconds
-        if self.queue_internal_url is not None:
-            result['QueueInternalUrl'] = self.queue_internal_url
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
-        if self.queue_url is not None:
-            result['QueueUrl'] = self.queue_url
         if self.visibility_timeout is not None:
             result['VisibilityTimeout'] = self.visibility_timeout
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -1286,20 +1231,16 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaximumMessageSize') is not None:
             self.maximum_message_size = m.get('MaximumMessageSize')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
         if m.get('PollingWaitSeconds') is not None:
             self.polling_wait_seconds = m.get('PollingWaitSeconds')
-        if m.get('QueueInternalUrl') is not None:
-            self.queue_internal_url = m.get('QueueInternalUrl')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
-        if m.get('QueueUrl') is not None:
-            self.queue_url = m.get('QueueUrl')
         if m.get('VisibilityTimeout') is not None:
             self.visibility_timeout = m.get('VisibilityTimeout')
         return self
 
 
 class ListQueueResponseBodyData(TeaModel):
     def __init__(self, page_data=None, page_num=None, page_size=None, pages=None, size=None, total=None):
@@ -1412,17 +1353,14 @@
 class ListQueueResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListQueueResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListQueueResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1485,24 +1423,22 @@
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class ListSubscriptionByTopicResponseBodyDataPageData(TeaModel):
     def __init__(self, create_time=None, endpoint=None, filter_tag=None, last_modify_time=None,
-                 notify_content_format=None, notify_strategy=None, subscription_name=None, subscription_url=None, topic_name=None,
-                 topic_owner=None):
+                 notify_content_format=None, notify_strategy=None, subscription_name=None, topic_name=None, topic_owner=None):
         self.create_time = create_time  # type: long
         self.endpoint = endpoint  # type: str
         self.filter_tag = filter_tag  # type: str
         self.last_modify_time = last_modify_time  # type: long
         self.notify_content_format = notify_content_format  # type: str
         self.notify_strategy = notify_strategy  # type: str
         self.subscription_name = subscription_name  # type: str
-        self.subscription_url = subscription_url  # type: str
         self.topic_name = topic_name  # type: str
         self.topic_owner = topic_owner  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1521,16 +1457,14 @@
             result['LastModifyTime'] = self.last_modify_time
         if self.notify_content_format is not None:
             result['NotifyContentFormat'] = self.notify_content_format
         if self.notify_strategy is not None:
             result['NotifyStrategy'] = self.notify_strategy
         if self.subscription_name is not None:
             result['SubscriptionName'] = self.subscription_name
-        if self.subscription_url is not None:
-            result['SubscriptionURL'] = self.subscription_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         if self.topic_owner is not None:
             result['TopicOwner'] = self.topic_owner
         return result
 
     def from_map(self, m=None):
@@ -1545,16 +1479,14 @@
             self.last_modify_time = m.get('LastModifyTime')
         if m.get('NotifyContentFormat') is not None:
             self.notify_content_format = m.get('NotifyContentFormat')
         if m.get('NotifyStrategy') is not None:
             self.notify_strategy = m.get('NotifyStrategy')
         if m.get('SubscriptionName') is not None:
             self.subscription_name = m.get('SubscriptionName')
-        if m.get('SubscriptionURL') is not None:
-            self.subscription_url = m.get('SubscriptionURL')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         if m.get('TopicOwner') is not None:
             self.topic_owner = m.get('TopicOwner')
         return self
 
 
@@ -1669,17 +1601,14 @@
 class ListSubscriptionByTopicResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListSubscriptionByTopicResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListSubscriptionByTopicResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1737,24 +1666,22 @@
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class ListTopicResponseBodyDataPageData(TeaModel):
     def __init__(self, create_time=None, last_modify_time=None, logging_enabled=None, max_message_size=None,
-                 message_count=None, message_retention_period=None, topic_inner_url=None, topic_name=None, topic_url=None):
+                 message_count=None, message_retention_period=None, topic_name=None):
         self.create_time = create_time  # type: long
         self.last_modify_time = last_modify_time  # type: long
         self.logging_enabled = logging_enabled  # type: bool
         self.max_message_size = max_message_size  # type: long
         self.message_count = message_count  # type: long
         self.message_retention_period = message_retention_period  # type: long
-        self.topic_inner_url = topic_inner_url  # type: str
         self.topic_name = topic_name  # type: str
-        self.topic_url = topic_url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTopicResponseBodyDataPageData, self).to_map()
         if _map is not None:
@@ -1769,20 +1696,16 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
         if self.message_count is not None:
             result['MessageCount'] = self.message_count
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
-        if self.topic_inner_url is not None:
-            result['TopicInnerUrl'] = self.topic_inner_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
-        if self.topic_url is not None:
-            result['TopicUrl'] = self.topic_url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('LastModifyTime') is not None:
@@ -1791,20 +1714,16 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
         if m.get('MessageCount') is not None:
             self.message_count = m.get('MessageCount')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
-        if m.get('TopicInnerUrl') is not None:
-            self.topic_inner_url = m.get('TopicInnerUrl')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
-        if m.get('TopicUrl') is not None:
-            self.topic_url = m.get('TopicUrl')
         return self
 
 
 class ListTopicResponseBodyData(TeaModel):
     def __init__(self, page_data=None, page_num=None, page_size=None, total=None):
         self.page_data = page_data  # type: list[ListTopicResponseBodyDataPageData]
         self.page_num = page_num  # type: long
@@ -1905,17 +1824,14 @@
 class ListTopicResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListTopicResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListTopicResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2084,17 +2000,14 @@
 class SetQueueAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: SetQueueAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(SetQueueAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2242,17 +2155,14 @@
 class SetSubscriptionAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: SetSubscriptionAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(SetSubscriptionAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2400,17 +2310,14 @@
 class SetTopicAttributesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: SetTopicAttributesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(SetTopicAttributesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2543,17 +2450,14 @@
 class SubscribeResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: SubscribeResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(SubscribeResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2696,17 +2600,14 @@
 class UnsubscribeResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UnsubscribeResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UnsubscribeResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/alibabacloud_mns_open20220119_py2.egg-info/PKG-INFO` & `alibabacloud_mns-open20220119_py2-1.0.1/alibabacloud_mns_open20220119_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mns-open20220119-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119_py2-1.0.0/setup.py` & `alibabacloud_mns-open20220119_py2-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mns-open20220119_py2.
 
-Created on 20/05/2022
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mns_open20220119"
 NAME = "alibabacloud_mns-open20220119_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Mns-open (20220119) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.1, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

