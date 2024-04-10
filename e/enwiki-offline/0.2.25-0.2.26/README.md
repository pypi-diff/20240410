# Comparing `tmp/enwiki_offline-0.2.25.tar.gz` & `tmp/enwiki_offline-0.2.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enwiki_offline-0.2.25.tar", max compression
+gzip compressed data, was "enwiki_offline-0.2.26.tar", max compression
```

## Comparing `enwiki_offline-0.2.25.tar` & `enwiki_offline-0.2.26.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2131 2024-04-09 22:17:45.819640 enwiki_offline-0.2.25/README.md
--rw-r--r--   0        0        0       49 2024-04-09 22:17:45.819640 enwiki_offline-0.2.25/enwiki_offline/__init__.py
--rw-r--r--   0        0        0     5507 2024-04-09 22:17:45.819640 enwiki_offline-0.2.25/enwiki_offline/enwiki_offline_api.py
--rw-r--r--   0        0        0     1188 2024-04-09 22:17:45.819640 enwiki_offline-0.2.25/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 enwiki_offline-0.2.25/setup.py
--rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 enwiki_offline-0.2.25/PKG-INFO
+-rw-r--r--   0        0        0     2870 2024-04-09 22:27:25.383888 enwiki_offline-0.2.26/README.md
+-rw-r--r--   0        0        0       49 2024-04-09 22:27:25.383888 enwiki_offline-0.2.26/enwiki_offline/__init__.py
+-rw-r--r--   0        0        0     5507 2024-04-09 22:27:25.383888 enwiki_offline-0.2.26/enwiki_offline/enwiki_offline_api.py
+-rw-r--r--   0        0        0     1188 2024-04-09 22:27:25.383888 enwiki_offline-0.2.26/pyproject.toml
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 enwiki_offline-0.2.26/setup.py
+-rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 enwiki_offline-0.2.26/PKG-INFO
```

### Comparing `enwiki_offline-0.2.25/README.md` & `enwiki_offline-0.2.26/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 # enwiki-offline
+High-performance offline access to Wikipedia data.
+
+These functions are helpful and essential for Linked Data / NLP applications that need to determine if a given entity has a corresponding Wikipedia entry.
+
+Knowing if an entity exists in Wikipedia (and what the ISO URL is) helps differentiate known (public) entities from entities unique to a data source.  Existential lookups can be helpful in either eliminating noise or boosting differentiating entities.
+
+Runtime access to this package does not require remote calls to DBpedia, Wikipedia, or other Linked data providers.  Offline access is stable and offers consistent performance with a disk-io tradeoff.  Slightly over 17,000 localized files are required to enable offline access.
 
 ## Functions
 ```python
 def exists(entity: str) -> bool
 ```
 Performs a case insensitive search and returns True if a Wikipedia entry exists for the input entity.  Synonyms, Partial and Fuzzy searches are not supported.  Exact matches only.
```

### Comparing `enwiki_offline-0.2.25/enwiki_offline/enwiki_offline_api.py` & `enwiki_offline-0.2.26/enwiki_offline/enwiki_offline_api.py`

 * *Files identical despite different names*

### Comparing `enwiki_offline-0.2.25/pyproject.toml` & `enwiki_offline-0.2.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 maintainers = ["Craig Trim <craigtrim@gmail.com>"]
 
 description = "Offline Access to Enwiki Entities"
 license = "MIT"
 name = "enwiki-offline"
 readme = "README.md"
-version = "0.2.25"
+version = "0.2.26"
 
 keywords = ["utility", "helper", "text", "matching"]
 repository = "https://github.com/craigtrim/enwiki-offline"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `enwiki_offline-0.2.25/setup.py` & `enwiki_offline-0.2.26/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'dvc']
 
 setup_kwargs = {
     'name': 'enwiki-offline',
-    'version': '0.2.25',
+    'version': '0.2.26',
     'description': 'Offline Access to Enwiki Entities',
-    'long_description': '# enwiki-offline\n\n## Functions\n```python\ndef exists(entity: str) -> bool\n```\nPerforms a case insensitive search and returns True if a Wikipedia entry exists for the input entity.  Synonyms, Partial and Fuzzy searches are not supported.  Exact matches only.\n\n```python\ndef is_ambiguous(entity: str) -> bool\n```\nReturns True if multiple Wikipedia entries exist for this term.\n\n```python\ndef titles(entity: str) -> Optional[List[str]]\n```\nReturns all Wikipedia Titles for this input entity.\n\n## Use Existing Data\nScroll down to the `DVC` section and use the `dvc pull` command to access the data.\n\n## Parsing Wikipedia Titles\nThe latest enwiki file can be downloaded from https://dumps.wikimedia.org/enwiki/\n\nYou only need to do this if\n1. You don\'t want to refresh from DVC\n2. You have a different version of the enwiki file\n```sh\npoetry run python drivers/parse_enwiki_all_titles.py "/path/to/file/enwiki-20240301-all-titles"\n```\n\n## DVC (Data Version Control)\n\n### Initialize DVC and Configure S3 Remote\nIn your project root, initialize DVC if you haven\'t already, and configure your S3 bucket as the remote storage. Replace `enwikioffline` with your actual S3 bucket name if it\'s different. Run:\n\n```shell\ndvc init\ndvc remote add -d myremote s3://enwikioffline\ndvc remote modify myremote profile enwiki_offline\n```\n\nThis setup:\n- Initializes DVC in your project.\n- Adds your S3 bucket as the default remote storage.\n- Configures DVC to use the `enwiki_offline` AWS profile for S3 operations.\n\n### Track and Push Data with DVC\nTo track the resources folder and push it to S3, execute:\n```shell\ndvc add resources\ngit add resources.dvc .gitignore\ngit commit -m "Track resources folder with DVC"\ndvc push\n```\n\nThis process:\n- Tracks the `resources` folder with DVC, creating a .dvc file.\n- Commits the DVC files to Git.\n- Pushes the data to your S3 bucket using the configured AWS profile.\n\n### Pull Data with DVC\nTo retrieve the data managed by DVC, use:\n```sh\ndvc pull\n```\nThis command pulls the data from S3 into your local `resources` folder, based on the current DVC setup and the latest `resources.dvc` file in your repository.\n',
+    'long_description': '# enwiki-offline\nHigh-performance offline access to Wikipedia data.\n\nThese functions are helpful and essential for Linked Data / NLP applications that need to determine if a given entity has a corresponding Wikipedia entry.\n\nKnowing if an entity exists in Wikipedia (and what the ISO URL is) helps differentiate known (public) entities from entities unique to a data source.  Existential lookups can be helpful in either eliminating noise or boosting differentiating entities.\n\nRuntime access to this package does not require remote calls to DBpedia, Wikipedia, or other Linked data providers.  Offline access is stable and offers consistent performance with a disk-io tradeoff.  Slightly over 17,000 localized files are required to enable offline access.\n\n## Functions\n```python\ndef exists(entity: str) -> bool\n```\nPerforms a case insensitive search and returns True if a Wikipedia entry exists for the input entity.  Synonyms, Partial and Fuzzy searches are not supported.  Exact matches only.\n\n```python\ndef is_ambiguous(entity: str) -> bool\n```\nReturns True if multiple Wikipedia entries exist for this term.\n\n```python\ndef titles(entity: str) -> Optional[List[str]]\n```\nReturns all Wikipedia Titles for this input entity.\n\n## Use Existing Data\nScroll down to the `DVC` section and use the `dvc pull` command to access the data.\n\n## Parsing Wikipedia Titles\nThe latest enwiki file can be downloaded from https://dumps.wikimedia.org/enwiki/\n\nYou only need to do this if\n1. You don\'t want to refresh from DVC\n2. You have a different version of the enwiki file\n```sh\npoetry run python drivers/parse_enwiki_all_titles.py "/path/to/file/enwiki-20240301-all-titles"\n```\n\n## DVC (Data Version Control)\n\n### Initialize DVC and Configure S3 Remote\nIn your project root, initialize DVC if you haven\'t already, and configure your S3 bucket as the remote storage. Replace `enwikioffline` with your actual S3 bucket name if it\'s different. Run:\n\n```shell\ndvc init\ndvc remote add -d myremote s3://enwikioffline\ndvc remote modify myremote profile enwiki_offline\n```\n\nThis setup:\n- Initializes DVC in your project.\n- Adds your S3 bucket as the default remote storage.\n- Configures DVC to use the `enwiki_offline` AWS profile for S3 operations.\n\n### Track and Push Data with DVC\nTo track the resources folder and push it to S3, execute:\n```shell\ndvc add resources\ngit add resources.dvc .gitignore\ngit commit -m "Track resources folder with DVC"\ndvc push\n```\n\nThis process:\n- Tracks the `resources` folder with DVC, creating a .dvc file.\n- Commits the DVC files to Git.\n- Pushes the data to your S3 bucket using the configured AWS profile.\n\n### Pull Data with DVC\nTo retrieve the data managed by DVC, use:\n```sh\ndvc pull\n```\nThis command pulls the data from S3 into your local `resources` folder, based on the current DVC setup and the latest `resources.dvc` file in your repository.\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/enwiki-offline',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `enwiki_offline-0.2.25/PKG-INFO` & `enwiki_offline-0.2.26/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enwiki-offline
-Version: 0.2.25
+Version: 0.2.26
 Summary: Offline Access to Enwiki Entities
 Home-page: https://github.com/craigtrim/enwiki-offline
 License: MIT
 Keywords: utility,helper,text,matching
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
@@ -17,14 +17,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: baseblock
 Requires-Dist: dvc
 Project-URL: Repository, https://github.com/craigtrim/enwiki-offline
 Description-Content-Type: text/markdown
 
 # enwiki-offline
+High-performance offline access to Wikipedia data.
+
+These functions are helpful and essential for Linked Data / NLP applications that need to determine if a given entity has a corresponding Wikipedia entry.
+
+Knowing if an entity exists in Wikipedia (and what the ISO URL is) helps differentiate known (public) entities from entities unique to a data source.  Existential lookups can be helpful in either eliminating noise or boosting differentiating entities.
+
+Runtime access to this package does not require remote calls to DBpedia, Wikipedia, or other Linked data providers.  Offline access is stable and offers consistent performance with a disk-io tradeoff.  Slightly over 17,000 localized files are required to enable offline access.
 
 ## Functions
 ```python
 def exists(entity: str) -> bool
 ```
 Performs a case insensitive search and returns True if a Wikipedia entry exists for the input entity.  Synonyms, Partial and Fuzzy searches are not supported.  Exact matches only.
```

