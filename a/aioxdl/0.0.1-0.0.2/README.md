# Comparing `tmp/aioxdl-0.0.1.tar.gz` & `tmp/aioxdl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.1.tar", last modified: Wed Apr 10 02:44:21 2024, max compression
+gzip compressed data, was "aioxdl-0.0.2.tar", last modified: Wed Apr 10 05:27:08 2024, max compression
```

## Comparing `aioxdl-0.0.1.tar` & `aioxdl-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:44:21.258625 aioxdl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 02:44:15.000000 aioxdl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 02:44:21.258625 aioxdl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 02:44:15.000000 aioxdl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:44:21.258625 aioxdl-0.0.1/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 02:44:15.000000 aioxdl-0.0.1/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-10 02:44:15.000000 aioxdl-0.0.1/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:44:21.258625 aioxdl-0.0.1/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 02:44:21.000000 aioxdl-0.0.1/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:44:21.258625 aioxdl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 02:44:15.000000 aioxdl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:08.667864 aioxdl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 05:27:03.000000 aioxdl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-10 05:27:08.667864 aioxdl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-10 05:27:03.000000 aioxdl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:08.663864 aioxdl-0.0.2/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 05:27:03.000000 aioxdl-0.0.2/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-10 05:27:03.000000 aioxdl-0.0.2/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:08.667864 aioxdl-0.0.2/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 05:27:08.000000 aioxdl-0.0.2/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:27:08.667864 aioxdl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 05:27:03.000000 aioxdl-0.0.2/setup.py
```

### Comparing `aioxdl-0.0.1/LICENSE` & `aioxdl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.1/PKG-INFO` & `aioxdl-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.1
+Version: 0.0.2
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,20 +22,40 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 <p align="center">
-    📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO X DL</a>
+    📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO DOWNLOADER</a>
 </p>
 
 <p align="center">
    <a href="https://telegram.me/clinton_abraham"><img src="https://img.shields.io/badge/𝑪𝒍𝒊𝒏𝒕𝒐𝒏 𝑨𝒃𝒓𝒂𝒉𝒂𝒎-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
    <a href="https://telegram.me/Space_x_bots"><img src="https://img.shields.io/badge/Sᴘᴀᴄᴇ ✗ ʙᴏᴛꜱ-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
    <a href="https://telegram.me/sources_codes"><img src="https://img.shields.io/badge/Sᴏᴜʀᴄᴇ ᴄᴏᴅᴇꜱ-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
 </p>
 
 ## INSTALLATION
 ```bash
 pip install aioxdl
 ```
+
+## USAGE
+
+```python
+import time, asyncio
+from aioxdl import Downloader
+
+async def progress(_, stime, tsize, dsize):
+	percentage = (dsize / tsize) * 100
+	print("{}%".format(round(percentage), 2))
+
+async def main():
+    core = Downloader()
+    file = "testfile.mkv"
+    link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
+    ou, _ = await core.start(link, file, progress=progress)
+    print(ou)
+
+asyncio.run(main())
+```
```

#### html2text {}

```diff
@@ -1,17 +1,22 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.1 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.2 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
-                                 ð¦ _A_I_O_ _X_ _D_L
+                              ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
-## INSTALLATION ```bash pip install aioxdl ```
+## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
+asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
+dsize): percentage = (dsize / tsize) * 100 print("{}%".format(round
+(percentage), 2)) async def main(): core = Downloader() file = "testfile.mkv"
+link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" ou, _ = await
+core.start(link, file, progress=progress) print(ou) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.1/aioxdl/module.py` & `aioxdl-0.0.2/aioxdl/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 return 200 if response.status == 200 else response.status
 
     async def display(self, progress):
         await progress(self.imesg, self.stime, self.tsize, self.dsize) if progress else None
 
 #=======================================================================================================
 
-    async def downadl(self, url, location, timeout, progress):
+    async def download(self, url, location, timeout, progress):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsize += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
                         chunks = await response.content.read(self.chunk)
                         if not chunks:
@@ -39,18 +39,18 @@
                         self.dsize += self.chunk
                         await self.display(progress)
 
                 return location
 
 #=======================================================================================================
 
-    async def download(self, url, location, timeout=1000, progress=None):
+    async def start(self, url, location, timeout=1000, progress=None):
         try:
             messages = None
-            location = await self.downadl(url, location, timeout, progress)
+            location = await self.download(url, location, timeout, progress)
         except Exception as errors:
             messages = errors
         
         return messages, location
 
 #=======================================================================================================
```

### Comparing `aioxdl-0.0.1/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.2/aioxdl.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.1
+Version: 0.0.2
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,20 +22,40 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 <p align="center">
-    📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO X DL</a>
+    📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO DOWNLOADER</a>
 </p>
 
 <p align="center">
    <a href="https://telegram.me/clinton_abraham"><img src="https://img.shields.io/badge/𝑪𝒍𝒊𝒏𝒕𝒐𝒏 𝑨𝒃𝒓𝒂𝒉𝒂𝒎-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
    <a href="https://telegram.me/Space_x_bots"><img src="https://img.shields.io/badge/Sᴘᴀᴄᴇ ✗ ʙᴏᴛꜱ-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
    <a href="https://telegram.me/sources_codes"><img src="https://img.shields.io/badge/Sᴏᴜʀᴄᴇ ᴄᴏᴅᴇꜱ-30302f?style=flat&logo=telegram" alt="telegram badge"/></a>
 </p>
 
 ## INSTALLATION
 ```bash
 pip install aioxdl
 ```
+
+## USAGE
+
+```python
+import time, asyncio
+from aioxdl import Downloader
+
+async def progress(_, stime, tsize, dsize):
+	percentage = (dsize / tsize) * 100
+	print("{}%".format(round(percentage), 2))
+
+async def main():
+    core = Downloader()
+    file = "testfile.mkv"
+    link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
+    ou, _ = await core.start(link, file, progress=progress)
+    print(ou)
+
+asyncio.run(main())
+```
```

#### html2text {}

```diff
@@ -1,17 +1,22 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.1 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.2 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
-                                 ð¦ _A_I_O_ _X_ _D_L
+                              ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
-## INSTALLATION ```bash pip install aioxdl ```
+## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
+asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
+dsize): percentage = (dsize / tsize) * 100 print("{}%".format(round
+(percentage), 2)) async def main(): core = Downloader() file = "testfile.mkv"
+link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" ou, _ = await
+core.start(link, file, progress=progress) print(ou) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.1/setup.py` & `aioxdl-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.1',
+    version='0.0.2',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     install_requires=['aiohttp'],
     long_description=long_description,
```

