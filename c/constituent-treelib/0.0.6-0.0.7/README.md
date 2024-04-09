# Comparing `tmp/constituent_treelib-0.0.6.tar.gz` & `tmp/constituent_treelib-0.0.7.tar.gz`

## Comparing `constituent_treelib-0.0.6.tar` & `constituent_treelib-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/CITATION.cff
--rw-r--r--   0        0        0    88631 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/Constituent_TreeLib_Quickstart.ipynb
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/pytest.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/requirements.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/__init__.py
--rw-r--r--   0        0        0    46339 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/core.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/errors.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/export.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/lang_models/__init__.py
--rw-r--r--   0        0        0   938013 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/constituent_treelib/lang_models/lid.176.ftz
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/tests/test_ctl_core.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/LICENSE
--rw-r--r--   0        0        0    16886 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/README.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 constituent_treelib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/CITATION.cff
+-rw-r--r--   0        0        0    88631 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/Constituent_TreeLib_Quickstart.ipynb
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/Dockerfile
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/ctl_app.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/constituent_treelib/__init__.py
+-rw-r--r--   0        0        0    45996 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/constituent_treelib/core.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/constituent_treelib/errors.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/constituent_treelib/export.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/tests/test_ctl_core.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/LICENSE
+-rw-r--r--   0        0        0    16886 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/README.md
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    18099 2020-02-02 00:00:00.000000 constituent_treelib-0.0.7/PKG-INFO
```

### Comparing `constituent_treelib-0.0.6/Constituent_TreeLib_Quickstart.ipynb` & `constituent_treelib-0.0.7/Constituent_TreeLib_Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `constituent_treelib-0.0.6/constituent_treelib/core.py` & `constituent_treelib-0.0.7/constituent_treelib/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import re
 import sys
 import nltk
 import spacy
 import benepar
 import huspacy
-import fasttext
 import contractions
 from nltk import Tree
 from pathlib import Path
 import importlib.resources
 from enum import Enum, auto
-from fasttext import FastText
+from langid.langid import LanguageIdentifier, model
 from typing import List, Dict, Set, Union, Generator
 
 # Package imports
-from . import lang_models
 from .errors import *
 from .export import export_figure
 
 
 class Structure(Enum):
     Complete = auto()
     WithoutTokenLeaves = auto()
@@ -267,14 +265,17 @@
             nlp parameter.
         """
 
         if sentence is None or isinstance(sentence, str) and len(sentence.strip()) == 0:
             raise SentenceError("The given sentence is either none or empty. Please provide a valid sentence in order "
                                 "to instantiate a ConstituentTree object.")
 
+        # Load the language detector model. 
+        self.lang_det = LanguageIdentifier.from_modelstring(model, norm_probs=True)        
+        
         # Detect the language of the given sentence in order to load the correct spaCy and benepar models.
         detected_language = Language.Unsupported
 
         if isinstance(sentence, str):
             detected_language = self.detect_language(sentence)
         elif isinstance(sentence, BracketedTree):
             extracted_sentence = " ".join(sentence.nltk_tree.leaves())
@@ -381,54 +382,47 @@
         # The given sentence is neither a string nor a valid nltk.Tree or a BracketedTree object.
         # Therefore, we cannot further proceed.
         else:
             raise SentenceError(f"To instantiate a ConstituentTree object, a non-empty sentence object "
                                 f"(a string, an nltk.Tree or a BracketedTree) must be provided. Type of the "
                                 f"given sentence: {type(sentence).__name__}.")
 
-    def detect_language(self, text: str, append_proba: bool = False, round_precision: int = 3, top_k_matches: int = 1,
-                        model: FastText._FastText = None):
-        """Detects the language of the given text using FastText.
+    
+    def detect_language(self, text: str, append_proba: bool = False, round_precision: int = 3, top_k_matches: int = 1):
+        """Detects the language of the given text using the pythob lib langid.
 
         Args:
             text: The text whose language is to be detected.
 
             append_proba: The probability regarding the detected language.
 
             round_precision: The accuracy of the probability to be rounded.
 
             top_k_matches: Number of k most likely detected languages. By default (k=1), the language with the
             highest detection probability is returned.
 
-            model: The desired language detection model.
-
         Returns:
-              The language of the given text (optionally, the top-k detected languages and the detection probability).
-        """
-        # Suppress FastText's annoying deprecation warning.
-        FastText.eprint = lambda x: None
-
-        # Load the default compressed model if no other model is provided. The none-compressed model can be
-        # downloaded from: https://fasttext.cc/docs/en/language-identification.html
-        # A performance comparison of the two models can be found at  https://fasttext.cc/blog/2017/10/02/blog-post.html
-        if not model:
-            with importlib.resources.path(lang_models, "lid.176.ftz") as resource:
-                model = fasttext.load_model(str(resource))
-
+            The language of the given text (optionally, the top-k detected languages and the detection probability).
+        """ 
+        
+        predictions = self.lang_det.rank(text)
+        
+        if top_k_matches > len(predictions):
+            raise ValueError(f"The given 'top_k_matches' exceeds the number of langid's known languages. "
+                            "Consider: top_k_matches < {len(predictions)}.")        
+        
+        predictions = predictions[0:top_k_matches]
         result = []
-        predictions = model.predict([text], k=top_k_matches)
-        predictions = list(zip(*predictions[0], *predictions[1]))
 
         for lang, proba in predictions:
-            lang = lang.replace('__label__', '')
             lang = self.lang_dict[lang] if lang in self.lang_dict else Language.Unsupported
             proba = round(proba, round_precision)
             result.append((lang, proba)) if append_proba else result.append(lang)
-        return result[0] if top_k_matches == 1 else result
-
+        return result[0] if top_k_matches == 1 else result    
+    
     def detect_spacy_langauge(self, nlp: spacy.Language = None):
         """ Translates the language identifier of the internal spaCy pipeline into a corresponding
         ConstituentTreelib.Langauge object.
 
         Returns:
             A ConstituentTreelib.Langauge object that represents the language of the spaCy pipeline.
         """
@@ -717,15 +711,15 @@
 
         phrases = []
         if tree.label() == phrasal_category:
             phrases.append(tree.copy(True))
 
         for child in tree:
             if isinstance(child, Tree):
-                temp = self._extract_phrases(child, phrasal_category)
+                temp = self._extract_phrases(child, phrasal_category, min_words_in_phrases)
                 if len(temp) > 0:
                     phrases.extend(temp)
 
         if min_words_in_phrases >= 2:
             return [p for p in phrases if len(p) >= min_words_in_phrases]
         else:
             return [p for p in phrases]
```

### Comparing `constituent_treelib-0.0.6/constituent_treelib/errors.py` & `constituent_treelib-0.0.7/constituent_treelib/errors.py`

 * *Files identical despite different names*

### Comparing `constituent_treelib-0.0.6/constituent_treelib/export.py` & `constituent_treelib-0.0.7/constituent_treelib/export.py`

 * *Files identical despite different names*

### Comparing `constituent_treelib-0.0.6/tests/test_ctl_core.py` & `constituent_treelib-0.0.7/tests/test_ctl_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,22 +75,14 @@
             ConstituentTree(sentence, nlp="")
 
     def test_error_nlp_pipeline_without_benepar_component(self):
         with pytest.raises(NLPPipelineError):
             sentence = "I will not instantiate a ConstituentTree object with an invalid nlp pipeline ever again."
             ConstituentTree(sentence, nlp=self.defect_nlp)
 
-    def test_error_nlp_pipeline_models_language_mismatch(self):
-        benepar_model = "benepar_fr2"
-        self.defect_nlp.add_pipe("benepar", config={"model": benepar_model})
-
-        with pytest.raises(LanguageError):
-            sentence = "I will not instantiate a ConstituentTree object with an invalid nlp pipeline ever again."
-            ConstituentTree(sentence, nlp=self.defect_nlp)
-
     def test_error_nlp_pipeline_models_sentence_language_mismatch(self):
         with pytest.raises(LanguageError):
             sentence = "Huch, das war jetzt nicht gewollt."
             ConstituentTree(sentence, nlp=self.nlp)
 
     def test_spacy_pos_tagging(self):
         doc = self.nlp("Today was a good day!")
@@ -166,9 +158,9 @@
 
     def test_svg_export(self):
         file_name = "tree.svg"
         sentence = "Python is an awesome coding language!"
         ConstituentTree(sentence, self.nlp).export_tree(file_name)
         with open(file_name, "rb") as file:
             md5_hash = hashlib.md5(file.read()).hexdigest()
-        assert md5_hash == "75cdbbeda69e84df53b6d07428e54244"
+        assert md5_hash == "d3e9fdbe78fee450f212d605584f3b2a"
         os.remove(file_name)
```

### Comparing `constituent_treelib-0.0.6/LICENSE` & `constituent_treelib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `constituent_treelib-0.0.6/README.md` & `constituent_treelib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `constituent_treelib-0.0.6/PKG-INFO` & `constituent_treelib-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: constituent_treelib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A lightweight Python library for constructing, processing, and visualizing constituent trees.
 Project-URL: Homepage, https://github.com/Halvani/constituent-treelib
 Project-URL: Bug Tracker, https://github.com/Halvani/constituent-treelib/issues
 Author: Oren Halvani
 License-File: LICENSE
 Keywords: constituency-parser,constituency-tree,export-to-pdf,export-to-png,export-to-svg,phrase-extraction,visualization
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Requires-Dist: benepar
 Requires-Dist: contractions
-Requires-Dist: fasttext
 Requires-Dist: huspacy
 Requires-Dist: ipython
+Requires-Dist: langid
 Requires-Dist: nltk
 Requires-Dist: pdfkit
 Requires-Dist: protobuf==3.20.3
 Requires-Dist: pytest
 Requires-Dist: spacy
 Requires-Dist: streamlit
 Requires-Dist: svgling
```

#### html2text {}

```diff
@@ -1,37 +1,43 @@
-Metadata-Version: 2.1 Name: constituent_treelib Version: 0.0.6 Summary: A
+Metadata-Version: 2.3 Name: constituent_treelib Version: 0.0.7 Summary: A
 lightweight Python library for constructing, processing, and visualizing
 constituent trees. Project-URL: Homepage, https://github.com/Halvani/
 constituent-treelib Project-URL: Bug Tracker, https://github.com/Halvani/
 constituent-treelib/issues Author: Oren Halvani License-File: LICENSE Keywords:
 constituency-parser,constituency-tree,export-to-pdf,export-to-png,export-to-
-svg,phrase-extraction,visualization Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: benepar Requires-
-Dist: contractions Requires-Dist: fasttext Requires-Dist: huspacy Requires-
-Dist: ipython Requires-Dist: nltk Requires-Dist: pdfkit Requires-Dist:
-protobuf==3.20.3 Requires-Dist: pytest Requires-Dist: spacy Requires-Dist:
-streamlit Requires-Dist: svgling Requires-Dist: tokenizers Requires-Dist: torch
-Requires-Dist: transformers[torch] Requires-Dist: wand Description-Content-
-Type: text/markdown # Constituent Treelib (CTL) A lightweight Python library
-for constructing, processing, and visualizing constituent trees. [![DOI](https:
-//zenodo.org/badge/DOI/10.5281/zenodo.7765147.svg)](https://doi.org/10.5281/
-zenodo.7765147) # Description CTL is a lightweight Python library that offers
-you a convenient way to parse sentences into _c_o_n_s_t_i_t_u_e_n_t_ _t_r_e_e_s, modify them
-according to their structure, as well as visualize and export them into various
-[file formats](#Export_visualization). In addition, you can extract phrases
-according to their phrasal categories (which can be used e.g., as features for
-various NLP tasks), validate already parsed sentences in bracket notation or
-convert them back into sentences. CTL is built on top of _*_*_b_e_n_e_p_a_r_*_* (*Berkeley
-Neural Parser*) as well as the two well-known NLP frameworks _*_*_s_p_a_C_y_*_* and
-_*_*_N_L_T_K_*_*. Here, spaCy is used for tokenization and sentence segmentation, while
-benepar performs the actual parsing of the sentences. NLTK, on the other hand,
-provides the fundamental data structure for storing and processing the parsed
-sentences. To gain a clearer picture of what a constituent tree looks like, we
-consider the following example. Let *S* denote the sentence...
+svg,phrase-extraction,visualization Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Python: >=3.6 Requires-Dist: benepar Requires-Dist: contractions Requires-Dist:
+huspacy Requires-Dist: ipython Requires-Dist: langid Requires-Dist: nltk
+Requires-Dist: pdfkit Requires-Dist: protobuf==3.20.3 Requires-Dist: pytest
+Requires-Dist: spacy Requires-Dist: streamlit Requires-Dist: svgling Requires-
+Dist: tokenizers Requires-Dist: torch Requires-Dist: transformers[torch]
+Requires-Dist: wand Description-Content-Type: text/markdown # Constituent
+Treelib (CTL) A lightweight Python library for constructing, processing, and
+visualizing constituent trees. [![DOI](https://zenodo.org/badge/DOI/10.5281/
+zenodo.7765147.svg)](https://doi.org/10.5281/zenodo.7765147) # Description CTL
+is a lightweight Python library that offers you a convenient way to parse
+sentences into _c_o_n_s_t_i_t_u_e_n_t_ _t_r_e_e_s, modify them according to their structure, as
+well as visualize and export them into various [file formats]
+(#Export_visualization). In addition, you can extract phrases according to
+their phrasal categories (which can be used e.g., as features for various NLP
+tasks), validate already parsed sentences in bracket notation or convert them
+back into sentences. CTL is built on top of _*_*_b_e_n_e_p_a_r_*_* (*Berkeley Neural
+Parser*) as well as the two well-known NLP frameworks _*_*_s_p_a_C_y_*_* and _*_*_N_L_T_K_*_*.
+Here, spaCy is used for tokenization and sentence segmentation, while benepar
+performs the actual parsing of the sentences. NLTK, on the other hand, provides
+the fundamental data structure for storing and processing the parsed sentences.
+To gain a clearer picture of what a constituent tree looks like, we consider
+the following example. Let *S* denote the sentence...
 ``` "Isaac Asimov was an American writer and professor of biochemistry at
 Boston University." ``` This sentence can be parsed into a bracketed tree
 string representation (shown below in a _*_P_e_n_n_ _t_r_e_e_-_b_a_n_k_* style) ``` (S (NP (NNP
 Isaac) (NNP Asimov)) (VP (VBD was) (NP (NP (DT an) (JJ American) (NN writer)
 (CC and) (NN professor)) (PP (IN of) (NP (NN biochemistry))) (PP (IN at) (NP
 (NNP Boston) (NNP University))))) (. .)) ``` which represents the actual
 constituent tree. However, since this notation is not really easy to read, we
```

