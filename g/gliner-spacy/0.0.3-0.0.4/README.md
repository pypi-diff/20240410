# Comparing `tmp/gliner-spacy-0.0.3.tar.gz` & `tmp/gliner-spacy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.3.tar", last modified: Mon Apr  8 09:17:58 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.4.tar", last modified: Wed Apr 10 04:18:08 2024, max compression
```

## Comparing `gliner-spacy-0.0.3.tar` & `gliner-spacy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.054637 gliner-spacy-0.0.3/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3221 2024-04-08 09:17:58.054519 gliner-spacy-0.0.3/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2540 2024-04-03 12:39:06.000000 gliner-spacy-0.0.3/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.053727 gliner-spacy-0.0.3/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.3/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2943 2024-04-08 09:15:55.000000 gliner-spacy-0.0.3/gliner_spacy/pipeline.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-08 09:17:58.054344 gliner-spacy-0.0.3/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3221 2024-04-08 09:17:57.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      247 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-08 09:17:58.000000 gliner-spacy-0.0.3/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-08 09:17:58.054689 gliner-spacy-0.0.3/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1271 2024-04-08 09:17:56.000000 gliner-spacy-0.0.3/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.146466 gliner-spacy-0.0.4/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.4/LICENSE
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-10 04:18:08.146341 gliner-spacy-0.0.4/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2651 2024-04-08 09:20:31.000000 gliner-spacy-0.0.4/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.145480 gliner-spacy-0.0.4/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.4/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2943 2024-04-08 09:15:55.000000 gliner-spacy-0.0.4/gliner_spacy/pipeline.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.146160 gliner-spacy-0.0.4/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      255 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-10 04:18:08.146509 gliner-spacy-0.0.4/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1278 2024-04-10 04:17:44.000000 gliner-spacy-0.0.4/setup.py
```

### Comparing `gliner-spacy-0.0.3/PKG-INFO` & `gliner-spacy-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # GLiNER SpaCy Wrapper
 
 ## Introduction
 This project is a wrapper for integrating [GLiNER](https://github.com/urchade/GLiNER), a Named Entity Recognition (NER) model, with the SpaCy Natural Language Processing (NLP) library. GLiNER, which stands for Generalized Language INdependent Entity Recognition, is an advanced model for recognizing entities in text. The SpaCy wrapper enables easy integration and use of GLiNER within the SpaCy environment, enhancing NER capabilities with GLiNER's advanced features.
 
 ## Features
@@ -85,10 +86,11 @@
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
+- `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.3/README.md` & `gliner-spacy-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -68,10 +68,11 @@
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
+- `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
 
 ## Contributing
-Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
+Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.3/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.4/gliner_spacy/pipeline.py`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.3/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.4/gliner_spacy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # GLiNER SpaCy Wrapper
 
 ## Introduction
 This project is a wrapper for integrating [GLiNER](https://github.com/urchade/GLiNER), a Named Entity Recognition (NER) model, with the SpaCy Natural Language Processing (NLP) library. GLiNER, which stands for Generalized Language INdependent Entity Recognition, is an advanced model for recognizing entities in text. The SpaCy wrapper enables easy integration and use of GLiNER within the SpaCy environment, enhancing NER capabilities with GLiNER's advanced features.
 
 ## Features
@@ -85,10 +86,11 @@
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
+- `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.3/setup.py` & `gliner-spacy-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of your README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gliner-spacy',  # Your package name
-    version='0.0.3',  # Initial version
+    version='0.0.4',  # Initial version
     author='William J. B. Mattingly',  # Your name
     description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Ensures correct rendering on PyPI
     url='https://github.com/theirstory/gliner-spacy',  # Your repository URL
     packages=find_packages(),
     install_requires=[
@@ -24,9 +24,9 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.7,<=3.10',
 )
```

