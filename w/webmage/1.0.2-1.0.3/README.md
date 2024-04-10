# Comparing `tmp/webmage-1.0.2.tar.gz` & `tmp/webmage-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webmage-1.0.2.tar", last modified: Tue Feb 28 16:50:08 2023, max compression
+gzip compressed data, was "webmage-1.0.3.tar", last modified: Wed Apr 10 20:08:47 2024, max compression
```

## Comparing `webmage-1.0.2.tar` & `webmage-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 vincjess (430751568) 1539093546        0 2023-02-28 16:50:08.919647 webmage-1.0.2/
--rwx------   0 vincjess (430751568) 1539093546     1081 2022-02-15 17:48:07.000000 webmage-1.0.2/LICENSE
--rw-r--r--   0 vincjess (430751568) 1539093546     9771 2023-02-28 16:50:08.919921 webmage-1.0.2/PKG-INFO
--rwx------   0 vincjess (430751568) 1539093546     9264 2022-06-14 20:36:59.000000 webmage-1.0.2/README
--rwx------   0 vincjess (430751568) 1539093546       96 2022-01-28 16:41:30.000000 webmage-1.0.2/pyproject.toml
--rwx------   0 vincjess (430751568) 1539093546      720 2023-02-28 16:50:08.921432 webmage-1.0.2/setup.cfg
-drwxr-xr-x   0 vincjess (430751568) 1539093546        0 2023-02-28 16:50:08.915275 webmage-1.0.2/webmage/
--rwx------   0 vincjess (430751568) 1539093546      616 2022-08-18 18:15:12.000000 webmage-1.0.2/webmage/__init__.py
--rwx------   0 vincjess (430751568) 1539093546    12565 2023-02-28 16:44:02.000000 webmage-1.0.2/webmage/dynamic.py
--rwx------   0 vincjess (430751568) 1539093546     2306 2022-08-18 18:56:47.000000 webmage-1.0.2/webmage/dynamic_rune.py
--rwx------   0 vincjess (430751568) 1539093546      774 2022-08-18 18:45:37.000000 webmage-1.0.2/webmage/dynamic_rune_array.py
--rwx------   0 vincjess (430751568) 1539093546     1546 2022-01-21 21:48:33.000000 webmage-1.0.2/webmage/static.py
--rwx------   0 vincjess (430751568) 1539093546      348 2022-01-21 21:48:33.000000 webmage-1.0.2/webmage/support.py
-drwxr-xr-x   0 vincjess (430751568) 1539093546        0 2023-02-28 16:50:08.919214 webmage-1.0.2/webmage.egg-info/
--rwx------   0 vincjess (430751568) 1539093546     9771 2023-02-28 16:50:04.000000 webmage-1.0.2/webmage.egg-info/PKG-INFO
--rwx------   0 vincjess (430751568) 1539093546      323 2023-02-28 16:50:04.000000 webmage-1.0.2/webmage.egg-info/SOURCES.txt
--rw-r--r--   0 vincjess (430751568) 1539093546        1 2023-02-28 16:50:04.000000 webmage-1.0.2/webmage.egg-info/dependency_links.txt
--rw-r--r--   0 vincjess (430751568) 1539093546       95 2023-02-28 16:50:04.000000 webmage-1.0.2/webmage.egg-info/requires.txt
--rw-r--r--   0 vincjess (430751568) 1539093546        8 2023-02-28 16:50:04.000000 webmage-1.0.2/webmage.egg-info/top_level.txt
+drwxr-xr-x   0 jvincent   (503) staff       (20)        0 2024-04-10 20:08:47.318154 webmage-1.0.3/
+-rwx------   0 jvincent   (503) staff       (20)     1081 2022-02-15 17:48:07.000000 webmage-1.0.3/LICENSE
+-rw-r--r--   0 jvincent   (503) staff       (20)     9926 2024-04-10 20:08:47.317622 webmage-1.0.3/PKG-INFO
+-rwx------   0 jvincent   (503) staff       (20)     9264 2022-06-14 20:36:59.000000 webmage-1.0.3/README
+-rwx------   0 jvincent   (503) staff       (20)       96 2022-01-28 16:41:30.000000 webmage-1.0.3/pyproject.toml
+-rwx------   0 jvincent   (503) staff       (20)      720 2024-04-10 20:08:47.319243 webmage-1.0.3/setup.cfg
+drwxr-xr-x   0 jvincent   (503) staff       (20)        0 2024-04-10 20:08:47.310101 webmage-1.0.3/webmage/
+-rwx------   0 jvincent   (503) staff       (20)      264 2024-04-10 19:55:02.000000 webmage-1.0.3/webmage/__init__.py
+-rw-r--r--   0 jvincent   (503) staff       (20)     2290 2024-04-10 19:57:57.000000 webmage-1.0.3/webmage/rune.py
+-rw-r--r--   0 jvincent   (503) staff       (20)      703 2024-04-10 19:57:57.000000 webmage-1.0.3/webmage/rune_list.py
+-rw-r--r--   0 jvincent   (503) staff       (20)    11627 2024-04-10 19:57:57.000000 webmage-1.0.3/webmage/spell.py
+-rw-r--r--   0 jvincent   (503) staff       (20)      348 2024-04-10 19:57:31.000000 webmage-1.0.3/webmage/support.py
+drwxr-xr-x   0 jvincent   (503) staff       (20)        0 2024-04-10 20:08:47.315915 webmage-1.0.3/webmage.egg-info/
+-rw-r--r--   0 jvincent   (503) staff       (20)     9926 2024-04-10 20:08:47.000000 webmage-1.0.3/webmage.egg-info/PKG-INFO
+-rwx------   0 jvincent   (503) staff       (20)      286 2024-04-10 20:08:47.000000 webmage-1.0.3/webmage.egg-info/SOURCES.txt
+-rwx------   0 jvincent   (503) staff       (20)        1 2024-04-10 20:08:47.000000 webmage-1.0.3/webmage.egg-info/dependency_links.txt
+-rwx------   0 jvincent   (503) staff       (20)       95 2024-04-10 20:08:47.000000 webmage-1.0.3/webmage.egg-info/requires.txt
+-rwx------   0 jvincent   (503) staff       (20)        8 2024-04-10 20:08:47.000000 webmage-1.0.3/webmage.egg-info/top_level.txt
```

### Comparing `webmage-1.0.2/LICENSE` & `webmage-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webmage-1.0.2/PKG-INFO` & `webmage-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: webmage
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library with built-in methods that make web scraping easier for dynamically loading pages.
 Home-page: https://github.com/javascriptorian/webmage
 Author: The JavaScriptorian
 Author-email: javascriptorian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: webdriver_manager>=3.8.5
+Requires-Dist: selenium>=4.8.2
+Requires-Dist: beautifulsoup4>=4.11.2
+Requires-Dist: undetected_chromedriver>=3.4.6
 
 # Description
 A wrapper around requests, BeautifulSoup, and Selenium (Chrome) to facilitate web scraping.
 
 # Installation
 ```pip install webmage```
```

### Comparing `webmage-1.0.2/README` & `webmage-1.0.3/README`

 * *Files identical despite different names*

### Comparing `webmage-1.0.2/setup.cfg` & `webmage-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = webmage
-version = 1.0.2
+version = 1.0.3
 author = The JavaScriptorian
 author_email = javascriptorian@gmail.com
 description = A library with built-in methods that make web scraping easier for dynamically loading pages.
 long_description = file: README
 long_description_content_type = text/markdown
 url = https://github.com/javascriptorian/webmage
 classifiers =
```

### Comparing `webmage-1.0.2/webmage/dynamic.py` & `webmage-1.0.3/webmage/spell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,74 @@
 import re
 from selenium import webdriver
+from selenium.webdriver.chrome.service import Service as ChromeService
+from selenium.webdriver.firefox.service import Service as FirefoxService
 from selenium.webdriver.common.by import By
 from time import sleep
-from webdriver_manager.chrome import ChromeDriverManager
-from webdriver_manager.firefox import GeckoDriverManager
-from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.common.exceptions import JavascriptException
-
 import json
-
 # Runes
-from .dynamic_rune_array import DynamicRuneArr
-from .dynamic_rune import DynamicRune
+from .rune_list import RuneList
+from .rune import Rune
 
-class DynamicSpell:
+class Spell:
     def __init__(self, url, driver_path=None, ghost=False, browser='chrome'):
         self.url = url
         self.driver_path = driver_path
         self.ghost = ghost
         self.browser = browser
 
         self.initialize_driver()
 
+
     def initialize_driver(self):
         # Get chrome driver if no path is given.
         if self.driver_path == None:
-            # Set options for Chrome
             if 'chrome' in self.browser:
                 options = webdriver.ChromeOptions()
                 if self.ghost:
                     options.add_argument('--headless')
-
-                if 'undetected' in self.browser:
-                    try:
-                        import undetected_chromedriver as uc
-                        self.driver_path = None
-                        self.driver = uc.Chrome(options=options)
-                    except Exception as e:
-                        ibrk = 0
-                        raise Exception('Certificate Verify Failed. Unable to get local issuer certificate. If you are on a Mac, then please try going to Macintosh HD > Applications > Python3.9 folder (or whatever version of python you\'re using) > double click on "Install Certificates.command" file.')
-                else:
-                    self.driver_path = ChromeDriverManager().install()
-                    # Remove all of the nonsense errors that are printed out.
-                    options.add_argument('--ignore-certificate-errors')
-                    options.add_argument('--ignore-ssl-errors')
-                    # Add network logging so that the network_log method works.
-                    options.add_experimental_option("excludeSwitches", ["enable-logging"])
-                    capabilities = DesiredCapabilities.CHROME
-                    capabilities["goog:loggingPrefs"] = {"performance": "ALL"}
-                    # Open the chrome browser.
-                    self.driver = webdriver.Chrome(self.driver_path, chrome_options=options, desired_capabilities=capabilities)
-            # Set options for Firefox
+                # Remove all of the nonsense errors that are printed out.
+                options.add_argument('--ignore-certificate-errors')
+                options.add_argument('--ignore-ssl-errors')
+                service = ChromeService()
+                self.driver = webdriver.Chrome(service=service, options=options)
             elif self.browser == 'firefox':
-                self.driver_path = GeckoDriverManager().install()
                 options = webdriver.FirefoxOptions()
                 if self.ghost:
-                    options.add_argument("--headless")
-                self.driver = webdriver.Firefox(executable_path=self.driver_path)
-
-        # Go to the initialized webpage.
+                    options.add_argument('--headless')
+                # Remove all of the nonsense errors that are printed out.
+                options.add_argument('--ignore-certificate-errors')
+                options.add_argument('--ignore-ssl-errors')
+                service = FirefoxService()
+                self.driver = webdriver.Firefox(service=service, options=options)
+            else:
+                raise Exception(f'{self.browser} is not a valid browser.')
         self.driver.get(self.url)
 
 
     def close(self):
         self.driver.close()
 
 
     # For selecting first item based on CSS selector.
     def select(self, css_selector):
-        return DynamicRune(self.driver.find_element(By.CSS_SELECTOR, css_selector), self.driver)
+        elements = self.driver.find_elements(By.CSS_SELECTOR, css_selector)
+        if len(elements) > 0:
+            return Rune(elements[0], self.driver)
+        else:
+            return None
 
 
     # For selecting first item based on CSS selector.
     def selectAll(self, css_selector):
-        return DynamicRuneArr([DynamicRune(i, self.driver)for i in self.driver.find_elements(By.CSS_SELECTOR, css_selector)])
+        return RuneList([Rune(i, self.driver)for i in self.driver.find_elements(By.CSS_SELECTOR, css_selector)])
 
     # Changes the URL of the original soup.
-    def change_url(self, url, retry=True):
+    def changeUrl(self, url, retry=True):
         if retry == False:
             self.driver.get(url)
             self.url = self.driver.current_url
         else:
             success = False
             while success == False:
                 try:
@@ -129,45 +117,45 @@
             if new_height == last_height:
                 break
             last_height = new_height
         # Go to next line after scroll completion.
         print('')
 
 
-    def delicate_scroll(self, wait_interval, scroll_count, scroll_pixel_length=500, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
+    def scrollByPixels(self, wait_interval, scroll_count, scroll_pixel_length=500, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
         counter = 1
 
         # Make the CSS Selector into a querySelector
         if scroll_css_selector != 'document.scrollingElement':
             scroll_css_selector = f'document.querySelector("{scroll_css_selector}")'
 
         # last_height = self.driver.execute_script(f"return {scroll_css_selector}.scrollHeight")
-        max_height = int(self.cast_js(f'return {scroll_css_selector}.scrollHeight'))
+        max_height = int(self.castJS(f'return {scroll_css_selector}.scrollHeight'))
         i = 0
 
         while counter <= scroll_count:
-            self.cast_js(f'{scroll_css_selector}.scrollTop = {i}')
+            self.castJS(f'{scroll_css_selector}.scrollTop = {i}')
             i += scroll_pixel_length
             # Wait to load page
             self.wait(wait_interval)
             if verbose:
                 print(f'\rScroll #{counter} completed!', end='')
             counter += 1
             # Execute callback function
             if callback:
                 callback(self)
 
             # If page is dynamically adding content to page, max_height will increment.
-            max_height = int(self.cast_js(f'return {scroll_css_selector}.scrollHeight'))
+            max_height = int(self.castJS(f'return {scroll_css_selector}.scrollHeight'))
 
         # Go to next line after scroll completion.
         print('')
 
 
-    def infinite_scroll(self, wait_interval, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
+    def infiniteScroll(self, wait_interval, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
         counter = 1
 
         # Make the CSS Selector into a querySelector
         if scroll_css_selector != 'document.scrollingElement':
             scroll_css_selector = f'document.querySelector("{scroll_css_selector}")'
 
         last_height = self.driver.execute_script(f"return {scroll_css_selector}.scrollHeight")
@@ -188,60 +176,60 @@
             if new_height == last_height:
                 break
             last_height = new_height
         # Go to next line after scroll completion.
         print('')
 
 
-    def delicate_infinite_scroll(self, wait_interval, scroll_pixel_length=500, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
+    def infiniteScrollByPixels(self, wait_interval, scroll_pixel_length=500, scroll_css_selector="document.scrollingElement", callback=None, verbose=True):
         counter = 1
 
         # Make the CSS Selector into a querySelector
         if scroll_css_selector != 'document.scrollingElement':
             scroll_css_selector = f'document.querySelector("{scroll_css_selector}")'
 
         # last_height = self.driver.execute_script(f"return {scroll_css_selector}.scrollHeight")
-        max_height = int(self.cast_js(f'return {scroll_css_selector}.scrollHeight'))
+        max_height = int(self.castJS(f'return {scroll_css_selector}.scrollHeight'))
         i = 0
 
         while max_height > i:
-            self.cast_js(f'{scroll_css_selector}.scrollTop = {i}')
+            self.castJS(f'{scroll_css_selector}.scrollTop = {i}')
             i += scroll_pixel_length
             # Wait to load page
             self.wait(wait_interval)
             if verbose:
                 print(f'\rScroll #{counter} completed!', end='')
             counter += 1
             # Execute callback function
             if callback:
                 callback(self)
 
             # If page is dynamically adding content to page, max_height will increment.
-            max_height = int(self.cast_js(f'return {scroll_css_selector}.scrollHeight'))
+            max_height = int(self.castJS(f'return {scroll_css_selector}.scrollHeight'))
 
         # Go to next line after scroll completion.
         print('')
 
     # Wait a certain amount of seconds to continue code.
     def wait(self, time_interval):
         sleep(time_interval)
 
     # Gets the end name of the URL
-    def get_slug(self):
+    def getSlug(self):
         # Get portion of URL after last forward slash.
         slug =  re.sub(r'^.+?/([^/]+?)$', r'\1', self.url)
         # Remove any hashes
         slug = re.sub(r'#[^#]+?$', r'', slug)
         # Remove any queries
         slug = re.sub(r'\?.+?$', r'', slug)
         return slug
 
 
 
-    def network_log(self):
+    def getNetworkLog(self):
         filtered_entries = []
         # Get the full performance log
         logs = self.driver.get_log('performance')
 
         for entry in logs:
             # Parse the entry.
             log = json.loads(entry["message"])["message"]
@@ -251,21 +239,21 @@
                 or "Network.request" in log["method"]
                 or "Network.webSocket" in log["method"]
             ):
                 filtered_entries.append(log)
         return filtered_entries
 
 
-    def cast_js(self, javaScript, arguments=None):
+    def castJS(self, javaScript, arguments=None):
         return self.driver.execute_script(javaScript, arguments)
 
 
-    def cast_in_discrete_tab(self, url, callback=False, payload=None):
+    def openTab(self, url, callback=False, payload=None):
         # Open a new tab to the url
-        self.cast_js(f"window.open('{url}', '_blank');")
+        self.castJS(f"window.open('{url}', '_blank');")
         # Get list of all tabs (handles)
         handles = self.driver.window_handles
         # Make focus on second handle
         self.driver.switch_to.window(handles[1])
         # Pause to allow tab to load
         self.wait(3)
         # Call the callback with the payload arguments
@@ -275,40 +263,42 @@
         # Close the tab
         self.driver.close()
         # Switch focus back to main handle
         self.driver.switch_to.window(handles[0])
 
         return payload
 
-    def take_screenshot(self, css_selector):
+    def getScreenshot(self, css_selector):
         return self.driver.find_element(By.CSS_SELECTOR, css_selector).screenshot_as_png
 
     def clear(self, css_selector):
         self.driver.find_element(By.CSS_SELECTOR, css_selector).clear()
 
     def type(self, css_selector, string):
         self.driver.find_element(By.CSS_SELECTOR, css_selector).send_keys(string)
 
     def destroy(self, css_selector):
         try:
-            self.cast_js(f"""
+            self.castJS(f"""
             let els = document.querySelectorAll('{css_selector}');
             els.length > 0 ? els[0].remove() : null;
             """)
         except JavascriptException as err:
             print('WebMage tried to destroyed an element that does not exist.')
 
     def destroyAll(self, css_selector):
         try:
-            self.cast_js(f"""
+            self.castJS(f"""
             document.querySelectorAll('{css_selector}')
                 .forEach(el => el.remove());
             """)
         except JavascriptException as err:
             print('WebMage tried to destroyed an element that does not exist.')
 
-    def switch_frames(self, css_selector):
+    def switchToDefaultContent(self):
         self.driver.switch_to.default_content()
+
+    def switchFrames(self, css_selector):
         self.driver.switch_to.frame(self.driver.find_element(By.CSS_SELECTOR, css_selector))
 
-    def get_page_source(self):
-        return self.driver.page_source
+    def getPageSource(self):
+        return self.driver.page_source
```

### Comparing `webmage-1.0.2/webmage/dynamic_rune.py` & `webmage-1.0.3/webmage/rune.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .support import style_attributes
-from .dynamic_rune_array import DynamicRuneArr
+from .rune_list import RuneList
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.common.by import By
 
-class DynamicRune:
+class Rune:
     def __init__(self, selenium_rune, driver):
         self.selenium_rune = selenium_rune
         self.driver = driver
         self.text = selenium_rune.text
         self.outerHTML = selenium_rune.get_attribute('outerHTML')
+        self.tagName = selenium_rune.get_attribute('tagName').lower()
 
     def __repr__(self):
         return f'{self.outerHTML}'
 
     def __str__(self):
         return f'{self.outerHTML}'
 
@@ -20,44 +20,43 @@
         value = self.selenium_rune.get_attribute(item_request)
         return value
 
     def __contains__(self, item_request):
         value = self.selenium_rune.get_attribute(item_request)
         return value
 
-    def cast_js(self, javaScript, arguments=None):
+    def castJS(self, javaScript, arguments=None):
         return self.driver.execute_script(javaScript, arguments)
 
     def select(self, css_selector):
-        return DynamicRune(self.selenium_rune.find_element(By.CSS_SELECTOR ,css_selector), self.driver)
+        return Rune(self.selenium_rune.find_element(By.CSS_SELECTOR ,css_selector), self.driver)
 
     def selectAll(self, css_selector):
-        return DynamicRuneArr([DynamicRune(i, self.driver) for i in self.selenium_rune.find_elements(By.CSS_SELECTOR, css_selector)])
+        return RuneList([Rune(i, self.driver) for i in self.selenium_rune.find_elements(By.CSS_SELECTOR, css_selector)])
 
-    def get_attributes(self):
+    def getAttributes(self):
         self.attributes = {}
         for attribute in self.selenium_rune.get_property('attributes'):
             self.attributes[attribute['nodeName']] = self.selenium_rune.get_attribute(attribute['nodeName'])
 
     def click(self):
         self.selenium_rune.click()
 
 
     def destroy(self, css_selector=None):
         # If no css_selector is provided, then delete the element itself.
         if css_selector == None:
-            self.cast_js("""
+            self.castJS("""
             arguments[0].remove();
             """, self.selenium_rune)        
         # If a css_selector is provided, then search for an element within the element to delete.
         else:
-            self.cast_js(f"""
+            self.castJS(f"""
             let els = arguments[0].querySelectorAll('{css_selector}');
             els.length > 0 ? els[0].remove() : null;
             """, self.selenium_rune)
 
     def destroyAll(self, css_selector):
-        self.cast_js(f"""
+        self.castJS(f"""
         arguments[0].querySelectorAll('{css_selector}')
             .forEach(el => el.remove());
         """, self.selenium_rune)
-
```

### Comparing `webmage-1.0.2/webmage.egg-info/PKG-INFO` & `webmage-1.0.3/webmage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: webmage
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library with built-in methods that make web scraping easier for dynamically loading pages.
 Home-page: https://github.com/javascriptorian/webmage
 Author: The JavaScriptorian
 Author-email: javascriptorian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: webdriver_manager>=3.8.5
+Requires-Dist: selenium>=4.8.2
+Requires-Dist: beautifulsoup4>=4.11.2
+Requires-Dist: undetected_chromedriver>=3.4.6
 
 # Description
 A wrapper around requests, BeautifulSoup, and Selenium (Chrome) to facilitate web scraping.
 
 # Installation
 ```pip install webmage```
```

