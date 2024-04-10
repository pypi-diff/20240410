# Comparing `tmp/diarium-cli-0.2.3.tar.gz` & `tmp/diarium-cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diarium-cli-0.2.3.tar", last modified: Mon Mar  7 20:20:36 2022, max compression
+gzip compressed data, was "diarium-cli-0.2.4.tar", last modified: Wed Apr 10 14:39:56 2024, max compression
```

## Comparing `diarium-cli-0.2.3.tar` & `diarium-cli-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-03-07 20:20:36.465976 diarium-cli-0.2.3/
--rw-rw-rw-   0        0        0    11558 2022-02-06 14:36:26.000000 diarium-cli-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      597 2022-03-07 20:20:36.465976 diarium-cli-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-02-06 15:12:32.000000 diarium-cli-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2022-03-07 20:20:36.437977 diarium-cli-0.2.3/diarium_cli/
--rw-rw-rw-   0        0        0        0 2022-02-07 01:02:14.000000 diarium-cli-0.2.3/diarium_cli/__init__.py
--rw-rw-rw-   0        0        0  4234901 2022-02-07 01:03:39.000000 diarium-cli-0.2.3/diarium_cli/english_words.txt
--rw-rw-rw-   0        0        0     2690 2022-03-07 20:15:19.000000 diarium-cli-0.2.3/diarium_cli/finder.py
--rw-rw-rw-   0        0        0      760 2022-02-07 01:03:38.000000 diarium-cli-0.2.3/diarium_cli/helper.py
--rw-rw-rw-   0        0        0     6063 2022-03-06 02:21:12.000000 diarium-cli-0.2.3/diarium_cli/journal.py
--rw-rw-rw-   0        0        0     2959 2022-03-06 02:23:48.000000 diarium-cli-0.2.3/diarium_cli/main.py
--rw-rw-rw-   0        0        0   869496 2022-02-07 19:08:11.000000 diarium-cli-0.2.3/diarium_cli/slovak_words.txt
-drwxrwxrwx   0        0        0        0 2022-03-07 20:20:36.464978 diarium-cli-0.2.3/diarium_cli.egg-info/
--rw-rw-rw-   0        0        0      597 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-03-07 20:20:36.000000 diarium-cli-0.2.3/diarium_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-06 16:21:29.000000 diarium-cli-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      646 2022-03-07 20:20:36.467977 diarium-cli-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 14:39:56.899879 diarium-cli-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2022-02-06 14:36:26.000000 diarium-cli-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      694 2024-04-10 14:39:56.898879 diarium-cli-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2022-02-06 15:12:32.000000 diarium-cli-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:39:56.878336 diarium-cli-0.2.4/diarium_cli/
+-rw-rw-rw-   0        0        0        0 2022-02-07 01:02:14.000000 diarium-cli-0.2.4/diarium_cli/__init__.py
+-rw-rw-rw-   0        0        0  4234901 2022-02-07 01:03:39.000000 diarium-cli-0.2.4/diarium_cli/english_words.txt
+-rw-rw-rw-   0        0        0     2819 2024-04-10 14:38:42.000000 diarium-cli-0.2.4/diarium_cli/finder.py
+-rw-rw-rw-   0        0        0      760 2022-02-07 01:03:38.000000 diarium-cli-0.2.4/diarium_cli/helper.py
+-rw-rw-rw-   0        0        0     6063 2022-03-06 02:21:12.000000 diarium-cli-0.2.4/diarium_cli/journal.py
+-rw-rw-rw-   0        0        0     2959 2022-03-06 02:23:48.000000 diarium-cli-0.2.4/diarium_cli/main.py
+-rw-rw-rw-   0        0        0   869496 2022-02-07 19:08:11.000000 diarium-cli-0.2.4/diarium_cli/slovak_words.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:39:56.898879 diarium-cli-0.2.4/diarium_cli.egg-info/
+-rw-rw-rw-   0        0        0      694 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 14:39:56.000000 diarium-cli-0.2.4/diarium_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-06 16:21:29.000000 diarium-cli-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      653 2024-04-10 14:39:56.900880 diarium-cli-0.2.4/setup.cfg
```

### Comparing `diarium-cli-0.2.3/LICENSE` & `diarium-cli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/diarium_cli/english_words.txt` & `diarium-cli-0.2.4/diarium_cli/english_words.txt`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/diarium_cli/finder.py` & `diarium-cli-0.2.4/diarium_cli/finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from io import StringIO
 from rich.progress import track
-from nltk.tokenize import sent_tokenize
+import nltk
 
 
 class Finder:
 
     def __init__(self, entries: dict[str, str]) -> None:
         self.entries = entries
         self.occurrences = 0
         self.exact_match = False
+        try:
+            _ = nltk.data.find('tokenizers/punkt.zip')
+        except LookupError:
+            nltk.download('punkt')
 
     def find_and_get_output(self, word: str, exact_match: bool) -> tuple[str, int]:
         return self._find(word, exact_match), self.occurrences
 
     def find_and_get_occurrences(self, word: str, exact_match: bool) -> int:
         self._find(word, exact_match)
         return self.occurrences
@@ -25,15 +29,15 @@
             self._find_word_in_file(entry, word)
             for entry in track(self.entries.items(), description=f"Searching for {word}")
         )
 
     def _find_word_in_file(self, entry: tuple[str, str], word: str) -> str:
         file_output = StringIO()
         date, text = entry
-        sentences = sent_tokenize(text)
+        sentences = nltk.tokenize.sent_tokenize(text)
         sentences_containing_word = [s for s in sentences if self._is_word_in_sentence(s, word)]
         if not sentences_containing_word:
             return file_output.getvalue()
         file_output.write(date + "\n")
         for sentence in sentences_containing_word:
             file_output.write(self._find_word_in_sentence(sentence, word) + "\n")
         file_output.write("\n")
@@ -63,7 +67,8 @@
         if len(word2) > len(word1):  # word1 longer or same
             word1, word2 = word2, word1
         if len(word1) - len(word2) >= len(word2):
             return False
         word1 = word1.lower()
         word2 = word2.lower()
         return word2 in word1
+
```

### Comparing `diarium-cli-0.2.3/diarium_cli/helper.py` & `diarium-cli-0.2.4/diarium_cli/helper.py`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/diarium_cli/journal.py` & `diarium-cli-0.2.4/diarium_cli/journal.py`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/diarium_cli/main.py` & `diarium-cli-0.2.4/diarium_cli/main.py`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/diarium_cli/slovak_words.txt` & `diarium-cli-0.2.4/diarium_cli/slovak_words.txt`

 * *Files identical despite different names*

### Comparing `diarium-cli-0.2.3/setup.cfg` & `diarium-cli-0.2.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6961 7269 756d 2d63 6c69 0d0a   = diarium-cli..
-00000020: 7665 7273 696f 6e20 3d20 302e 322e 330d  version = 0.2.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 322e 340d  version = 0.2.4.
 00000030: 0a61 7574 686f 7220 3d20 5965 6c6f 760d  .author = Yelov.
 00000040: 0a64 6573 6372 6970 7469 6f6e 203d 2043  .description = C
 00000050: 4c49 2074 6f6f 6c20 666f 7220 6a6f 7572  LI tool for jour
 00000060: 6e61 6c69 6e67 2061 7070 2044 6961 7269  naling app Diari
 00000070: 756d 0d0a 6c6f 6e67 5f64 6573 6372 6970  um..long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
@@ -22,20 +22,20 @@
 00000150: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
 00000160: 3e3d 332e 370d 0a69 6e63 6c75 6465 5f70  >=3.7..include_p
 00000170: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
 00000180: 7565 0d0a 696e 7374 616c 6c5f 7265 7175  ue..install_requ
 00000190: 6972 6573 203d 200d 0a09 636c 6963 6b0d  ires = ...click.
 000001a0: 0a09 636c 6963 6b2d 7368 656c 6c0d 0a09  ..click-shell...
 000001b0: 7269 6368 0d0a 0975 6e69 6465 636f 6465  rich...unidecode
-000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000001d0: 6b61 6765 5f64 6174 615d 0d0a 2a20 3d20  kage_data]..* = 
-000001e0: 0d0a 0965 6e67 6c69 7368 5f77 6f72 6473  ...english_words
-000001f0: 2e74 7874 0d0a 0973 6c6f 7661 6b5f 776f  .txt...slovak_wo
-00000200: 7264 732e 7478 740d 0a0d 0a5b 6f70 7469  rds.txt....[opti
-00000210: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
-00000220: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
-00000230: 7473 203d 200d 0a09 6469 6172 6975 6d2d  ts = ...diarium-
-00000240: 636c 693d 6469 6172 6975 6d5f 636c 692e  cli=diarium_cli.
-00000250: 6d61 696e 3a63 6c69 0d0a 0d0a 5b65 6767  main:cli....[egg
-00000260: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000270: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000280: 2030 0d0a 0d0a                            0....
+000001c0: 0d0a 096e 6c74 6b0d 0a0d 0a5b 6f70 7469  ...nltk....[opti
+000001d0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+000001e0: 5d0d 0a2a 203d 200d 0a09 656e 676c 6973  ]..* = ...englis
+000001f0: 685f 776f 7264 732e 7478 740d 0a09 736c  h_words.txt...sl
+00000200: 6f76 616b 5f77 6f72 6473 2e74 7874 0d0a  ovak_words.txt..
+00000210: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000220: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
+00000230: 655f 7363 7269 7074 7320 3d20 0d0a 0964  e_scripts = ...d
+00000240: 6961 7269 756d 2d63 6c69 3d64 6961 7269  iarium-cli=diari
+00000250: 756d 5f63 6c69 2e6d 6169 6e3a 636c 690d  um_cli.main:cli.
+00000260: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000270: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000280: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

