# Comparing `tmp/mm_sdk-0.1.374.tar.gz` & `tmp/mm_sdk-0.1.375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_sdk-0.1.374.tar", max compression
+gzip compressed data, was "mm_sdk-0.1.375.tar", max compression
```

## Comparing `mm_sdk-0.1.374.tar` & `mm_sdk-0.1.375.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      943 2024-04-04 12:20:13.260074 mm_sdk-0.1.374/pyproject.toml
--rw-r--r--   0        0        0     1615 2023-08-28 20:35:53.000000 mm_sdk-0.1.374/sdk/__init__.py
--rw-r--r--   0        0        0     3260 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/admitad.py
--rw-r--r--   0        0        0     3235 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/analytics.py
--rw-r--r--   0        0        0      770 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/barcode_recognizer.py
--rw-r--r--   0        0        0      251 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/base.py
--rw-r--r--   0        0        0     3961 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/cash_register.py
--rw-r--r--   0        0        0      644 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/click_again.py
--rw-r--r--   0        0        0     8565 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/client.py
--rw-r--r--   0        0        0      714 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/cryptopro.py
--rw-r--r--   0        0        0     2504 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/elk.py
--rw-r--r--   0        0        0     1661 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/face_detector.py
--rw-r--r--   0        0        0     4361 2024-02-06 16:30:14.000000 mm_sdk-0.1.374/sdk/gift.py
--rw-r--r--   0        0        0    20030 2024-04-04 11:55:45.000000 mm_sdk-0.1.374/sdk/gigtest.py
--rw-r--r--   0        0        0        0 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/mis/__init__.py
--rw-r--r--   0        0        0     3449 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/mis/client.py
--rw-r--r--   0        0        0     3471 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/mis/crm.py
--rw-r--r--   0        0        0     3322 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/mis/lab.py
--rw-r--r--   0        0        0     3630 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/mis/lmk.py
--rw-r--r--   0        0        0     5188 2024-03-03 21:11:34.000000 mm_sdk-0.1.374/sdk/mis/mobil.py
--rw-r--r--   0        0        0      620 2024-02-06 16:30:14.000000 mm_sdk-0.1.374/sdk/mis/samd.py
--rw-r--r--   0        0        0     1295 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/mis/standalone.py
--rw-r--r--   0        0        0      577 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/mis/widgets.py
--rw-r--r--   0        0        0     4158 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/mobile_backend.py
--rw-r--r--   0        0        0      858 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/notemaster.py
--rw-r--r--   0        0        0     2878 2023-07-10 15:32:19.000000 mm_sdk-0.1.374/sdk/notification.py
--rw-r--r--   0        0        0     2607 2024-04-04 12:17:02.000000 mm_sdk-0.1.374/sdk/nsirosminzdrav.py
--rw-r--r--   0        0        0     5311 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/personal.py
--rw-r--r--   0        0        0    17080 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/pre_record.py
--rw-r--r--   0        0        0     1740 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/prodoctorov.py
--rw-r--r--   0        0        0     1738 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/reestr.py
--rw-r--r--   0        0        0     1343 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/roistat.py
--rw-r--r--   0        0        0     4226 2024-04-04 11:55:45.000000 mm_sdk-0.1.374/sdk/samd.py
--rw-r--r--   0        0        0      961 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/site_mobilmed.py
--rw-r--r--   0        0        0      687 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/sms.py
--rw-r--r--   0        0        0        0 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-11-02 10:40:21.000000 mm_sdk-0.1.374/sdk/utils/django_request_id.py
--rw-r--r--   0        0        0     5349 2023-01-25 15:18:03.000000 mm_sdk-0.1.374/sdk/yandex_courier.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.374/setup.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.374/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-04-10 14:45:27.279710 mm_sdk-0.1.375/pyproject.toml
+-rw-r--r--   0        0        0     1615 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/__init__.py
+-rw-r--r--   0        0        0     3260 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/admitad.py
+-rw-r--r--   0        0        0     3235 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/analytics.py
+-rw-r--r--   0        0        0      770 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/barcode_recognizer.py
+-rw-r--r--   0        0        0      251 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/base.py
+-rw-r--r--   0        0        0     3961 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/cash_register.py
+-rw-r--r--   0        0        0      644 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/click_again.py
+-rw-r--r--   0        0        0     8565 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/client.py
+-rw-r--r--   0        0        0      714 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/cryptopro.py
+-rw-r--r--   0        0        0     2504 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/elk.py
+-rw-r--r--   0        0        0     1661 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/face_detector.py
+-rw-r--r--   0        0        0     4361 2023-11-27 12:09:09.000000 mm_sdk-0.1.375/sdk/gift.py
+-rw-r--r--   0        0        0    20030 2024-03-26 14:29:33.000000 mm_sdk-0.1.375/sdk/gigtest.py
+-rw-r--r--   0        0        0        0 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/mis/__init__.py
+-rw-r--r--   0        0        0     3449 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/mis/client.py
+-rw-r--r--   0        0        0     3471 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/mis/crm.py
+-rw-r--r--   0        0        0     3322 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/mis/lab.py
+-rw-r--r--   0        0        0     3630 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/mis/lmk.py
+-rw-r--r--   0        0        0     5188 2024-03-03 21:06:55.000000 mm_sdk-0.1.375/sdk/mis/mobil.py
+-rw-r--r--   0        0        0      620 2023-11-27 12:09:09.000000 mm_sdk-0.1.375/sdk/mis/samd.py
+-rw-r--r--   0        0        0     1295 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/mis/standalone.py
+-rw-r--r--   0        0        0      577 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/mis/widgets.py
+-rw-r--r--   0        0        0     4158 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/mobile_backend.py
+-rw-r--r--   0        0        0      858 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/notemaster.py
+-rw-r--r--   0        0        0     2878 2023-07-06 11:21:02.000000 mm_sdk-0.1.375/sdk/notification.py
+-rw-r--r--   0        0        0     2607 2024-04-10 14:41:48.000000 mm_sdk-0.1.375/sdk/nsirosminzdrav.py
+-rw-r--r--   0        0        0     5311 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/personal.py
+-rw-r--r--   0        0        0    17080 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/pre_record.py
+-rw-r--r--   0        0        0     1740 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/prodoctorov.py
+-rw-r--r--   0        0        0     1738 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/reestr.py
+-rw-r--r--   0        0        0     1343 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/roistat.py
+-rw-r--r--   0        0        0     4377 2024-04-10 14:41:48.000000 mm_sdk-0.1.375/sdk/samd.py
+-rw-r--r--   0        0        0      961 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/site_mobilmed.py
+-rw-r--r--   0        0        0      687 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/sms.py
+-rw-r--r--   0        0        0        0 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-11-13 15:42:34.000000 mm_sdk-0.1.375/sdk/utils/django_request_id.py
+-rw-r--r--   0        0        0     5349 2023-01-25 14:48:25.000000 mm_sdk-0.1.375/sdk/yandex_courier.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.375/setup.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.375/PKG-INFO
```

### Comparing `mm_sdk-0.1.374/pyproject.toml` & `mm_sdk-0.1.375/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mm-sdk"
-version = "0.1.374"
+version = "0.1.375"
 description = ""
 authors = ["dyus <dyuuus@gmail.com>"]
 packages = [
     { include = "sdk" },
 ]
 
 [build-system]
```

### Comparing `mm_sdk-0.1.374/sdk/__init__.py` & `mm_sdk-0.1.375/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/admitad.py` & `mm_sdk-0.1.375/sdk/admitad.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/analytics.py` & `mm_sdk-0.1.375/sdk/analytics.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/barcode_recognizer.py` & `mm_sdk-0.1.375/sdk/barcode_recognizer.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/cash_register.py` & `mm_sdk-0.1.375/sdk/cash_register.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/click_again.py` & `mm_sdk-0.1.375/sdk/click_again.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/client.py` & `mm_sdk-0.1.375/sdk/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/cryptopro.py` & `mm_sdk-0.1.375/sdk/cryptopro.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/elk.py` & `mm_sdk-0.1.375/sdk/elk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/face_detector.py` & `mm_sdk-0.1.375/sdk/face_detector.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/gift.py` & `mm_sdk-0.1.375/sdk/gift.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/gigtest.py` & `mm_sdk-0.1.375/sdk/gigtest.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/client.py` & `mm_sdk-0.1.375/sdk/mis/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/crm.py` & `mm_sdk-0.1.375/sdk/mis/crm.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/lab.py` & `mm_sdk-0.1.375/sdk/mis/lab.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/lmk.py` & `mm_sdk-0.1.375/sdk/mis/lmk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/mobil.py` & `mm_sdk-0.1.375/sdk/mis/mobil.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/samd.py` & `mm_sdk-0.1.375/sdk/mis/samd.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/standalone.py` & `mm_sdk-0.1.375/sdk/mis/standalone.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mis/widgets.py` & `mm_sdk-0.1.375/sdk/mis/widgets.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/mobile_backend.py` & `mm_sdk-0.1.375/sdk/mobile_backend.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/notemaster.py` & `mm_sdk-0.1.375/sdk/notemaster.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/notification.py` & `mm_sdk-0.1.375/sdk/notification.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/nsirosminzdrav.py` & `mm_sdk-0.1.375/sdk/nsirosminzdrav.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/personal.py` & `mm_sdk-0.1.375/sdk/personal.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/pre_record.py` & `mm_sdk-0.1.375/sdk/pre_record.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/prodoctorov.py` & `mm_sdk-0.1.375/sdk/prodoctorov.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/reestr.py` & `mm_sdk-0.1.375/sdk/reestr.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/roistat.py` & `mm_sdk-0.1.375/sdk/roistat.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/samd.py` & `mm_sdk-0.1.375/sdk/samd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 from enum import IntEnum
-from typing import List, Optional
+from typing import List, Literal, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from .client import Empty, HttpUrl, SDKClient, SDKResponse
 
 
 class OrderType(IntEnum):
     lmk = 0
     prof = 1
@@ -155,14 +155,17 @@
 class AddMedRecordRequest(BaseModel):
     mis_id: str  # номер заявки
     order_type: OrderType
     creation_date: datetime.datetime  # lmk - order_time / prof - exams_start
     med_center: MedCenter
     patient: AddPatientRequest
     order: Order
+    samd_type: Literal["103", "194", "230"] = Field(
+        description="Доступные типы документов samd"
+    )
     head_doctor: Optional[Doctor]
     exams: List[Exam]
     lab_services: List[LabService]
     functional_diagnostics: List[FuncDiag]
     vaccinations: List[Vaccine]
```

### Comparing `mm_sdk-0.1.374/sdk/site_mobilmed.py` & `mm_sdk-0.1.375/sdk/site_mobilmed.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/sms.py` & `mm_sdk-0.1.375/sdk/sms.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/sdk/yandex_courier.py` & `mm_sdk-0.1.375/sdk/yandex_courier.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.374/setup.py` & `mm_sdk-0.1.375/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0', 'pydantic>=1.7.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mm-sdk',
-    'version': '0.1.374',
+    'version': '0.1.375',
     'description': '',
     'long_description': 'None',
     'author': 'dyus',
     'author_email': 'dyuuus@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mm_sdk-0.1.374/PKG-INFO` & `mm_sdk-0.1.375/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mm-sdk
-Version: 0.1.374
+Version: 0.1.375
 Summary: 
 Author: dyus
 Author-email: dyuuus@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

