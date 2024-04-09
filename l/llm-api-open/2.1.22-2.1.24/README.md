# Comparing `tmp/llm-api-open-2.1.22.tar.gz` & `tmp/llm-api-open-2.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-api-open-2.1.22.tar", last modified: Fri Apr  5 16:16:56 2024, max compression
+gzip compressed data, was "llm-api-open-2.1.24.tar", last modified: Tue Apr  9 22:01:48 2024, max compression
```

## Comparing `llm-api-open-2.1.22.tar` & `llm-api-open-2.1.24.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.114415 llm-api-open-2.1.22/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.106414 llm-api-open-2.1.22/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/configs/chatgpt.json
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/configs/ms_copilot.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:16:56.114415 llm-api-open-2.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.106414 llm-api-open-2.1.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/llm_api_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/assistantGetLastMessage.js
--rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/conversationSearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/proxy_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/external_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/module_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/ms_copilot/
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/conversationManage.js
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/conversationParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/ms_copilot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/proxy_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.133995 llm-api-open-2.1.24/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.133995 llm-api-open-2.1.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 22:01:48.000000 llm-api-open-2.1.24/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:01:48.137995 llm-api-open-2.1.24/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43383 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 22:01:44.000000 llm-api-open-2.1.24/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm-api-open-2.1.22/LICENSE` & `llm-api-open-2.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/PKG-INFO` & `llm-api-open-2.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.22
+Version: 2.1.24
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `llm-api-open-2.1.22/README.md` & `llm-api-open-2.1.24/README.md`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/configs/chatgpt.json` & `llm-api-open-2.1.24/configs/chatgpt.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/configs/ms_copilot.json` & `llm-api-open-2.1.24/configs/ms_copilot.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/setup.py` & `llm-api-open-2.1.24/setup.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/llm_api_open.egg-info/PKG-INFO` & `llm-api-open-2.1.24/src/llm_api_open.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.22
+Version: 2.1.24
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `llm-api-open-2.1.22/src/llm_api_open.egg-info/SOURCES.txt` & `llm-api-open-2.1.24/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/_version.py` & `llm-api-open-2.1.24/src/lmao/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "2.1.22"
+__version__ = "2.1.24"
```

### Comparing `llm-api-open-2.1.22/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm-api-open-2.1.24/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/chatgpt/chatgpt_api.py` & `llm-api-open-2.1.24/src/lmao/chatgpt/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/chatgpt/conversationSearch.js` & `llm-api-open-2.1.24/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/chatgpt/proxy_extension.py` & `llm-api-open-2.1.24/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/external_api.py` & `llm-api-open-2.1.24/src/lmao/external_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/main.py` & `llm-api-open-2.1.24/src/lmao/main.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/module_wrapper.py` & `llm-api-open-2.1.24/src/lmao/module_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/ms_copilot/conversationManage.js` & `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationManage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.22/src/lmao/ms_copilot/conversationParser.js` & `llm-api-open-2.1.24/src/lmao/ms_copilot/conversationParser.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -270,36 +270,38 @@
             if (metaContent !== null) {
                 result.meta = metaContent.innerText;
             }
         }
 
         // Text response
         else if (cibMessage.getAttribute("type") === "text") {
-            // Get and check for text block
-            const textBlock = cibMessage.shadowRoot.querySelector("cib-shared > div > div > div.ac-textBlock");
-            if (textBlock !== null) {
-                // Create a copy
-                const textBlockClone = textBlock.cloneNode(true);
-
-                // Find and fix code blocks
-                // {"code block placeholder": "code block content", ...}
-                const codeBlocks = {};
-                for (const child of textBlockClone.children) {
-                    preformatRecursion(child, codeBlocks);
-                }
+            // Get and check for text blocks
+            const textBlocks = cibMessage.shadowRoot.querySelectorAll("cib-shared > div > div > div.ac-textBlock");
+            if (textBlocks.length !== 0) {
+                for (const textBlock of textBlocks) {
+                    // Create a copy
+                    const textBlockClone = textBlock.cloneNode(true);
+
+                    // Find and fix code blocks
+                    // {"code block placeholder": "code block content", ...}
+                    const codeBlocks = {};
+                    for (const child of textBlockClone.children) {
+                        preformatRecursion(child, codeBlocks);
+                    }
 
-                if (result.text === undefined) {
-                    result.text = textBlockClone.innerHTML;
-                } else {
-                    result.text += textBlockClone.innerHTML;
+                    if (result.text === undefined) {
+                        result.text = textBlockClone.innerHTML;
+                    } else {
+                        result.text += textBlockClone.innerHTML;
+                    }
+                    result.code_blocks = codeBlocks;
                 }
-                result.code_blocks = codeBlocks;
             }
 
-            // No text block
+            // No text blocks
             else {
                 const textMessageContent = cibMessage.shadowRoot.querySelector("cib-shared > div.content.text-message-content");
                 if (textMessageContent !== null) {
                     if (result.text === undefined) {
                         result.text = "<p>" + textMessageContent.innerText + "</p>";
                     } else {
                         result.text += "<p>" + textMessageContent.innerText + "</p>";
@@ -435,8 +437,10 @@
     // Log and return error as string
     catch (error) {
         console.error(error);
         return {
             error: "" + error
         };
     }
-}
+}
+
+actionHandle("parse");
```

### Comparing `llm-api-open-2.1.22/src/lmao/ms_copilot/ms_copilot_api.py` & `llm-api-open-2.1.24/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -877,14 +877,17 @@
         Args:
             url (str or None, optional): URL to load or None to refresh. Defaults to None
             restart_session_on_error (bool, optional): call session_close() and session_start() on error
 
         Returns:
             bool: True if loaded successfully, False if not
         """
+        # Reset timer
+        self._refresher_timer = time.time()
+
         # Wait a bit just in case
         time.sleep(0.5)
 
         retries_counter = 0
         while True:
             try:
                 # Set timeout
@@ -1008,16 +1011,15 @@
                     self.driver
                     and not self._refresher_dont_refresh_flag
                     and time_current - self._refresher_timer > auto_refresh_interval
                 ):
                     # Set busy flag
                     self._refresher_busy = True
 
-                    # Refresh page
-                    self._refresher_timer = time_current
+                    # Refresh page (self._refresher_timer will be set inside this function)
                     if not self._load_or_refresh():
                         raise Exception("Unable to auto-refresh page")
 
                     # Save cookies
                     self.cookies_save()
 
                 # Clear busy flag
```

### Comparing `llm-api-open-2.1.22/src/lmao/ms_copilot/proxy_extension.py` & `llm-api-open-2.1.24/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*

