# Comparing `tmp/recognizer-1.3.tar.gz` & `tmp/recognizer-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognizer-1.3.tar", last modified: Tue Feb 13 14:25:50 2024, max compression
+gzip compressed data, was "recognizer-1.4.tar", last modified: Wed Apr 10 18:51:04 2024, max compression
```

## Comparing `recognizer-1.3.tar` & `recognizer-1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.906748 recognizer-1.3/
--rw-rw-rw-   0        0        0    35702 2024-01-12 14:27:30.000000 recognizer-1.3/LICENSE
--rw-rw-rw-   0        0        0     5192 2024-02-13 14:25:50.906199 recognizer-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3606 2024-02-12 19:20:35.000000 recognizer-1.3/README.md
--rw-rw-rw-   0        0        0      671 2024-02-04 17:14:14.000000 recognizer-1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.864008 recognizer-1.3/recognizer/
--rw-rw-rw-   0        0        0      135 2024-02-12 19:20:35.000000 recognizer-1.3/recognizer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.875877 recognizer-1.3/recognizer/agents/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:48:41.000000 recognizer-1.3/recognizer/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.881484 recognizer-1.3/recognizer/agents/playwright/
--rw-rw-rw-   0        0        0      137 2024-02-04 16:47:09.000000 recognizer-1.3/recognizer/agents/playwright/__init__.py
--rw-rw-rw-   0        0        0     8172 2024-02-12 19:07:43.000000 recognizer-1.3/recognizer/agents/playwright/async_control.py
--rw-rw-rw-   0        0        0     7863 2024-02-12 19:10:56.000000 recognizer-1.3/recognizer/agents/playwright/sync_control.py
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.890881 recognizer-1.3/recognizer/components/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:53:31.000000 recognizer-1.3/recognizer/components/__init__.py
--rw-rw-rw-   0        0        0     3766 2024-02-04 17:57:59.000000 recognizer-1.3/recognizer/components/detection_processor.py
--rw-rw-rw-   0        0        0    16437 2024-02-12 19:55:24.000000 recognizer-1.3/recognizer/components/detector.py
--rw-rw-rw-   0        0        0     5956 2024-02-05 16:00:57.000000 recognizer-1.3/recognizer/components/image_processor.py
--rw-rw-rw-   0        0        0      824 2024-01-09 16:22:35.000000 recognizer-1.3/recognizer/components/prompt_handler.py
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.904090 recognizer-1.3/recognizer.egg-info/
--rw-rw-rw-   0        0        0     5192 2024-02-13 14:25:50.000000 recognizer-1.3/recognizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-02-13 14:25:50.000000 recognizer-1.3/recognizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 14:25:50.000000 recognizer-1.3/recognizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-12 15:03:39.000000 recognizer-1.3/recognizer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       98 2024-02-13 14:25:50.000000 recognizer-1.3/recognizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-13 14:25:50.000000 recognizer-1.3/recognizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1500 2024-02-13 14:25:50.908395 recognizer-1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-13 14:25:50.901347 recognizer-1.3/tests/
--rw-rw-rw-   0        0        0     2375 2024-02-04 16:48:35.000000 recognizer-1.3/tests/test_detector.py
--rw-rw-rw-   0        0        0     3875 2024-02-04 16:48:35.000000 recognizer-1.3/tests/test_inputs.py
--rw-rw-rw-   0        0        0      609 2024-02-06 20:12:10.000000 recognizer-1.3/tests/test_playwright_async.py
--rw-rw-rw-   0        0        0      547 2024-02-09 18:34:17.000000 recognizer-1.3/tests/test_playwright_sync.py
--rw-rw-rw-   0        0        0    15976 2024-02-06 20:11:52.000000 recognizer-1.3/tests/test_recaptcha_sites.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.530548 recognizer-1.4/
+-rw-rw-rw-   0        0        0    35702 2024-01-12 14:27:30.000000 recognizer-1.4/LICENSE
+-rw-rw-rw-   0        0        0     5437 2024-04-10 18:51:04.529042 recognizer-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2024-03-17 19:15:07.000000 recognizer-1.4/README.md
+-rw-rw-rw-   0        0        0      671 2024-02-04 17:14:14.000000 recognizer-1.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.473090 recognizer-1.4/recognizer/
+-rw-rw-rw-   0        0        0      135 2024-03-17 19:14:15.000000 recognizer-1.4/recognizer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.483686 recognizer-1.4/recognizer/agents/
+-rw-rw-rw-   0        0        0        0 2024-02-02 17:48:41.000000 recognizer-1.4/recognizer/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.494874 recognizer-1.4/recognizer/agents/playwright/
+-rw-rw-rw-   0        0        0      137 2024-02-04 16:47:09.000000 recognizer-1.4/recognizer/agents/playwright/__init__.py
+-rw-rw-rw-   0        0        0     8178 2024-03-17 19:54:40.000000 recognizer-1.4/recognizer/agents/playwright/async_control.py
+-rw-rw-rw-   0        0        0     7869 2024-02-19 18:14:47.000000 recognizer-1.4/recognizer/agents/playwright/sync_control.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.504621 recognizer-1.4/recognizer/components/
+-rw-rw-rw-   0        0        0        0 2024-02-14 16:24:12.000000 recognizer-1.4/recognizer/components/__init__.py
+-rw-rw-rw-   0        0        0     3766 2024-02-04 17:57:59.000000 recognizer-1.4/recognizer/components/detection_processor.py
+-rw-rw-rw-   0        0        0    16418 2024-04-09 15:53:06.000000 recognizer-1.4/recognizer/components/detector.py
+-rw-rw-rw-   0        0        0     5956 2024-02-05 16:00:57.000000 recognizer-1.4/recognizer/components/image_processor.py
+-rw-rw-rw-   0        0        0      824 2024-01-09 16:22:35.000000 recognizer-1.4/recognizer/components/prompt_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.526525 recognizer-1.4/recognizer.egg-info/
+-rw-rw-rw-   0        0        0     5437 2024-04-10 18:51:04.000000 recognizer-1.4/recognizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-04-10 18:51:04.000000 recognizer-1.4/recognizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 18:51:04.000000 recognizer-1.4/recognizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 18:51:03.000000 recognizer-1.4/recognizer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      106 2024-04-10 18:51:04.000000 recognizer-1.4/recognizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 18:51:04.000000 recognizer-1.4/recognizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1510 2024-04-10 18:51:04.531556 recognizer-1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 18:51:04.524964 recognizer-1.4/tests/
+-rw-rw-rw-   0        0        0     2375 2024-02-04 16:48:35.000000 recognizer-1.4/tests/test_detector.py
+-rw-rw-rw-   0        0        0     3875 2024-02-04 16:48:35.000000 recognizer-1.4/tests/test_inputs.py
+-rw-rw-rw-   0        0        0      609 2024-02-06 20:12:10.000000 recognizer-1.4/tests/test_playwright_async.py
+-rw-rw-rw-   0        0        0      547 2024-02-09 18:34:17.000000 recognizer-1.4/tests/test_playwright_sync.py
+-rw-rw-rw-   0        0        0    15976 2024-03-17 19:55:04.000000 recognizer-1.4/tests/test_recaptcha_sites.py
```

### Comparing `recognizer-1.3/LICENSE` & `recognizer-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/PKG-INFO` & `recognizer-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recognizer
-Version: 1.3
+Version: 1.4
 Summary: 🦉Gracefully face reCAPTCHA challenge with ultralytics YOLOv8-seg, CLIPs VIT-B/16 and CLIP-Seg/RD64. Implemented in playwright or an easy-to-use API.
 Home-page: https://github.com/Vinyzu/recognizer
 Author: Vinyzu
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/Vinyzu/reCognizer
 Project-URL: Tracker, https://github.com/Vinyzu/reCognizer/issues
 Keywords: botright,playwright,browser,automation,fingerprints,fingerprinting,dataset,data,recaptcha,captcha
@@ -25,18 +25,21 @@
 Requires-Dist: transformers
 Requires-Dist: numpy
 Requires-Dist: playwright
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: mypy; extra == "testing"
 Requires-Dist: flake8; extra == "testing"
-Requires-Dist: tox; extra == "testing"
+Requires-Dist: black; extra == "testing"
+Requires-Dist: isort; extra == "testing"
 
-# reCognizer v1.3
+# reCognizer v1.4
 ![Tests & Linting](https://github.com/Vinyzu/recognizer/actions/workflows/ci.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/recognizer.svg?color=1182C3)](https://pypi.org/project/recognizer/)
+[![Downloads](https://static.pepy.tech/badge/recognizer)](https://pepy.tech/project/recognizer)
 
 
 #### reCognizer is a free-to-use AI based [reCaptcha](https://developers.google.com/recaptcha) Solver. <br> Usable with an easy-to-use API, also available for Async and Sync Playwright. <br> You can pass almost any format into the Challenger, from full-page screenshots, only-captcha images and no-border images to single images in a list.
 
 #### Note: You Should use an undetected browser engine like [Botright](https://github.com/Vinyzu/Botright) to solve the Captchas consistently. <br>  reCaptcha detects normal Playwright easily and you probably wont get any successful solves despite correct recognitions.
 
 ## Install it from PyPI
@@ -147,13 +150,13 @@
 
 ## Thanks to
 
 [QIN2DIM](https://github.com/QIN2DIM) (For basic project structure)
 
 ---
 
-![Version](https://img.shields.io/badge/reCognizer-v1.3-blue)
+![Version](https://img.shields.io/badge/reCognizer-v1.4-blue)
 ![License](https://img.shields.io/badge/License-GNU%20GPL-green)
 ![Python](https://img.shields.io/badge/Python-v3.x-lightgrey)
 
 [![my-discord](https://img.shields.io/badge/My_Discord-000?style=for-the-badge&logo=google-chat&logoColor=blue)](https://discordapp.com/users/935224495126487150)
 [![buy-me-a-coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-000?style=for-the-badge&logo=ko-fi&logoColor=brown)](https://ko-fi.com/vinyzu)
```

### Comparing `recognizer-1.3/README.md` & `recognizer-1.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# reCognizer v1.3
+# reCognizer v1.4
 ![Tests & Linting](https://github.com/Vinyzu/recognizer/actions/workflows/ci.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/recognizer.svg?color=1182C3)](https://pypi.org/project/recognizer/)
+[![Downloads](https://static.pepy.tech/badge/recognizer)](https://pepy.tech/project/recognizer)
 
 
 #### reCognizer is a free-to-use AI based [reCaptcha](https://developers.google.com/recaptcha) Solver. <br> Usable with an easy-to-use API, also available for Async and Sync Playwright. <br> You can pass almost any format into the Challenger, from full-page screenshots, only-captcha images and no-border images to single images in a list.
 
 #### Note: You Should use an undetected browser engine like [Botright](https://github.com/Vinyzu/Botright) to solve the Captchas consistently. <br>  reCaptcha detects normal Playwright easily and you probably wont get any successful solves despite correct recognitions.
 
 ## Install it from PyPI
@@ -114,13 +116,13 @@
 
 ## Thanks to
 
 [QIN2DIM](https://github.com/QIN2DIM) (For basic project structure)
 
 ---
 
-![Version](https://img.shields.io/badge/reCognizer-v1.3-blue)
+![Version](https://img.shields.io/badge/reCognizer-v1.4-blue)
 ![License](https://img.shields.io/badge/License-GNU%20GPL-green)
 ![Python](https://img.shields.io/badge/Python-v3.x-lightgrey)
 
 [![my-discord](https://img.shields.io/badge/My_Discord-000?style=for-the-badge&logo=google-chat&logoColor=blue)](https://discordapp.com/users/935224495126487150)
 [![buy-me-a-coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-000?style=for-the-badge&logo=ko-fi&logoColor=brown)](https://ko-fi.com/vinyzu)
```

### Comparing `recognizer-1.3/pyproject.toml` & `recognizer-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/recognizer/agents/playwright/async_control.py` & `recognizer-1.4/recognizer/agents/playwright/async_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             return False
 
         return await label_obj.is_visible()
 
     async def click_checkbox(self) -> bool:
         # Clicking Captcha Checkbox
         try:
-            checkbox = self.page.frame_locator("iframe[title='reCAPTCHA']")
+            checkbox = self.page.frame_locator("iframe[title='reCAPTCHA']").first
             await checkbox.locator(".recaptcha-checkbox-border").click()
             return True
         except TimeoutError:
             return False
 
     async def detect_tiles(self, prompt: str, area_captcha: bool) -> bool:
         image = await self.page.screenshot(full_page=True)
```

### Comparing `recognizer-1.3/recognizer/agents/playwright/sync_control.py` & `recognizer-1.4/recognizer/agents/playwright/sync_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             return False
 
         return label_obj.is_visible()
 
     def click_checkbox(self) -> bool:
         # Clicking Captcha Checkbox
         try:
-            checkbox = self.page.frame_locator("iframe[title='reCAPTCHA']")
+            checkbox = self.page.frame_locator("iframe[title='reCAPTCHA']").first
             checkbox.locator(".recaptcha-checkbox-border").click()
             return True
         except TimeoutError:
             return False
 
     def detect_tiles(self, prompt: str, area_captcha: bool) -> bool:
         image = self.page.screenshot(full_page=True)
```

### Comparing `recognizer-1.3/recognizer/components/detection_processor.py` & `recognizer-1.4/recognizer/components/detection_processor.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/recognizer/components/detector.py` & `recognizer-1.4/recognizer/components/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,19 +193,19 @@
 
         return response
 
     def clipseg_detect_rd64(self, image: NDArray[generic], task_type: str, tiles_amount: int) -> List[bool]:
         response = [False for _ in range(tiles_amount)]
         segment_label = self.area_captcha_labels[task_type]
 
-        inputs = detection_models.seg_processor(text=segment_label, images=[image], padding="max_length", return_tensors="pt")
+        inputs = detection_models.seg_processor(text=segment_label, images=[image], return_tensors="pt")
         with no_grad():
             outputs = detection_models.seg_model(**inputs)
 
-        heatmap = outputs.logits
+        heatmap = outputs.logits[0]
         # Get the normalized adjusted threshold for the heatmap
         adjusted_normalized_heatmap = (heatmap - heatmap.min()) / (heatmap.max() - heatmap.min()) * 2.5
         threshold = heatmap.max() - adjusted_normalized_heatmap.mean()
         # Create the Threshold mask for the Heatmap
         threshold_mask = (heatmap > threshold).float()
 
         # Getting Tile Size from threshold mask
```

### Comparing `recognizer-1.3/recognizer/components/image_processor.py` & `recognizer-1.4/recognizer/components/image_processor.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/recognizer/components/prompt_handler.py` & `recognizer-1.4/recognizer/components/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/recognizer.egg-info/PKG-INFO` & `recognizer-1.4/recognizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recognizer
-Version: 1.3
+Version: 1.4
 Summary: 🦉Gracefully face reCAPTCHA challenge with ultralytics YOLOv8-seg, CLIPs VIT-B/16 and CLIP-Seg/RD64. Implemented in playwright or an easy-to-use API.
 Home-page: https://github.com/Vinyzu/recognizer
 Author: Vinyzu
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/Vinyzu/reCognizer
 Project-URL: Tracker, https://github.com/Vinyzu/reCognizer/issues
 Keywords: botright,playwright,browser,automation,fingerprints,fingerprinting,dataset,data,recaptcha,captcha
@@ -25,18 +25,21 @@
 Requires-Dist: transformers
 Requires-Dist: numpy
 Requires-Dist: playwright
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: mypy; extra == "testing"
 Requires-Dist: flake8; extra == "testing"
-Requires-Dist: tox; extra == "testing"
+Requires-Dist: black; extra == "testing"
+Requires-Dist: isort; extra == "testing"
 
-# reCognizer v1.3
+# reCognizer v1.4
 ![Tests & Linting](https://github.com/Vinyzu/recognizer/actions/workflows/ci.yml/badge.svg)
+[![](https://img.shields.io/pypi/v/recognizer.svg?color=1182C3)](https://pypi.org/project/recognizer/)
+[![Downloads](https://static.pepy.tech/badge/recognizer)](https://pepy.tech/project/recognizer)
 
 
 #### reCognizer is a free-to-use AI based [reCaptcha](https://developers.google.com/recaptcha) Solver. <br> Usable with an easy-to-use API, also available for Async and Sync Playwright. <br> You can pass almost any format into the Challenger, from full-page screenshots, only-captcha images and no-border images to single images in a list.
 
 #### Note: You Should use an undetected browser engine like [Botright](https://github.com/Vinyzu/Botright) to solve the Captchas consistently. <br>  reCaptcha detects normal Playwright easily and you probably wont get any successful solves despite correct recognitions.
 
 ## Install it from PyPI
@@ -147,13 +150,13 @@
 
 ## Thanks to
 
 [QIN2DIM](https://github.com/QIN2DIM) (For basic project structure)
 
 ---
 
-![Version](https://img.shields.io/badge/reCognizer-v1.3-blue)
+![Version](https://img.shields.io/badge/reCognizer-v1.4-blue)
 ![License](https://img.shields.io/badge/License-GNU%20GPL-green)
 ![Python](https://img.shields.io/badge/Python-v3.x-lightgrey)
 
 [![my-discord](https://img.shields.io/badge/My_Discord-000?style=for-the-badge&logo=google-chat&logoColor=blue)](https://discordapp.com/users/935224495126487150)
 [![buy-me-a-coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-000?style=for-the-badge&logo=ko-fi&logoColor=brown)](https://ko-fi.com/vinyzu)
```

### Comparing `recognizer-1.3/recognizer.egg-info/SOURCES.txt` & `recognizer-1.4/recognizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/setup.cfg` & `recognizer-1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -84,11 +84,12 @@
 00000530: 676e 697a 6572 2c20 7265 636f 676e 697a  gnizer, recogniz
 00000540: 6572 2e2a 2c20 4c49 4345 4e53 450d 0a65  er.*, LICENSE..e
 00000550: 7863 6c75 6465 203d 2074 6573 7473 2c20  xclude = tests, 
 00000560: 2e67 6974 6875 620d 0a0d 0a5b 6f70 7469  .github....[opti
 00000570: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
 00000580: 7265 5d0d 0a74 6573 7469 6e67 203d 200d  re]..testing = .
 00000590: 0a09 7079 7465 7374 0d0a 096d 7970 790d  ..pytest...mypy.
-000005a0: 0a09 666c 616b 6538 0d0a 0974 6f78 0d0a  ..flake8...tox..
-000005b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000005c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000005d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000005a0: 0a09 666c 616b 6538 0d0a 0962 6c61 636b  ..flake8...black
+000005b0: 0d0a 0969 736f 7274 0d0a 0d0a 5b65 6767  ...isort....[egg
+000005c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000005d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000005e0: 2030 0d0a 0d0a                            0....
```

### Comparing `recognizer-1.3/tests/test_detector.py` & `recognizer-1.4/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/tests/test_inputs.py` & `recognizer-1.4/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/tests/test_playwright_async.py` & `recognizer-1.4/tests/test_playwright_async.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/tests/test_playwright_sync.py` & `recognizer-1.4/tests/test_playwright_sync.py`

 * *Files identical despite different names*

### Comparing `recognizer-1.3/tests/test_recaptcha_sites.py` & `recognizer-1.4/tests/test_recaptcha_sites.py`

 * *Files identical despite different names*

