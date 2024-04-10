# Comparing `tmp/nonebot_adapter_minecraft-1.0.8.post5.tar.gz` & `tmp/nonebot_adapter_minecraft-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_minecraft-1.0.8.post5.tar", max compression
+gzip compressed data, was "nonebot_adapter_minecraft-1.1.0.tar", max compression
```

## Comparing `nonebot_adapter_minecraft-1.0.8.post5.tar` & `nonebot_adapter_minecraft-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1065 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/LICENSE
--rw-r--r--   0        0        0     1693 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/README.md
--rw-r--r--   0        0        0      361 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/__init__.py
--rw-r--r--   0        0        0     8733 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/adapter.py
--rw-r--r--   0        0        0     2317 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.py
--rw-r--r--   0        0        0     1165 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.pyi
--rw-r--r--   0        0        0     3794 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/collator.py
--rw-r--r--   0        0        0      527 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/compat.py
--rw-r--r--   0        0        0      310 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/config.py
--rw-r--r--   0        0        0     1392 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/__init__.py
--rw-r--r--   0        0        0     3561 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/base.py
--rw-r--r--   0        0        0     1680 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/fabric.py
--rw-r--r--   0        0        0      951 2024-04-08 12:41:06.956018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/forge.py
--rw-r--r--   0        0        0      604 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/minecraft.py
--rw-r--r--   0        0        0     1775 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/spigot.py
--rw-r--r--   0        0        0     2138 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/exception.py
--rw-r--r--   0        0        0     4844 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/message.py
--rw-r--r--   0        0        0     5468 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/model.py
--rw-r--r--   0        0        0     1008 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/utils.py
--rw-r--r--   0        0        0     1549 2024-04-08 12:41:06.960018 nonebot_adapter_minecraft-1.0.8.post5/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.0.8.post5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1693 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/README.md
+-rw-r--r--   0        0        0      386 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/__init__.py
+-rw-r--r--   0        0        0     8733 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/adapter.py
+-rw-r--r--   0        0        0     2317 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.py
+-rw-r--r--   0        0        0     1165 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.pyi
+-rw-r--r--   0        0        0     3794 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/collator.py
+-rw-r--r--   0        0        0      527 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/compat.py
+-rw-r--r--   0        0        0      310 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/config.py
+-rw-r--r--   0        0        0     1392 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/__init__.py
+-rw-r--r--   0        0        0     3621 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/base.py
+-rw-r--r--   0        0        0     1578 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/fabric.py
+-rw-r--r--   0        0        0     1424 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/forge.py
+-rw-r--r--   0        0        0      598 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/minecraft.py
+-rw-r--r--   0        0        0     1818 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/spigot.py
+-rw-r--r--   0        0        0     2138 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/exception.py
+-rw-r--r--   0        0        0     4844 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/message.py
+-rw-r--r--   0        0        0     5468 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/model.py
+-rw-r--r--   0        0        0      366 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/permission.py
+-rw-r--r--   0        0        0     1008 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/utils.py
+-rw-r--r--   0        0        0     1543 2024-04-10 14:17:18.949326 nonebot_adapter_minecraft-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.1.0/PKG-INFO
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/LICENSE` & `nonebot_adapter_minecraft-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/README.md` & `nonebot_adapter_minecraft-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/adapter.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/bot.pyi` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/collator.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/compat.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/__init__.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/base.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from nonebot.typing import overrides
 from pydantic import BaseModel
 
 from ..message import Message
 
 
 class Event(BaseEvent):
+    """事件基类"""
     timestamp: int
     post_type: str
     event_name: str
     server_name: str
     sub_type: str
 
     @overrides(BaseEvent)
@@ -50,16 +51,17 @@
 
         class Config(ConfigDict):
             extra = "allow"
 
 
 # Models
 class BasePlayer(BaseModel):
-    # 玩家信息
+    """玩家基类"""
     nickname: str
+    is_op: Optional[bool] = None
 
     if PYDANTIC_V2:
         model_config = ConfigDict(extra="allow")
     else:
 
         class Config(ConfigDict):
             extra = "allow"
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/fabric.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/fabric.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,39 +27,39 @@
     is_sneaking: Optional[bool] = None
     is_sleeping: Optional[bool] = None
     is_climbing: Optional[bool] = None
     is_swimming: Optional[bool] = None
 
 
 class ServerMessageEvent(BaseChatEvent):
-    """Fabric FabricServerMessageEvent API"""
+    """Fabric 聊天事件"""
 
-    event_name: Literal["FabricServerMessageEvent"]
+    event_name: Literal["ServerMessageEvent"]
     player: Player
 
 
 class ServerCommandMessageEvent(BasePlayerCommandEvent):
-    """Fabric FabricServerCommandMessageEvent API"""
+    """Fabric 玩家命令事件"""
 
-    event_name: Literal["FabricServerCommandMessageEvent"]
+    event_name: Literal["ServerCommandMessageEvent"]
     player: Player
 
 
 class ServerLivingEntityAfterDeathEvent(BaseDeathEvent):
-    """Fabric FabricServerLivingEntityAfterDeathEvent API"""
+    """ServerLivingEntityAfterDeathEvent API"""
 
-    event_name: Literal["FabricServerLivingEntityAfterDeathEvent"]
+    event_name: Literal["ServerLivingEntityAfterDeathEvent"]
     player: Player
 
 
 class ServerPlayConnectionJoinEvent(BaseJoinEvent):
-    """Fabric FabricServerPlayConnectionJoinEvent API"""
+    """ServerPlayConnectionJoinEvent API"""
 
-    event_name: Literal["FabricServerPlayConnectionJoinEvent"]
+    event_name: Literal["ServerPlayConnectionJoinEvent"]
     player: Player
 
 
 class ServerPlayConnectionDisconnectEvent(BaseQuitEvent):
-    """Fabric FabricServerPlayConnectionDisconnectEvent API"""
+    """ServerPlayConnectionDisconnectEvent API"""
 
-    event_name: Literal["FabricServerPlayConnectionDisconnectEvent"]
+    event_name: Literal["ServerPlayConnectionDisconnectEvent"]
     player: Player
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/minecraft.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/minecraft.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 
 from .base import BasePlayer, BaseChatEvent, BaseJoinEvent, BaseQuitEvent
 
 
 class Player(BasePlayer):
-    """原版 玩家信息"""
+    """原版 Player"""
 
 
 class PlayerChatEvent(BaseChatEvent):
     """原版 玩家聊天事件"""
 
     event_name: Literal["MinecraftPlayerChatEvent"]
     player: Player
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/event/spigot.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/spigot.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from .base import (
     BasePlayer,
     BaseChatEvent,
     BaseJoinEvent,
     BaseQuitEvent,
     BaseDeathEvent,
-    BasePlayerCommandEvent
+    BasePlayerCommandEvent,
 )
 
 
 class Player(BasePlayer):
-    """玩家信息"""
+    """Spigot Player"""
+
     uuid: Optional[str] = None
     display_name: Optional[str] = None
     player_list_name: Optional[str] = None
     is_health_scaled: Optional[bool] = None
     address: Optional[str] = None
     is_sprinting: Optional[bool] = None
     walk_speed: Optional[float] = None
@@ -33,34 +34,39 @@
     total_exp: Optional[int] = None
     player_time: Optional[int] = None
     is_player_time_relative: Optional[bool] = None
     is_op: Optional[bool] = None
 
 
 class AsyncPlayerChatEvent(BaseChatEvent):
-    """聊天事件"""
+    """Spigot 聊天事件"""
+
     event_name: Literal["AsyncPlayerChatEvent"]
     player: Player
 
 
 class PlayerCommandPreprocessEvent(BasePlayerCommandEvent):
-    """玩家命令事件"""
+    """Spigot 玩家命令事件"""
+
     event_name: Literal["PlayerCommandPreprocessEvent"]
     player: Player
 
 
 class PlayerDeathEvent(BaseDeathEvent):
-    """玩家死亡事件"""
+    """Spigot 玩家死亡事件"""
+
     event_name: Literal["PlayerDeathEvent"]
     player: Player
 
 
 class PlayerJoinEvent(BaseJoinEvent):
-    """玩家加入事件"""
+    """Spigot 玩家加入事件"""
+
     event_name: Literal["PlayerJoinEvent"]
     player: Player
 
 
 class PlayerQuitEvent(BaseQuitEvent):
-    """玩家离开事件"""
+    """Spigot 玩家离开事件"""
+
     event_name: Literal["PlayerQuitEvent"]
     player: Player
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/exception.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/message.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/model.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/nonebot/adapters/minecraft/utils.py` & `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/pyproject.toml` & `nonebot_adapter_minecraft-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-minecraft"
-version = "1.0.8.post5"
+version = "1.1.0"
 description = "NoneBot2与MineCraft Server互通的适配器。"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post5/PKG-INFO` & `nonebot_adapter_minecraft-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-minecraft
-Version: 1.0.8.post5
+Version: 1.1.0
 Summary: NoneBot2与MineCraft Server互通的适配器。
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

