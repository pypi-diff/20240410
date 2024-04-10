# Comparing `tmp/kindwise_api_client-0.4.0.tar.gz` & `tmp/kindwise_api_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindwise_api_client-0.4.0.tar", max compression
+gzip compressed data, was "kindwise_api_client-0.4.1.tar", max compression
```

## Comparing `kindwise_api_client-0.4.0.tar` & `kindwise_api_client-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    15020 2024-03-11 10:40:14.148629 kindwise_api_client-0.4.0/README.md
--rw-r--r--   0        0        0      321 2024-03-11 11:43:39.517221 kindwise_api_client-0.4.0/kindwise/__init__.py
--rw-r--r--   0        0        0    10300 2024-03-11 11:40:18.859253 kindwise_api_client-0.4.0/kindwise/core.py
--rw-r--r--   0        0        0     1694 2024-03-11 11:33:15.477209 kindwise_api_client-0.4.0/kindwise/crop_health.py
--rw-r--r--   0        0        0      877 2024-03-11 11:37:18.138380 kindwise_api_client-0.4.0/kindwise/insect.py
--rw-r--r--   0        0        0     6245 2024-03-11 11:42:11.302796 kindwise_api_client-0.4.0/kindwise/models.py
--rw-r--r--   0        0        0      887 2024-03-11 11:37:18.161380 kindwise_api_client-0.4.0/kindwise/mushroom.py
--rw-r--r--   0        0        0    14236 2024-03-11 11:42:11.333796 kindwise_api_client-0.4.0/kindwise/plant.py
--rw-r--r--   0        0        0      447 2024-03-06 15:57:33.494722 kindwise_api_client-0.4.0/kindwise/resources/views.crop_health.crop.json
--rw-r--r--   0        0        0     1570 2024-03-07 10:56:31.473071 kindwise_api_client-0.4.0/kindwise/resources/views.crop_health.disease.json
--rw-r--r--   0        0        0     1424 2024-01-18 07:57:54.888526 kindwise_api_client-0.4.0/kindwise/resources/views.insect.json
--rw-r--r--   0        0        0     2695 2024-01-18 07:57:54.888526 kindwise_api_client-0.4.0/kindwise/resources/views.mushroom.json
--rw-r--r--   0        0        0     1338 2024-01-18 07:57:54.888526 kindwise_api_client-0.4.0/kindwise/resources/views.plant.disease.json
--rw-r--r--   0        0        0     2425 2024-01-18 07:57:54.888526 kindwise_api_client-0.4.0/kindwise/resources/views.plant.json
--rw-r--r--   0        0        0      308 2024-03-06 16:17:37.491207 kindwise_api_client-0.4.0/kindwise/settings.py
--rw-r--r--   0        0        0        0 2024-01-18 07:57:54.889526 kindwise_api_client-0.4.0/kindwise/tests/__init__.py
--rw-r--r--   0        0        0     8816 2024-03-07 10:56:13.230952 kindwise_api_client-0.4.0/kindwise/tests/conftest.py
--rw-r--r--   0        0        0   100105 2024-01-18 07:57:54.889526 kindwise_api_client-0.4.0/kindwise/tests/resources/images/aloe-vera.jpg
--rw-r--r--   0        0        0   109179 2024-01-18 07:57:54.890526 kindwise_api_client-0.4.0/kindwise/tests/resources/images/amanita_muscaria.jpg
--rw-r--r--   0        0        0     6289 2024-01-18 07:57:54.890526 kindwise_api_client-0.4.0/kindwise/tests/resources/images/bee.jpeg
--rw-r--r--   0        0        0   448975 2024-01-18 07:57:54.891526 kindwise_api_client-0.4.0/kindwise/tests/resources/images/padli.png
--rw-r--r--   0        0        0   128013 2024-02-28 12:17:25.046703 kindwise_api_client-0.4.0/kindwise/tests/resources/images/potato.late_blight.jpg
--rw-r--r--   0        0        0    17581 2024-01-18 08:59:13.545635 kindwise_api_client-0.4.0/kindwise/tests/test_core.py
--rw-r--r--   0        0        0     1036 2024-03-07 10:54:57.698459 kindwise_api_client-0.4.0/kindwise/tests/test_crop.py
--rw-r--r--   0        0        0      846 2024-03-07 10:34:09.699392 kindwise_api_client-0.4.0/kindwise/tests/test_insect.py
--rw-r--r--   0        0        0      977 2024-01-18 07:57:54.892526 kindwise_api_client-0.4.0/kindwise/tests/test_mushroom.py
--rw-r--r--   0        0        0    47687 2024-03-11 11:45:15.328684 kindwise_api_client-0.4.0/kindwise/tests/test_plant.py
--rw-r--r--   0        0        0      751 2024-03-11 11:47:49.203427 kindwise_api_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    16314 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.0/setup.py
--rw-r--r--   0        0        0    15684 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 08:34:31.234839 kindwise_api_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0    15417 2024-04-10 14:53:25.786549 kindwise_api_client-0.4.1/README.md
+-rw-r--r--   0        0        0      342 2024-04-10 14:52:36.952691 kindwise_api_client-0.4.1/kindwise/__init__.py
+-rw-r--r--   0        0        0    10089 2024-04-10 14:43:46.804522 kindwise_api_client-0.4.1/kindwise/core.py
+-rw-r--r--   0        0        0     1694 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/crop_health.py
+-rw-r--r--   0        0        0      877 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/insect.py
+-rw-r--r--   0        0        0     6245 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/models.py
+-rw-r--r--   0        0        0      887 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/mushroom.py
+-rw-r--r--   0        0        0    14236 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/plant.py
+-rw-r--r--   0        0        0      447 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.crop.json
+-rw-r--r--   0        0        0     1570 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.disease.json
+-rw-r--r--   0        0        0     1424 2023-12-04 10:18:11.804140 kindwise_api_client-0.4.1/kindwise/resources/views.insect.json
+-rw-r--r--   0        0        0     2695 2023-12-04 09:08:49.453559 kindwise_api_client-0.4.1/kindwise/resources/views.mushroom.json
+-rw-r--r--   0        0        0     1338 2023-12-04 10:41:58.031606 kindwise_api_client-0.4.1/kindwise/resources/views.plant.disease.json
+-rw-r--r--   0        0        0     2425 2023-12-04 10:29:52.198769 kindwise_api_client-0.4.1/kindwise/resources/views.plant.json
+-rw-r--r--   0        0        0      308 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/settings.py
+-rw-r--r--   0        0        0        0 2023-11-21 14:46:34.497403 kindwise_api_client-0.4.1/kindwise/tests/__init__.py
+-rw-r--r--   0        0        0     8975 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/tests/conftest.py
+-rw-r--r--   0        0        0   100105 2023-11-28 08:59:44.985422 kindwise_api_client-0.4.1/kindwise/tests/resources/images/aloe-vera.jpg
+-rw-r--r--   0        0        0   109179 2023-11-28 14:48:26.224560 kindwise_api_client-0.4.1/kindwise/tests/resources/images/amanita_muscaria.jpg
+-rw-r--r--   0        0        0     6289 2023-11-22 08:44:35.598900 kindwise_api_client-0.4.1/kindwise/tests/resources/images/bee.jpeg
+-rw-r--r--   0        0        0   448975 2023-06-22 12:24:49.335643 kindwise_api_client-0.4.1/kindwise/tests/resources/images/padli.png
+-rw-r--r--   0        0        0   128013 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/tests/resources/images/potato.late_blight.jpg
+-rw-r--r--   0        0        0    18267 2024-04-10 14:50:31.251909 kindwise_api_client-0.4.1/kindwise/tests/test_core.py
+-rw-r--r--   0        0        0     1039 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_crop.py
+-rw-r--r--   0        0        0      894 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_insect.py
+-rw-r--r--   0        0        0     1025 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_mushroom.py
+-rw-r--r--   0        0        0    47760 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_plant.py
+-rw-r--r--   0        0        0      751 2024-04-10 15:01:03.960592 kindwise_api_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    16704 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.1/setup.py
+-rw-r--r--   0        0        0    16081 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.1/PKG-INFO
```

### Comparing `kindwise_api_client-0.4.0/README.md` & `kindwise_api_client-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 [admin.kindwise.com](https://admin.kindwise.com).
 
 ## Quick Start
 
 To use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.
 
 ```python
-from kindwise.plant import PlantApi
-from kindwise.models import PlantIdentification, UsageInfo
+from kindwise import PlantApi, PlantIdentification, UsageInfo
 
 # initialize plant.id api
 # "PLANT_API_KEY" environment variable can be set instead of specifying api_key
 api = PlantApi(api_key='your_api_key')
 
 # get usage information
 usage: UsageInfo = api.usage_info()
@@ -62,26 +61,26 @@
 - [plant.id](https://web.plant.id/plant-identification-api/)
 - [insect.id](https://insect.kindwise.com)
 - [mushroom.id](https://mushroom.kindwise.com)
 - [crop.health](https://crop.kindwise.com)
 
 Each system has its class, which is used to make requests to the API. Each class has the following methods:
 
-| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        | 
-|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------| 
-| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                | 
+| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        |
+|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
+| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |
 
 Datetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in
 local timezone.
 
 ### Documentation
 
 #### available_details
@@ -183,14 +182,23 @@
 with open('path/to/image.jpg', 'rb') as image :
     identification_from_file: PlantIdentification = api.identify(image)
 
 # identification created from base64 encoded image
 with open('path/to/image.jpg', 'rb') as image :
     image_in_base64 = base64.b64encode(image.read())
     identification_from_base64: PlantIdentification = api.identify(image)
+
+# identification created from PIL.Image.Image object
+from PIL import Image
+image = Image.open('path/to/image.jpg')
+identification_from_pil: PlantIdentification = api.identify(image)
+
+# identification created from image url
+image_url = 'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e'
+identification_from_url: PlantIdentification = api.identify(image_url)
 ```
 
 When you don't want to wait until the identification is finished, you can specify `asynchronous=True` and
 get `access_token`  or `custom_id` if specified and retrieve the answer later.
 
 ```python
 from kindwise import PlantApi, PlantIdentification
@@ -280,23 +288,29 @@
 method is similar to `identify` method, but it returns only health assessment. Details differs for each system.
 
 ```python
 from datetime import datetime
 
 from kindwise import PlantApi, HealthAssessment
 
-api = PlantApi(api_key='your_api_key')
+api = PlantApi(api_key="your_api_key")
 # the same as in identify method
-images = ['path/to/image1.jpg', 'path/to/image2.jpg', 'path/to/image3.jpg', 'path/to/image4.jpg', 'path/to/image5.jpg']
+images = [
+    "path/to/image1.jpg",
+    "path/to/image2.jpg",
+    "path/to/image3.jpg",
+    "path/to/image4.jpg",
+    "path/to/image5.jpg",
+]
 
 # details included in identification
-details = ['local_name', 'description', 'treatment', 'cause', 'image']
+details = ["local_name", "description", "treatment", "cause", "image"]
 
 # specify up to 3 languages
-language = ['en', 'cs']
+language = ["en", "cs"]
 
 # default for similar_images is True
 similar_images = True
 
 # where was an image taken
 latitude_longitude = (49.20340, 16.57318)
 
@@ -325,14 +339,15 @@
     similar_images=similar_images,
     latitude_longitude=latitude_longitude,
     custom_id=custom_id,
     full_disease_list=full_disease_list,
     date_time=date_time,
     max_image_size=max_image_size,
 )
+
 ```
 
 When you don't want to wait until the identification is finished, you can specify `asynchronous=True` similar
 to [`identify`](#identify) method.
 
 #### get_health_assessment
```

### Comparing `kindwise_api_client-0.4.0/kindwise/core.py` & `kindwise_api_client-0.4.1/kindwise/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,19 +34,32 @@
         return f'{self.identification_url}/{token}/feedback'
 
     def _make_api_call(self, url, method: str, data: dict | None = None):
         headers = {
             'Content-Type': 'application/json',
             'Api-Key': self.api_key,
         }
-        return requests.request(method, url, json=data, headers=headers)
+        response = requests.request(method, url, json=data, headers=headers)
+        if not response.ok:
+            raise ValueError(f'Error while making an API call: {response.status_code=} {response.text=}')
+        return response
 
     @staticmethod
     def _encode_image(image: PurePath | str | bytes | BinaryIO | Image.Image, max_image_size: int | None) -> str:
-        if isinstance(image, str) and len(image) <= 250:  # first try str as a path to a file
+        def get_image_from_url() -> None | bytes:
+            if not isinstance(image, str) or not image.startswith(('http://', 'https://')):
+                return None
+            response = requests.get(image)
+            if not response.ok:
+                return None
+            return response.content
+
+        if _img := get_image_from_url():
+            image = _img
+        elif isinstance(image, str) and len(image) <= 250:  # first try str as a path to a file
             image = Path(image)
         if isinstance(image, PurePath):  # Path
             with open(image, 'rb') as f:
                 buffer = io.BytesIO(f.read())
         elif hasattr(image, 'read') and hasattr(image, 'seek') and hasattr(image, 'mode'):  # BinaryIO
             if 'rb' not in image.mode:  # what will it do if this is not there
                 raise ValueError(f'Invalid file mode {image.mode=}, expected "rb"(binary mode)')
@@ -155,18 +168,16 @@
             **kwargs,
         )
         query = self._build_query(
             details=details, language=language, asynchronous=asynchronous, extra_get_params=extra_get_params, **kwargs
         )
         url = f'{self.identification_url}{query}'
         response = self._make_api_call(url, 'POST', payload)
-        if not response.ok:
-            raise ValueError(f'Error while creating an identification: {response.status_code=} {response.text=}')
         data = response.json()
-        return data if as_dict else self.identification_class.from_dict(response.json())
+        return data if as_dict else self.identification_class.from_dict(data)
 
     def _build_query(
         self,
         details: str | list[str] = None,
         language: str | list[str] = None,
         asynchronous: bool = False,
         extra_get_params: str | dict[str, str] = None,
@@ -198,48 +209,40 @@
         language: str | list[str] = None,
         extra_get_params: str | dict[str, str] = None,
         as_dict: bool = False,
     ) -> IdentificationType | dict:
         query = self._build_query(details=details, language=language, extra_get_params=extra_get_params)
         url = f'{self.identification_url}/{token}{query}'
         response = self._make_api_call(url, 'GET')
-        if not response.ok:
-            raise ValueError(f'Error while getting an identification: {response.status_code=} {response.text=}')
         data = response.json()
-        return data if as_dict else self.identification_class.from_dict(response.json())
+        return data if as_dict else self.identification_class.from_dict(data)
 
     def delete_identification(self, identification: IdentificationType | str | int) -> bool:
         token = identification.access_token if isinstance(identification, Identification) else identification
         url = f'{self.identification_url}/{token}'
-        response = self._make_api_call(url, 'DELETE')
-        if not response.ok:
-            raise ValueError(f'Error while deleting an identification: {response.status_code=} {response.text=}')
+        self._make_api_call(url, 'DELETE')
         return True
 
     def usage_info(self, as_dict: bool = False) -> UsageInfo | dict:
         response = self._make_api_call(self.usage_info_url, 'GET')
-        if not response.ok:
-            raise ValueError(f'Error while getting an usage info: {response.status_code=} {response.text=}')
         data = response.json()
-        return data if as_dict else UsageInfo.from_dict(response.json())
+        return data if as_dict else UsageInfo.from_dict(data)
 
     def feedback(
         self, identification: IdentificationType | str | int, comment: str | None = None, rating: int | None = None
     ) -> bool:
         token = identification.access_token if isinstance(identification, Identification) else identification
         if comment is None and rating is None:
             raise ValueError('Either comment or rating must be provided')
         data = {}
         if comment is not None:
             data['comment'] = comment
         if rating is not None:
             data['rating'] = rating
-        response = self._make_api_call(self.feedback_url(token), 'POST', data)
-        if not response.ok:
-            raise ValueError(f'Error while sending a feedback: {response.status_code=} {response.text=}')
+        self._make_api_call(self.feedback_url(token), 'POST', data)
         return True
 
     @property
     @abc.abstractmethod
     def views_path(self) -> Path:
         ...
```

### Comparing `kindwise_api_client-0.4.0/kindwise/crop_health.py` & `kindwise_api_client-0.4.1/kindwise/crop_health.py`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/insect.py` & `kindwise_api_client-0.4.1/kindwise/insect.py`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/models.py` & `kindwise_api_client-0.4.1/kindwise/models.py`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/mushroom.py` & `kindwise_api_client-0.4.1/kindwise/mushroom.py`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/plant.py` & `kindwise_api_client-0.4.1/kindwise/plant.py`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/resources/views.crop_health.disease.json` & `kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.disease.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/resources/views.insect.json` & `kindwise_api_client-0.4.1/kindwise/resources/views.insect.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/resources/views.mushroom.json` & `kindwise_api_client-0.4.1/kindwise/resources/views.mushroom.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/resources/views.plant.disease.json` & `kindwise_api_client-0.4.1/kindwise/resources/views.plant.disease.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/resources/views.plant.json` & `kindwise_api_client-0.4.1/kindwise/resources/views.plant.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/conftest.py` & `kindwise_api_client-0.4.1/kindwise/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 
 SYSTEMS = ['insect', 'mushroom', 'plant', 'crop']
 
 TEST_DIR = Path(__file__).resolve().parent
 IMAGE_DIR = TEST_DIR / 'resources' / 'images'
 MOCK_REQUESTS = True
 
+skip_integration_tests = pytest.mark.skipif(
+    bool(os.environ.get('SKIP_INTEGRATION_TESTS', False)), reason='Skipping because due to inability to contact staging'
+)
+
 
 @pytest.fixture
 def api_key():
     return 'b2a2f2c0-5e1a-4e4a-8b9a-5b6b0e2e2b9a'
 
 
 @contextmanager
 def staging_api(api, system):
     assert system.lower() in SYSTEMS
     staging_host = os.getenv(f'{system.upper()}_STAGING_HOST')
-    assert staging_host is not None, f'{system.capitalize()}_STAGING_HOST is not set in .env file'
+    assert staging_host is not None, f'{system.upper()}_STAGING_HOST is not set in .env file'
     api_key = os.getenv(f'{system.upper()}_STAGING_API_KEY')
-    assert api_key is not None, f'{system.capitalize()}_STAGING_API_KEY is not set in .env file'
+    assert api_key is not None, f'{system.upper()}_STAGING_API_KEY is not set in .env file'
     with patch.object(api, 'host', staging_host):
         with patch.object(api, 'api_key', api_key):
             yield api
 
 
 def run_test_requests_to_server(api, system_name, image_path, identification_type, model_name='classification'):
     assert system_name.lower() in SYSTEMS
```

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/resources/images/aloe-vera.jpg` & `kindwise_api_client-0.4.1/kindwise/tests/resources/images/aloe-vera.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/resources/images/amanita_muscaria.jpg` & `kindwise_api_client-0.4.1/kindwise/tests/resources/images/amanita_muscaria.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/resources/images/bee.jpeg` & `kindwise_api_client-0.4.1/kindwise/tests/resources/images/bee.jpeg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/resources/images/padli.png` & `kindwise_api_client-0.4.1/kindwise/tests/resources/images/padli.png`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/resources/images/potato.late_blight.jpg` & `kindwise_api_client-0.4.1/kindwise/tests/resources/images/potato.late_blight.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/test_core.py` & `kindwise_api_client-0.4.1/kindwise/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 import base64
 import io
 from datetime import datetime
-from pathlib import PurePath
+from pathlib import PurePath, Path
 
 import pytest
 from PIL import Image
 
-from kindwise.insect import InsectApi
 from kindwise.models import (
     Identification,
     Result,
     Input,
     Classification,
     Suggestion,
     SimilarImage,
     IdentificationStatus,
 )
 from .conftest import IMAGE_DIR
 from .. import settings
+from ..core import KindwiseApi
+
+
+class TestApi(KindwiseApi):
+    host = 'http://test.id'
+
+    @property
+    def identification_url(self):
+        return f'{self.host}/api/v1/identification'
+
+    @property
+    def usage_info_url(self):
+        return f'{self.host}/api/v1/usage_info'
+
+    @property
+    def views_path(self) -> Path:
+        return settings.APP_DIR / 'resources' / f'views.insect.json'
 
 
 @pytest.fixture
 def api(api_key):
-    api_ = InsectApi(api_key=api_key)
+    api_ = TestApi(api_key=api_key)
     return api_
 
 
 @pytest.fixture
 def identification():
     return Identification(
         access_token='TDp7etcIfwK8LCh',
@@ -135,21 +151,26 @@
 
 @pytest.fixture
 def image_path():
     return IMAGE_DIR / 'bee.jpeg'
 
 
 @pytest.fixture
-def image_base64(image_path):
+def image(image_path):
     with open(image_path, 'rb') as file:
-        return base64.b64encode(file.read()).decode('ascii')
+        return file.read()
+
+
+@pytest.fixture
+def image_base64(image):
+    return base64.b64encode(image).decode('ascii')
 
 
 def test_identify(
-    api, api_key, identification, identification_dict, image_path, image_base64, requests_mock, request_matcher
+    api, api_key, identification, identification_dict, image_path, image, image_base64, requests_mock, request_matcher
 ):
     # check result
     request_matcher.check_identify_request(expected_result=identification, max_image_size=None)
     # check as_dict
     request_matcher.check_identify_request(expected_result=identification_dict, max_image_size=None, as_dict=True)
     # check similar images
     request_matcher.check_identify_request(expected_payload=[('similar_images', False)], similar_images=False)
@@ -216,14 +237,20 @@
     pure_path = PurePath(settings.APP_DIR) / 'tests' / 'resources' / 'images' / 'padli.png'
     pure_path_base64 = api._encode_image(pure_path, 1500)
     request_matcher.check_identify_request(expected_payload=[('images', [pure_path_base64])], image=pure_path)
     # accept image as a PIL image
     # with open(image_path, 'rb') as f:
     img = Image.open(image_path)
     request_matcher.check_identify_request(image=img, max_image_size=None)
+    # accept image as url
+    requests_mock.get('http://example.com/image.jpg', content=image)
+    request_matcher.check_identify_request(
+        image='http://example.com/image.jpg', max_image_size=None, expected_payload=[('images', [image_base64])]
+    )
+
     # check if image is resized
     with open(image_path, 'rb') as f:
         img = Image.open(f)
         max_size = max(img.size)
         new_size = max_size - 100
 
     def run_test_resize(img):
```

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/test_crop.py` & `kindwise_api_client-0.4.1/kindwise/tests/test_crop.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from kindwise.models import Identification
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
 from .. import CropHealthApi
 from ..crop_health import CropIdentification
 
 
-def test_requests_to_insect_server(api_key):
+@skip_integration_tests
+def test_requests_to_crop_server(api_key):
     run_test_requests_to_server(
         CropHealthApi(api_key=api_key),
         'crop',
         IMAGE_DIR / 'potato.late_blight.jpg',
         CropIdentification,
         model_name='disease',
     )
```

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/test_insect.py` & `kindwise_api_client-0.4.1/kindwise/tests/test_insect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from kindwise.models import Identification
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
 from ..insect import InsectApi
 
 
+@skip_integration_tests
 def test_requests_to_insect_server(api_key):
     run_test_requests_to_server(InsectApi(api_key=api_key), 'insect', IMAGE_DIR / 'bee.jpeg', Identification)
 
 
 def test_available_details(api_key):
     expected_view_names = {
         'common_names',
```

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/test_mushroom.py` & `kindwise_api_client-0.4.1/kindwise/tests/test_mushroom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from kindwise.models import Identification
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
 from ..mushroom import MushroomApi
 
 
+@skip_integration_tests
 def test_requests_to_mushroom_server(api_key):
     run_test_requests_to_server(
         MushroomApi(api_key=api_key), 'mushroom', IMAGE_DIR / 'amanita_muscaria.jpg', Identification
     )
 
 
 def test_available_details(api_key):
```

### Comparing `kindwise_api_client-0.4.0/kindwise/tests/test_plant.py` & `kindwise_api_client-0.4.1/kindwise/tests/test_plant.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,21 @@
     HealthAssessmentResult,
     RawPlantIdentification,
     RawPlantResult,
     RawClassification,
     TaxaSpecificSuggestion,
     PlantInput,
 )
-from .conftest import IMAGE_DIR, run_test_requests_to_server, staging_api, run_test_available_details
+from .conftest import (
+    IMAGE_DIR,
+    run_test_requests_to_server,
+    staging_api,
+    run_test_available_details,
+    skip_integration_tests,
+)
 from ..plant import PlantApi
 
 
 @pytest.fixture
 def api(api_key):
     api_ = PlantApi(api_key=api_key)
     return api_
@@ -832,14 +838,15 @@
     identification.custom_id = 123
     requests_mock.delete(f'{api.identification_url}/{identification.custom_id}', json=True)
     response = api.delete_identification(identification.custom_id)
     request_record = requests_mock.request_history.pop()
     assert request_record.url == f'{api.identification_url}/{identification.custom_id}'
 
 
+@skip_integration_tests
 def test_requests_to_plant_server(api: PlantApi, image_path):
     system_name = 'plant'
     run_test_requests_to_server(api, system_name, image_path, PlantIdentification)
     with staging_api(api, system_name) as api:
         custom_id = random.randint(1000000, 2000000)
         date_time = datetime.now()
         print(f'Health assessment asynchronous with {custom_id=} and {date_time=}:')
```

### Comparing `kindwise_api_client-0.4.0/pyproject.toml` & `kindwise_api_client-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kindwise-api-client"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python SDK toolkit for integrating Kindwise API"
 authors = ["Simon Plhak <simon.plhak@flowerchecker.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/flowerchecker/kindwise"
 packages = [
     { include = "kindwise"},
```

### Comparing `kindwise_api_client-0.4.0/setup.py` & `kindwise_api_client-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
  'kindwise.tests': ['resources/images/*']}
 
 install_requires = \
 ['pillow', 'python-dotenv', 'requests']
 
 setup_kwargs = {
     'name': 'kindwise-api-client',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Python SDK toolkit for integrating Kindwise API',
-    'long_description': '# Kindwise sdk for python\n\nPython SDK toolkit for integrating Kindwise API into your application. This Python SDK provides a convenient way to\ninteract with the Kindwise API for plant, insect, and mushroom identification. The SDK is organized into different\nmodules, each corresponding to a specific domain ([plant](https://web.plant.id/plant-identification-api/),\n[insect](https://www.kindwise.com/insect-id), [mushroom](https://www.kindwise.com/mushroom-id)). You can always use our\nAPI without our SDK, the documentation can be found on the following links:\n\n- [plant.id](https://plant.id/docs)\n- [insect.id](https://insect.kindwise.com/docs)\n- [mushroom.id](https://mushroom.kindwise.com/docs)\n- [crop.health](https://crop.kindwise.com/docs)\n\n## Setup\n\n### Install\n\n```bash\npip install kindwise\n```\n\n### API key\n\nThe API key serves to identify your account and is required to make requests to the API. Get API key at\n[admin.kindwise.com](https://admin.kindwise.com).\n\n## Quick Start\n\nTo use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.\n\n```python\nfrom kindwise.plant import PlantApi\nfrom kindwise.models import PlantIdentification, UsageInfo\n\n# initialize plant.id api\n# "PLANT_API_KEY" environment variable can be set instead of specifying api_key\napi = PlantApi(api_key=\'your_api_key\')\n\n# get usage information\nusage: UsageInfo = api.usage_info()\n\n# identify plant by image\nlatitude_longitude = (49.20340, 16.57318)\n# pass the image as a path\nimage_path = \'path/to/plant_image.jpg\'\n# make identification\nidentification: PlantIdentification = api.identify(image_path, latitude_longitude=latitude_longitude)\n\n# get identification by a token with changed views\n# this method can be used to modify additional information in identification or to get identification from database\n# also works with identification.custom_id\nidentification_with_different_views: PlantIdentification = api.get_identification(identification.access_token)\n\n# delete identification\napi.delete_identification(identification)  # also works with identification.access_token or identification.custom_id\n```\n\n## Structure\n\nSDK supports the following Kindwise systems:\n\n- [plant.id](https://web.plant.id/plant-identification-api/)\n- [insect.id](https://insect.kindwise.com)\n- [mushroom.id](https://mushroom.kindwise.com)\n- [crop.health](https://crop.kindwise.com)\n\nEach system has its class, which is used to make requests to the API. Each class has the following methods:\n\n| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        | \n|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------| \n| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | \n| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | \n| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                | \n| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | \n| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                | \n\nDatetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in\nlocal timezone.\n\n### Documentation\n\n#### available_details\n\nReturns details which can be used to specify additional information for `identify` method. `\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_details = api.available_details()\n```\n\n#### identify\n\nCreates a new identification. In one identification, you can include up to 5 images.\n\n```python\nimport base64\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, PlantIdentification, ClassificationLevel\n\napi = PlantApi(api_key=\'your_api_key\')\n# this creates one identification composed of 5 images(not 5 different identifications)\n#\n# as input image is accepted path to an image(str / pathlib.Path), base64 encoded stream(bytes/string), stream(bytes/string),\n# or file object(supports read,seek and mode methods)\n# or PIL.Image.Image object\n# or list of images\nimages = [\'path/to/image1.jpg\', \'path/to/image2.jpg\', \'path/to/image3.jpg\', \'path/to/image4.jpg\', \'path/to/image5.jpg\']\n\n# details included in identification\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n\n# disease details included in health identification(only used if health=True)\n# disease_details parameter is only available for plant.id\ndisease_details = [\'local_name\', \'description\', \'treatment\', \'cause\']\n\n# specify up to 3 languages\nlanguage = [\'en\', \'cs\']\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# include health assessment in your identification by specifying health=\'all\',\n# also use health=\'only\' to get HealthAssessment(health assessment only)\n# health assessment is only available for plant.id\nhealth = \'all\'\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# specify into what depth should be the plant classified\n# choose from ClassificationLevel.SPECIES, ClassificationLevel.GENUS, ClassificationLevel.ALL\n# default is ClassificationLevel.SPECIES\nclassification_level = ClassificationLevel.SPECIES\n# in case of need to merge results for different taxon levels yourself, set classification_raw=True\n# be aware that the result will be in type kindwise.models.RawPlantIdentification\nclassification_raw = False\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: PlantIdentification = api.identify(\n    images,\n    details=details,\n    disease_details=disease_details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    health=health,\n    custom_id=custom_id,\n    date_time=date_time,\n    max_image_size=max_image_size,\n    classification_level=classification_level,\n    classification_raw=classification_raw,\n    extra_get_params=extra_get_params,\n    extra_post_params=extra_post_params,\n)\n\n# identification created from stream\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_stream: PlantIdentification = api.identify(image.read())\n\n# identification created from file object\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_file: PlantIdentification = api.identify(image)\n\n# identification created from base64 encoded image\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    image_in_base64 = base64.b64encode(image.read())\n    identification_from_base64: PlantIdentification = api.identify(image)\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` and\nget `access_token`  or `custom_id` if specified and retrieve the answer later.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\nimage = \'path/to/image.jpg\'\nidentification: PlantIdentification = api.identify(image, asynchronous=True)\n# now do something else\n# ...\n# and later get identification by access_token or custom_id\nidentification: PlantIdentification = api.get_identification(identification.access_token, details=[\'common_names\'])\n```\n\n#### get_identification\n\nGet identification by token. You can specify which details you want to get. We store your identifications for 6 months.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n# details included in identification, can be different from used in identification create\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n# language can also differ from used in identification create\nlanguage = \'de\'\nidentification: PlantIdentification = api.get_identification(access_token, details=details, language=language)\n```\n\n#### delete_identification\n\nDeletes identification from our database. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.delete_identification(custom_id)\n```\n\n#### usage_info\n\nGives you information about your api key usage.\n\n```python\nfrom kindwise import PlantApi, UsageInfo\n\napi = PlantApi(api_key=\'your_api_key\')\n\nusage_info: UsageInfo = api.usage_info()\n```\n\n#### feedback\n\nSend feedback for identification. You can specify a comment(string) or rating(int) in feedback. At least one of comment\nand rating must be specified. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.feedback(custom_id, comment=\'comment\', rating=5)\n```\n\n#### available_disease_details\n\nReturns details which can be used to specify additional information for `health_assessment` method. Only available for\nplant.id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_disease_details = api.available_disease_details()\n```\n\n#### health_assessment\n\nReturns only health assessment for identification. Health assessment is only available for plant.id. `health_assessment`\nmethod is similar to `identify` method, but it returns only health assessment. Details differs for each system.\n\n```python\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key=\'your_api_key\')\n# the same as in identify method\nimages = [\'path/to/image1.jpg\', \'path/to/image2.jpg\', \'path/to/image3.jpg\', \'path/to/image4.jpg\', \'path/to/image5.jpg\']\n\n# details included in identification\ndetails = [\'local_name\', \'description\', \'treatment\', \'cause\', \'image\']\n\n# specify up to 3 languages\nlanguage = [\'en\', \'cs\']\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# list of suggested diseases also contains general diseases such as "Abiotic", default is False\nfull_disease_list = True\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: HealthAssessment = api.health_assessment(\n    images,\n    details=details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    custom_id=custom_id,\n    full_disease_list=full_disease_list,\n    date_time=date_time,\n    max_image_size=max_image_size,\n)\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` similar\nto [`identify`](#identify) method.\n\n#### get_health_assessment\n\nGet a health assessment for identification. You can specify which details you want to get. We store your identifications\nfor 6 months.\n\n```python\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n\n# details included in identification can be different from those used in identification creation\ndetails = [\'classification\', \'local_name\']\n\n# language can also differ from what is used in identification creation\nlanguage = \'de\'\n\nfull_disease_list = False\n\nidentification: HealthAssessment = api.get_health_assessment(\n    access_token,\n    details=details,\n    language=language,\n    full_disease_list=full_disease_list\n)\n```\n\n#### delete_health_assessment\n\nDelete health assessment for identification.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or HealthAssessment object\napi.delete_health_assessment(custom_id)\n```\n',
+    'long_description': '# Kindwise sdk for python\n\nPython SDK toolkit for integrating Kindwise API into your application. This Python SDK provides a convenient way to\ninteract with the Kindwise API for plant, insect, and mushroom identification. The SDK is organized into different\nmodules, each corresponding to a specific domain ([plant](https://web.plant.id/plant-identification-api/),\n[insect](https://www.kindwise.com/insect-id), [mushroom](https://www.kindwise.com/mushroom-id)). You can always use our\nAPI without our SDK, the documentation can be found on the following links:\n\n- [plant.id](https://plant.id/docs)\n- [insect.id](https://insect.kindwise.com/docs)\n- [mushroom.id](https://mushroom.kindwise.com/docs)\n- [crop.health](https://crop.kindwise.com/docs)\n\n## Setup\n\n### Install\n\n```bash\npip install kindwise\n```\n\n### API key\n\nThe API key serves to identify your account and is required to make requests to the API. Get API key at\n[admin.kindwise.com](https://admin.kindwise.com).\n\n## Quick Start\n\nTo use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification, UsageInfo\n\n# initialize plant.id api\n# "PLANT_API_KEY" environment variable can be set instead of specifying api_key\napi = PlantApi(api_key=\'your_api_key\')\n\n# get usage information\nusage: UsageInfo = api.usage_info()\n\n# identify plant by image\nlatitude_longitude = (49.20340, 16.57318)\n# pass the image as a path\nimage_path = \'path/to/plant_image.jpg\'\n# make identification\nidentification: PlantIdentification = api.identify(image_path, latitude_longitude=latitude_longitude)\n\n# get identification by a token with changed views\n# this method can be used to modify additional information in identification or to get identification from database\n# also works with identification.custom_id\nidentification_with_different_views: PlantIdentification = api.get_identification(identification.access_token)\n\n# delete identification\napi.delete_identification(identification)  # also works with identification.access_token or identification.custom_id\n```\n\n## Structure\n\nSDK supports the following Kindwise systems:\n\n- [plant.id](https://web.plant.id/plant-identification-api/)\n- [insect.id](https://insect.kindwise.com)\n- [mushroom.id](https://mushroom.kindwise.com)\n- [crop.health](https://crop.kindwise.com)\n\nEach system has its class, which is used to make requests to the API. Each class has the following methods:\n\n| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        |\n|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------|\n| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |\n\nDatetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in\nlocal timezone.\n\n### Documentation\n\n#### available_details\n\nReturns details which can be used to specify additional information for `identify` method. `\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_details = api.available_details()\n```\n\n#### identify\n\nCreates a new identification. In one identification, you can include up to 5 images.\n\n```python\nimport base64\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, PlantIdentification, ClassificationLevel\n\napi = PlantApi(api_key=\'your_api_key\')\n# this creates one identification composed of 5 images(not 5 different identifications)\n#\n# as input image is accepted path to an image(str / pathlib.Path), base64 encoded stream(bytes/string), stream(bytes/string),\n# or file object(supports read,seek and mode methods)\n# or PIL.Image.Image object\n# or list of images\nimages = [\'path/to/image1.jpg\', \'path/to/image2.jpg\', \'path/to/image3.jpg\', \'path/to/image4.jpg\', \'path/to/image5.jpg\']\n\n# details included in identification\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n\n# disease details included in health identification(only used if health=True)\n# disease_details parameter is only available for plant.id\ndisease_details = [\'local_name\', \'description\', \'treatment\', \'cause\']\n\n# specify up to 3 languages\nlanguage = [\'en\', \'cs\']\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# include health assessment in your identification by specifying health=\'all\',\n# also use health=\'only\' to get HealthAssessment(health assessment only)\n# health assessment is only available for plant.id\nhealth = \'all\'\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# specify into what depth should be the plant classified\n# choose from ClassificationLevel.SPECIES, ClassificationLevel.GENUS, ClassificationLevel.ALL\n# default is ClassificationLevel.SPECIES\nclassification_level = ClassificationLevel.SPECIES\n# in case of need to merge results for different taxon levels yourself, set classification_raw=True\n# be aware that the result will be in type kindwise.models.RawPlantIdentification\nclassification_raw = False\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: PlantIdentification = api.identify(\n    images,\n    details=details,\n    disease_details=disease_details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    health=health,\n    custom_id=custom_id,\n    date_time=date_time,\n    max_image_size=max_image_size,\n    classification_level=classification_level,\n    classification_raw=classification_raw,\n    extra_get_params=extra_get_params,\n    extra_post_params=extra_post_params,\n)\n\n# identification created from stream\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_stream: PlantIdentification = api.identify(image.read())\n\n# identification created from file object\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_file: PlantIdentification = api.identify(image)\n\n# identification created from base64 encoded image\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    image_in_base64 = base64.b64encode(image.read())\n    identification_from_base64: PlantIdentification = api.identify(image)\n\n# identification created from PIL.Image.Image object\nfrom PIL import Image\nimage = Image.open(\'path/to/image.jpg\')\nidentification_from_pil: PlantIdentification = api.identify(image)\n\n# identification created from image url\nimage_url = \'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e\'\nidentification_from_url: PlantIdentification = api.identify(image_url)\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` and\nget `access_token`  or `custom_id` if specified and retrieve the answer later.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\nimage = \'path/to/image.jpg\'\nidentification: PlantIdentification = api.identify(image, asynchronous=True)\n# now do something else\n# ...\n# and later get identification by access_token or custom_id\nidentification: PlantIdentification = api.get_identification(identification.access_token, details=[\'common_names\'])\n```\n\n#### get_identification\n\nGet identification by token. You can specify which details you want to get. We store your identifications for 6 months.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n# details included in identification, can be different from used in identification create\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n# language can also differ from used in identification create\nlanguage = \'de\'\nidentification: PlantIdentification = api.get_identification(access_token, details=details, language=language)\n```\n\n#### delete_identification\n\nDeletes identification from our database. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.delete_identification(custom_id)\n```\n\n#### usage_info\n\nGives you information about your api key usage.\n\n```python\nfrom kindwise import PlantApi, UsageInfo\n\napi = PlantApi(api_key=\'your_api_key\')\n\nusage_info: UsageInfo = api.usage_info()\n```\n\n#### feedback\n\nSend feedback for identification. You can specify a comment(string) or rating(int) in feedback. At least one of comment\nand rating must be specified. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.feedback(custom_id, comment=\'comment\', rating=5)\n```\n\n#### available_disease_details\n\nReturns details which can be used to specify additional information for `health_assessment` method. Only available for\nplant.id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_disease_details = api.available_disease_details()\n```\n\n#### health_assessment\n\nReturns only health assessment for identification. Health assessment is only available for plant.id. `health_assessment`\nmethod is similar to `identify` method, but it returns only health assessment. Details differs for each system.\n\n```python\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key="your_api_key")\n# the same as in identify method\nimages = [\n    "path/to/image1.jpg",\n    "path/to/image2.jpg",\n    "path/to/image3.jpg",\n    "path/to/image4.jpg",\n    "path/to/image5.jpg",\n]\n\n# details included in identification\ndetails = ["local_name", "description", "treatment", "cause", "image"]\n\n# specify up to 3 languages\nlanguage = ["en", "cs"]\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# list of suggested diseases also contains general diseases such as "Abiotic", default is False\nfull_disease_list = True\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: HealthAssessment = api.health_assessment(\n    images,\n    details=details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    custom_id=custom_id,\n    full_disease_list=full_disease_list,\n    date_time=date_time,\n    max_image_size=max_image_size,\n)\n\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` similar\nto [`identify`](#identify) method.\n\n#### get_health_assessment\n\nGet a health assessment for identification. You can specify which details you want to get. We store your identifications\nfor 6 months.\n\n```python\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n\n# details included in identification can be different from those used in identification creation\ndetails = [\'classification\', \'local_name\']\n\n# language can also differ from what is used in identification creation\nlanguage = \'de\'\n\nfull_disease_list = False\n\nidentification: HealthAssessment = api.get_health_assessment(\n    access_token,\n    details=details,\n    language=language,\n    full_disease_list=full_disease_list\n)\n```\n\n#### delete_health_assessment\n\nDelete health assessment for identification.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or HealthAssessment object\napi.delete_health_assessment(custom_id)\n```\n',
     'author': 'Simon Plhak',
     'author_email': 'simon.plhak@flowerchecker.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/flowerchecker/kindwise',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kindwise_api_client-0.4.0/PKG-INFO` & `kindwise_api_client-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kindwise-api-client
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python SDK toolkit for integrating Kindwise API
 Home-page: https://github.com/flowerchecker/kindwise
 License: MIT
 Author: Simon Plhak
 Author-email: simon.plhak@flowerchecker.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,16 +44,15 @@
 [admin.kindwise.com](https://admin.kindwise.com).
 
 ## Quick Start
 
 To use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.
 
 ```python
-from kindwise.plant import PlantApi
-from kindwise.models import PlantIdentification, UsageInfo
+from kindwise import PlantApi, PlantIdentification, UsageInfo
 
 # initialize plant.id api
 # "PLANT_API_KEY" environment variable can be set instead of specifying api_key
 api = PlantApi(api_key='your_api_key')
 
 # get usage information
 usage: UsageInfo = api.usage_info()
@@ -81,26 +80,26 @@
 - [plant.id](https://web.plant.id/plant-identification-api/)
 - [insect.id](https://insect.kindwise.com)
 - [mushroom.id](https://mushroom.kindwise.com)
 - [crop.health](https://crop.kindwise.com)
 
 Each system has its class, which is used to make requests to the API. Each class has the following methods:
 
-| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        | 
-|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------| 
-| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                | 
-| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | 
-| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                | 
+| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        |
+|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
+| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |
 
 Datetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in
 local timezone.
 
 ### Documentation
 
 #### available_details
@@ -202,14 +201,23 @@
 with open('path/to/image.jpg', 'rb') as image :
     identification_from_file: PlantIdentification = api.identify(image)
 
 # identification created from base64 encoded image
 with open('path/to/image.jpg', 'rb') as image :
     image_in_base64 = base64.b64encode(image.read())
     identification_from_base64: PlantIdentification = api.identify(image)
+
+# identification created from PIL.Image.Image object
+from PIL import Image
+image = Image.open('path/to/image.jpg')
+identification_from_pil: PlantIdentification = api.identify(image)
+
+# identification created from image url
+image_url = 'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e'
+identification_from_url: PlantIdentification = api.identify(image_url)
 ```
 
 When you don't want to wait until the identification is finished, you can specify `asynchronous=True` and
 get `access_token`  or `custom_id` if specified and retrieve the answer later.
 
 ```python
 from kindwise import PlantApi, PlantIdentification
@@ -299,23 +307,29 @@
 method is similar to `identify` method, but it returns only health assessment. Details differs for each system.
 
 ```python
 from datetime import datetime
 
 from kindwise import PlantApi, HealthAssessment
 
-api = PlantApi(api_key='your_api_key')
+api = PlantApi(api_key="your_api_key")
 # the same as in identify method
-images = ['path/to/image1.jpg', 'path/to/image2.jpg', 'path/to/image3.jpg', 'path/to/image4.jpg', 'path/to/image5.jpg']
+images = [
+    "path/to/image1.jpg",
+    "path/to/image2.jpg",
+    "path/to/image3.jpg",
+    "path/to/image4.jpg",
+    "path/to/image5.jpg",
+]
 
 # details included in identification
-details = ['local_name', 'description', 'treatment', 'cause', 'image']
+details = ["local_name", "description", "treatment", "cause", "image"]
 
 # specify up to 3 languages
-language = ['en', 'cs']
+language = ["en", "cs"]
 
 # default for similar_images is True
 similar_images = True
 
 # where was an image taken
 latitude_longitude = (49.20340, 16.57318)
 
@@ -344,14 +358,15 @@
     similar_images=similar_images,
     latitude_longitude=latitude_longitude,
     custom_id=custom_id,
     full_disease_list=full_disease_list,
     date_time=date_time,
     max_image_size=max_image_size,
 )
+
 ```
 
 When you don't want to wait until the identification is finished, you can specify `asynchronous=True` similar
 to [`identify`](#identify) method.
 
 #### get_health_assessment
```

