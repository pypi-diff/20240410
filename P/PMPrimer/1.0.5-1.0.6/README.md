# Comparing `tmp/PMPrimer-1.0.5.tar.gz` & `tmp/PMPrimer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PMPrimer-1.0.5.tar", last modified: Sat Oct 14 06:12:15 2023, max compression
+gzip compressed data, was "PMPrimer-1.0.6.tar", last modified: Wed Apr 10 14:48:43 2024, max compression
```

## Comparing `PMPrimer-1.0.5.tar` & `PMPrimer-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2023-10-14 06:12:15.922626 PMPrimer-1.0.5/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1087 2023-07-20 05:53:27.000000 PMPrimer-1.0.5/LICENSE
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2023-10-14 06:12:15.918194 PMPrimer-1.0.5/PKG-INFO
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2023-10-14 06:12:15.593036 PMPrimer-1.0.5/PMPrimer.egg-info/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/PKG-INFO
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      420 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/SOURCES.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)        1 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/dependency_links.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       51 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/entry_points.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       47 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/requires.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)        6 2023-10-14 06:12:15.000000 PMPrimer-1.0.5/PMPrimer.egg-info/top_level.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10176 2023-10-14 05:24:11.000000 PMPrimer-1.0.5/README.md
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2023-10-14 06:12:15.882832 PMPrimer-1.0.5/piece/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      211 2023-10-14 05:06:16.000000 PMPrimer-1.0.5/piece/__auxiliary__.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       15 2023-07-20 05:53:27.000000 PMPrimer-1.0.5/piece/__init__.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    11170 2023-10-13 16:43:18.000000 PMPrimer-1.0.5/piece/piecebase.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     9104 2023-10-14 05:58:30.000000 PMPrimer-1.0.5/piece/piecedataprogress.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1328 2023-10-13 16:04:55.000000 PMPrimer-1.0.5/piece/piecedefine.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10807 2023-10-14 05:29:27.000000 PMPrimer-1.0.5/piece/piecedesign.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    19052 2023-07-20 05:53:27.000000 PMPrimer-1.0.5/piece/pieceevaluate.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    31580 2023-10-14 04:58:49.000000 PMPrimer-1.0.5/piece/piecemain.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     6819 2023-09-06 06:58:05.000000 PMPrimer-1.0.5/piece/piecentry.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      547 2023-10-14 06:12:15.922626 PMPrimer-1.0.5/setup.cfg
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      805 2023-10-14 05:06:16.000000 PMPrimer-1.0.5/setup.py
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.408625 PMPrimer-1.0.6/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1087 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/LICENSE
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       22 2024-04-10 14:04:14.000000 PMPrimer-1.0.6/MANIFEST.in
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-04-10 14:48:43.392596 PMPrimer-1.0.6/PKG-INFO
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.376972 PMPrimer-1.0.6/PMPrimer.egg-info/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/PKG-INFO
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      502 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)        1 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       51 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/entry_points.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       47 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/requires.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)        6 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/top_level.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10176 2023-10-14 05:24:11.000000 PMPrimer-1.0.6/README.md
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.187999 PMPrimer-1.0.6/piece/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      211 2024-04-10 14:30:05.000000 PMPrimer-1.0.6/piece/__auxiliary__.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       15 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/__init__.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    11218 2024-04-10 14:24:08.000000 PMPrimer-1.0.6/piece/piecebase.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     9104 2023-10-14 05:58:30.000000 PMPrimer-1.0.6/piece/piecedataprogress.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1328 2023-10-13 16:04:55.000000 PMPrimer-1.0.6/piece/piecedefine.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10894 2023-11-06 07:57:09.000000 PMPrimer-1.0.6/piece/piecedesign.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    19300 2024-04-10 14:22:33.000000 PMPrimer-1.0.6/piece/pieceevaluate.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    31580 2023-10-14 04:58:49.000000 PMPrimer-1.0.6/piece/piecemain.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     6819 2023-09-06 06:58:05.000000 PMPrimer-1.0.6/piece/piecentry.py
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.314145 PMPrimer-1.0.6/piece/static/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)  2920768 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/static/muscle5.1.linux_intel64
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)   832512 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/static/muscle5.1.win64.exe
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      547 2024-04-10 14:48:43.410734 PMPrimer-1.0.6/setup.cfg
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      836 2024-04-10 14:30:04.000000 PMPrimer-1.0.6/setup.py
```

### Comparing `PMPrimer-1.0.5/LICENSE` & `PMPrimer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/PKG-INFO` & `PMPrimer-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PMPrimer
-Version: 1.0.5
+Version: 1.0.6
 Summary: automated design of multiplex PCR primer pairs for diverse templates
 Home-page: https://github.com/AGIScuipeng/PMPrimer
 Author: Nerium
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `PMPrimer-1.0.5/PMPrimer.egg-info/PKG-INFO` & `PMPrimer-1.0.6/PMPrimer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PMPrimer
-Version: 1.0.5
+Version: 1.0.6
 Summary: automated design of multiplex PCR primer pairs for diverse templates
 Home-page: https://github.com/AGIScuipeng/PMPrimer
 Author: Nerium
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `PMPrimer-1.0.5/README.md` & `PMPrimer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/piece/piecebase.py` & `PMPrimer-1.0.6/piece/piecebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 创建人员: Nerium
 创建日期: 2022/08/31
 更改人员: Nerium
-更改日期: 2023/10/14
+更改日期: 2024/04/10
 '''
 
 from .piecedefine import *
 
 from collections import Counter
 import primer3
 import math
@@ -331,35 +331,35 @@
     if reverse : return [''.join(DEFAULT_DNA_REFLECT_DICT[bp] for bp in res[::-1]) for res in res_list]
     return res_list
 
 '''
 创建人员: Nerium
 创建日期: 2022/08/31
 更改人员: Nerium
-更改日期: 2022/12/09
+更改日期: 2024/04/10
 '''
 #基础模块，log等功能都在其中
 class piecebase() :
     def __init__(self, level=BASE_DEBUG_LEVEL0) -> None:
         self._level = max(BASE_DEBUG_LEVEL0, min(BASE_DEBUG_LEVEL3, level))
         self._time = str(int(time.time()))
 
     '''
     创建人员: Nerium
     创建日期: 2022/08/31
     更改人员: Nerium
-    更改日期: 2022/11/16
+    更改日期: 2024/04/10
     '''
     def baselog(self, msg, ends='\n') :
-        print(msg, end=ends)
+        print(msg, end=ends, flush=True)
 
     def debuglog(self, setlevel, msg, ends='\n') :
-        if setlevel & self._level : print('\033[0;33;40m{}\033[0m'.format(msg), end=ends)
+        if setlevel & self._level : print('\033[0;33;40m{}\033[0m'.format(msg), end=ends, flush=True)
 
     def successlog(self, msg, ends='\n') :
-        print('\033[0;32;40m{}\033[0m'.format(msg), end=ends)
+        print('\033[0;32;40m{}\033[0m'.format(msg), end=ends, flush=True)
 
     def warnlog(self, msg, ends='\n') :
-        print('\033[0;36;40m{}\033[0m'.format(msg), end=ends)
+        print('\033[0;36;40m{}\033[0m'.format(msg), end=ends, flush=True)
 
     def errorlog(self, msg, ends='\n') :
         raise SystemExit('\033[0;31;40m{}\033[0m'.format(msg))
```

### Comparing `PMPrimer-1.0.5/piece/piecedataprogress.py` & `PMPrimer-1.0.6/piece/piecedataprogress.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/piece/piecedefine.py` & `PMPrimer-1.0.6/piece/piecedefine.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/piece/piecedesign.py` & `PMPrimer-1.0.6/piece/piecedesign.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 创建日期: 2022/08/31
 更改人员: Nerium
 更改日期: 2023/03/06
 '''
 #多序列比对、保守区间遍历、PCR设计等
 class piecedesign() :
     def __init__(self, pbase, todo_path, filepath, design_opt) -> None:
+        import re
+        import os
         self._todo_path = todo_path
         self.__design_opt = design_opt
         self.__platform = platform.system()
 
         self.filepath = filepath
-        self.tmpfile_path = self.filepath.replace('.fasta', '.mc.fasta') if self.filepath is not None and '.fasta' in self.filepath else pbase.errorlog('文件路径为空，或命名错误')
-
+        self.tmpfile_path = re.sub(r"\.fasta|\.afa|\.fa", ".mc.fasta", self.filepath) if self.filepath is not None and os.path.splitext(self.filepath)[1] in [ '.fasta', '.afa', '.fa'] else pbase.errorlog('文件路径为空，或命名错误')
         self._base = pbase
 
     '''
     创建人员: Nerium
     创建日期: 2022/08/31
     更改人员: Nerium
     更改日期: 2023/03/01
```

### Comparing `PMPrimer-1.0.5/piece/pieceevaluate.py` & `PMPrimer-1.0.6/piece/pieceevaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,16 @@
                 if len({'_'.join(s.split('_')[:2]) for s in list(v)}) == 1 :
                     merge_spe_set.add('_'.join(list(v)[0].split('_')[:2]))
                 if len(v) == 1 :
                     merge_sub_set.add(list(v)[0])
 
         #在种和亚种的层次上都要统计分辨能力
         genuscnt, specnt, subcnt = len(genuset), len(speset), len(subset)
+        if genuscnt == 0 or specnt == 0 or subcnt == 0 : self._base.errorlog('Please try to maintain the format of fasta like >id genus species variant subspecies, separated by spaces, and replace the rest \
+with your content except for variant.')
         self._base.debuglog(BASE_DEBUG_LEVEL1, '属数量：{0}；物种数量：{1}；亚种数量：{2}/ Genus Number: {0}; Species Number: {1}; Subspecies Number: {2}'.format(genuscnt, specnt, subcnt))
 
         self._base.baselog('\n'.join(['{}, 有效长度 {} bp : 属 {}%; 种{:.2f}%; 亚种 {:.2f}%'.format(k, self._effective_len[k], (len(v[0])/genuscnt)*100, (len(v[1])/specnt)*100, (len(v[2])/subcnt)*100) for k, v in reso.items()]))
         self._resolution = reso; self._statistic_cnt = (genuset, speset, subset)
 
         if self.__evaluate_opt['merge'] :
             self._base.baselog('合并后物种分辨力为/ Resolution Of Amplicon After Merged：{:.2f}%'.format(len(merge_spe_set)*100/len(speset)))
```

### Comparing `PMPrimer-1.0.5/piece/piecemain.py` & `PMPrimer-1.0.6/piece/piecemain.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/piece/piecentry.py` & `PMPrimer-1.0.6/piece/piecentry.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.5/setup.cfg` & `PMPrimer-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PMPrimer
-version = 1.0.5
+version = 1.0.6
 author = Nerium
 long_description = file: README.md # 从文件中读取
 license = MIT
 url = 'https://github.com/AGIScuipeng/PMPrimer'
 classifiers = 
 	Environment :: Console
 	Operating System :: Microsoft :: Windows
```

### Comparing `PMPrimer-1.0.5/setup.py` & `PMPrimer-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PMPrimer",
-    version="1.0.5",
+    version="1.0.6",
     author="Nerium",
     description="automated design of multiplex PCR primer pairs for diverse templates",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AGIScuipeng/PMPrimer",
     packages=setuptools.find_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Environment :: Console",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
     ],
```

