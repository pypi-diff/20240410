# Comparing `tmp/vectara-0.0.1.tar.gz` & `tmp/vectara-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-0.0.1.tar", last modified: Wed Nov 22 06:43:24 2023, max compression
+gzip compressed data, was "vectara-0.0.2.tar", last modified: Tue Apr  9 22:43:09 2024, max compression
```

## Comparing `vectara-0.0.1.tar` & `vectara-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2023-11-22 06:43:24.347012 vectara-0.0.1/
--rw-rw-r--   0 forrest   (1000) forrest   (1000)    35149 2023-11-22 00:46:38.000000 vectara-0.0.1/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43749 2023-11-22 06:43:24.347012 vectara-0.0.1/PKG-INFO
--rw-rw-r--   0 forrest   (1000) forrest   (1000)     2707 2023-11-22 05:36:38.000000 vectara-0.0.1/README.md
--rw-rw-r--   0 forrest   (1000) forrest   (1000)      621 2023-11-22 06:43:19.000000 vectara-0.0.1/pyproject.toml
--rw-rw-r--   0 forrest   (1000) forrest   (1000)      151 2023-11-22 06:43:24.347012 vectara-0.0.1/setup.cfg
-drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2023-11-22 06:43:24.347012 vectara-0.0.1/src/
-drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2023-11-22 06:43:24.347012 vectara-0.0.1/src/vectara/
--rw-rw-r--   0 forrest   (1000) forrest   (1000)    13267 2023-11-22 05:35:00.000000 vectara-0.0.1/src/vectara/__init__.py
--rw-rw-r--   0 forrest   (1000) forrest   (1000)      179 2023-11-21 20:58:02.000000 vectara-0.0.1/src/vectara/__main__.py
-drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2023-11-22 06:43:24.347012 vectara-0.0.1/src/vectara.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43749 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/PKG-INFO
--rw-rw-r--   0 forrest   (1000) forrest   (1000)      302 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/SOURCES.txt
--rw-rw-r--   0 forrest   (1000) forrest   (1000)        1 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/dependency_links.txt
--rw-rw-r--   0 forrest   (1000) forrest   (1000)       50 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/entry_points.txt
--rw-rw-r--   0 forrest   (1000) forrest   (1000)       64 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/requires.txt
--rw-rw-r--   0 forrest   (1000) forrest   (1000)        8 2023-11-22 06:43:24.000000 vectara-0.0.1/src/vectara.egg-info/top_level.txt
+drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2024-04-09 22:43:09.440794 vectara-0.0.2/
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)    35149 2024-01-21 15:32:15.000000 vectara-0.0.2/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    47663 2024-04-09 22:43:09.440794 vectara-0.0.2/PKG-INFO
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)     6622 2024-04-09 22:33:27.000000 vectara-0.0.2/README.md
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)      621 2024-04-09 22:33:27.000000 vectara-0.0.2/pyproject.toml
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)      151 2024-04-09 22:43:09.440794 vectara-0.0.2/setup.cfg
+drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2024-04-09 22:43:09.436794 vectara-0.0.2/src/
+drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2024-04-09 22:43:09.436794 vectara-0.0.2/src/vectara/
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)    21025 2024-04-09 22:42:26.000000 vectara-0.0.2/src/vectara/__init__.py
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)      179 2024-01-21 15:32:15.000000 vectara-0.0.2/src/vectara/__main__.py
+drwxrwxr-x   0 forrest   (1000) forrest   (1000)        0 2024-04-09 22:43:09.440794 vectara-0.0.2/src/vectara.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    47663 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/PKG-INFO
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)      302 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/SOURCES.txt
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)        1 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/dependency_links.txt
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)       50 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/entry_points.txt
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)       64 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/requires.txt
+-rw-rw-r--   0 forrest   (1000) forrest   (1000)        8 2024-04-09 22:43:09.000000 vectara-0.0.2/src/vectara.egg-info/top_level.txt
```

### Comparing `vectara-0.0.1/LICENSE` & `vectara-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vectara-0.0.1/PKG-INFO` & `vectara-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial Python SDK and CLI
 Author-email: Forrest Sheng Bao <forrest@vectara.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,69 +687,93 @@
 Requires-Dist: textwrap3
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 Requires-Dist: tqdm
 Requires-Dist: IPython
 Requires-Dist: fire
 
-# An UNofficial Python SDK and CLI for Vectara's RAG platform 
+# An UNofficial Python SDK and CLI for Vectara's RAG platform
 
-It supports major features of Vectara's RAG platform for you to build your own search engine. 
+It supports major features of Vectara's RAG platform for you to build your own search engine.
 
-Additional features: 
-* It expands the upload function to allow you to upload a list of files or all files under a directory in one function call. 
-* Renders query results in beautiful Markdown printout.
+Additional features:
+
+* It expands the upload function to allow you to upload a list of files or all files under a directory in one function call.
+* Renders query results in beautiful Markdown printout (see `demo.ipynb`).
+* It supports logging user feedback from the GUI in a local SQLite database for evaluating the quality of search and RAG. 
+
+**If you like this SDK/CLI/GUI, give us a star on Github!**
 
 ## Installation
 
 ```bash
-# pip install from Github
+# Stable
+pip install vectara
+
+# Nightly
 pip install "git+https://github.com/forrestbao/vectara-python-cli.git"
 ```
 
-## Usage 
+## Usage
 
 ### Credentials
 
-You can obtain the Vectara credentials following [this guide](https://docs.vectara.com/docs/learn/authentication/oauth-2). 
-Then set up your Vectara credentials as environment variables. 
+This client supports authentication in both Vectara's [Personal API key](https://docs.vectara.com/docs/console-ui/personal-api-key) and [OAuth2](https://docs.vectara.com/docs/console-ui/app-clients). In either case, you need to obtain [customer ID](https://docs.vectara.com/docs/console-ui/vectara-console-overview#view-the-customer-id) as well. 
+
+Following the convention of OpenAI's client, we recommend setting credentials as environment variables. You can save them as a bash script and simply `source` it before using the SDK or CLI.
 
 ```bash
-export VECTARA_CUSTOMER_ID=123
+export VECTARA_CUSTOMER_ID=123 # Required regardless of the authentication method
+
+# Set API Key if you plan to use Personal API Key to authenticate
+export VECTARA_API_KEY=abc
+
+# Set the following two variables if you plan to use OAuth2 to authenticate
 export VECTARA_CLIENT_ID=abc
 export VECTARA_CLIENT_SECRET=xyz
+
+# If both API key and OAuth2 credentials are set, the SDK will use API key only.
+
+# optional, if you are using a proxy like LlaMasterKey https://github.com/TexteaInc/LlaMasterKey/
+export VECTARA_BASE_URL="http://127.0.0.1:8000/vectara"
+export VECTARA_PROXY_MODE=true # Enable proxy mode
 ```
 
-This unofficial SDK and CLI will read your credentials from the environment variables above. The ability to pass in credentials as arguments is also supported.
+Alternatively, you can pass in your credentials as arguments when initializing the client. See it from the complete code. 
+
+### Using the Python SDK 
 
-### Python 
-Try the Jupyter notebook `demo.ipynb` or read the docstring. 
+Try the Jupyter notebook `demo.ipynb`, the script `demo.py`, or read the docstring.
 
 ```python
-from vectara import vectara
+from vectara import vectara, post_process_query_result
 
-client = vectara() # get default credentials from environment variables 
-                   # You can also manually pass in your credentials as arguments
+client = vectara() # get credentials from environment variables 
 
 corpus_id = client.create_corpus('my knowledge base')
 
-client.upload(corpus_id, 'one_file.pdf', description='My precious doc')  # add one file to the corpus 
+client.upload(corpus_id, 'one_file.pdf', description='A scientific paper')  # add one file to the corpus 
 client.upload(corpus_id, 'a_folder_of_documents') # add all files under a folder to the corpus
-client.upload(corpus_id, ['user_manual.md', 'notes.txt'], description=['user manual', 'my memory']) # add a list of files to the corpus
+client.upload(corpus_id, ['README.md', 'demo.py'], description=['README', 'demo code']) # add a list of files to the corpus
 
-client.query(corpus_id, 'Vectara allows me to search for anything, right?', top_k=5) # query the corpus for top 5 answers
+r = client.query(corpus_id, 'How to set credentials? ', top_k=5) # query the corpus for top 5 answers, return a JSON string 
+print (post_process_query_result(r)) # post process the query result to get a list of answers
+
+r = client.query(corpus_id, 'How to set credentials? ', top_k=5, return_summary=False) # query the corpus for top 5 answers, no summary, just search, return a JSON string
+print (post_process_query_result(r)) # post process the query result to get a list of answers
 
 client.reset_corpus(corpus_id) # delete all documents in the corpus
 ```
 
-### Command line 
-To learn the command line usage, run `vectara --help`. 
+### Command line
+
+To learn the command line usage, run `vectara --help`.
+
+You must set up your Vectara credentials as environment variables before using the command line interface.
 
-You must set up your Vectara credentials as environment variables before using the command line interface. 
-    
 ```bash
 # create a corpus
 vectara create_corpus 'my knowledge base'
 # output: corpus_id = 12
 
 # upload a file to the corpus
 vectara upload 12 one_file.pdf # corpurs_id = 12
@@ -760,18 +784,70 @@
 # query the corpus
 vectara query 12 'Vectara allows me to search for anything, right?' --top_k=5  # corpurs_id = 12
 
 # reset the corpus
 vectara reset_corpus 12 # corpurs_id = 12
 ```
 
-### Beautiful Markdown printout 
+### Web interface via Funix
+
+The SDK can be converted into a web interface via [Funix](http://funix.io). You can drag and drop to add a file to your Vectara corpus.
+
+```python
+pip install funix
+funix src/vectara/__init__.py 
+```
+
+Then you can access the web interface at `http://localhost:3000` (the port number maybe different if port 3000 is occupied).
+
+Below please find the screenshots.
+
+![Initiate Vectara](./screenshots/initiate.png)
+
+![Create a corpus](./screenshots/create_corpus.png)
+
+![Upload a file](./screenshots/upload.gif)
+
+![Query the corpus](./screenshots/query.png)
+
+**Known bugs**: Funix seems to have some memory leakage issues that the web interface may freeze after uploading a file. If that happens, please kill the process and restart the web interface.
+
+### Stylish query results
+
+The query results are typeset Markdown ready to be rendered. A query result includes the following info:
 
+* A summary with citations and matching scores with respect to the query
+* References cited by the summary
 
+```markdown
+### Here is the answer
+To rearrange objects, you can utilize the "direction" attribute in a Funix decorator [1]. Manually resizing and positioning objects can be a tedious and inefficient process [2]. Another approach is to use a collision-free algorithm for auto-layout, where scopes will be resized to fit the objects inside [4]. An example of arranging objects in a column-reverse direction can be seen in the ChatGPT multiturn app [3]. Additionally, organizing your canvas with scopes can help in rearranging objects effectively [5]. Remember to experiment with these methods to find the best arrangement for your specific needs.
+
+### References:
+    
+1. From document **funix.md** (matchness=0.673933):
+  _...You can change their order and orientation using the "direction" attribute in a Funix decorator...._
+
+2. From document **codepod.md** (matchness=0.65305215):
+  _...It is painful and inefficient to resize and position the pods and scopes manually...._
+
+3. From document **funix.md** (matchness=0.6520513):
+  _...The example below shall be self-explaining:
+A more advanced example is our ChatGPT multiturn app where "direction = "column-reverse"" so the message you type stays at the bottom...._
+
+4. From document **codepod.md** (matchness=0.6495899):
+  _...default}alt="Example banner"width="600"/>
+After auto-layout, the pods and scopes are organized by a collision-free algorithm, and the scopes will be resized to fit the pods inside...._
+
+5. From document **codepod.md** (matchness=0.6460015):
+  _...Organize your Canvas with scopes..._
+```
 
 ## Questions
-Contact forrest at vectara dot come 
+
+Contact forrest at vectara dot com
 
 ## Disclaimer
+
 This is an UNofficial SDK and CLI for Vectara's RAG platform.
 Use at your own risk.
 Vectara does NOT provide support for this SDK or CLI.
```

### Comparing `vectara-0.0.1/pyproject.toml` & `vectara-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vectara"
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 authors = [
     { name = "Forrest Sheng Bao", email = "forrest@vectara.com" }
 ]
 license = { file = "LICENSE" }
 description = "An unofficial Python SDK and CLI"
 requires-python = ">=3.10"
```

### Comparing `vectara-0.0.1/src/vectara.egg-info/PKG-INFO` & `vectara-0.0.2/src/vectara.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial Python SDK and CLI
 Author-email: Forrest Sheng Bao <forrest@vectara.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,69 +687,93 @@
 Requires-Dist: textwrap3
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 Requires-Dist: tqdm
 Requires-Dist: IPython
 Requires-Dist: fire
 
-# An UNofficial Python SDK and CLI for Vectara's RAG platform 
+# An UNofficial Python SDK and CLI for Vectara's RAG platform
 
-It supports major features of Vectara's RAG platform for you to build your own search engine. 
+It supports major features of Vectara's RAG platform for you to build your own search engine.
 
-Additional features: 
-* It expands the upload function to allow you to upload a list of files or all files under a directory in one function call. 
-* Renders query results in beautiful Markdown printout.
+Additional features:
+
+* It expands the upload function to allow you to upload a list of files or all files under a directory in one function call.
+* Renders query results in beautiful Markdown printout (see `demo.ipynb`).
+* It supports logging user feedback from the GUI in a local SQLite database for evaluating the quality of search and RAG. 
+
+**If you like this SDK/CLI/GUI, give us a star on Github!**
 
 ## Installation
 
 ```bash
-# pip install from Github
+# Stable
+pip install vectara
+
+# Nightly
 pip install "git+https://github.com/forrestbao/vectara-python-cli.git"
 ```
 
-## Usage 
+## Usage
 
 ### Credentials
 
-You can obtain the Vectara credentials following [this guide](https://docs.vectara.com/docs/learn/authentication/oauth-2). 
-Then set up your Vectara credentials as environment variables. 
+This client supports authentication in both Vectara's [Personal API key](https://docs.vectara.com/docs/console-ui/personal-api-key) and [OAuth2](https://docs.vectara.com/docs/console-ui/app-clients). In either case, you need to obtain [customer ID](https://docs.vectara.com/docs/console-ui/vectara-console-overview#view-the-customer-id) as well. 
+
+Following the convention of OpenAI's client, we recommend setting credentials as environment variables. You can save them as a bash script and simply `source` it before using the SDK or CLI.
 
 ```bash
-export VECTARA_CUSTOMER_ID=123
+export VECTARA_CUSTOMER_ID=123 # Required regardless of the authentication method
+
+# Set API Key if you plan to use Personal API Key to authenticate
+export VECTARA_API_KEY=abc
+
+# Set the following two variables if you plan to use OAuth2 to authenticate
 export VECTARA_CLIENT_ID=abc
 export VECTARA_CLIENT_SECRET=xyz
+
+# If both API key and OAuth2 credentials are set, the SDK will use API key only.
+
+# optional, if you are using a proxy like LlaMasterKey https://github.com/TexteaInc/LlaMasterKey/
+export VECTARA_BASE_URL="http://127.0.0.1:8000/vectara"
+export VECTARA_PROXY_MODE=true # Enable proxy mode
 ```
 
-This unofficial SDK and CLI will read your credentials from the environment variables above. The ability to pass in credentials as arguments is also supported.
+Alternatively, you can pass in your credentials as arguments when initializing the client. See it from the complete code. 
+
+### Using the Python SDK 
 
-### Python 
-Try the Jupyter notebook `demo.ipynb` or read the docstring. 
+Try the Jupyter notebook `demo.ipynb`, the script `demo.py`, or read the docstring.
 
 ```python
-from vectara import vectara
+from vectara import vectara, post_process_query_result
 
-client = vectara() # get default credentials from environment variables 
-                   # You can also manually pass in your credentials as arguments
+client = vectara() # get credentials from environment variables 
 
 corpus_id = client.create_corpus('my knowledge base')
 
-client.upload(corpus_id, 'one_file.pdf', description='My precious doc')  # add one file to the corpus 
+client.upload(corpus_id, 'one_file.pdf', description='A scientific paper')  # add one file to the corpus 
 client.upload(corpus_id, 'a_folder_of_documents') # add all files under a folder to the corpus
-client.upload(corpus_id, ['user_manual.md', 'notes.txt'], description=['user manual', 'my memory']) # add a list of files to the corpus
+client.upload(corpus_id, ['README.md', 'demo.py'], description=['README', 'demo code']) # add a list of files to the corpus
 
-client.query(corpus_id, 'Vectara allows me to search for anything, right?', top_k=5) # query the corpus for top 5 answers
+r = client.query(corpus_id, 'How to set credentials? ', top_k=5) # query the corpus for top 5 answers, return a JSON string 
+print (post_process_query_result(r)) # post process the query result to get a list of answers
+
+r = client.query(corpus_id, 'How to set credentials? ', top_k=5, return_summary=False) # query the corpus for top 5 answers, no summary, just search, return a JSON string
+print (post_process_query_result(r)) # post process the query result to get a list of answers
 
 client.reset_corpus(corpus_id) # delete all documents in the corpus
 ```
 
-### Command line 
-To learn the command line usage, run `vectara --help`. 
+### Command line
+
+To learn the command line usage, run `vectara --help`.
+
+You must set up your Vectara credentials as environment variables before using the command line interface.
 
-You must set up your Vectara credentials as environment variables before using the command line interface. 
-    
 ```bash
 # create a corpus
 vectara create_corpus 'my knowledge base'
 # output: corpus_id = 12
 
 # upload a file to the corpus
 vectara upload 12 one_file.pdf # corpurs_id = 12
@@ -760,18 +784,70 @@
 # query the corpus
 vectara query 12 'Vectara allows me to search for anything, right?' --top_k=5  # corpurs_id = 12
 
 # reset the corpus
 vectara reset_corpus 12 # corpurs_id = 12
 ```
 
-### Beautiful Markdown printout 
+### Web interface via Funix
+
+The SDK can be converted into a web interface via [Funix](http://funix.io). You can drag and drop to add a file to your Vectara corpus.
+
+```python
+pip install funix
+funix src/vectara/__init__.py 
+```
+
+Then you can access the web interface at `http://localhost:3000` (the port number maybe different if port 3000 is occupied).
+
+Below please find the screenshots.
+
+![Initiate Vectara](./screenshots/initiate.png)
+
+![Create a corpus](./screenshots/create_corpus.png)
+
+![Upload a file](./screenshots/upload.gif)
+
+![Query the corpus](./screenshots/query.png)
+
+**Known bugs**: Funix seems to have some memory leakage issues that the web interface may freeze after uploading a file. If that happens, please kill the process and restart the web interface.
+
+### Stylish query results
+
+The query results are typeset Markdown ready to be rendered. A query result includes the following info:
 
+* A summary with citations and matching scores with respect to the query
+* References cited by the summary
 
+```markdown
+### Here is the answer
+To rearrange objects, you can utilize the "direction" attribute in a Funix decorator [1]. Manually resizing and positioning objects can be a tedious and inefficient process [2]. Another approach is to use a collision-free algorithm for auto-layout, where scopes will be resized to fit the objects inside [4]. An example of arranging objects in a column-reverse direction can be seen in the ChatGPT multiturn app [3]. Additionally, organizing your canvas with scopes can help in rearranging objects effectively [5]. Remember to experiment with these methods to find the best arrangement for your specific needs.
+
+### References:
+    
+1. From document **funix.md** (matchness=0.673933):
+  _...You can change their order and orientation using the "direction" attribute in a Funix decorator...._
+
+2. From document **codepod.md** (matchness=0.65305215):
+  _...It is painful and inefficient to resize and position the pods and scopes manually...._
+
+3. From document **funix.md** (matchness=0.6520513):
+  _...The example below shall be self-explaining:
+A more advanced example is our ChatGPT multiturn app where "direction = "column-reverse"" so the message you type stays at the bottom...._
+
+4. From document **codepod.md** (matchness=0.6495899):
+  _...default}alt="Example banner"width="600"/>
+After auto-layout, the pods and scopes are organized by a collision-free algorithm, and the scopes will be resized to fit the pods inside...._
+
+5. From document **codepod.md** (matchness=0.6460015):
+  _...Organize your Canvas with scopes..._
+```
 
 ## Questions
-Contact forrest at vectara dot come 
+
+Contact forrest at vectara dot com
 
 ## Disclaimer
+
 This is an UNofficial SDK and CLI for Vectara's RAG platform.
 Use at your own risk.
 Vectara does NOT provide support for this SDK or CLI.
```

