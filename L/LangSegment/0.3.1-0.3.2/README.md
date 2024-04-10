# Comparing `tmp/LangSegment-0.3.1-py3-none-any.whl.zip` & `tmp/LangSegment-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21195 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    44850 b- defN 24-Apr-07 05:24 LangSegment/LangSegment.py
--rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-07 05:25 LangSegment/__init__.py
--rw-rw-rw-  2.0 fat    15227 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 24-Apr-07 05:25 LangSegment-0.3.1.dist-info/RECORD
-6 files, 60937 bytes uncompressed, 20331 bytes compressed:  66.6%
+Zip file size: 21120 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    44709 b- defN 24-Apr-10 11:27 LangSegment/LangSegment.py
+-rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-10 11:27 LangSegment/__init__.py
+-rw-rw-rw-  2.0 fat    15251 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/RECORD
+6 files, 60820 bytes uncompressed, 20256 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: LangSegment/LangSegment.py
 Comment: 
 
 Filename: LangSegment/__init__.py
 Comment: 
 
-Filename: LangSegment-0.3.1.dist-info/METADATA
+Filename: LangSegment-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: LangSegment-0.3.1.dist-info/WHEEL
+Filename: LangSegment-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: LangSegment-0.3.1.dist-info/top_level.txt
+Filename: LangSegment-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: LangSegment-0.3.1.dist-info/RECORD
+Filename: LangSegment-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## LangSegment/LangSegment.py

```diff
@@ -313,15 +313,15 @@
             cleans_text = LangSegment._cleans_text(cleans_text)
             # fix:Langid's recognition of short sentences is inaccurate, and it is spliced longer.
             if not EOS and len(cleans_text) <= 2:
                 lines[nextId] = f'{text}{nextText}'
                 continue
             language,score = LangSegment._lang_classify(cleans_text)
             prev_language , prev_text = LangSegment._get_prev_data(words)
-            if (not language in LANG_ZH_JA or score < 0.95) and all('\u4e00' <= c <= '\u9fff' for c in cleans_text):language,score = LANG_ZH,1
+            if language != LANG_ZH and all('\u4e00' <= c <= '\u9fff' for c in cleans_text):language,score = LANG_ZH,1
             if len(cleans_text) <= 5 and LangSegment._is_chinese(cleans_text):
                 filters_string = LangSegment._get_filters_string()
                 if score < LangSegment.LangPriorityThreshold and len(filters_string) > 0:
                     index_ja , index_zh = filters_string.find(LANG_JA) , filters_string.find(LANG_ZH)
                     if index_ja != -1 and index_ja < index_zh:language = LANG_JA
                     elif index_zh != -1 and index_zh < index_ja:language = LANG_ZH
                 if LangSegment._is_japanese_kana(cleans_text):language = LANG_JA
@@ -780,16 +780,14 @@
 비 오는 날에 음악을 듣는 것을 즐깁니다。
 J'aime écouter de la musique les jours de pluie.
 Tôi thích nghe nhạc vào những ngày mưa.
 Мне нравится слушать музыку в дождливую погоду.
 ฉันชอบฟังเพลงในวันที่ฝนตก
 """
 
-    text = "那我们拆分来看一下：Part A（传统阅读理解）,每题0.5分，共10分，第二部分"
-
 
     # 进行分词：（接入TTS项目仅需一行代码调用）Segmentation: (Only one line of code is required to access the TTS project)
     langlist = LangSegment.getTexts(text)
     printList(langlist)
     
     
     # 语种统计:Language statistics:
```

## LangSegment/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .LangSegment import LangSegment,getTexts,classify,getCounts,printList,setfilters,getfilters,setPriorityThreshold,getPriorityThreshold,setEnablePreview,getEnablePreview,setKeepPinyin,getKeepPinyin
 
 # release
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 # develop
 __develop__ = 'dev-0.0.1'
```

## Comparing `LangSegment-0.3.1.dist-info/METADATA` & `LangSegment-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: LangSegment
-Version: 0.3.1
+Version: 0.3.2
 Summary: This is a multilingual tokenization tool that currently supports for zh/ja/en/ko, and more languages.
 Home-page: https://github.com/juntaosun/LangSegment
 Author: sunnyboxs
 License: BSD
 Keywords: language detection,language identification,langid,langid.py,nlp,language
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,15 +36,15 @@
 https://github.com/adbar/py3langid  
 
 
 功能：将文章或句子里的例如（中/英/日/韩），按不同语言自动识别分词，使文本更适合AI处理。    
 本代码专为各种 TTS 项目的前端文本多语种混合标注区分，多语言混合训练和推理而编写。
 
 ## 最近更新：News   
-* 版本：v0.3.0   （更新帮助见下文）。
+* 版本：v0.3.2  fix （更新帮助见下文）。
 * 添加支持： "zh"中文（数字拼音pinyin），保留多音字（音素）指定。 
 * 添加支持： "ru"俄语Russian / "th"泰语Thai。
 * 添加支持： "fr"法语French  / "vi"越南语Vietnamese。
 * 语言优先级，置信度评分和阀值。
 * 优化字符处理。fix: LangSegment.setfilters    
 * 更细致的处理，中日英韩，分词更精准！  
 * 多语言过滤组功能（默认:中/英/日/韩）！帮您自动清理不需要的语言内容。   
@@ -126,15 +127,15 @@
 ```python
 TTS语音合成（英文字母）大小写拼读规则：
 （1）需要单个字母发音就大写，比如：USA，USB，ChatGPT，LCD，GPU，CEO。
 （2）其它情况正常拼读，就按正常拼写。比如：Nvidia ， Cuda 或者全小写 （nvidia ， cuda ）
 ```
 
 ## 拼音保留：支持（多音字）  
-> 版本支持：>= 0.3.0  
+> 版本支持：>= 0.3.2  
 > 常见需求：直接修改 TTS 的汉字读音，保留拼音输入。  
 ```python
 # 开启汉语拼音保留，（TTS标准：数字拼音格式），默认关闭。  
 LangSegment.setKeepPinyin(True)  
 
 # 汉字拼音指定示例：以下句子，括号中的拼音，均识别为中文。
 text = "这个字的读音是角(jue2)色，而不是角(jiao3)色"  
@@ -287,7 +288,8 @@
 > 备注：多语种混合文本转语音合成（TTS），中/日/英/韩/已完成测试。  
 其它语种未作具体测试，如有Bug和优化建议，欢迎提出或指正，感谢~。  
 Note: The speech synthesis test content is currently mainly for four categories: Chinese, Japanese, English and Korean.     
 Other languages have not been specifically tested. If there are any bugs or optimization suggestions, please feel free to raise them or correct them. Thank you~  
 Special thanks to the following projects: [py3langid](https://github.com/adbar/py3langid)
 ---
 ---
+
```

### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: LangSegment Version: 0.3.1 Summary: This is a
+Metadata-Version: 2.1 Name: LangSegment Version: 0.3.2 Summary: This is a
 multilingual tokenization tool that currently supports for zh/ja/en/ko, and
 more languages. Home-page: https://github.com/juntaosun/LangSegment Author:
 sunnyboxs License: BSD Keywords: language detection,language
-identification,langid,langid.py,nlp,language Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Requires-Dist: numpy >=1.19.5 Requires-Dist:
-py3langid >=0.2.2 # LangSegment
+identification,langid,langid.py,nlp,language Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+BSD License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6 Description-Content-Type: text/markdown Requires-Dist: numpy
+>=1.19.5 Requires-Dist: py3langid >=0.2.2 # LangSegment
 **ç®ä»ï¼å®æ¯ä¸ä¸ªå¼ºå¤§çå¤è¯­è¨ï¼97ç§è¯­è¨ï¼çæ··åææ¬èªå¨åè¯å·¥å·ã
 [ä¸­/æ¥/è±/é©ï¼å·²æµè¯]** **ä¸»è¦ç¨éï¼âä¸å£æ°â è®©ä½ ç TTS
 è¯­é³åæé¡¹ç® VITS
 è¯´åºå¤å½è¯­è¨ï¼å¤è¯­ç§æ··åææ¬çåè¯æ¨çï¼åé¢å¤çè®­ç»ã**
 **åè¯æ¯æï¼ä¸­æ/è±æ/æ¥æ/é©è¯­/æ³è¯­/è¶åè¯­/ä¿è¯­/æ³°è¯­/**
 ![image](./example.png) å®åºäº py3langid çæ©å±å®ç°ï¼>=python3.6ï¼ã
 ``LangSegment`` It is a multi-lingual (97 languages) text content automatic
@@ -22,15 +22,15 @@
 TTS (Text-to-Speech) synthesis projects, preprocessing of multilingual text
 mixing for both training and inference. >Implementation based on
 py3langidï¼See LICENSE file for more info. https://github.com/adbar/py3langid
 åè½ï¼å°æç« æå¥å­éçä¾å¦ï¼ä¸­/è±/æ¥/
 é©ï¼ï¼æä¸åè¯­è¨èªå¨è¯å«åè¯ï¼ä½¿ææ¬æ´éåAIå¤çã
 æ¬ä»£ç ä¸ä¸ºåç§ TTS
 é¡¹ç®çåç«¯ææ¬å¤è¯­ç§æ··åæ æ³¨åºåï¼å¤è¯­è¨æ··åè®­ç»åæ¨çèç¼åã
-## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.0 ï¼æ´æ°å¸®å©è§ä¸æï¼ã *
+## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.2 fix ï¼æ´æ°å¸®å©è§ä¸æï¼ã *
 æ·»å æ¯æï¼
 "zh"ä¸­æï¼æ°å­æ¼é³pinyinï¼ï¼ä¿çå¤é³å­ï¼é³ç´ ï¼æå®ã *
 æ·»å æ¯æï¼ "ru"ä¿è¯­Russian / "th"æ³°è¯­Thaiã * æ·»å æ¯æï¼
 "fr"æ³è¯­French / "vi"è¶åè¯­Vietnameseã *
 è¯­è¨ä¼åçº§ï¼ç½®ä¿¡åº¦è¯ååéå¼ã * ä¼åå­ç¬¦å¤çãfix:
 LangSegment.setfilters * æ´ç»è´çå¤çï¼ä¸­æ¥è±é©ï¼åè¯æ´ç²¾åï¼
 * å¤è¯­è¨è¿æ»¤ç»åè½ï¼é»è®¤:ä¸­/è±/æ¥/
@@ -84,15 +84,15 @@
 å¶ä¸­è±æç¼©åå­æ¯å¦âLCDâï¼è±ææ ååé³ä¸ºâL-C-Dâï¼ #
 èå¨è¯­é³åæTTSé¡¹ç®ä¸­ï¼ä¸è¬ç¨ç©ºæ ¼éå¼å­æ¯æ¥åç¬åé³ï¼âL
 C Dâ ``` ## è±ææ¼è¯»ï¼æ¯æ ```python
 TTSè¯­é³åæï¼è±æå­æ¯ï¼å¤§å°åæ¼è¯»è§åï¼
 ï¼1ï¼éè¦åä¸ªå­æ¯åé³å°±å¤§åï¼æ¯å¦ï¼USAï¼USBï¼ChatGPTï¼LCDï¼GPUï¼CEOã
 ï¼2ï¼å¶å®æåµæ­£å¸¸æ¼è¯»ï¼å°±ææ­£å¸¸æ¼åãæ¯å¦ï¼Nvidia ï¼ Cuda
 æèå¨å°å ï¼nvidia ï¼ cuda ï¼ ``` ##
-æ¼é³ä¿çï¼æ¯æï¼å¤é³å­ï¼ > çæ¬æ¯æï¼>= 0.3.0 >
+æ¼é³ä¿çï¼æ¯æï¼å¤é³å­ï¼ > çæ¬æ¯æï¼>= 0.3.2 >
 å¸¸è§éæ±ï¼ç´æ¥ä¿®æ¹ TTS çæ±å­è¯»é³ï¼ä¿çæ¼é³è¾å¥ã
 ```python #
 å¼å¯æ±è¯­æ¼é³ä¿çï¼ï¼TTSæ åï¼æ°å­æ¼é³æ ¼å¼ï¼ï¼é»è®¤å³é­ã
 LangSegment.setKeepPinyin(True) #
 æ±å­æ¼é³æå®ç¤ºä¾ï¼ä»¥ä¸å¥å­ï¼æ¬å·ä¸­çæ¼é³ï¼åè¯å«ä¸ºä¸­æã
 text = "è¿ä¸ªå­çè¯»é³æ¯è§(jue2)è²ï¼èä¸æ¯è§(jiao3)è²" ``` ##
 åè¯çº éï¼å¾éè¦ï¼
```

