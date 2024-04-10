# Comparing `tmp/ros-cdk-ddospro-1.0.23.tar.gz` & `tmp/ros-cdk-ddospro-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ddospro-1.0.23.tar", last modified: Mon Mar  4 07:37:21 2024, max compression
+gzip compressed data, was "dist/ros-cdk-ddospro-1.0.24.tar", last modified: Wed Apr 10 03:10:30 2024, max compression
```

## Comparing `ros-cdk-ddospro-1.0.23.tar` & `ros-cdk-ddospro-1.0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1900 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/
--rw-r--r--   0 root         (0) root         (0)   109499 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/_jsii/
--rw-r--r--   0 root         (0) root         (0)      427 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45286 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/_jsii/ros-cdk-ddospro@1.0.23.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-04 07:37:21.000000 ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/
+-rw-r--r--   0 root         (0) root         (0)   120981 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47859 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/_jsii/ros-cdk-ddospro@1.0.24.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-10 03:10:30.000000 ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/top_level.txt
```

### Comparing `ros-cdk-ddospro-1.0.23/LICENSE` & `ros-cdk-ddospro-1.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ddospro-1.0.23/PKG-INFO` & `ros-cdk-ddospro-1.0.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ddospro
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DDOSPRO Construct Library
```

### Comparing `ros-cdk-ddospro-1.0.23/setup.py` & `ros-cdk-ddospro-1.0.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ddospro",
-    "version": "1.0.23",
+    "version": "1.0.24",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ros_cdk_ddospro",
         "ros_cdk_ddospro._jsii"
     ],
     "package_data": {
         "ros_cdk_ddospro._jsii": [
-            "ros-cdk-ddospro@1.0.23.jsii.tgz"
+            "ros-cdk-ddospro@1.0.24.jsii.tgz"
         ],
         "ros_cdk_ddospro": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro/__init__.py` & `ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         "function_version": "functionVersion",
         "normal_bandwidth": "normalBandwidth",
         "normal_qps": "normalQps",
         "period": "period",
         "period_unit": "periodUnit",
         "port_count": "portCount",
         "product_plan": "productPlan",
+        "tags": "tags",
     },
 )
 class PremiumInstanceProps:
     def __init__(
         self,
         *,
         burst_bandwidth_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
@@ -138,40 +139,43 @@
         function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         product_plan: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosPremiumInstance.TagsProperty", typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``PremiumInstance``.
 
         See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-premiuminstance
 
         :param burst_bandwidth_mode: Property burstBandwidthMode: The metering method of the 95th percentile burstable clean bandwidth. Valid values: 0: disables the burstable clean bandwidth feature. 1: enables the burstable clean bandwidth feature and uses the daily 95th percentile metering method. 2: enables the burstable clean bandwidth feature and uses the monthly 95th percentile metering method.
         :param domain_count: Property domainCount: The number of domain names that you want to protect. The value of DomainCount varies based on the value of ProductPlan. If you set ProductPlan to 0, you can set DomainCount to a value that ranges from 10 to 200. The value must be a multiple of 10. If you set ProductPlan to 1, you can set DomainCount to a value that ranges from 10 to 200. The value must be a multiple of 10. If you set ProductPlan to 2, you do not need to specify this parameter. If you set ProductPlan to 3, you can set DomainCount to a value that ranges from 10 to 200. The value must be a multiple of 10.
         :param function_version: Property functionVersion: The function plan of the instance. Valid values: 0: the Standard function plan 1: the Enhanced function plan.
         :param normal_bandwidth: Property normalBandwidth: The clean bandwidth provided by the instance. Unit: Mbit/s. The value of NormalBandwidth varies based on the value of ProductPlan. If you set ProductPlan to 0, you can set NormalBandwidth to 100, 150, 200, 250, or 300. If you set ProductPlan to 1, you can set NormalBandwidth to 100, 150, 200, 250, or 300. If you set ProductPlan to 2, you can set NormalBandwidth to 10, 20, 30, 40, 50, 60, 70, 80, 90, or 100. If you set ProductPlan to 3, you can set NormalBandwidth to 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 150, or 200.
         :param normal_qps: Property normalQps: The clean QPS provided by the instance. The value of NormalQps varies based on the value of ProductPlan. If you set ProductPlan to 0, you can set NormalQps to a value that ranges from 500 to 100000. The value must be a multiple of 100. If you set ProductPlan to 1, you can set NormalQps to a value that ranges from 1000 to 100000. The value must be a multiple of 100. If you set ProductPlan to 2, you do not need to specify this parameter. If you set ProductPlan to 3, you can set NormalQps to a value that ranges from 500 to 100000. The value must be a multiple of 100.
         :param period: Property period: The subscription period of the firewallIf PeriodUnit is Month, the valid range is 1, 2, 3, 4, 5, 6, 12, 24 If PeriodUnit is Year, the valid range is 1, 2.
         :param period_unit: Property periodUnit: The unit of the subscription duration. Valid values: Month Year Default value: Month.
         :param port_count: Property portCount: The number of ports that you want to protect. The value of PortCount varies based on the value of ProductPlan. If you set ProductPlan to 0, you can set PortCount to a value that ranges from 5 to 400. The value must be a multiple of 5. If you set ProductPlan to 1, you can set PortCount to a value that ranges from 5 to 400. The value must be a multiple of 5. If you set ProductPlan to 2, you do not need to specify this parameter. If you set ProductPlan to 3, you can set PortCount to a value that ranges from 5 to 400. The value must be a multiple of 5.
         :param product_plan: Property productPlan: The mitigation plan of the instance. Valid values: 0: the Insurance mitigation plan 1: the Unlimited mitigation plan 2: the Chinese Mainland Acceleration (CMA) mitigation plan 3: the Secure Chinese Mainland Acceleration (Sec-CMA) mitigation plan
+        :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__33b9c9df9785aa47941a76764139beab5cf0b2655ff0df91ee406d53cfcc5f09)
             check_type(argname="argument burst_bandwidth_mode", value=burst_bandwidth_mode, expected_type=type_hints["burst_bandwidth_mode"])
             check_type(argname="argument domain_count", value=domain_count, expected_type=type_hints["domain_count"])
             check_type(argname="argument function_version", value=function_version, expected_type=type_hints["function_version"])
             check_type(argname="argument normal_bandwidth", value=normal_bandwidth, expected_type=type_hints["normal_bandwidth"])
             check_type(argname="argument normal_qps", value=normal_qps, expected_type=type_hints["normal_qps"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument port_count", value=port_count, expected_type=type_hints["port_count"])
             check_type(argname="argument product_plan", value=product_plan, expected_type=type_hints["product_plan"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if burst_bandwidth_mode is not None:
             self._values["burst_bandwidth_mode"] = burst_bandwidth_mode
         if domain_count is not None:
             self._values["domain_count"] = domain_count
         if function_version is not None:
             self._values["function_version"] = function_version
@@ -183,14 +187,16 @@
             self._values["period"] = period
         if period_unit is not None:
             self._values["period_unit"] = period_unit
         if port_count is not None:
             self._values["port_count"] = port_count
         if product_plan is not None:
             self._values["product_plan"] = product_plan
+        if tags is not None:
+            self._values["tags"] = tags
 
     @builtins.property
     def burst_bandwidth_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''Property burstBandwidthMode: The metering method of the 95th percentile burstable clean bandwidth.
 
@@ -309,14 +315,23 @@
         1: the Unlimited mitigation plan
         2: the Chinese Mainland Acceleration (CMA) mitigation plan
         3: the Secure Chinese Mainland Acceleration (Sec-CMA) mitigation plan
         '''
         result = self._values.get("product_plan")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List["RosPremiumInstance.TagsProperty"]]:
+        '''Property tags: Tags to attach to instance.
+
+        Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List["RosPremiumInstance.TagsProperty"]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -428,14 +443,15 @@
         "function_version": "functionVersion",
         "normal_qps": "normalQps",
         "period": "period",
         "period_unit": "periodUnit",
         "port_count": "portCount",
         "service_bandwidth": "serviceBandwidth",
         "service_partner": "servicePartner",
+        "tags": "tags",
     },
 )
 class ProInstanceProps:
     def __init__(
         self,
         *,
         address_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
@@ -447,14 +463,15 @@
         function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosProInstance.TagsProperty", typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ProInstance``.
 
         See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-proinstance
 
         :param address_type: Property addressType: The IP version of the IP address. Valid values: Ipv4、Ipv6
         :param bandwidth: Property bandwidth: The burstable protection bandwidth. Unit: Gbit/s. The burstable protection bandwidth must be greater than or equal to the basic protection bandwidth. The value of Bandwidth varies based on the value of BaseBandwidth.
@@ -465,14 +482,15 @@
         :param function_version: Property functionVersion: The function plan of the instance. Valid values: 0: the Standard function plan 1: the Enhanced function plan.
         :param normal_qps: Property normalQps: The clean queries per second (QPS) provided by the instance. Valid values: 3000 to 100000. The value must be a multiple of 100.
         :param period: Property period: The subscription period of the firewallIf PeriodUnit is Month, the valid range is 1, 2, 3, 4, 5, 6, 12, 24 If PeriodUnit is Year, the valid range is 1, 2.
         :param period_unit: Property periodUnit: The unit of the subscription duration. Valid values: Month Year Default value: Month.
         :param port_count: Property portCount: The number of ports that you want to protect. Valid values: 50 to 400. The value must be a multiple of 5.
         :param service_bandwidth: Property serviceBandwidth: The clean bandwidth provided by the instance. Unit: Mbit/s. Valid values: 100 to 5000. The value must be a multiple of 50.
         :param service_partner: Property servicePartner: The type of the protection line. Set the value to coop-line-001, which indicates the default protection line.
+        :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c44bbb8ec4583870dc506e63c23a9ac3be0833397db59206ab27de71af81cf4e)
             check_type(argname="argument address_type", value=address_type, expected_type=type_hints["address_type"])
             check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
             check_type(argname="argument base_bandwidth", value=base_bandwidth, expected_type=type_hints["base_bandwidth"])
             check_type(argname="argument burst_bandwidth_mode", value=burst_bandwidth_mode, expected_type=type_hints["burst_bandwidth_mode"])
@@ -481,14 +499,15 @@
             check_type(argname="argument function_version", value=function_version, expected_type=type_hints["function_version"])
             check_type(argname="argument normal_qps", value=normal_qps, expected_type=type_hints["normal_qps"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument port_count", value=port_count, expected_type=type_hints["port_count"])
             check_type(argname="argument service_bandwidth", value=service_bandwidth, expected_type=type_hints["service_bandwidth"])
             check_type(argname="argument service_partner", value=service_partner, expected_type=type_hints["service_partner"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if address_type is not None:
             self._values["address_type"] = address_type
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
         if base_bandwidth is not None:
             self._values["base_bandwidth"] = base_bandwidth
@@ -508,14 +527,16 @@
             self._values["period_unit"] = period_unit
         if port_count is not None:
             self._values["port_count"] = port_count
         if service_bandwidth is not None:
             self._values["service_bandwidth"] = service_bandwidth
         if service_partner is not None:
             self._values["service_partner"] = service_partner
+        if tags is not None:
+            self._values["tags"] = tags
 
     @builtins.property
     def address_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''Property addressType: The IP version of the IP address.
 
@@ -660,14 +681,23 @@
         '''Property servicePartner: The type of the protection line.
 
         Set the value to coop-line-001, which indicates the default protection line.
         '''
         result = self._values.get("service_partner")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List["RosProInstance.TagsProperty"]]:
+        '''Property tags: Tags to attach to instance.
+
+        Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List["RosProInstance.TagsProperty"]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -981,28 +1011,103 @@
         value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c25b1df443a5877fcd2648a0afd35b88806de85f765fa995d81c94104e3d6b8a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productPlan", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="tags")
+    def tags(self) -> typing.Optional[typing.List["RosPremiumInstance.TagsProperty"]]:
+        '''
+        :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        return typing.cast(typing.Optional[typing.List["RosPremiumInstance.TagsProperty"]], jsii.get(self, "tags"))
+
+    @tags.setter
+    def tags(
+        self,
+        value: typing.Optional[typing.List["RosPremiumInstance.TagsProperty"]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9c180226d9e42f003edbf0b5612dd961e17bb08011a675d0d4bd598e04df731b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "tags", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-ddospro.RosPremiumInstance.TagsProperty",
+        jsii_struct_bases=[],
+        name_mapping={"key": "key", "value": "value"},
+    )
+    class TagsProperty:
+        def __init__(
+            self,
+            *,
+            key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ) -> None:
+            '''
+            :param key: 
+            :param value: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__d647de052945d5ace2a723703090aab896298ba7bd5d0ef9bd13a255dcd3ca68)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "key": key,
+            }
+            if value is not None:
+                self._values["value"] = value
+
+        @builtins.property
+        def key(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: key: undefined
+            '''
+            result = self._values.get("key")
+            assert result is not None, "Required property 'key' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def value(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: value: undefined
+            '''
+            result = self._values.get("value")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "TagsProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ddospro.RosPremiumInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
         "burst_bandwidth_mode": "burstBandwidthMode",
         "domain_count": "domainCount",
         "function_version": "functionVersion",
         "normal_bandwidth": "normalBandwidth",
         "normal_qps": "normalQps",
         "period": "period",
         "period_unit": "periodUnit",
         "port_count": "portCount",
         "product_plan": "productPlan",
+        "tags": "tags",
     },
 )
 class RosPremiumInstanceProps:
     def __init__(
         self,
         *,
         burst_bandwidth_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
@@ -1010,40 +1115,43 @@
         function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         product_plan: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosPremiumInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``RosPremiumInstance``.
 
         See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-premiuminstance
 
         :param burst_bandwidth_mode: 
         :param domain_count: 
         :param function_version: 
         :param normal_bandwidth: 
         :param normal_qps: 
         :param period: 
         :param period_unit: 
         :param port_count: 
         :param product_plan: 
+        :param tags: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e509db68cbc2a6b93f835fc7fc4874eab89c46ad0d88001ba8599e405f85e5de)
             check_type(argname="argument burst_bandwidth_mode", value=burst_bandwidth_mode, expected_type=type_hints["burst_bandwidth_mode"])
             check_type(argname="argument domain_count", value=domain_count, expected_type=type_hints["domain_count"])
             check_type(argname="argument function_version", value=function_version, expected_type=type_hints["function_version"])
             check_type(argname="argument normal_bandwidth", value=normal_bandwidth, expected_type=type_hints["normal_bandwidth"])
             check_type(argname="argument normal_qps", value=normal_qps, expected_type=type_hints["normal_qps"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument port_count", value=port_count, expected_type=type_hints["port_count"])
             check_type(argname="argument product_plan", value=product_plan, expected_type=type_hints["product_plan"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if burst_bandwidth_mode is not None:
             self._values["burst_bandwidth_mode"] = burst_bandwidth_mode
         if domain_count is not None:
             self._values["domain_count"] = domain_count
         if function_version is not None:
             self._values["function_version"] = function_version
@@ -1055,14 +1163,16 @@
             self._values["period"] = period
         if period_unit is not None:
             self._values["period_unit"] = period_unit
         if port_count is not None:
             self._values["port_count"] = port_count
         if product_plan is not None:
             self._values["product_plan"] = product_plan
+        if tags is not None:
+            self._values["tags"] = tags
 
     @builtins.property
     def burst_bandwidth_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property:
@@ -1197,14 +1307,22 @@
         1: the Unlimited mitigation plan
         2: the Chinese Mainland Acceleration (CMA) mitigation plan
         3: the Secure Chinese Mainland Acceleration (Sec-CMA) mitigation plan
         '''
         result = self._values.get("product_plan")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List[RosPremiumInstance.TagsProperty]]:
+        '''
+        :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List[RosPremiumInstance.TagsProperty]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1582,14 +1700,88 @@
         value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__09a2f952ce4f933a42625bdd924cb7fdae05cacc6ed938f4a7a0c971ae8eb42f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "servicePartner", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="tags")
+    def tags(self) -> typing.Optional[typing.List["RosProInstance.TagsProperty"]]:
+        '''
+        :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        return typing.cast(typing.Optional[typing.List["RosProInstance.TagsProperty"]], jsii.get(self, "tags"))
+
+    @tags.setter
+    def tags(
+        self,
+        value: typing.Optional[typing.List["RosProInstance.TagsProperty"]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__959edfbe54a57bf7469c7f7e2f7517803256234378ef4773b025f38fa68e4420)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "tags", value)
+
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-ddospro.RosProInstance.TagsProperty",
+        jsii_struct_bases=[],
+        name_mapping={"key": "key", "value": "value"},
+    )
+    class TagsProperty:
+        def __init__(
+            self,
+            *,
+            key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+            value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        ) -> None:
+            '''
+            :param key: 
+            :param value: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(_typecheckingstub__dcb197886757f3a8d7f04ff2cae020e1a170b76e81448c92e4d84deef1cc1ee8)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            self._values: typing.Dict[builtins.str, typing.Any] = {
+                "key": key,
+            }
+            if value is not None:
+                self._values["value"] = value
+
+        @builtins.property
+        def key(self) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+            '''
+            :Property: key: undefined
+            '''
+            result = self._values.get("key")
+            assert result is not None, "Required property 'key' is missing"
+            return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+        @builtins.property
+        def value(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
+            '''
+            :Property: value: undefined
+            '''
+            result = self._values.get("value")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "TagsProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-ddospro.RosProInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
         "address_type": "addressType",
         "bandwidth": "bandwidth",
@@ -1600,14 +1792,15 @@
         "function_version": "functionVersion",
         "normal_qps": "normalQps",
         "period": "period",
         "period_unit": "periodUnit",
         "port_count": "portCount",
         "service_bandwidth": "serviceBandwidth",
         "service_partner": "servicePartner",
+        "tags": "tags",
     },
 )
 class RosProInstanceProps:
     def __init__(
         self,
         *,
         address_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
@@ -1619,14 +1812,15 @@
         function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
         service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosProInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``RosProInstance``.
 
         See https://www.alibabacloud.com/help/ros/developer-reference/aliyun-ddospro-proinstance
 
         :param address_type: 
         :param bandwidth: 
@@ -1637,14 +1831,15 @@
         :param function_version: 
         :param normal_qps: 
         :param period: 
         :param period_unit: 
         :param port_count: 
         :param service_bandwidth: 
         :param service_partner: 
+        :param tags: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ecad0fcb5a638f7a89dba11c887c8b939e3386c25d1e9da5d2f582b2def8a158)
             check_type(argname="argument address_type", value=address_type, expected_type=type_hints["address_type"])
             check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
             check_type(argname="argument base_bandwidth", value=base_bandwidth, expected_type=type_hints["base_bandwidth"])
             check_type(argname="argument burst_bandwidth_mode", value=burst_bandwidth_mode, expected_type=type_hints["burst_bandwidth_mode"])
@@ -1653,14 +1848,15 @@
             check_type(argname="argument function_version", value=function_version, expected_type=type_hints["function_version"])
             check_type(argname="argument normal_qps", value=normal_qps, expected_type=type_hints["normal_qps"])
             check_type(argname="argument period", value=period, expected_type=type_hints["period"])
             check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
             check_type(argname="argument port_count", value=port_count, expected_type=type_hints["port_count"])
             check_type(argname="argument service_bandwidth", value=service_bandwidth, expected_type=type_hints["service_bandwidth"])
             check_type(argname="argument service_partner", value=service_partner, expected_type=type_hints["service_partner"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if address_type is not None:
             self._values["address_type"] = address_type
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
         if base_bandwidth is not None:
             self._values["base_bandwidth"] = base_bandwidth
@@ -1680,14 +1876,16 @@
             self._values["period_unit"] = period_unit
         if port_count is not None:
             self._values["port_count"] = port_count
         if service_bandwidth is not None:
             self._values["service_bandwidth"] = service_bandwidth
         if service_partner is not None:
             self._values["service_partner"] = service_partner
+        if tags is not None:
+            self._values["tags"] = tags
 
     @builtins.property
     def address_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property: addressType: The IP version of the IP address. Valid values: Ipv4、Ipv6
@@ -1846,14 +2044,22 @@
     ) -> typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]]:
         '''
         :Property: servicePartner: The type of the protection line. Set the value to coop-line-001, which indicates the default protection line.
         '''
         result = self._values.get("service_partner")
         return typing.cast(typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]], result)
 
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List[RosProInstance.TagsProperty]]:
+        '''
+        :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List[RosProInstance.TagsProperty]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1915,14 +2121,15 @@
     function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     product_plan: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[RosPremiumInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2e2c0ee9ebbc884f99cdb63a875d176538e2f18c4cb99a5bfbd35011c2010269(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
@@ -1967,14 +2174,15 @@
     function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[RosProInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a99e16ce9cfb5e0990d1e19a0ed74921a9a224b5d6f16b65a595dd882fa5dd0e(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
@@ -2046,25 +2254,40 @@
 
 def _typecheckingstub__c25b1df443a5877fcd2648a0afd35b88806de85f765fa995d81c94104e3d6b8a(
     value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__9c180226d9e42f003edbf0b5612dd961e17bb08011a675d0d4bd598e04df731b(
+    value: typing.Optional[typing.List[RosPremiumInstance.TagsProperty]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d647de052945d5ace2a723703090aab896298ba7bd5d0ef9bd13a255dcd3ca68(
+    *,
+    key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__e509db68cbc2a6b93f835fc7fc4874eab89c46ad0d88001ba8599e405f85e5de(
     *,
     burst_bandwidth_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     domain_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     product_plan: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[RosPremiumInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__91071cfc3d0eceb23634781d5e42a1a2f8f6940cfb83f91bd11e2934d4c2573a(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
@@ -2160,14 +2383,28 @@
 
 def _typecheckingstub__09a2f952ce4f933a42625bdd924cb7fdae05cacc6ed938f4a7a0c971ae8eb42f(
     value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__959edfbe54a57bf7469c7f7e2f7517803256234378ef4773b025f38fa68e4420(
+    value: typing.Optional[typing.List[RosProInstance.TagsProperty]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dcb197886757f3a8d7f04ff2cae020e1a170b76e81448c92e4d84deef1cc1ee8(
+    *,
+    key: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    value: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__ecad0fcb5a638f7a89dba11c887c8b939e3386c25d1e9da5d2f582b2def8a158(
     *,
     address_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     base_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     burst_bandwidth_mode: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     domain_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
@@ -2175,10 +2412,11 @@
     function_version: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     normal_qps: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     period_unit: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     port_count: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_bandwidth: typing.Optional[typing.Union[jsii.Number, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     service_partner: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[RosProInstance.TagsProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `ros-cdk-ddospro-1.0.23/src/ros_cdk_ddospro.egg-info/PKG-INFO` & `ros-cdk-ddospro-1.0.24/src/ros_cdk_ddospro.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ddospro
-Version: 1.0.23
+Version: 1.0.24
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DDOSPRO Construct Library
```

