# Comparing `tmp/edit_distance_correction-1.1.2-py3-none-any.whl.zip` & `tmp/edit_distance_correction-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 100720 bytes, number of entries: 17
+Zip file size: 101073 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      139 b- defN 24-Feb-05 09:12 edit_distance_correction/__init__.py
 -rw-r--r--  2.0 unx     1256 b- defN 24-Feb-23 02:50 edit_distance_correction/correction.csv
--rw-r--r--  2.0 unx     9734 b- defN 24-Mar-05 08:25 edit_distance_correction/correction.py
--rw-r--r--  2.0 unx     9496 b- defN 24-Feb-05 03:06 edit_distance_correction/correction_2.py
+-rw-r--r--  2.0 unx    11816 b- defN 24-Apr-10 06:57 edit_distance_correction/correction.py
+-rw-r--r--  2.0 unx     9578 b- defN 24-Mar-19 02:11 edit_distance_correction/correction_copy.py
 -rw-r--r--  2.0 unx     1089 b- defN 24-Feb-27 08:37 edit_distance_correction/heteronym.txt
--rw-r--r--  2.0 unx     6741 b- defN 24-Mar-05 06:47 edit_distance_correction/same_stroke.txt
--rw-r--r--  2.0 unx     1732 b- defN 24-Mar-05 08:15 edit_distance_correction/target_words
+-rw-r--r--  2.0 unx     6795 b- defN 24-Mar-11 07:24 edit_distance_correction/same_stroke.txt
+-rw-r--r--  2.0 unx     1765 b- defN 24-Mar-25 11:40 edit_distance_correction/target_words
 -rw-r--r--  2.0 unx      546 b- defN 24-Mar-05 08:16 edit_distance_correction/temp.py
 -rw-r--r--  2.0 unx   305220 b- defN 24-Mar-05 02:49 edit_distance_correction/temp.txt
--rw-r--r--  2.0 unx      712 b- defN 24-Mar-01 07:52 edit_distance_correction/test.py
--rw-r--r--  2.0 unx     1877 b- defN 24-Mar-05 07:35 edit_distance_correction/test_file
--rw-r--r--  2.0 unx     8663 b- defN 24-Mar-05 08:26 edit_distance_correction/utils.py
+-rw-r--r--  2.0 unx      391 b- defN 24-Mar-20 06:47 edit_distance_correction/test.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-Mar-25 11:40 edit_distance_correction/test_file
+-rw-r--r--  2.0 unx     8819 b- defN 24-Mar-25 11:38 edit_distance_correction/utils.py
 -rw-r--r--  2.0 unx     1676 b- defN 24-Jan-25 06:28 edit_distance_correction/valid_pinyin
--rw-r--r--  2.0 unx      291 b- defN 24-Mar-05 12:59 edit_distance_correction-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-05 12:59 edit_distance_correction-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-Mar-05 12:59 edit_distance_correction-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1574 b- defN 24-Mar-05 12:59 edit_distance_correction-1.1.2.dist-info/RECORD
-17 files, 350863 bytes uncompressed, 98076 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx      291 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/RECORD
+17 files, 353415 bytes uncompressed, 98423 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -3,15 +3,15 @@
 
 Filename: edit_distance_correction/correction.csv
 Comment: 
 
 Filename: edit_distance_correction/correction.py
 Comment: 
 
-Filename: edit_distance_correction/correction_2.py
+Filename: edit_distance_correction/correction_copy.py
 Comment: 
 
 Filename: edit_distance_correction/heteronym.txt
 Comment: 
 
 Filename: edit_distance_correction/same_stroke.txt
 Comment: 
@@ -33,20 +33,20 @@
 
 Filename: edit_distance_correction/utils.py
 Comment: 
 
 Filename: edit_distance_correction/valid_pinyin
 Comment: 
 
-Filename: edit_distance_correction-1.1.2.dist-info/METADATA
+Filename: edit_distance_correction-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: edit_distance_correction-1.1.2.dist-info/WHEEL
+Filename: edit_distance_correction-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: edit_distance_correction-1.1.2.dist-info/top_level.txt
+Filename: edit_distance_correction-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: edit_distance_correction-1.1.2.dist-info/RECORD
+Filename: edit_distance_correction-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edit_distance_correction/correction.py

```diff
@@ -1,14 +1,15 @@
 import Levenshtein
 import edit_distance_correction.utils as utils
 import pandas as pd
 import re
 from itertools import chain
 import os
 import time
+import kenlm
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 class Corrector:
     def __init__(self):
         self.max_k = 0
         #pinyin:set(word)
@@ -19,21 +20,26 @@
         self.start_word_di = dict()
         self.correction_dict = dict()
         self.original_dict = dict()
         self.same_stroke_dict = dict()
         self.same_stroke_head = set()
         self.heteronym_dict = dict()
         self.gram = dict()
+        self.lm = None
         self.valid_pinyin = set()
         self._load_correction()
         self._load_same_stroke()
         self._load_valid_pinyin()
         self._load_heteronym_dict()
+        #self._load_language_model()
 
 
+    def _load_language_model(self):
+        self.lm = kenlm.Model(self.language_model_path)
+
     def _load_valid_pinyin(self):
         self.valid_pinyin = utils.read_files(_get_module_path("valid_pinyin"))
 
 
     def _load_correction(self):
         correction = pd.read_csv(_get_module_path("correction.csv"), na_values=[''], keep_default_na=False)
         for original, corr in zip(correction["original"], correction["correction"]):
@@ -128,14 +134,37 @@
                             second_res.append([second_temp, start, end, temp])
             if not break_flag:
                 end -= 1
         res.reverse()
         return res, second_res
 
 
+    def max_backward_match_list(self, cuts, word_list, vocab, max_k=10):
+        res = []
+        end = len(word_list)
+        while end > 0:
+            break_flag = False
+            for i in range(max_k):
+                start = end - max_k + i
+                if start < 0: continue
+                # temp = "".join(word_list[start:end])
+                temps = utils.get_all_list(word_list[start:end])
+                for temp in temps:
+                    temp = "".join(temp)
+                    if temp in vocab:
+                        res.append([temp, start, end])
+                        break_flag = True
+                if break_flag:
+                    end = start
+            if not break_flag:
+                end -= 1
+        res.reverse()
+        return res
+
+
     def recall_word(self, query):
         #temp_cuts = jieba.lcut(query)
         temp_cuts = utils.cut(query)
         cuts = []
         for cut in temp_cuts:
             if re.search("^[a-zA-Z]+$", cut) is not None:
                 res = utils.pinyin_split(cut, self.valid_pinyin)
@@ -153,36 +182,37 @@
         for cut in cuts:
             qp = utils.get_pinyin(cut, mode="pinyin")
             query_pinyin_list.append(qp)
         res, second_res = self.max_backward_match_transform(query_pinyin_list, self.pinyin_di, max_k=self.max_k * 5)
         jianpin_res = utils.max_backward_match(cuts, self.start_word_di, max_k=1)
         #stroke_res = [utils.max_backward_match(elem, self.target_word, max_k=10) for elem in cuts_stroke]
         #stroke_res = list(chain(*stroke_res))
-        print(cuts_stroke)
-        stroke_res = utils.max_backward_match_list(cuts_stroke, self.target_word, max_k=self.max_k)
-        insider = []
-        outsider = []
+        #todo:这里找到一个直接返回，实际上最好收集所有可能再比较最好的
+        stroke_res = self.max_backward_match_list(cuts, cuts_stroke, self.target_word, max_k=self.max_k)
+        stroke_res = utils.combine_same_position(stroke_res)
+        first_pinyin_r = []
+        second_pinyin_r = []
         for elem in res:
             original = "".join(cuts[elem[1]:elem[2]])
             pinyin = "".join(query_pinyin_list[elem[1]:elem[2]])
             candidates = []
             for word in self.pinyin_di.get(pinyin, []):
                 transform_words = utils.get_all([[char, utils.get_pinyin(char, "pinyin")] for char in word])
                 candidates.append([word, min([Levenshtein.distance(w, original) for w in transform_words]), elem[1], elem[2]])
             candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), candidates))
             candidates = sorted(candidates, key=lambda x: x[1])
-            #candidates = [candidates[0]] if len(candidates) > 0 else []
             i = len(candidates)
             if len(candidates) > 1:
                 for ii in range(1, len(candidates)):
                     if candidates[ii][1] > candidates[0][1]:
                         i = ii
                         break
             candidates = candidates[:i]
-            insider.extend(candidates)
+            if len(candidates) > 0:
+                first_pinyin_r.append([elem[1], elem[2], [word[0] for word in candidates]])
         for elem in second_res:
             original = "".join(cuts[elem[1]:elem[2]])
             pinyin = elem[0]
             candidates = []
             for word in self.pinyin_di.get(pinyin, []):
                 transform_words = utils.get_all([[char, utils.get_pinyin(char, "pinyin")] for char in word])
                 candidates.append(
@@ -192,38 +222,57 @@
             i = len(candidates)
             if len(candidates) > 1:
                 for ii in range(1, len(candidates)):
                     if candidates[ii][1] > candidates[0][1]:
                         i = ii
                         break
             candidates = candidates[:i]
-            outsider.extend(candidates)
-        all_candidates = utils.check_conflict(insider, outsider)
-        outsider = []
+            if len(candidates) > 0:
+                second_pinyin_r.append([elem[1], elem[2], [word[0] for word in candidates]])
+        jianpin_r = []
         for elem in jianpin_res:
-            for e in self.start_word_di[elem[0]]:
-                outsider.append([e, 0, elem[1], elem[2]])
-        all_candidates = utils.check_conflict(all_candidates, outsider)
-        outsider = []
+            jianpin_r.append([elem[1], elem[2], self.start_word_di[elem[0]]])
+            # for e in self.start_word_di[elem[0]]:
+            #     jianpin_r.append([e, 0, elem[1], elem[2]])
+
+        stroke_r = []
         for elem in stroke_res:
-            correct = elem[0]
-            original = query[elem[1]:elem[2]]
-            #correct_pinyin = self.target_word[correct]
-            correct_pinyins = self.target_word[correct]
-            original_pinyin = utils.get_pinyin(original, mode="pinyin")
-            outsider.append([correct, Levenshtein.distance(correct, original) + min(
-                [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins]),
-                             elem[1],
-                             elem[2]])
+            start, end = elem[0], elem[1]
+            original = query[start : end]
+            candidates = []
+            for correct in elem[2]:
+                #correct_pinyin = self.target_word[correct]
+                correct_pinyins = self.target_word[correct]
+                original_pinyin = utils.get_pinyin(original, mode="pinyin")
+                candidates.append([correct, Levenshtein.distance(correct, original) + min(
+                    [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins])])
+                # stroke_r.append([correct, Levenshtein.distance(correct, original) + min(
+                #     [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins]),
+                #                  elem[1],
+                #                  elem[2]])
+            candidates = list(filter(lambda x: x[0] != original, candidates))
+            candidates = sorted(candidates, key=lambda x: x[1])
+            i = len(candidates)
+            if len(candidates) > 1:
+                for ii in range(1, len(candidates)):
+                    if candidates[ii][1] > candidates[0][1]:
+                        i = ii
+                        break
+            candidates = candidates[:i]
+            if len(candidates) > 0:
+                stroke_r.append([start, end, [word[0] for word in candidates]])
 
-            #outsider.append([correct, Levenshtein.distance(correct, original) + Levenshtein.distance(correct_pinyin, original_pinyin), elem[1], elem[2]])
+        all_candidates = utils.check_conflict(first_pinyin_r, second_pinyin_r)
+        all_candidates = utils.check_conflict(all_candidates, jianpin_r)
+        all_candidates = utils.check_conflict(all_candidates, stroke_r)
 
-        all_candidates = utils.check_conflict(all_candidates, outsider)
-        all_candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), all_candidates))
+        #all_candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), all_candidates))
         res = utils.get_correct(all_candidates, cuts)
+        #暂时取第一个，实际可以算分比较
+        res = res[0]
         return res
```

## edit_distance_correction/same_stroke.txt

```diff
@@ -341,8 +341,17 @@
 帅	师
 大	犬	夫	天
 固	涸
 格	恪
 檫	擦
 著	着	者
 （ (
-) ）
+) ）
+1 一
+2 二
+3 三
+4 四
+5 五
+6 六
+7 七
+8 八
+9 九
```

## edit_distance_correction/target_words

```diff
@@ -1,8 +1,9 @@
 话费
+化肥
 充话费
 牛人
 六人行
 电脑
 长度
 最好
 贵州茅台
@@ -125,8 +126,10 @@
 教育缴费
 组织经费
 直销
 直销银行
 保险（分红型）
 华润信托悦财宝21号
 东吴新产业精选b
+红塔证券
+孩童证券
```

## edit_distance_correction/test.py

```diff
@@ -14,18 +14,21 @@
     print(time.time() - start)
     start = time.time()
     print("\n")
 
 
 
 
-#费时最大：stroke_res = [utils.max_backward_match(elem, self.target_word, max_k=10) for elem in cuts_stroke]
-#形近字虽然用gram做了初筛，但不影响量级，相关组合太多n*n*n...
 
-# c = Corrector()
-# c.load_target_words(["1303XM2:1303XM26547891303XM2:1303XM281303XM2:1303XM2"])
-# res = c.recall_word("16181")
+
+
+
+
+
+
+
+
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## edit_distance_correction/test_file

```diff
@@ -68,8 +68,13 @@
 保险(fenhongxing）
 华润型托悦财宝21号华润型托悦财宝21号
 华润型托悦财宝21号电lao每甬证券你们说gui周茅台怎么样gzmt华润型托悦财宝21号华润型托悦财宝21号电lao
 华润型托悦财宝21号华润型托悦财宝21号华润型托悦财宝21号华润型托悦财宝21号华润型托悦财宝21号
 冻吴新产业精选A国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国A役指数增强保险（分红刑）
 冻吴新产业精选a国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国a役指数增强保险（分红刑）
 东吴新产业精选b
-东吴新产业精选B
+东吴新产业精选B
+冻吴新产业精选A国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国A役指数增强保险（分红刑）冻吴新产业精选A国信安泰中短债A华润信托悦财宝21号财通够策略福鑫华安MSCI中国A役指数增强保险（分红刑）
+冻吴新产业精选A国信安泰中短债a华润信托悦财宝21号责通够策略副鑫华安MSCI中国
+咖啡贵州maotai
+gzmt
+gzmt华妃swerwjrjweewjweqj害同振券
```

## edit_distance_correction/utils.py

```diff
@@ -73,34 +73,22 @@
                 break
         if not break_flag:
             end -= 1
     res.reverse()
     return res
 
 
-def max_backward_match_list(word_list, vocab, max_k=10):
-    res = []
-    end = len(word_list)
-    while end > 0:
-        break_flag = False
-        for i in range(max_k):
-            start = end - max_k + i
-            if start < 0: continue
-            #temp = "".join(word_list[start:end])
-            temps = get_all_list(word_list[start:end])
-            for temp in temps:
-                temp = "".join(temp)
-                if temp in vocab:
-                    res.append([temp, start, end])
-                    end = start
-                    break_flag = True
-                    break
-        if not break_flag:
-            end -= 1
-    res.reverse()
+#arr:[[word, start, end], ...]
+def combine_same_position(arr):
+    di = dict()
+    for elem in arr:
+        if elem[1] not in di:
+            di[elem[1]] = []
+        di[elem[1]].append(elem)
+    res = [(elem[0][1], elem[0][2], [e[0] for e in elem]) for elem in di.values()]
     return res
 
 
 #所有的组合先生成再计算和判断
 def get_all_combinations(query_pinyin_list, max_k=5):
     for i in range(len(query_pinyin_list)):
         end = max_k + 1 if max_k + 1 < len(query_pinyin_list) else len(query_pinyin_list)
@@ -148,36 +136,55 @@
 #判断是否冲突，冲突时保留insider部分，去掉outsider冲突的部分
 #insider: [[i, j, ..]]  outsider[[i, j, ..]]
 def check_conflict(insider, outsider):
     res = insider
     for o in outsider:
         flag = True
         for ins in res:
-            if not (o[2] >= ins[3] or o[3] <= ins[2]):
+            if not (o[0] >= ins[1] or o[1] <= ins[0]):
                 flag = False
                 break
         if flag: res.append(o)
     return res
 
 
 #候选改正词和分词结果还原得到最终改正结果
 def get_correct(candidates, cuts):
-    res = ""
-    candidates_dict = {cand[2]:{"end": cand[3], "word": cand[0]} for cand in candidates}
-    i = 0
-    while i < len(cuts):
-        if i in candidates_dict:
-            res += candidates_dict[i]["word"]
-            i = candidates_dict[i]["end"]
-        else:
-            res += cuts[i]
-            i += 1
+    res = []
+    cands = sorted(candidates, key=lambda x: x[0])
+    for i, cand in enumerate(cands):
+        before_start = cands[i-1][1] if i != 0 else 0
+        before_end = cand[0]
+        if before_start != before_end:
+            res.append(["".join(cuts[before_start: before_end])])
+        res.append(cand[2])
+    if len(cands) == 0:
+        res.append(["".join(cuts)])
+    else:
+        if cands[-1][1] != len(cuts):
+            res.append(["".join(cuts[cands[-1][1]:])])
+    res = get_all(res)
     return res
 
 
+
+
+    # res = ""
+    # candidates_dict = {cand[2]:{"end": cand[3], "word": cand[0]} for cand in candidates}
+    # i = 0
+    # while i < len(cuts):
+    #     if i in candidates_dict:
+    #         res += candidates_dict[i]["word"]
+    #         i = candidates_dict[i]["end"]
+    #     else:
+    #         res += cuts[i]
+    #         i += 1
+    # return res
+
+
 #用自己的多音字字典拓展多音字拼音
 def _heteronym_pinyin(s, heteronym_dict):
     li = []
     for ch in s:
         if re.match('[\u4e00-\u9fa5]+', ch) is not None:
             original = pinyin(ch, style=pypinyin.NORMAL)[0]
             temp = set(original).union(heteronym_dict.get(ch, set()))
```

## Comparing `edit_distance_correction/correction_2.py` & `edit_distance_correction/correction_copy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import Levenshtein
-import pypinyin
 import edit_distance_correction.utils as utils
 import pandas as pd
 import re
-import jieba
 from itertools import chain
 import os
+import time
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 class Corrector:
     def __init__(self):
         self.max_k = 0
         #pinyin:set(word)
         self.pinyin_di = dict()
         self.target_word = dict()
         #start:set(pinyin)
-        self.start_pinyin_di = dict()
+        # self.start_pinyin_di = dict()
         self.start_word_di = dict()
         self.correction_dict = dict()
+        self.original_dict = dict()
         self.same_stroke_dict = dict()
         self.same_stroke_head = set()
+        self.heteronym_dict = dict()
         self.gram = dict()
         self.valid_pinyin = set()
         self._load_correction()
         self._load_same_stroke()
         self._load_valid_pinyin()
+        self._load_heteronym_dict()
 
 
     def _load_valid_pinyin(self):
         self.valid_pinyin = utils.read_files(_get_module_path("valid_pinyin"))
 
 
     def _load_correction(self):
-        correction = pd.read_excel(_get_module_path("correction.xlsx"))
+        correction = pd.read_csv(_get_module_path("correction.csv"), na_values=[''], keep_default_na=False)
         for original, corr in zip(correction["original"], correction["correction"]):
             if original not in self.correction_dict:
                 self.correction_dict[original] = set()
             self.correction_dict[original].add(corr)
 
 
     def _load_same_stroke(self):
@@ -53,39 +55,51 @@
                             if elem1 not in self.same_stroke_dict:
                                 self.same_stroke_dict[elem1] = set()
                             self.same_stroke_dict[elem1].add(elem2)
 
 
     def load_target_words(self, target_words):
         for word in target_words:
+            #word = word.lower()
             if len(word) > self.max_k:
-                self.max_k = min(10, len(word))
-            res = utils.get_pinyin(word, True)
-            if res["pinyin"] not in self.pinyin_di:
-                self.pinyin_di[res["pinyin"]] = set()
-            self.pinyin_di[res["pinyin"]].add(word)
-            if res["start"] not in self.start_pinyin_di:
-                self.start_pinyin_di[res["start"]] = set()
-            self.start_pinyin_di[res["start"]].add(res["pinyin"])
-            if res["start"] not in self.start_word_di:
-                self.start_word_di[res["start"]] = set()
-            self.start_word_di[res["start"]].add(word)
+                self.max_k = len(word)
+            all_res = utils.get_pinyin(word, "all", True, self.heteronym_dict)
+            for res in all_res:
+                if res["pinyin"] not in self.pinyin_di:
+                    self.pinyin_di[res["pinyin"]] = set()
+                self.pinyin_di[res["pinyin"]].add(word)
+                # if re.match('^[\u4e00-\u9fa5]+$', word) is not None:
+                #     if res["start"] not in self.start_pinyin_di:
+                #         self.start_pinyin_di[res["start"]] = set()
+                #     self.start_pinyin_di[res["start"]].add(res["pinyin"])
+                if re.match('^[\u4e00-\u9fa5]+$', word) is not None:
+                    if res["start"] not in self.start_word_di:
+                        self.start_word_di[res["start"]] = set()
+                    self.start_word_di[res["start"]].add(word)
+                if word not in self.target_word:
+                    self.target_word[word] = set()
+                self.target_word[word].add(res["pinyin"])
             if len(word) > 0:
                 self.same_stroke_head.add(word[0])
-            self.target_word[word] = res["pinyin"]
 
             for i in range(len(word)):
                 if word[i] not in self.gram:
                     self.gram[word[i]] = set()
                 if i == len(word) - 1:
                     self.gram[word[i]].add("")
                 else:
                     self.gram[word[i]].add(word[i+1])
 
 
+    def _load_heteronym_dict(self):
+        lines = utils.read_files(_get_module_path("heteronym.txt"))
+        for line in lines:
+            utils.process_heteronym_line(line, self.heteronym_dict)
+
+
     def _transform_pinyin(self, pinyin, include_self=False):
         res = utils.replace_char(pinyin, self.correction_dict, max_k=6)
         res = res.union(utils.transform_char(pinyin))
         if include_self:
             res.add(pinyin)
         return res
 
@@ -127,88 +141,83 @@
                 res = utils.pinyin_split(cut, self.valid_pinyin)
                 if res is None:
                     cuts.append(cut)
                 else:
                     cuts.extend(res)
             else:
                 cuts.append(cut)
-
-        # cuts_stroke = [utils.get_all([list(self.same_stroke_dict.get(char, [char])) for char in cut]) for cut in cuts]
-        # cuts_stroke = utils.get_all_list(cuts_stroke)
-        # print(cuts_stroke)
         cuts_stroke = utils.get_stroke_replace(cuts, self.gram, self.same_stroke_dict, self.same_stroke_head)
-        cuts_stroke = utils.get_all_list(cuts_stroke)
+        #cuts_stroke = utils.get_all_list(cuts_stroke)
+        #print(len(cuts_stroke))
 
         query_pinyin, query_start_pinyin, query_pinyin_list = "", "", []
         for cut in cuts:
             qp = utils.get_pinyin(cut, mode="pinyin")
             query_pinyin_list.append(qp)
-        #todo:多种召回无法结合：简拼，全拼，全拼转换，形近字
-        #todo:目前只取一个，后面考虑怎样展示，多种可能的排列组合？
-        res, second_res = self.max_backward_match_transform(query_pinyin_list, self.pinyin_di, max_k=10)
+        res, second_res = self.max_backward_match_transform(query_pinyin_list, self.pinyin_di, max_k=self.max_k * 5)
         jianpin_res = utils.max_backward_match(cuts, self.start_word_di, max_k=1)
-        stroke_res = [utils.max_backward_match(elem, self.target_word, max_k=10) for elem in cuts_stroke]
-        stroke_res = list(chain(*stroke_res))
+        #stroke_res = [utils.max_backward_match(elem, self.target_word, max_k=10) for elem in cuts_stroke]
+        #stroke_res = list(chain(*stroke_res))
+        print(cuts_stroke)
+        stroke_res = utils.max_backward_match_list(cuts_stroke, self.target_word, max_k=self.max_k)
         insider = []
         outsider = []
         for elem in res:
             original = "".join(cuts[elem[1]:elem[2]])
             pinyin = "".join(query_pinyin_list[elem[1]:elem[2]])
             candidates = []
             for word in self.pinyin_di.get(pinyin, []):
                 transform_words = utils.get_all([[char, utils.get_pinyin(char, "pinyin")] for char in word])
                 candidates.append([word, min([Levenshtein.distance(w, original) for w in transform_words]), elem[1], elem[2]])
-            #candidates = [[word, min(Levenshtein.distance(word, original), Levenshtein.distance(pinyin, original)), elem[1], elem[2]] for word in self.pinyin_di.get(pinyin, [])]
             candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), candidates))
             candidates = sorted(candidates, key=lambda x: x[1])
-            # todo: 暂时取一个，实际上应该分析
-            candidates = [candidates[0]] if len(candidates) > 0 else []
-            # i = len(candidates)
-            # if len(candidates) > 1:
-            #     for ii in range(1, len(candidates)):
-            #         if candidates[ii][1] > candidates[0][1]:
-            #             i = ii
-            #             break
-            # candidates = candidates[:i]
+            #candidates = [candidates[0]] if len(candidates) > 0 else []
+            i = len(candidates)
+            if len(candidates) > 1:
+                for ii in range(1, len(candidates)):
+                    if candidates[ii][1] > candidates[0][1]:
+                        i = ii
+                        break
+            candidates = candidates[:i]
             insider.extend(candidates)
         for elem in second_res:
             original = "".join(cuts[elem[1]:elem[2]])
             pinyin = elem[0]
             candidates = []
             for word in self.pinyin_di.get(pinyin, []):
                 transform_words = utils.get_all([[char, utils.get_pinyin(char, "pinyin")] for char in word])
                 candidates.append(
                     [word, min([Levenshtein.distance(w, original) for w in transform_words]), elem[1], elem[2]])
-            #candidates = [[word, min(Levenshtein.distance(word, original), Levenshtein.distance(pinyin, original)), elem[1], elem[2]] for word in self.pinyin_di.get(pinyin, [])]
             candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), candidates))
             candidates = sorted(candidates, key=lambda x: x[1])
-            # todo: 暂时取一个，实际上应该分析
-            candidates = [candidates[0]] if len(candidates) > 0 else []
-            # i = len(candidates)
-            # if len(candidates) > 1:
-            #     for ii in range(1, len(candidates)):
-            #         if candidates[ii][1] > candidates[0][1]:
-            #             i = ii
-            #             break
-            # candidates = candidates[:i]
+            i = len(candidates)
+            if len(candidates) > 1:
+                for ii in range(1, len(candidates)):
+                    if candidates[ii][1] > candidates[0][1]:
+                        i = ii
+                        break
+            candidates = candidates[:i]
             outsider.extend(candidates)
         all_candidates = utils.check_conflict(insider, outsider)
         outsider = []
         for elem in jianpin_res:
-            # todo: 暂时取一个，实际上应该分析
-            outsider.append([list(self.start_word_di[elem[0]])[0], 0, elem[1], elem[2]])
-        all_candidates= utils.check_conflict(all_candidates, outsider)
-
+            for e in self.start_word_di[elem[0]]:
+                outsider.append([e, 0, elem[1], elem[2]])
+        all_candidates = utils.check_conflict(all_candidates, outsider)
         outsider = []
         for elem in stroke_res:
             correct = elem[0]
             original = query[elem[1]:elem[2]]
-            correct_pinyin = self.target_word[correct]
+            #correct_pinyin = self.target_word[correct]
+            correct_pinyins = self.target_word[correct]
             original_pinyin = utils.get_pinyin(original, mode="pinyin")
-            outsider.append([correct, Levenshtein.distance(correct, original) + Levenshtein.distance(correct_pinyin, original_pinyin), elem[1], elem[2]])
+            outsider.append([correct, Levenshtein.distance(correct, original) + min(
+                [Levenshtein.distance(correct_pinyin, original_pinyin) for correct_pinyin in correct_pinyins]),
+                             elem[1],
+                             elem[2]])
 
         all_candidates = utils.check_conflict(all_candidates, outsider)
         all_candidates = list(filter(lambda x: x[0] != "".join(cuts[x[2]: x[3]]), all_candidates))
         res = utils.get_correct(all_candidates, cuts)
         return res
```

## Comparing `edit_distance_correction-1.1.2.dist-info/RECORD` & `edit_distance_correction-1.1.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 edit_distance_correction/__init__.py,sha256=iEwR-MyXazzbaotC3qWLZykxG-cA4hyVlazXyWsxR2c,139
 edit_distance_correction/correction.csv,sha256=Z15Pkoxu0BqTse-b0Vx6p8VhDVRi_2ct3NjCB84OuTA,1256
-edit_distance_correction/correction.py,sha256=QV2WxNeweJJHqZ0Vp_2h2YYVmrO4YX73iElhXdxlRXc,9734
-edit_distance_correction/correction_2.py,sha256=sG7ZZxTde-HtODz28C_h-8zwGQTa5H2M9jRG6A2DjfQ,9496
+edit_distance_correction/correction.py,sha256=Q6AQXNoUgv9vJ8YUoLk-LSNAlctl3CTa35KC_YBhQBo,11816
+edit_distance_correction/correction_copy.py,sha256=uKZjntYbrVUc695RAZMId4lnnjgihl4Vg1_c-NhvIL8,9578
 edit_distance_correction/heteronym.txt,sha256=-cGHvlDxqZm9QuTUEClUx7kLDETYZaNGc8QhJqV1kyI,1089
-edit_distance_correction/same_stroke.txt,sha256=rOrgIlpqY-WJzUitqlzcDp5ei04RkyUPOIfxIC2fWM0,6741
-edit_distance_correction/target_words,sha256=XW1RKikwfDYUEILDhWdz-VPl0UAjLKBqusks1u049_c,1732
+edit_distance_correction/same_stroke.txt,sha256=IBODeWIgQwun_Si-cysULmEkGCKDQe1SOSG2beegIkM,6795
+edit_distance_correction/target_words,sha256=BOmPlH8n0A7xsaD8S0n9f3JCzN7nm9IHMtRJltiu1XI,1765
 edit_distance_correction/temp.py,sha256=s35J407s6ap1dkWg0AKmeL_nLM059RwcwAR-GZqcOEw,546
 edit_distance_correction/temp.txt,sha256=2l1TiLjVg9Kij3XsOg3IJhmC1hVZtimzHB_kuZvVkbY,305220
-edit_distance_correction/test.py,sha256=VOnyE3o4EI4LNkmT5QEhQKPVx-iraZdmwB4Ha0n3Lcs,712
-edit_distance_correction/test_file,sha256=iODRVfHmAPd91kgML6I99omHrKJxwBPD8wtnk02-IiE,1877
-edit_distance_correction/utils.py,sha256=P2UasohcgKeOYvX11JvCdxi07J_rsgN-DUUw-xu_Qi0,8663
+edit_distance_correction/test.py,sha256=oG_UfMwTOEBAFlLD_N7CJzmDwvNibktFNaDR1dcR0m0,391
+edit_distance_correction/test_file,sha256=_XlLhGNIFbjfQKmkkVmCIHl-izGjhGOXUUnsLbJTy6A,2339
+edit_distance_correction/utils.py,sha256=XtywpJdMVp_50kfMyqhEYo5UBhXk3E-3HejnfICCLPc,8819
 edit_distance_correction/valid_pinyin,sha256=6EqB5E8P3jAIukFOBvQtagZ4DCqQCjemjwo2bykSpJc,1676
-edit_distance_correction-1.1.2.dist-info/METADATA,sha256=pby9mnhLMnM75HTYBWLDa3Xp4bwDsdXDS-I8tUR7fyI,291
-edit_distance_correction-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-edit_distance_correction-1.1.2.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
-edit_distance_correction-1.1.2.dist-info/RECORD,,
+edit_distance_correction-1.1.3.dist-info/METADATA,sha256=Nq2gz45IXu7TraOUW0OvvuaKGkmgvtC-FqCsrBmR41I,291
+edit_distance_correction-1.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+edit_distance_correction-1.1.3.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
+edit_distance_correction-1.1.3.dist-info/RECORD,,
```

