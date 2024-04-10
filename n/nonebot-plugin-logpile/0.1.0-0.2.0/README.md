# Comparing `tmp/nonebot-plugin-logpile-0.1.0.tar.gz` & `tmp/nonebot-plugin-logpile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-logpile-0.1.0.tar", last modified: Tue May  9 20:58:15 2023, max compression
+gzip compressed data, was "nonebot-plugin-logpile-0.2.0.tar", last modified: Wed Apr 10 13:55:12 2024, max compression
```

## Comparing `nonebot-plugin-logpile-0.1.0.tar` & `nonebot-plugin-logpile-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-05-09 20:58:08.641753 nonebot-plugin-logpile-0.1.0/LICENSE
--rw-r--r--   0        0        0     2342 2023-05-09 20:58:08.641753 nonebot-plugin-logpile-0.1.0/README.md
--rw-r--r--   0        0        0      930 2023-05-09 20:58:08.641753 nonebot-plugin-logpile-0.1.0/nonebot_plugin_logpile/__init__.py
--rw-r--r--   0        0        0      634 2023-05-09 20:58:08.641753 nonebot-plugin-logpile-0.1.0/nonebot_plugin_logpile/config.py
--rw-r--r--   0        0        0      535 2023-05-09 20:58:08.641753 nonebot-plugin-logpile-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 nonebot-plugin-logpile-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-10 13:55:09.684780 nonebot-plugin-logpile-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2342 2024-04-10 13:55:09.684780 nonebot-plugin-logpile-0.2.0/README.md
+-rw-r--r--   0        0        0     1187 2024-04-10 13:55:09.684780 nonebot-plugin-logpile-0.2.0/nonebot_plugin_logpile/__init__.py
+-rw-r--r--   0        0        0      635 2024-04-10 13:55:09.684780 nonebot-plugin-logpile-0.2.0/nonebot_plugin_logpile/config.py
+-rw-r--r--   0        0        0      535 2024-04-10 13:55:09.684780 nonebot-plugin-logpile-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 nonebot-plugin-logpile-0.2.0/PKG-INFO
```

### Comparing `nonebot-plugin-logpile-0.1.0/LICENSE` & `nonebot-plugin-logpile-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-logpile-0.1.0/README.md` & `nonebot-plugin-logpile-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,9 +69,9 @@
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | logpile_path | 否 | `cwd/log` | 日志文件保存路径，默认保存在当前工作目录下的 `log` 文件夹中 |
-| logpile_level | 否 | ERROR | 日志保存等级，可以为列表或者字符串。如果是字符串，那么保存当前等级及以下所有等级的日志，否则只保存列表中的等级 |
+| logpile_level | 否 | ERROR | 日志保存等级，可以为列表或者字符串。如果是字符串，那么保存当前等级及以上所有等级的日志，否则只保存列表中的等级 |
 | logpile_retention | 否 | 14 | 日志文件保留时长，默认保留14天，自动清理过期日志 |
```

#### html2text {}

```diff
@@ -11,10 +11,10 @@
 logpile æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_logpile"] ##
 âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | logpile_path | å¦ |
 `cwd/log` | æ¥å¿æä»¶ä¿å­è·¯å¾ï¼é»è®¤ä¿å­å¨å½åå·¥ä½ç®å½ä¸ç
 `log` æä»¶å¤¹ä¸­ | | logpile_level | å¦ | ERROR |
-æ¥å¿ä¿å­ç­çº§ï¼å¯ä»¥ä¸ºåè¡¨æèå­ç¬¦ä¸²ãå¦ææ¯å­ç¬¦ä¸²ï¼é£ä¹ä¿å­å½åç­çº§åä»¥ä¸ææç­çº§çæ¥å¿ï¼å¦ååªä¿å­åè¡¨ä¸­çç­çº§
+æ¥å¿ä¿å­ç­çº§ï¼å¯ä»¥ä¸ºåè¡¨æèå­ç¬¦ä¸²ãå¦ææ¯å­ç¬¦ä¸²ï¼é£ä¹ä¿å­å½åç­çº§åä»¥ä¸ææç­çº§çæ¥å¿ï¼å¦ååªä¿å­åè¡¨ä¸­çç­çº§
 | | logpile_retention | å¦ | 14 |
 æ¥å¿æä»¶ä¿çæ¶é¿ï¼é»è®¤ä¿ç14å¤©ï¼èªå¨æ¸çè¿ææ¥å¿ |
```

### Comparing `nonebot-plugin-logpile-0.1.0/nonebot_plugin_logpile/__init__.py` & `nonebot-plugin-logpile-0.2.0/nonebot_plugin_logpile/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-from datetime import datetime
-from typing import Any, Dict, List, Tuple, Union, get_args
+from typing import Any, Dict, List, Tuple, Union
 
-from nonebot import get_driver, logger
+from nonebot import get_plugin_config, logger
+from nonebot.plugin import PluginMetadata
 
 from .config import Config, LevelName
 
-pc = Config.parse_obj(get_driver().config)
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-logpile",
+    description="将 nonebot 的日志记录保存到本地文件",
+    usage="",
+    config=Config,
+)
+pc = get_plugin_config(Config)
 
 LOG_CONFIG = {
     "rotation": "00:00",
     "enqueue": True,
     "encoding": "utf-8",
     "retention": f"{pc.logpile_retention} days",
 }
 
 
 def file_handler(
     levels: Union[LevelName, Tuple[LevelName]],
 ) -> List[Dict[str, Any]]:
-    if not isinstance(levels, tuple):
-        level_names = get_args(LevelName)
-        minimum = level_names.index(levels)
-        levels = level_names[minimum:]
+    if isinstance(levels, str):
+        return [
+            {
+                "sink": pc.logpile_path / "{time:YYYY-MM-DD}.log",
+                "level": levels,
+                **LOG_CONFIG,
+            }
+        ]
     return [
         {
-            "sink": pc.logpile_path
-            / level.lower()
-            / f"{level.lower()}-{datetime.now().date()}.log",
+            "sink": pc.logpile_path / level.lower() / "{time:YYYY-MM-DD}.log",
             "level": level,
+            "filter": lambda record, level=level: record["level"].name == level,
             **LOG_CONFIG,
         }
         for level in levels
     ]
 
 
 for handler in file_handler(pc.logpile_level):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot-plugin-logpile-0.1.0/nonebot_plugin_logpile/config.py` & `nonebot-plugin-logpile-0.2.0/nonebot_plugin_logpile/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pydantic import BaseModel, Extra, validator
 
 LevelName = Literal["TRACE", "DEBUG", "INFO", "SUCCESS", "WARNING", "ERROR", "CRITICAL"]
 
 
 class Config(BaseModel, extra=Extra.ignore):
-    logpile_path: Path = Path.cwd() / "log"
+    logpile_path: Path = Path.cwd() / "logs"
     logpile_level: Union[LevelName, Tuple[LevelName]] = "ERROR"
     logpile_retention: int = 14
 
     @validator("logpile_path")
     def check_path(cls, v: Path) -> Path:
         if v.exists() and not v.is_dir():
             raise ValueError("必须是有效的文件目录")
```

### Comparing `nonebot-plugin-logpile-0.1.0/PKG-INFO` & `nonebot-plugin-logpile-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-logpile
-Version: 0.1.0
+Version: 0.2.0
 Summary: NoneBot2 local log files
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/A-kirami/nonebot-plugin-logpile
 Project-URL: Repository, https://github.com/A-kirami/nonebot-plugin-logpile
 Description-Content-Type: text/markdown
@@ -80,10 +80,10 @@
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | logpile_path | 否 | `cwd/log` | 日志文件保存路径，默认保存在当前工作目录下的 `log` 文件夹中 |
-| logpile_level | 否 | ERROR | 日志保存等级，可以为列表或者字符串。如果是字符串，那么保存当前等级及以下所有等级的日志，否则只保存列表中的等级 |
+| logpile_level | 否 | ERROR | 日志保存等级，可以为列表或者字符串。如果是字符串，那么保存当前等级及以上所有等级的日志，否则只保存列表中的等级 |
 | logpile_retention | 否 | 14 | 日志文件保留时长，默认保留14天，自动清理过期日志 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-logpile Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-logpile Version: 0.2.0 Summary:
 NoneBot2 local log files License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 A-kirami/nonebot-plugin-logpile Project-URL: Repository, https://github.com/A-
 kirami/nonebot-plugin-logpile Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-logpile _â¨ æ¬å°æ¥å¿ä¿å­ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -16,10 +16,10 @@
 logpile æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_logpile"] ##
 âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | logpile_path | å¦ |
 `cwd/log` | æ¥å¿æä»¶ä¿å­è·¯å¾ï¼é»è®¤ä¿å­å¨å½åå·¥ä½ç®å½ä¸ç
 `log` æä»¶å¤¹ä¸­ | | logpile_level | å¦ | ERROR |
-æ¥å¿ä¿å­ç­çº§ï¼å¯ä»¥ä¸ºåè¡¨æèå­ç¬¦ä¸²ãå¦ææ¯å­ç¬¦ä¸²ï¼é£ä¹ä¿å­å½åç­çº§åä»¥ä¸ææç­çº§çæ¥å¿ï¼å¦ååªä¿å­åè¡¨ä¸­çç­çº§
+æ¥å¿ä¿å­ç­çº§ï¼å¯ä»¥ä¸ºåè¡¨æèå­ç¬¦ä¸²ãå¦ææ¯å­ç¬¦ä¸²ï¼é£ä¹ä¿å­å½åç­çº§åä»¥ä¸ææç­çº§çæ¥å¿ï¼å¦ååªä¿å­åè¡¨ä¸­çç­çº§
 | | logpile_retention | å¦ | 14 |
 æ¥å¿æä»¶ä¿çæ¶é¿ï¼é»è®¤ä¿ç14å¤©ï¼èªå¨æ¸çè¿ææ¥å¿ |
```

