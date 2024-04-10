# Comparing `tmp/nonebot_plugin_callapi-0.2.0.tar.gz` & `tmp/nonebot_plugin_callapi-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_callapi-0.2.0.tar", last modified: Sun Mar 10 10:47:58 2024, max compression
+gzip compressed data, was "nonebot_plugin_callapi-0.2.0.post1.tar", last modified: Wed Apr 10 14:15:33 2024, max compression
```

## Comparing `nonebot_plugin_callapi-0.2.0.tar` & `nonebot_plugin_callapi-0.2.0.post1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-03-10 10:47:47.247563 nonebot_plugin_callapi-0.2.0/LICENSE
--rw-r--r--   0        0        0     4980 2024-03-10 10:47:47.247563 nonebot_plugin_callapi-0.2.0/README.md
--rw-r--r--   0        0        0      530 2024-03-10 10:47:47.247563 nonebot_plugin_callapi-0.2.0/nonebot_plugin_callapi/__init__.py
--rw-r--r--   0        0        0     7710 2024-03-10 10:47:47.247563 nonebot_plugin_callapi-0.2.0/nonebot_plugin_callapi/__main__.py
--rw-r--r--   0        0        0      172 2024-03-10 10:47:47.247563 nonebot_plugin_callapi-0.2.0/nonebot_plugin_callapi/config.py
--rw-r--r--   0        0        0      682 2024-03-10 10:47:58.527624 nonebot_plugin_callapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-10 14:15:20.990566 nonebot_plugin_callapi-0.2.0.post1/LICENSE
+-rw-r--r--   0        0        0     4804 2024-04-10 14:15:20.990566 nonebot_plugin_callapi-0.2.0.post1/README.md
+-rw-r--r--   0        0        0      616 2024-04-10 14:15:20.990566 nonebot_plugin_callapi-0.2.0.post1/nonebot_plugin_callapi/__init__.py
+-rw-r--r--   0        0        0     7710 2024-04-10 14:15:20.990566 nonebot_plugin_callapi-0.2.0.post1/nonebot_plugin_callapi/__main__.py
+-rw-r--r--   0        0        0      172 2024-04-10 14:15:20.990566 nonebot_plugin_callapi-0.2.0.post1/nonebot_plugin_callapi/config.py
+-rw-r--r--   0        0        0      685 2024-04-10 14:15:33.906727 nonebot_plugin_callapi-0.2.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.2.0.post1/PKG-INFO
```

### Comparing `nonebot_plugin_callapi-0.2.0/LICENSE` & `nonebot_plugin_callapi-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.2.0/README.md` & `nonebot_plugin_callapi-0.2.0.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -147,23 +147,17 @@
 
 ### [felinae98/nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere)
 
 多适配器消息发送支持（本插件用来发送图片）
 
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
@@ -31,15 +31,13 @@
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ITCraftDevelopmentTeam/XDbot2](https://github.com/
 ITCraftDevelopmentTeam/XDbot2) åè½å¯å ### [MeetWq/pil-utils](https://
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¢ç¨ alconna ### 0.1.3 - å é¤æä»¶èªèº«å¯¹ Telegram
-æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡ ### 0.1.2
-- ð NoneBot 2.0 ð ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
-æªåè½¬ä¹å¤ççé®é¢
+**[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 - æ¢ç¨ alconna ###
+0.1.3 - å é¤æä»¶èªèº«å¯¹ Telegram æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé
+Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡ ### 0.1.2 - ð NoneBot 2.0 ð ### 0.1.1 -
+ä¿®å¤ææ¬ç±» Segment æªåè½¬ä¹å¤ççé®é¢
```

### Comparing `nonebot_plugin_callapi-0.2.0/nonebot_plugin_callapi/__init__.py` & `nonebot_plugin_callapi-0.2.0.post1/nonebot_plugin_callapi/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from nonebot.plugin import PluginMetadata, require
+from nonebot.plugin import PluginMetadata, inherit_supported_adapters, require
 
-require("nonebot_plugin_saa")
+require("nonebot_plugin_alconna")
 
 from .__main__ import HELP_TEXT  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.0"
+__version__ = "0.2.0.post1"
 __plugin_meta__ = PluginMetadata(
     name="CallAPI",
     description="使用指令来调用 Bot 的 API",
     usage=HELP_TEXT,
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-callapi",
     type="application",
     config=ConfigModel,
-    supported_adapters=None,
+    supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
     extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_callapi-0.2.0/nonebot_plugin_callapi/__main__.py` & `nonebot_plugin_callapi-0.2.0.post1/nonebot_plugin_callapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.2.0/pyproject.toml` & `nonebot_plugin_callapi-0.2.0.post1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 dynamic = []
 description = "Use bot command to call its API"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
-    "nonebot-plugin-alconna>=0.40.0rc1",
+    "nonebot-plugin-alconna>=0.40.1",
     "Pygments>=2.15.1",
     "pil-utils>=0.1.7",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.0.post1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-callapi"
```

### Comparing `nonebot_plugin_callapi-0.2.0/PKG-INFO` & `nonebot_plugin_callapi-0.2.0.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-callapi
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: Use bot command to call its API
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1
+Requires-Dist: nonebot-plugin-alconna>=0.40.1
 Requires-Dist: Pygments>=2.15.1
 Requires-Dist: pil-utils>=0.1.7
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
@@ -162,23 +162,17 @@
 
 ### [felinae98/nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere)
 
 多适配器消息发送支持（本插件用来发送图片）
 
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
-Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.2.0 Summary: Use
-bot command to call its API Home-page: https://github.com/lgc-NB2Dev/nonebot-
-plugin-callapi Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.2.0.post1
+Summary: Use bot command to call its API Home-page: https://github.com/lgc-
+NB2Dev/nonebot-plugin-callapi Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-callapi Requires-Python: <4.0,>=3.9 Requires-Dist:
-nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1 Requires-Dist:
+nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.1 Requires-Dist:
 Pygments>=2.15.1 Requires-Dist: pil-utils>=0.1.7 Description-Content-Type:
 text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # NoneBot-Plugin-CallAPI _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_[python]
                             _[_p_d_m_-_m_a_n_a_g_e_d_]_[_w_a_k_a_t_i_m_e_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
@@ -39,15 +39,13 @@
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ITCraftDevelopmentTeam/XDbot2](https://github.com/
 ITCraftDevelopmentTeam/XDbot2) åè½å¯å ### [MeetWq/pil-utils](https://
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¢ç¨ alconna ### 0.1.3 - å é¤æä»¶èªèº«å¯¹ Telegram
-æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡ ### 0.1.2
-- ð NoneBot 2.0 ð ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
-æªåè½¬ä¹å¤ççé®é¢
+**[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 - æ¢ç¨ alconna ###
+0.1.3 - å é¤æä»¶èªèº«å¯¹ Telegram æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé
+Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡ ### 0.1.2 - ð NoneBot 2.0 ð ### 0.1.1 -
+ä¿®å¤ææ¬ç±» Segment æªåè½¬ä¹å¤ççé®é¢
```

