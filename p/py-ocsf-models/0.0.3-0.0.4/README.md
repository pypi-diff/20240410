# Comparing `tmp/py_ocsf_models-0.0.3.tar.gz` & `tmp/py_ocsf_models-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ocsf_models-0.0.3.tar", max compression
+gzip compressed data, was "py_ocsf_models-0.0.4.tar", max compression
```

## Comparing `py_ocsf_models-0.0.3.tar` & `py_ocsf_models-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11345 2024-03-06 15:31:21.265125 py_ocsf_models-0.0.3/LICENSE
--rw-r--r--   0        0        0     2332 2024-03-11 12:09:10.837734 py_ocsf_models-0.0.3/README.md
--rw-r--r--   0        0        0       23 2024-03-11 12:09:10.839183 py_ocsf_models-0.0.3/py_ocsf_models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 15:31:21.266538 py_ocsf_models-0.0.3/py_ocsf_models/events/__init__.py
--rw-r--r--   0        0        0     4027 2024-03-14 12:31:19.320043 py_ocsf_models-0.0.3/py_ocsf_models/events/base_event.py
--rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267031 py_ocsf_models-0.0.3/py_ocsf_models/events/findings/__init__.py
--rw-r--r--   0        0        0     7740 2024-03-14 12:31:19.320325 py_ocsf_models-0.0.3/py_ocsf_models/events/findings/detection_finding.py
--rw-r--r--   0        0        0     8441 2024-03-11 12:09:10.840439 py_ocsf_models-0.0.3/py_ocsf_models/events/findings/finding.py
--rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267967 py_ocsf_models-0.0.3/py_ocsf_models/objects/__init__.py
--rw-r--r--   0        0        0     1105 2024-03-11 12:09:10.840756 py_ocsf_models-0.0.3/py_ocsf_models/objects/account.py
--rw-r--r--   0        0        0     1314 2024-03-06 15:31:21.268346 py_ocsf_models-0.0.3/py_ocsf_models/objects/api.py
--rw-r--r--   0        0        0     1151 2024-03-06 15:31:21.268692 py_ocsf_models-0.0.3/py_ocsf_models/objects/cloud.py
--rw-r--r--   0        0        0     1274 2024-03-06 15:31:21.268963 py_ocsf_models-0.0.3/py_ocsf_models/objects/container.py
--rw-r--r--   0        0        0     6676 2024-03-11 12:09:10.841141 py_ocsf_models-0.0.3/py_ocsf_models/objects/device.py
--rw-r--r--   0        0        0     3533 2024-03-06 15:31:21.269601 py_ocsf_models-0.0.3/py_ocsf_models/objects/device_hardware_info.py
--rw-r--r--   0        0        0     2078 2024-03-11 12:09:10.841513 py_ocsf_models-0.0.3/py_ocsf_models/objects/dns_query.py
--rw-r--r--   0        0        0      879 2024-03-11 12:09:10.841860 py_ocsf_models-0.0.3/py_ocsf_models/objects/enrichment.py
--rw-r--r--   0        0        0     1985 2024-03-11 12:09:10.842241 py_ocsf_models-0.0.3/py_ocsf_models/objects/evidence_artifacts.py
--rw-r--r--   0        0        0        0 2024-03-06 15:31:21.270134 py_ocsf_models-0.0.3/py_ocsf_models/objects/finding_info.py
--rw-r--r--   0        0        0     1883 2024-03-11 12:09:10.842541 py_ocsf_models-0.0.3/py_ocsf_models/objects/fingerprint.py
--rw-r--r--   0        0        0     1540 2024-03-06 15:31:21.270417 py_ocsf_models-0.0.3/py_ocsf_models/objects/geolocation.py
--rw-r--r--   0        0        0     1064 2024-03-11 12:09:10.842863 py_ocsf_models-0.0.3/py_ocsf_models/objects/group.py
--rw-r--r--   0        0        0      832 2024-03-06 15:31:21.270778 py_ocsf_models-0.0.3/py_ocsf_models/objects/image.py
--rw-r--r--   0        0        0     1431 2024-03-06 15:31:21.271013 py_ocsf_models-0.0.3/py_ocsf_models/objects/kb_article.py
--rw-r--r--   0        0        0     2735 2024-03-06 15:31:21.271448 py_ocsf_models-0.0.3/py_ocsf_models/objects/ldap_person.py
--rw-r--r--   0        0        0     5100 2024-03-11 12:09:10.843189 py_ocsf_models-0.0.3/py_ocsf_models/objects/metadata.py
--rw-r--r--   0        0        0     2996 2024-03-06 15:31:21.271939 py_ocsf_models-0.0.3/py_ocsf_models/objects/mitre_attack.py
--rw-r--r--   0        0        0     1847 2024-03-11 12:09:10.843473 py_ocsf_models-0.0.3/py_ocsf_models/objects/network_interface.py
--rw-r--r--   0        0        0     6923 2024-03-11 12:09:10.843766 py_ocsf_models-0.0.3/py_ocsf_models/objects/observable.py
--rw-r--r--   0        0        0     2320 2024-03-11 12:09:10.844124 py_ocsf_models-0.0.3/py_ocsf_models/objects/operating_system.py
--rw-r--r--   0        0        0      799 2024-03-11 12:09:10.844545 py_ocsf_models-0.0.3/py_ocsf_models/objects/organization.py
--rw-r--r--   0        0        0     1882 2024-03-11 12:09:10.844874 py_ocsf_models-0.0.3/py_ocsf_models/objects/product.py
--rw-r--r--   0        0        0     1688 2024-03-10 09:15:43.853081 py_ocsf_models-0.0.3/py_ocsf_models/objects/related_event.py
--rw-r--r--   0        0        0      822 2024-03-06 15:31:21.273171 py_ocsf_models-0.0.3/py_ocsf_models/objects/remediation.py
--rw-r--r--   0        0        0      892 2024-03-11 12:09:10.845163 py_ocsf_models-0.0.3/py_ocsf_models/objects/request_elements.py
--rw-r--r--   0        0        0     1786 2024-03-11 12:09:10.845495 py_ocsf_models-0.0.3/py_ocsf_models/objects/resource_details.py
--rw-r--r--   0        0        0     1582 2024-03-11 12:09:10.845781 py_ocsf_models-0.0.3/py_ocsf_models/objects/response_elements.py
--rw-r--r--   0        0        0      931 2024-03-06 15:31:21.273846 py_ocsf_models-0.0.3/py_ocsf_models/objects/service.py
--rw-r--r--   0        0        0     2096 2024-03-06 15:31:21.274093 py_ocsf_models-0.0.3/py_ocsf_models/objects/user.py
--rw-r--r--   0        0        0     2951 2024-03-06 15:31:21.274373 py_ocsf_models-0.0.3/py_ocsf_models/objects/vulnerability_details.py
--rw-r--r--   0        0        0     1401 2024-03-14 12:31:19.321359 py_ocsf_models-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 py_ocsf_models-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-03-06 15:31:21.265125 py_ocsf_models-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2332 2024-03-11 12:09:10.837734 py_ocsf_models-0.0.4/README.md
+-rw-r--r--   0        0        0       23 2024-03-11 12:09:10.839183 py_ocsf_models-0.0.4/py_ocsf_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.266538 py_ocsf_models-0.0.4/py_ocsf_models/events/__init__.py
+-rw-r--r--   0        0        0     4027 2024-04-10 07:15:58.360679 py_ocsf_models-0.0.4/py_ocsf_models/events/base_event.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267031 py_ocsf_models-0.0.4/py_ocsf_models/events/findings/__init__.py
+-rw-r--r--   0        0        0     7740 2024-03-14 12:31:19.320325 py_ocsf_models-0.0.4/py_ocsf_models/events/findings/detection_finding.py
+-rw-r--r--   0        0        0     8441 2024-03-11 12:09:10.840439 py_ocsf_models-0.0.4/py_ocsf_models/events/findings/finding.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267967 py_ocsf_models-0.0.4/py_ocsf_models/objects/__init__.py
+-rw-r--r--   0        0        0     1105 2024-03-11 12:09:10.840756 py_ocsf_models-0.0.4/py_ocsf_models/objects/account.py
+-rw-r--r--   0        0        0     1314 2024-03-06 15:31:21.268346 py_ocsf_models-0.0.4/py_ocsf_models/objects/api.py
+-rw-r--r--   0        0        0     1151 2024-03-06 15:31:21.268692 py_ocsf_models-0.0.4/py_ocsf_models/objects/cloud.py
+-rw-r--r--   0        0        0     1274 2024-03-06 15:31:21.268963 py_ocsf_models-0.0.4/py_ocsf_models/objects/container.py
+-rw-r--r--   0        0        0     6676 2024-03-11 12:09:10.841141 py_ocsf_models-0.0.4/py_ocsf_models/objects/device.py
+-rw-r--r--   0        0        0     3533 2024-03-06 15:31:21.269601 py_ocsf_models-0.0.4/py_ocsf_models/objects/device_hardware_info.py
+-rw-r--r--   0        0        0     2078 2024-03-11 12:09:10.841513 py_ocsf_models-0.0.4/py_ocsf_models/objects/dns_query.py
+-rw-r--r--   0        0        0      879 2024-03-11 12:09:10.841860 py_ocsf_models-0.0.4/py_ocsf_models/objects/enrichment.py
+-rw-r--r--   0        0        0     1985 2024-03-11 12:09:10.842241 py_ocsf_models-0.0.4/py_ocsf_models/objects/evidence_artifacts.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.270134 py_ocsf_models-0.0.4/py_ocsf_models/objects/finding_info.py
+-rw-r--r--   0        0        0     1883 2024-03-11 12:09:10.842541 py_ocsf_models-0.0.4/py_ocsf_models/objects/fingerprint.py
+-rw-r--r--   0        0        0     1540 2024-03-06 15:31:21.270417 py_ocsf_models-0.0.4/py_ocsf_models/objects/geolocation.py
+-rw-r--r--   0        0        0     1064 2024-03-11 12:09:10.842863 py_ocsf_models-0.0.4/py_ocsf_models/objects/group.py
+-rw-r--r--   0        0        0      832 2024-03-06 15:31:21.270778 py_ocsf_models-0.0.4/py_ocsf_models/objects/image.py
+-rw-r--r--   0        0        0     1431 2024-03-06 15:31:21.271013 py_ocsf_models-0.0.4/py_ocsf_models/objects/kb_article.py
+-rw-r--r--   0        0        0     2735 2024-03-06 15:31:21.271448 py_ocsf_models-0.0.4/py_ocsf_models/objects/ldap_person.py
+-rw-r--r--   0        0        0     5100 2024-03-11 12:09:10.843189 py_ocsf_models-0.0.4/py_ocsf_models/objects/metadata.py
+-rw-r--r--   0        0        0     2996 2024-03-06 15:31:21.271939 py_ocsf_models-0.0.4/py_ocsf_models/objects/mitre_attack.py
+-rw-r--r--   0        0        0     1847 2024-03-11 12:09:10.843473 py_ocsf_models-0.0.4/py_ocsf_models/objects/network_interface.py
+-rw-r--r--   0        0        0     6923 2024-03-11 12:09:10.843766 py_ocsf_models-0.0.4/py_ocsf_models/objects/observable.py
+-rw-r--r--   0        0        0     2320 2024-03-11 12:09:10.844124 py_ocsf_models-0.0.4/py_ocsf_models/objects/operating_system.py
+-rw-r--r--   0        0        0      799 2024-03-11 12:09:10.844545 py_ocsf_models-0.0.4/py_ocsf_models/objects/organization.py
+-rw-r--r--   0        0        0     1882 2024-03-11 12:09:10.844874 py_ocsf_models-0.0.4/py_ocsf_models/objects/product.py
+-rw-r--r--   0        0        0     1688 2024-03-10 09:15:43.853081 py_ocsf_models-0.0.4/py_ocsf_models/objects/related_event.py
+-rw-r--r--   0        0        0      822 2024-03-06 15:31:21.273171 py_ocsf_models-0.0.4/py_ocsf_models/objects/remediation.py
+-rw-r--r--   0        0        0      892 2024-03-11 12:09:10.845163 py_ocsf_models-0.0.4/py_ocsf_models/objects/request_elements.py
+-rw-r--r--   0        0        0     1786 2024-03-11 12:09:10.845495 py_ocsf_models-0.0.4/py_ocsf_models/objects/resource_details.py
+-rw-r--r--   0        0        0     1582 2024-03-11 12:09:10.845781 py_ocsf_models-0.0.4/py_ocsf_models/objects/response_elements.py
+-rw-r--r--   0        0        0      931 2024-03-06 15:31:21.273846 py_ocsf_models-0.0.4/py_ocsf_models/objects/service.py
+-rw-r--r--   0        0        0     2096 2024-03-06 15:31:21.274093 py_ocsf_models-0.0.4/py_ocsf_models/objects/user.py
+-rw-r--r--   0        0        0     2951 2024-03-06 15:31:21.274373 py_ocsf_models-0.0.4/py_ocsf_models/objects/vulnerability_details.py
+-rw-r--r--   0        0        0     1476 2024-04-10 07:16:38.541253 py_ocsf_models-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 py_ocsf_models-0.0.4/PKG-INFO
```

### Comparing `py_ocsf_models-0.0.3/LICENSE` & `py_ocsf_models-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/README.md` & `py_ocsf_models-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/events/base_event.py` & `py_ocsf_models-0.0.4/py_ocsf_models/events/base_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
     - Raw Data (raw_data) [Optional]: Original data as received from the source.
     - Severity (severity) [Optional]: The event/finding severity, normalized to the caption of the severity_id value. In the case of 'Other', it is defined by the source.
     - Severity ID (severity_id) [Required]: The level of severity assigned to the event/finding.
     - Status (status) [Optional]: The normalized status of the Finding set by the consumer normalized to the caption of the status_id value. In the case of 'Other', it is defined by the source.
     - Status Code (status_code) [Optional]: The event status code, as reported by the event source. For example, in a Windows Failed Authentication event, this would be the value of 'Failure Code', e.g. 0x18.
     - Status Details (status_detail) [Optional]: The status details contains additional information about the event/finding outcome.
     - Status ID (status_id) [Optional]: The normalized status identifier of the Finding, set by the consumer.
-    - Unmapped Data (unmapped_data) [Optional]: The attributes that are not mapped to the event schema. The names and values of those attributes are specific to the event source.
+    - Unmapped Data (unmapped) [Optional]: The attributes that are not mapped to the event schema. The names and values of those attributes are specific to the event source.
     """
 
     enrichments: Optional[list[Enrichment]]
     message: Optional[str]
     metadata: Metadata
     observables: Optional[list[Observable]]
     raw_data: Optional[str]
     severity_id: SeverityID
     severity: Optional[str]
     status: Optional[str]
     status_code: Optional[str]
     status_detail: Optional[str]
     status_id: Optional[StatusID]
-    unmapped_data: object
+    unmapped: Optional[object]
```

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/events/findings/detection_finding.py` & `py_ocsf_models-0.0.4/py_ocsf_models/events/findings/detection_finding.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/events/findings/finding.py` & `py_ocsf_models-0.0.4/py_ocsf_models/events/findings/finding.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/account.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/account.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/api.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/api.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/cloud.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/cloud.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/container.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/container.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/device.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/device.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/device_hardware_info.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/device_hardware_info.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/dns_query.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/dns_query.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/enrichment.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/enrichment.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/evidence_artifacts.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/evidence_artifacts.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/fingerprint.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/fingerprint.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/geolocation.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/geolocation.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/group.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/group.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/image.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/image.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/kb_article.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/kb_article.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/ldap_person.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/ldap_person.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/metadata.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/metadata.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/mitre_attack.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/mitre_attack.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/network_interface.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/network_interface.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/observable.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/observable.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/operating_system.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/operating_system.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/organization.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/organization.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/product.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/product.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/related_event.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/related_event.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/remediation.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/remediation.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/request_elements.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/request_elements.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/resource_details.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/resource_details.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/response_elements.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/response_elements.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/service.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/service.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/user.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/user.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/py_ocsf_models/objects/vulnerability_details.py` & `py_ocsf_models-0.0.4/py_ocsf_models/objects/vulnerability_details.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.0.3/PKG-INFO` & `py_ocsf_models-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py-ocsf-models
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a Python implementation of the OCSF models. The models are used to represent the data of the OCSF Schema defined in https://schema.ocsf.io/.
 License: Apache-2.0
 Author: Prowler Team
 Author-email: engineering@prowler.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@prowler.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: email-validator (==2.1.0.post1)
+Requires-Dist: email-validator (==2.1.1)
 Requires-Dist: pydantic (==1.10.14)
 Project-URL: Changelog, https://github.com/prowler-cloud/py-ocsf-models/releases
 Project-URL: Documentation, https://docs.prowler.cloud
 Project-URL: Homepage, https://github.com/prowler-cloud/py-ocsf-models
 Project-URL: Issue tracker, https://github.com/prowler-cloud/py-ocsf-models/issues
 Description-Content-Type: text/markdown
```

