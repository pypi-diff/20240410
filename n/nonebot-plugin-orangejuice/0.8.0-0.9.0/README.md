# Comparing `tmp/nonebot-plugin-orangejuice-0.8.0.tar.gz` & `tmp/nonebot-plugin-orangejuice-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-orangejuice-0.8.0.tar", last modified: Tue Apr  9 10:33:22 2024, max compression
+gzip compressed data, was "nonebot-plugin-orangejuice-0.9.0.tar", last modified: Wed Apr 10 04:04:11 2024, max compression
```

## Comparing `nonebot-plugin-orangejuice-0.8.0.tar` & `nonebot-plugin-orangejuice-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:33:22.284862 nonebot-plugin-orangejuice-0.8.0/
--rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     4959 2024-04-09 10:33:22.279861 nonebot-plugin-orangejuice-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:33:22.196580 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/
--rw-rw-rw-   0        0        0     6590 2024-04-09 10:28:03.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Card.py
--rw-rw-rw-   0        0        0      581 2024-04-09 10:25:58.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Config.py
--rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Deck.py
--rw-rw-rw-   0        0        0     1010 2024-04-09 07:53:11.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Emote.py
--rw-rw-rw-   0        0        0    10337 2024-04-09 10:22:07.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Ess.py
--rw-rw-rw-   0        0        0     5814 2024-04-09 10:24:20.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Le.py
--rw-rw-rw-   0        0        0     3044 2024-03-27 04:25:49.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Mixer.py
--rw-rw-rw-   0        0        0    12051 2024-04-09 03:16:37.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Stats.py
--rw-rw-rw-   0        0        0     2408 2024-04-09 03:50:32.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:33:22.268270 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/
--rw-rw-rw-   0        0        0     4959 2024-04-09 10:33:22.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2024-04-09 10:33:22.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:33:22.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      200 2024-04-09 10:33:22.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-09 10:33:22.000000 nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2024-04-09 03:50:27.000000 nonebot-plugin-orangejuice-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 10:33:22.284862 nonebot-plugin-orangejuice-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.774775 nonebot-plugin-orangejuice-0.9.0/
+-rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     4959 2024-04-10 04:04:11.772782 nonebot-plugin-orangejuice-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.731794 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/
+-rw-rw-rw-   0        0        0     7334 2024-04-10 04:01:14.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Card.py
+-rw-rw-rw-   0        0        0      581 2024-04-09 10:25:58.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Config.py
+-rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Deck.py
+-rw-rw-rw-   0        0        0     1010 2024-04-09 07:53:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Emote.py
+-rw-rw-rw-   0        0        0    10337 2024-04-09 10:22:07.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Ess.py
+-rw-rw-rw-   0        0        0     9075 2024-04-10 02:39:25.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Le.py
+-rw-rw-rw-   0        0        0     3044 2024-03-27 04:25:49.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Mixer.py
+-rw-rw-rw-   0        0        0    12144 2024-04-10 04:01:59.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Stats.py
+-rw-rw-rw-   0        0        0     2408 2024-04-10 04:03:49.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.769775 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/
+-rw-rw-rw-   0        0        0     4959 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      200 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-04-10 04:03:56.000000 nonebot-plugin-orangejuice-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 04:04:11.776301 nonebot-plugin-orangejuice-0.9.0/setup.cfg
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/LICENSE` & `nonebot-plugin-orangejuice-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/PKG-INFO` & `nonebot-plugin-orangejuice-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.8.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.0 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/README.md` & `nonebot-plugin-orangejuice-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Card.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import Tuple, Union
+import json
+import os
+import re
+from typing import Dict, Tuple, Union
 
 import aiomysql
 import asyncio
 from fuzzywuzzy import fuzz
 
-from nonebot import logger
+from nonebot import logger, get_driver
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, GroupMessageEvent, PrivateMessageEvent 
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 
 from .Config import plugin_config
 from .Ess import ess
 
 BaseClass = Tuple[Tuple[str, str, str, str]]
 
-tables = ['cardDeck', 'cardHyper', 'cardOther', 'unitCharacter', 'unitNPC']
+tables = ['cardDeck', 'cardHyper', 'cardOther', 'unitCharacter', 'unitNPC'] # cardBossSkill is special so not in here.
 groups = {'原版': 'ordinary', '合作': 'coop', '赏金': 'bounty', '其他': 'other'}
 
 def B2Q(string: str):
     return string.replace('~', '～').replace('&', '＆').replace('(', '（').replace(')', '）').replace('!', '！')
 
 class Card:
     def __init__(self) -> None:
@@ -35,14 +38,18 @@
         cursor = await self.db.cursor()
 
         for table in tables:
             await cursor.execute(f"SELECT i18nkey, name_, nameEn, groupData FROM {table}")
             setattr(self, table, await cursor.fetchall())
         
         self.db.close()
+        
+        regex_path = os.path.join(os.path.dirname(__file__), 'resources', 'card', 'regex.json')
+        self.regex: Dict[str, str] = json.load(open(regex_path, 'r', encoding='utf-8'))
+        
         return self
 
     async def help(self, matcher: Matcher):
         help_msg: str = '''橙汁查卡
     #card <name> [group] [table]
     查卡
     #icon <name> [group] [table]
@@ -57,64 +64,73 @@
             if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Card']:
                 return None
             args = arg.extract_plain_text().split(' ')
 
             if args == [''] or args is None or args[0] == 'help':
                 await self.help(matcher)
                 return None
-
+            
+            # input
             name = args[0]
             target_group = None
             target_table = None
+            # output
+            now_id = ''
+            now_table = ''
+            now_score = 0
 
+            # input parse
             for arg in args:
                 if arg in groups.keys():
                     target_group = groups[arg]
                 elif arg in groups.values():
                     target_group = arg
                 elif arg in tables:
                     target_table = arg
-
-            id = ''
-            now_score = 0
+            
+            for regex, key in self.regex.items():
+               if re.match(regex, name):
+                   name = key        
+            
             for table in tables:
                 if target_table and target_table != table:
                     continue
                 table_attr: BaseClass = getattr(self, table)
                 for tuple in table_attr:
                     if target_group:
                         if tuple[3] != target_group:
                             continue
                         score = max(fuzz.ratio(B2Q(name), tuple[1]), fuzz.ratio(name, tuple[2]))
                         if score > now_score:
-                            id = tuple[0]
+                            now_id = tuple[0]
                             now_table = table
                             now_score = score
                     else:
                         score = max(fuzz.ratio(B2Q(name), tuple[1]), fuzz.ratio(name, tuple[2])) + (1 if tuple[3] == 'ordinary' else 0)
                         if score > now_score:
-                            id = tuple[0]
+                            now_id = tuple[0]
                             now_table = table
                             now_score = score
             
             if now_score < plugin_config.match_score:
                 await matcher.send('没有这张卡啦~')
                 return None
 
             if now_table.startswith('unit'):
-                img = f'http://interface.100oj.com/interface/render/cardunit.php?key={id}'
+                img = f'http://interface.100oj.com/interface/render/cardunit.php?key={now_id}'
                 await matcher.send(MessageSegment.image(img))
                 return None
             else:
-                img = f'http://interface.100oj.com/interface/render/{now_table.lower()}.php?key={id}'
+                img = f'http://interface.100oj.com/interface/render/{now_table.lower()}.php?key={now_id}'
                 await matcher.send(MessageSegment.image(img))
                 return None                               
 
-        except:
-            await matcher.finish('诶鸭出错啦~')
+        except Exception as e:
+            await matcher.send('诶鸭出错啦~')
+            raise e
 
     async def icon(self, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent], arg: Message = CommandArg()) -> None:
         try:
             if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Card']:
                 return None
             args = arg.extract_plain_text().split(' ')
 
@@ -158,11 +174,17 @@
             if now_score < plugin_config.match_score:
                 await matcher.send('没有这张卡啦~')
                 return None
 
             img = f'http://interface.100oj.com/interface/util/icon.php?key={id}&size=256&lossless=true'
             await matcher.send(MessageSegment.image(img))
             return None                     
-        except:
-            await matcher.finish('诶鸭出错啦~')
-
-card = asyncio.run(Card().get_data())
+        except Exception as e:
+            await matcher.send('诶鸭出错啦~')
+            raise e
+
+card: Card = Card()
+driver = get_driver()
+
+@driver.on_startup
+async def init_card() -> None:
+    await card.get_data()
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Config.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Deck.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Deck.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Emote.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Emote.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Ess.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Ess.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Mixer.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Mixer.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/Stats.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import re
 from typing import Dict, Union
 
-from nonebot import logger
+from nonebot import logger, get_driver
 
 import asyncio
 import aiohttp
 import aiosqlite
 
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, PrivateMessageEvent, Message, MessageSegment
@@ -249,8 +249,13 @@
                         limit: str = str(min(int(args[1]), 10))
                         await self.send_stats(matcher, steam64id=steam64id, limit=limit)
                     case _:
                         await self.send_stats(matcher, steam64id=steam64id)
             case _:
                 await self.help(matcher)
 
-stats: Stats = asyncio.run(Stats().init_database())
+stats: Stats = Stats()
+driver = get_driver()
+
+@driver.on_startup
+async def init_card() -> None:
+    await stats.init_database()
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice/__init__.py` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     usage= r'See Sorabot Docs.',
     type="application",
     supported_adapters={"~onebot.v11"},
     homepage="https://github.com/FDCraft/nonebot-plugin-orangejuice",
     config=Config,
     extra={
         'author': 'Polaris_Light',
-        'version': '0.8.0',
+        'version': '0.9.0',
         'priority': 10
     }
 )
 
 import re
 
 from nonebot import on_command, on_regex
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.8.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.0 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.8.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt` & `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.8.0/pyproject.toml` & `nonebot-plugin-orangejuice-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-orangejuice"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.0.0-beta.1",
     "nonebot-plugin-apscheduler>=0.4.0",
     "cachetools>=5.0.0",
     "aiohttp>=3.8.0",
     "aiosqlite>=0.20.0",
```

