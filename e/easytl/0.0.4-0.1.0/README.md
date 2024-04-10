# Comparing `tmp/easytl-0.0.4.tar.gz` & `tmp/easytl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.0.4.tar", last modified: Mon Apr  8 10:36:09 2024, max compression
+gzip compressed data, was "easytl-0.1.0.tar", last modified: Wed Apr 10 05:59:40 2024, max compression
```

## Comparing `easytl-0.0.4.tar` & `easytl-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.950820 easytl-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.942819 easytl-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.946820 easytl-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 10:35:55.000000 easytl-0.0.4/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-08 10:35:55.000000 easytl-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-08 10:35:55.000000 easytl-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 10:36:09.950820 easytl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-08 10:35:55.000000 easytl-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-08 10:35:55.000000 easytl-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:36:09.950820 easytl-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.946820 easytl-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.946820 easytl-0.0.4/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15114 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    20656 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 10:35:55.000000 easytl-0.0.4/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:36:09.946820 easytl-0.0.4/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 10:36:09.000000 easytl-0.0.4/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 10:36:09.000000 easytl-0.0.4/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:36:09.000000 easytl-0.0.4/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 10:36:09.000000 easytl-0.0.4/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 10:36:09.000000 easytl-0.0.4/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.216667 easytl-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-10 05:59:26.000000 easytl-0.1.0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-10 05:59:26.000000 easytl-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-10 05:59:26.000000 easytl-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-10 05:59:40.220667 easytl-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-10 05:59:26.000000 easytl-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 05:59:26.000000 easytl-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:59:40.220667 easytl-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.216667 easytl-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/top_level.txt
```

### Comparing `easytl-0.0.4/.github/workflows/workflow.yml` & `easytl-0.1.0/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/.gitignore` & `easytl-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/LICENSE.md` & `easytl-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/PKG-INFO` & `easytl-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.0.4
+Version: 0.1.0
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `easytl-0.0.4/README.md` & `easytl-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/pyproject.toml` & `easytl-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0"
 ]
 
 name = "easytl"
-version = "v0.0.4"
+version = "v0.1.0"
 authors = [
   { name="Bikatr7", email="Tetralon07@gmail.com" },
 ]
 description = "Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `easytl-0.0.4/src/easytl/__init__.py` & `easytl-0.1.0/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/classes.py` & `easytl-0.1.0/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/deepl_service.py` & `easytl-0.1.0/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/easytl.py` & `easytl-0.1.0/src/easytl/easytl.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/exceptions.py` & `easytl-0.1.0/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/gemini_service.py` & `easytl-0.1.0/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.0.4/src/easytl/openai_service.py` & `easytl-0.1.0/src/easytl/openai_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,32 +345,43 @@
         Returns:
         num_tokens (int) : The number of tokens.
         cost (float) : The cost of the translation.
         model (string) : The model used for the translation.
 
         """
 
+        cost_modifier = 1.0
+
         if(translation_instructions is None):
             translation_instructions = OpenAIService._default_translation_instructions.content
 
         if(isinstance(text, typing.Iterable)):
 
             if(not isinstance(text,str) and not _is_iterable_of_strings(text)):
                 raise ValueError("The text must be a string or an iterable of strings.")
-
-            ## since instructions are paired with the text, we need to repeat the instructions for index
-            translation_instructions = translation_instructions * len(text) # type: ignore
+            
+            if(isinstance(text, ModelTranslationMessage) or isinstance(text, SystemTranslationMessage)):
+                ## since instructions are paired with the text, we need to repeat the instructions for index
+                ## this only works if the text is pre-built ModelTranslationMessage or SystemTranslationMessage objects
+                ## otherwise, the instructions will be repeated for each item in the iterable which is not the intended behavior
+                translation_instructions = translation_instructions * len(text) # type: ignore
+
+            else:
+                ## otherwise, we can really only estimate.
+                cost_modifier = 2.5
 
             text = _convert_iterable_to_str(text)
 
         if(isinstance(translation_instructions, typing.Iterable)):
             translation_instructions = _convert_iterable_to_str(translation_instructions)
 
         if(model is None):
             model = OpenAIService._default_model
 
         ## not exactly how the text will be formatted, but it's close enough for the purposes of estimating the cost as tokens should be the same
         total_text_to_estimate = f"{translation_instructions}\n{text}"
         
         _num_tokens, _cost, _ = _estimate_cost(total_text_to_estimate, model)
 
+        _cost = _cost * cost_modifier
+
         return _num_tokens, _cost, model
```

### Comparing `easytl-0.0.4/src/easytl/util.py` & `easytl-0.1.0/src/easytl/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -250,95 +250,118 @@
 
     assert model in ALLOWED_OPENAI_MODELS or model in ALLOWED_GEMINI_MODELS, f"""EasyTL does not support : {model}"""
 
     ## default models are first, then the rest are sorted by price case
     if(price_case is None):
 
         if(model == "gpt-3.5-turbo"):
-            print("Warning: gpt-3.5-turbo may change over time. Returning num tokens assuming gpt-3.5-turbo-1106 as it is the most recent version of gpt-3.5-turbo.")
-            return _estimate_cost(text, model="gpt-3.5-turbo-1106", price_case=2)
+            print("Warning: gpt-3.5-turbo may change over time. Estimating cost assuming gpt-3.5-turbo-0125 as it is the most recent version of gpt-3.5-turbo.")
+            return _estimate_cost(text, model="gpt-3.5-turbo-0125")
+        
+        elif(model == "gpt-3.5-turbo-16k"):
+            print("Warning: gpt-3.5-turbo-16k may change over time. Estimating cost assuming gpt-3.5-turbo-16k-0613 as it is the most recent version of gpt-3.5-turbo-16k.")
+            return _estimate_cost(text, model="gpt-3.5-turbo-16k-0613")
         
         elif(model == "gpt-4"):
-            print("Warning: gpt-4 may change over time. Returning num tokens assuming gpt-4-1106-preview as it is the most recent version of gpt-4.")
-            return _estimate_cost(text, model="gpt-4-1106-preview", price_case=4)
+            print("Warning: gpt-4 may change over time. Estimating cost assuming gpt-4-0613 as it is the most recent version of gpt-4.")
+            return _estimate_cost(text, model="gpt-4-0613")
         
+        elif(model == "gpt-4-32k"):
+            print("Warning: gpt-4-32k may change over time. Estimating cost assuming gpt-4-32k-0613 as it is the most recent version of gpt-4-32k.")
+            return _estimate_cost(text, model="gpt-4-32k-0613")
+        
+        elif(model == "gpt-4-turbo"):
+            print("Warning: gpt-4-turbo may change over time. Estimating cost assuming gpt-4-turbo-2024-04-09 as it is the most recent version of gpt-4-turbo.")
+            return _estimate_cost(text, model="gpt-4-turbo-2024-04-09")
+                
         elif(model == "gpt-4-turbo-preview"):
-            print("Warning: gpt-4-turbo-preview may change over time. Returning num tokens assuming gpt-4-0125-preview as it is the most recent version of gpt-4-turbo-preview.")
-            return _estimate_cost(text, model="gpt-4-0125-preview", price_case=4)
+            print("Warning: gpt-4-turbo-preview may change over time. Estimating cost assuming gpt-4-0125-preview as it is the most recent version of gpt-4-turbo-preview.")
+            return _estimate_cost(text, model="gpt-4-0125-preview")
+        
+        elif(model == "gpt-4-vision-preview"):
+            print("Warning: gpt-4-vision-preview may change over time. Estimating cost assuming gpt-4-1106-vision-preview as it is the most recent version of gpt-4-1106-vision-preview.")
+            return _estimate_cost(text, model="gpt-4-1106-vision-preview")
         
         elif(model == "gpt-3.5-turbo-0613"):
-            print("Warning: gpt-3.5-turbo-0613 is considered depreciated by OpenAI as of November 6, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-1106.")
+            print("Warning: gpt-3.5-turbo-0613 is considered depreciated by OpenAI as of November 6, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-0125.")
             return _estimate_cost(text, model=model, price_case=1)
 
         elif(model == "gpt-3.5-turbo-0301"):
-            print("Warning: gpt-3.5-turbo-0301 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-1106 unless you are specifically trying to break the filter.")
+            print("Warning: gpt-3.5-turbo-0301 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-0125 unless you are specifically trying to break the filter.")
             return _estimate_cost(text, model=model, price_case=1)
         
         elif(model == "gpt-3.5-turbo-1106"):
+            print("Warning: gpt-3.5-turbo-1106 is outdated, consider switching to gpt-3.5-turbo-0125.")
             return _estimate_cost(text, model=model, price_case=2)
         
         elif(model == "gpt-3.5-turbo-0125"):
             return _estimate_cost(text, model=model, price_case=7)
-        
+            
         elif(model == "gpt-3.5-turbo-16k-0613"):
             print("Warning: gpt-3.5-turbo-16k-0613 is considered depreciated by OpenAI as of November 6, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-1106.")
             return _estimate_cost(text, model=model, price_case=3)
         
         elif(model == "gpt-4-1106-preview"):
-            return _estimate_cost(text, model=model, price_case=4)
+            return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gpt-4-0125-preview"):
-            return _estimate_cost(text, model=model, price_case=4)
+            return _estimate_cost(text, model=model, price_case=8)
+        
+        elif(model == "gpt-4-1106-vision-preview"):
+            return _estimate_cost(text, model=model, price_case=8)
+        
+        elif(model == "gpt-4-turbo-2024-04-09"):
+            return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gpt-4-0314"):
             print("Warning: gpt-4-0314 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-4-0613.")
             return _estimate_cost(text, model=model, price_case=5)
         
         elif(model == "gpt-4-0613"):
             return _estimate_cost(text, model=model, price_case=5)
-        
+                
         elif(model == "gpt-4-32k-0314"):
             print("Warning: gpt-4-32k-0314 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-4-32k-0613.")
             return _estimate_cost(text, model=model, price_case=6)
         
         elif(model == "gpt-4-32k-0613"):
             return _estimate_cost(text, model=model, price_case=6)
         
         elif(model == "gemini-pro"):
-            print(f"Warning: gemini-pro may change over time. Returning num tokens assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
+            print(f"Warning: gemini-pro may change over time. Estimating cost assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
             return _estimate_cost(text, model="gemini-1.0-pro-001", price_case=8)
         
         elif(model == "gemini-pro-vision"):
-            print("Warning: gemini-pro-vision may change over time. Returning num tokens assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
+            print("Warning: gemini-pro-vision may change over time. Estimating cost assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
             return _estimate_cost(text, model="gemini-1.0-pro-vision-001", price_case=8)
         
-        elif(model == "gemini-ultra"):
-            return _estimate_cost(text, model=model, price_case=8)
+       ## elif(model == "gemini-ultra"):
+    ##        return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro"):
-            print(f"Warning: gemini-1.0-pro may change over time. Returning num tokens assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
+            print(f"Warning: gemini-1.0-pro may change over time. Estimating cost assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
             return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-vision"):
-            print("Warning: gemini-1.0-pro-vision may change over time. Returning num tokens assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
+            print("Warning: gemini-1.0-pro-vision may change over time. Estimating cost assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
             return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-latest"):
-            print(f"Warning: gemini-1.0-pro-latest may change over time. Returning num tokens assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
+            print(f"Warning: gemini-1.0-pro-latest may change over time. Estimating cost assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
             return _estimate_cost(text, model="gemini-1.0-pro-001", price_case=8)
         
         elif(model == "gemini-1.0-pro-vision-latest"):
-            print("Warning: gemini-1.0-pro-vision-latest may change over time. Returning num tokens assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
+            print("Warning: gemini-1.0-pro-vision-latest may change over time. Estimating cost assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
             return _estimate_cost(text, model="gemini-1.0-pro-vision-001", price_case=8)
         
         elif(model == "gemini-1.5-pro-latest"):
             return _estimate_cost(text, model=model, price_case=8)
         
-        elif(model == "gemini-1.0-ultra-latest"):
-            return _estimate_cost(text, model=model, price_case=8)
+  ##      elif(model == "gemini-1.0-ultra-latest"):
+      ##      return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-001"):
             return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-vision-001"):
             return _estimate_cost(text, model=model, price_case=8)
         
@@ -371,69 +394,80 @@
 
         return _num_tokens, _min_cost, model
     
     ## _type checker doesn't like the chance of None being returned, so we raise an exception here if it gets to this point, which it shouldn't
     raise Exception("An unknown error occurred while calculating the minimum cost of translation.")
 
 ##-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
 ## https://platform.openai.com/docs/models/overview
 ALLOWED_OPENAI_MODELS  = [
     "gpt-3.5-turbo",
-    "gpt-4",
-    "gpt-4-turbo-preview",
     "gpt-3.5-turbo-0301",
-    "gpt-4-0314",
-    "gpt-4-32k-0314",
-    "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-0125",
-    "gpt-3.5-turbo-16k-0613",
+    "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-1106",
+    "gpt-3.5-turbo-16k",
+    "gpt-3.5-turbo-16k-0613",
+    "gpt-4",
+    "gpt-4-0314",
     "gpt-4-0613",
+    "gpt-4-32k",
+    "gpt-4-32k-0314",
     "gpt-4-32k-0613",
+    "gpt-4-turbo",
+    "gpt-4-turbo-preview",
+    "gpt-4-turbo-2024-04-09",
+    "gpt-4-0125-preview",
     "gpt-4-1106-preview",
-    "gpt-4-0125-preview"
+    "gpt-4-vision-preview",
+    "gpt-4-1106-vision-preview",
 ]
 
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
 ## https://ai.google.dev/models/gemini
 ALLOWED_GEMINI_MODELS = [
     "gemini-1.0-pro-001",
-    "gemini-1.0-pro-vision-001",
     "gemini-1.0-pro",
-    "gemini-1.0-pro-vision",
     "gemini-1.0-pro-latest",
+    "gemini-1.0-pro-vision-001",
+    "gemini-1.0-pro-vision",
     "gemini-1.0-pro-vision-latest",
     "gemini-1.5-pro-latest",
-    "gemini-1.0-ultra-latest",
+  ##  "gemini-1.0-ultra-latest",
     "gemini-pro",
     "gemini-pro-vision",
-    "gemini-ultra"
+  ##  "gemini-ultra"
 ]
 
-## Costs are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-02
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
 MODEL_COSTS = {
-    "gpt-3.5-turbo": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
-    "gpt-4": {"price_case": 4, "_input_cost": 0.01, "_output_cost": 0.03},
-    "gpt-4-turbo-preview": {"price_case": 4, "_input_cost": 0.01, "_output_cost": 0.03},
-    "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
+    # Grouping GPT-3.5 models together
+    "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-0301": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
+    "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-1106": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
-    "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-16k-0613": {"price_case": 3, "_input_cost": 0.0030, "_output_cost": 0.0040},
-    "gpt-4-1106-preview": {"price_case": 4, "_input_cost": 0.01, "_output_cost": 0.03},
-    "gpt-4-0125-preview": {"price_case": 4, "_input_cost": 0.01, "_output_cost": 0.03},
+    
+    # Grouping GPT-4 models by their capabilities and versions
     "gpt-4-0314": {"price_case": 5, "_input_cost": 0.03, "_output_cost": 0.06},
     "gpt-4-0613": {"price_case": 5, "_input_cost": 0.03, "_output_cost": 0.06},
     "gpt-4-32k-0314": {"price_case": 6, "_input_cost": 0.06, "_output_cost": 0.012},
     "gpt-4-32k-0613": {"price_case": 6, "_input_cost": 0.06, "_output_cost": 0.012},
-    "gemini-1.0-pro-001": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-pro-vision-001": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-pro": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-pro-vision": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-pro-latest": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-pro-vision-latest": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.5-pro-latest": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-1.0-ultra-latest": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-pro": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-pro-vision": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0},
-    "gemini-ultra": {"price_case": 8, "_input_cost": 0.0, "_output_cost": 0.0}
+    "gpt-4-1106-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
+    "gpt-4-0125-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
+    "gpt-4-1106-vision-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
+    "gpt-4-turbo-2024-04-09": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
+    
+    # Grouping Gemini models together
+    "gemini-1.0-pro-001": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.0-pro-vision-001": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.0-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.0-pro-vision": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.0-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.0-pro-vision-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.5-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+ ##   "gemini-1.0-ultra-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-pro-vision": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+ ##   "gemini-ultra": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0}
 }
```

### Comparing `easytl-0.0.4/src/easytl.egg-info/PKG-INFO` & `easytl-0.1.0/src/easytl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.0.4
+Version: 0.1.0
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

