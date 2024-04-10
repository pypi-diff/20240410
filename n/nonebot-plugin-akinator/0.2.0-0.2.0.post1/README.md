# Comparing `tmp/nonebot_plugin_akinator-0.2.0.tar.gz` & `tmp/nonebot_plugin_akinator-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_akinator-0.2.0.tar", last modified: Sun Mar 10 11:36:10 2024, max compression
+gzip compressed data, was "nonebot_plugin_akinator-0.2.0.post1.tar", last modified: Wed Apr 10 14:25:18 2024, max compression
```

## Comparing `nonebot_plugin_akinator-0.2.0.tar` & `nonebot_plugin_akinator-0.2.0.post1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1069 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/LICENSE
--rw-r--r--   0        0        0     4843 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/README.md
--rw-r--r--   0        0        0      672 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/__init__.py
--rw-r--r--   0        0        0     3428 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/__main__.py
--rw-r--r--   0        0        0       39 2024-03-10 11:35:59.452026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.git
--rw-r--r--   0        0        0     1873 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      200 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1103 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      749 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1128 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1799 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.gitignore
--rw-r--r--   0        0        0      173 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.readthedocs.yml
--rw-r--r--   0        0        0     5328 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1082 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/LICENSE
--rw-r--r--   0        0        0       34 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/MANIFEST.in
--rw-r--r--   0        0        0     1994 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/README.rst
--rw-r--r--   0        0        0      380 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/__init__.py
--rw-r--r--   0        0        0    12713 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/akinator.py
--rw-r--r--   0        0        0      356 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
--rw-r--r--   0        0        0    14076 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
--rw-r--r--   0        0        0     2526 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/exceptions.py
--rw-r--r--   0        0        0     5761 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/utils.py
--rw-r--r--   0        0        0      321 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/docs/conf.py
--rw-r--r--   0        0        0    11653 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/docs/index.rst
--rw-r--r--   0        0        0        6 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/docs/requirements.txt
--rw-r--r--   0        0        0      620 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/examples/aki.py
--rw-r--r--   0        0        0      907 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/examples/async_aki.py
--rw-r--r--   0        0        0      681 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/pyproject.toml
--rw-r--r--   0        0        0       18 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/requirements.txt
--rw-r--r--   0        0        0     1437 2024-03-10 11:35:59.460026 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/setup.py
--rw-r--r--   0        0        0      277 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/config.py
--rw-r--r--   0        0        0    10536 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/game.py
--rw-r--r--   0        0        0    11528 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/bg.jpg
--rw-r--r--   0        0        0    43524 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/concentration_intense.webp
--rw-r--r--   0        0        0    46462 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/confiant.webp
--rw-r--r--   0        0        0    45550 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/etonnement.webp
--rw-r--r--   0        0        0    49318 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/inspiration_forte.webp
--rw-r--r--   0        0        0    45300 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/inspiration_legere.webp
--rw-r--r--   0        0        0    50740 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/leger_decouragement.webp
--rw-r--r--   0        0        0    40432 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/mobile.webp
--rw-r--r--   0        0        0    36506 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/serein.webp
--rw-r--r--   0        0        0    45464 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/surprise.webp
--rw-r--r--   0        0        0    42668 2024-03-10 11:35:58.816029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/tension.webp
--rw-r--r--   0        0        0    54230 2024-03-10 11:35:58.820029 nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/vrai_decouragement.webp
--rw-r--r--   0        0        0      801 2024-03-10 11:36:10.491980 nonebot_plugin_akinator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 nonebot_plugin_akinator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/LICENSE
+-rw-r--r--   0        0        0     4661 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/README.md
+-rw-r--r--   0        0        0      727 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/__init__.py
+-rw-r--r--   0        0        0     3428 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/__main__.py
+-rw-r--r--   0        0        0       39 2024-04-10 14:25:01.706462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.git
+-rw-r--r--   0        0        0     1873 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      200 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1103 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      749 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1128 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1799 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.gitignore
+-rw-r--r--   0        0        0      173 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.readthedocs.yml
+-rw-r--r--   0        0        0     5328 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1082 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/LICENSE
+-rw-r--r--   0        0        0       34 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/MANIFEST.in
+-rw-r--r--   0        0        0     1994 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/README.rst
+-rw-r--r--   0        0        0      380 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/__init__.py
+-rw-r--r--   0        0        0    12713 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/akinator.py
+-rw-r--r--   0        0        0      356 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
+-rw-r--r--   0        0        0    14076 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
+-rw-r--r--   0        0        0     2526 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/exceptions.py
+-rw-r--r--   0        0        0     5761 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/utils.py
+-rw-r--r--   0        0        0      321 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/docs/conf.py
+-rw-r--r--   0        0        0    11653 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/docs/index.rst
+-rw-r--r--   0        0        0        6 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/docs/requirements.txt
+-rw-r--r--   0        0        0      620 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/examples/aki.py
+-rw-r--r--   0        0        0      907 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/examples/async_aki.py
+-rw-r--r--   0        0        0      681 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/requirements.txt
+-rw-r--r--   0        0        0     1437 2024-04-10 14:25:01.714462 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/setup.py
+-rw-r--r--   0        0        0      277 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/config.py
+-rw-r--r--   0        0        0    10536 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/game.py
+-rw-r--r--   0        0        0    11528 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/bg.jpg
+-rw-r--r--   0        0        0    43524 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/concentration_intense.webp
+-rw-r--r--   0        0        0    46462 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/confiant.webp
+-rw-r--r--   0        0        0    45550 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/etonnement.webp
+-rw-r--r--   0        0        0    49318 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/inspiration_forte.webp
+-rw-r--r--   0        0        0    45300 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/inspiration_legere.webp
+-rw-r--r--   0        0        0    50740 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/leger_decouragement.webp
+-rw-r--r--   0        0        0    40432 2024-04-10 14:25:01.306460 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/mobile.webp
+-rw-r--r--   0        0        0    36506 2024-04-10 14:25:01.310459 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/serein.webp
+-rw-r--r--   0        0        0    45464 2024-04-10 14:25:01.310459 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/surprise.webp
+-rw-r--r--   0        0        0    42668 2024-04-10 14:25:01.310459 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/tension.webp
+-rw-r--r--   0        0        0    54230 2024-04-10 14:25:01.310459 nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/vrai_decouragement.webp
+-rw-r--r--   0        0        0      804 2024-04-10 14:25:18.734578 nonebot_plugin_akinator-0.2.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 nonebot_plugin_akinator-0.2.0.post1/PKG-INFO
```

### Comparing `nonebot_plugin_akinator-0.2.0/LICENSE` & `nonebot_plugin_akinator-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/README.md` & `nonebot_plugin_akinator-0.2.0.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -147,23 +147,17 @@
 
 ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils/)
 
 - Pillow 工具库
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
-
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
-
-  </details>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 换用 alconna
```

#### html2text {}

```diff
@@ -26,14 +26,13 @@
 NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text]
 (https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/
 QQ%E5%9B%BE%E7%89%8720230415063607.png) ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [Infiniticity/akinator.py](https://github.com/
 Infiniticity/akinator.py) - Akinator API çå°è£ ### [MeetWq/pil-utils]
-(https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¢ç¨ alconna ### 0.1.3 - æ¯ææ´å¤å¹³å° -
+(https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå© **
+[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 - æ¢ç¨ alconna ###
+0.1.3 - æ¯ææ´å¤å¹³å° -
 å é¤çåºè§è²åç»§ç»­ççåè½ï¼å ä¸ºæ Bug
```

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/__init__.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_session")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.0"
+__version__ = "0.2.0.post1"
 __plugin_meta__ = PluginMetadata(
     name="Akinator",
     description="网络天才",
     usage="使用 `akinator` 指令开始让我猜人物吧！",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-akinator",
     type="application",
     config=ConfigModel,
-    supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
+    supported_adapters=inherit_supported_adapters(
+        "nonebot_plugin_alconna",
+        "nonebot_plugin_session",
+    ),
     extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/__main__.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/.gitignore` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/LICENSE` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/README.rst` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/akinator.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/exceptions.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/exceptions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/akinator/utils.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/akinator/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/docs/index.rst` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/examples/aki.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/examples/aki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/examples/async_aki.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/examples/async_aki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/pyproject.toml` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/akinator/setup.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/akinator/setup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/game.py` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/bg.jpg` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/concentration_intense.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/concentration_intense.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/confiant.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/confiant.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/etonnement.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/etonnement.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/inspiration_forte.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/inspiration_forte.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/inspiration_legere.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/inspiration_legere.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/leger_decouragement.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/leger_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/mobile.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/mobile.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/serein.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/serein.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/surprise.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/surprise.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/tension.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/tension.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/nonebot_plugin_akinator/res/vrai_decouragement.webp` & `nonebot_plugin_akinator-0.2.0.post1/nonebot_plugin_akinator/res/vrai_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_akinator-0.2.0/pyproject.toml` & `nonebot_plugin_akinator-0.2.0.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 dynamic = []
 description = "Internet Genius - Akinator"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
-    "nonebot-plugin-alconna>=0.40.0rc1",
+    "nonebot-plugin-alconna>=0.40.1",
     "nonebot-plugin-session>=0.1.0",
     "aiohttp>=3.8.4",
     "pil-utils>=0.1.6",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.0.post1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc2333/nonebot-plugin-akinator"
```

### Comparing `nonebot_plugin_akinator-0.2.0/PKG-INFO` & `nonebot_plugin_akinator-0.2.0.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-akinator
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: Internet Genius - Akinator
 Home-page: https://github.com/lgc2333/nonebot-plugin-akinator
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc2333/nonebot-plugin-akinator
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1
+Requires-Dist: nonebot-plugin-alconna>=0.40.1
 Requires-Dist: nonebot-plugin-session>=0.1.0
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pil-utils>=0.1.6
 Requires-Dist: aiodns>=3.0.0; extra == "extra"
 Requires-Dist: cchardet>=2.1.7; extra == "extra"
 Provides-Extra: extra
 Description-Content-Type: text/markdown
@@ -166,23 +166,17 @@
 
 ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils/)
 
 - Pillow 工具库
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
-
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
-
-  </details>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 换用 alconna
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.2.0 Summary:
-Internet Genius - Akinator Home-page: https://github.com/lgc2333/nonebot-
-plugin-akinator Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.2.0.post1
+Summary: Internet Genius - Akinator Home-page: https://github.com/lgc2333/
+nonebot-plugin-akinator Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc2333/
 nonebot-plugin-akinator Requires-Python: <4.0,>=3.9 Requires-Dist:
-nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1 Requires-Dist:
+nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.1 Requires-Dist:
 nonebot-plugin-session>=0.1.0 Requires-Dist: aiohttp>=3.8.4 Requires-Dist: pil-
 utils>=0.1.6 Requires-Dist: aiodns>=3.0.0; extra == "extra" Requires-Dist:
 cchardet>=2.1.7; extra == "extra" Provides-Extra: extra Description-Content-
 Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # NoneBot-Plugin-Akinator _â¨ ç½ç»å¤©æ â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]_[_w_a_k_a_t_i_m_e_]
@@ -36,14 +36,13 @@
 NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text]
 (https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/
 QQ%E5%9B%BE%E7%89%8720230415063607.png) ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [Infiniticity/akinator.py](https://github.com/
 Infiniticity/akinator.py) - Akinator API çå°è£ ### [MeetWq/pil-utils]
-(https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¢ç¨ alconna ### 0.1.3 - æ¯ææ´å¤å¹³å° -
+(https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå© **
+[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 - æ¢ç¨ alconna ###
+0.1.3 - æ¯ææ´å¤å¹³å° -
 å é¤çåºè§è²åç»§ç»­ççåè½ï¼å ä¸ºæ Bug
```

