# Comparing `tmp/alibabacloud_mns-open20220119-1.0.0.tar.gz` & `tmp/alibabacloud_mns-open20220119-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.0.tar", last modified: Fri May 20 06:06:32 2022, max compression
+gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.1.tar", last modified: Wed Apr 10 10:13:58 2024, max compression
```

## Comparing `alibabacloud_mns-open20220119-1.0.0.tar` & `alibabacloud_mns-open20220119-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48282 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/client.py
--rw-r--r--   0 root         (0) root         (0)   101582 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      447 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-20 06:06:32.000000 alibabacloud_mns-open20220119-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2637 2022-05-20 06:06:31.000000 alibabacloud_mns-open20220119-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48282 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/client.py
+-rw-r--r--   0 root         (0) root         (0)    96228 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/setup.py
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/LICENSE` & `alibabacloud_mns-open20220119-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.0/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mns-open20220119
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/mns-open-20220119/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/README-CN.md` & `alibabacloud_mns-open20220119-1.0.1/README-CN.md`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/mns-open-20220119/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/README.md` & `alibabacloud_mns-open20220119-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/mns-open-20220119/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/client.py` & `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119/models.py` & `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,17 +173,14 @@
         body: CreateQueueResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -354,17 +351,14 @@
         body: CreateTopicResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -523,17 +517,14 @@
         body: DeleteQueueResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -651,17 +642,14 @@
         body: DeleteTopicResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -723,32 +711,28 @@
         delay_seconds: int = None,
         inactive_messages: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         maximum_message_size: int = None,
         message_retention_period: int = None,
         polling_wait_seconds: int = None,
-        queue_internal_url: str = None,
         queue_name: str = None,
-        queue_url: str = None,
         visibility_timeout: int = None,
     ):
         self.active_messages = active_messages
         self.create_time = create_time
         self.delay_messages = delay_messages
         self.delay_seconds = delay_seconds
         self.inactive_messages = inactive_messages
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
-        self.queue_internal_url = queue_internal_url
         self.queue_name = queue_name
-        self.queue_url = queue_url
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -772,20 +756,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -804,20 +784,16 @@
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
     def __init__(
@@ -886,17 +862,14 @@
         body: GetQueueAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -961,26 +934,24 @@
         create_time: int = None,
         endpoint: str = None,
         filter_tag: str = None,
         last_modify_time: int = None,
         notify_content_format: str = None,
         notify_strategy: str = None,
         subscription_name: str = None,
-        subscription_url: str = None,
         topic_name: str = None,
         topic_owner: str = None,
     ):
         self.create_time = create_time
         self.endpoint = endpoint
         self.filter_tag = filter_tag
         self.last_modify_time = last_modify_time
         self.notify_content_format = notify_content_format
         self.notify_strategy = notify_strategy
         self.subscription_name = subscription_name
-        self.subscription_url = subscription_url
         self.topic_name = topic_name
         self.topic_owner = topic_owner
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -999,16 +970,14 @@
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
 
     def from_map(self, m: dict = None):
@@ -1023,16 +992,14 @@
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
 
 
@@ -1103,17 +1070,14 @@
         body: GetSubscriptionAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1171,27 +1135,23 @@
         self,
         create_time: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         max_message_size: int = None,
         message_count: int = None,
         message_retention_period: int = None,
-        topic_inner_url: str = None,
         topic_name: str = None,
-        topic_url: str = None,
     ):
         self.create_time = create_time
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.max_message_size = max_message_size
         self.message_count = message_count
         self.message_retention_period = message_retention_period
-        self.topic_inner_url = topic_inner_url
         self.topic_name = topic_name
-        self.topic_url = topic_url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1206,20 +1166,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('LastModifyTime') is not None:
@@ -1228,20 +1184,16 @@
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
     def __init__(
         self,
         code: int = None,
@@ -1308,17 +1260,14 @@
         body: GetTopicAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1392,32 +1341,28 @@
         delay_seconds: int = None,
         inactive_messages: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         maximum_message_size: int = None,
         message_retention_period: int = None,
         polling_wait_seconds: int = None,
-        queue_internal_url: str = None,
         queue_name: str = None,
-        queue_url: str = None,
         visibility_timeout: int = None,
     ):
         self.active_messages = active_messages
         self.create_time = create_time
         self.delay_messages = delay_messages
         self.delay_seconds = delay_seconds
         self.inactive_messages = inactive_messages
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
-        self.queue_internal_url = queue_internal_url
         self.queue_name = queue_name
-        self.queue_url = queue_url
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1441,20 +1386,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -1473,20 +1414,16 @@
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
     def __init__(
@@ -1620,17 +1557,14 @@
         body: ListQueueResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1707,26 +1641,24 @@
         create_time: int = None,
         endpoint: str = None,
         filter_tag: str = None,
         last_modify_time: int = None,
         notify_content_format: str = None,
         notify_strategy: str = None,
         subscription_name: str = None,
-        subscription_url: str = None,
         topic_name: str = None,
         topic_owner: str = None,
     ):
         self.create_time = create_time
         self.endpoint = endpoint
         self.filter_tag = filter_tag
         self.last_modify_time = last_modify_time
         self.notify_content_format = notify_content_format
         self.notify_strategy = notify_strategy
         self.subscription_name = subscription_name
-        self.subscription_url = subscription_url
         self.topic_name = topic_name
         self.topic_owner = topic_owner
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1745,16 +1677,14 @@
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
 
     def from_map(self, m: dict = None):
@@ -1769,16 +1699,14 @@
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
 
 
@@ -1914,17 +1842,14 @@
         body: ListSubscriptionByTopicResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1994,27 +1919,23 @@
         self,
         create_time: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         max_message_size: int = None,
         message_count: int = None,
         message_retention_period: int = None,
-        topic_inner_url: str = None,
         topic_name: str = None,
-        topic_url: str = None,
     ):
         self.create_time = create_time
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.max_message_size = max_message_size
         self.message_count = message_count
         self.message_retention_period = message_retention_period
-        self.topic_inner_url = topic_inner_url
         self.topic_name = topic_name
-        self.topic_url = topic_url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -2029,20 +1950,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('LastModifyTime') is not None:
@@ -2051,20 +1968,16 @@
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
     def __init__(
         self,
         page_data: List[ListTopicResponseBodyDataPageData] = None,
@@ -2184,17 +2097,14 @@
         body: ListTopicResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2389,17 +2299,14 @@
         body: SetQueueAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2570,17 +2477,14 @@
         body: SetSubscriptionAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2751,17 +2655,14 @@
         body: SetTopicAttributesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2915,17 +2816,14 @@
         body: SubscribeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3090,17 +2988,14 @@
         body: UnsubscribeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/alibabacloud_mns_open20220119.egg-info/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mns-open20220119
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/mns-open-20220119/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_mns-open20220119-1.0.0/setup.py` & `alibabacloud_mns-open20220119-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mns-open20220119.
 
-Created on 20/05/2022
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mns_open20220119"
 NAME = "alibabacloud_mns-open20220119" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Mns-open (20220119) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

