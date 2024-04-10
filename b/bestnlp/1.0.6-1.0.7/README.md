# Comparing `tmp/bestnlp-1.0.6-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1912406 bytes, number of entries: 10
+Zip file size: 1912533 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
 -rw-r--r--  2.0 unx  5071852 b- defN 24-Mar-29 09:38 bestnlp/dict.txt
--rw-r--r--  2.0 unx     7351 b- defN 24-Apr-07 08:53 bestnlp/new_word_discovery.py
+-rw-r--r--  2.0 unx     7670 b- defN 24-Apr-09 10:58 bestnlp/new_word_discovery.py
 -rw-r--r--  2.0 unx     4182 b- defN 24-Apr-07 06:43 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
--rw-r--r--  2.0 unx      842 b- defN 24-Apr-03 02:41 bestnlp/utils.py
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 09:00 bestnlp-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 09:00 bestnlp-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 09:00 bestnlp-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-07 09:00 bestnlp-1.0.6.dist-info/RECORD
-10 files, 5089610 bytes uncompressed, 1911056 bytes compressed:  62.5%
+-rw-r--r--  2.0 unx      958 b- defN 24-Apr-09 10:58 bestnlp/utils.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-10 02:17 bestnlp-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 02:17 bestnlp-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-10 02:17 bestnlp-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-10 02:17 bestnlp-1.0.7.dist-info/RECORD
+10 files, 5090045 bytes uncompressed, 1911183 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.6.dist-info/METADATA
+Filename: bestnlp-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.6.dist-info/WHEEL
+Filename: bestnlp-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.6.dist-info/top_level.txt
+Filename: bestnlp-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.6.dist-info/RECORD
+Filename: bestnlp-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/new_word_discovery.py

```diff
@@ -145,17 +145,24 @@
                     di[word] = [final_entropy, l_e, r_e]
         di = sorted(di.items(), key=lambda x: x[1][0], reverse=True)
         di = di[:int(len(freq_di) * percent / 100)]
         di = {key: value for key, value in di}
         return di
 
 
-    def extract_keyword(self, filename, sentences=None, k_min=2, k_max=5, mode="word", min_freq=5, entropy_percent=20, ami_percent=20, write_mode=True, write_name="details.csv"):
-        if sentences is None:
-            sentences = utils.read_txt(filename)
+    def extract_keyword(self, sentence_list=None, filename=None, k_min=2, k_max=5, mode="word", min_freq=5, entropy_percent=20, ami_percent=20, write_mode=True, write_name="details.csv"):
+        if sentence_list is None and filename is None:
+            print("must input parameters sentence_list or filename!")
+            return
+        sentences = []
+        if sentence_list is not None:
+            sentences.extend(sentence_list)
+        if filename is not None:
+            sentences.extend(utils.read_txt(filename))
+        sentences = utils.split_sentence(sentences)
         write_df = {"word":[], "ami":[], "entropy":[], "l_e":[], "r_e":[], "pos":[], "freq":[], "idf":[], "score":[]}
         freq_di, word_num, idf_di = self.calculate_frequency(sentences, k_min, k_max, mode)
         entropy_di = self.L_entropy(freq_di, percent=entropy_percent)
         print(len(entropy_di))
         ami_di = self.ami(freq_di, word_num, percent=ami_percent)
         print(len(ami_di))
         structure_di = self.structure(freq_di)
```

## bestnlp/utils.py

```diff
@@ -1,19 +1,27 @@
 import re
 
+
 def read_txt(filename):
     sentences = []
     with open(filename, "r") as f:
         for line in f:
-            res = re.split("[,，。.、;；\'\"\(\)“（）【】\[\]\?？:：!！\s+]", line)
-            sentences.extend(res)
-    sentences = list(set(sentences))
+            sentences.append(line.strip())
     return sentences
 
 
+def split_sentence(sentences):
+    res = []
+    for sentence in sentences:
+        temp = re.split("[,，。.、;；\'\"\(\)“（）【】\[\]\?？:：!！\s+]", sentence)
+        res.extend(temp)
+    res = list(set(res))
+    return res
+
+
 def is_same_set(s1, s2):
     return len(s1 & s2) == len(s1) == len(s2)
 
 
 def merge_dicts_sum(dict1, dict2):
     for key in dict2:
         if key in dict1:
```

