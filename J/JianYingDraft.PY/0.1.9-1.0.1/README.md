# Comparing `tmp/jianyingdraft_py-0.1.9.tar.gz` & `tmp/jianyingdraft_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianyingdraft_py-0.1.9.tar", max compression
+gzip compressed data, was "jianyingdraft_py-1.0.1.tar", max compression
```

## Comparing `jianyingdraft_py-0.1.9.tar` & `jianyingdraft_py-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.9/JianYingDraft/__init__.py
--rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-0.1.9/JianYingDraft/core/__init__.py
--rw-r--r--   0        0        0     9306 2024-03-30 11:43:51.292222 jianyingdraft_py-0.1.9/JianYingDraft/core/draft.py
--rw-r--r--   0        0        0     7174 2024-03-29 05:25:41.499997 jianyingdraft_py-0.1.9/JianYingDraft/core/media.py
--rw-r--r--   0        0        0     1387 2024-03-29 05:25:48.612581 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaAudio.py
--rw-r--r--   0        0        0     1364 2024-03-29 05:26:30.317548 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaFactory.py
--rw-r--r--   0        0        0     1507 2024-03-29 05:26:00.190295 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaImage.py
--rw-r--r--   0        0        0     1520 2024-03-29 05:26:08.208537 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaText.py
--rw-r--r--   0        0        0     1530 2024-03-29 05:26:20.813825 jianyingdraft_py-0.1.9/JianYingDraft/core/mediaVideo.py
--rw-r--r--   0        0        0     9469 2024-03-29 05:26:20.773543 jianyingdraft_py-0.1.9/JianYingDraft/core/template.py
--rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-0.1.9/JianYingDraft/template/draft_content.json
--rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-0.1.9/JianYingDraft/template/draft_meta_info.json
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-0.1.9/JianYingDraft/utils/__init__.py
--rw-r--r--   0        0        0      866 2024-03-29 02:21:54.415368 jianyingdraft_py-0.1.9/JianYingDraft/utils/tools.py
--rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-0.1.9/LICENSE
--rw-r--r--   0        0        0      546 2024-03-30 11:44:15.873229 jianyingdraft_py-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1550 2024-03-29 15:44:39.369561 jianyingdraft_py-0.1.9/README.md
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 jianyingdraft_py-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.1/JianYingDraft/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-1.0.1/JianYingDraft/core/__init__.py
+-rw-r--r--   0        0        0     9941 2024-04-09 10:35:35.917283 jianyingdraft_py-1.0.1/JianYingDraft/core/draft.py
+-rw-r--r--   0        0        0     9058 2024-04-09 08:15:14.757157 jianyingdraft_py-1.0.1/JianYingDraft/core/media.py
+-rw-r--r--   0        0        0     1995 2024-04-10 01:11:08.019622 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaAudio.py
+-rw-r--r--   0        0        0     1151 2024-04-10 03:23:50.885126 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaEffect.py
+-rw-r--r--   0        0        0     1230 2024-04-01 09:46:41.819510 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaFactory.py
+-rw-r--r--   0        0        0     1247 2024-04-10 01:09:28.398551 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaImage.py
+-rw-r--r--   0        0        0     1530 2024-04-09 07:37:42.070377 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaText.py
+-rw-r--r--   0        0        0     2531 2024-04-10 03:27:20.508108 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaVideo.py
+-rw-r--r--   0        0        0    12608 2024-04-10 00:11:08.923813 jianyingdraft_py-1.0.1/JianYingDraft/core/template.py
+-rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-1.0.1/JianYingDraft/template/draft_content.json
+-rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-1.0.1/JianYingDraft/template/draft_meta_info.json
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.1/JianYingDraft/utils/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-10 03:14:16.715755 jianyingdraft_py-1.0.1/JianYingDraft/utils/dataStruct.py
+-rw-r--r--   0        0        0     2259 2024-04-10 02:15:15.252696 jianyingdraft_py-1.0.1/JianYingDraft/utils/innerBizTypes.py
+-rw-r--r--   0        0        0     2466 2024-04-10 03:03:35.832827 jianyingdraft_py-1.0.1/JianYingDraft/utils/tools.py
+-rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-1.0.1/LICENSE
+-rw-r--r--   0        0        0      546 2024-04-10 03:31:58.760798 jianyingdraft_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1558 2024-04-08 21:29:46.189767 jianyingdraft_py-1.0.1/README.md
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 jianyingdraft_py-1.0.1/PKG-INFO
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/draft.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/draft.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from BasicLibrary.configHelper import ConfigHelper
 from BasicLibrary.data.dateTimeHelper import DateTimeHelper
 
 from JianYingDraft.utils import tools
 from JianYingDraft.core.media import Media
 from JianYingDraft.core.mediaFactory import MediaFactory
+from JianYingDraft.core.mediaEffect import MediaEffect
 from JianYingDraft.core import template
 
 
 class Draft:
     _draft_content_file_base_name = "draft_content.json"
     _draft_meta_info_file_base_name = "draft_meta_info.json"
 
@@ -55,45 +56,65 @@
         self._materials_in_draft_content: {} = self._draft_content_data['materials']  # 草稿内容库的素材
 
         self._materials_in_draft_meta_info: {} = self._draft_meta_info_data['draft_materials']  # 草稿元数据库的素材
         self._videos_material_in_draft_meta_info = self._materials_in_draft_meta_info[0]['value']
         self._audios_material_in_draft_meta_info = self._materials_in_draft_meta_info[6]['value']  # type为8的那条
 
         self._tracks_in_draft_content: [] = self._draft_content_data['tracks']  # 草稿内容库的轨道
+        pass
 
-        # 存储本草稿用到的所有的媒体
-        self._all_medias = []
-
-    def add_media(self, media_file_full_name: str, start=0, duration=0, index=0):
+    def add_media(self, media_file_full_name: str, start=0, duration=0, index=0, **kwargs):
         """
         添加媒体到草稿
         """
+        _index = index
 
-        # TODO:xiedali@2024/03/28 需要重新确认以下index的作用，其应该是表示轨道信息的时候使用，不需要向media传送
+        media = MediaFactory.create(media_file_full_name, start=start, duration=duration, **kwargs)
 
-        media = MediaFactory.create(media_file_full_name, start=start, duration=duration, index=index)
-
-        # TODO:xiedali@2024/03/30 需要确认逻辑，当添加同一个媒体文件进入草稿的时候，是否可以只添加一个material和多个trace的segment就可以。
-        # 将媒体存入媒体容器
-        self._all_medias.append(media)
+        if media is None:
+            return
+        pass
 
         # 将媒体信息添加到draft的素材库
         self.__add_media_to_content_materials(media)
 
         # 将媒体信息添加到draft的轨道库
-        self.__add_media_to_content_tracks(media)
+        self.__add_media_to_content_tracks(media, start=start)
 
         # 将媒体信息添加到draft的元数据库
         self.__add_media_to_meta_info(media)
+        pass
+
+    def add_effect(self, effect_name_or_resource_id: str | int, start=0, duration=0, index=0, **kwargs):
+        """
+        添加特效到草稿
+        @param index:
+        @param duration:
+        @param start:
+        @param effect_name_or_resource_id: 特效的名称或资源ID（内置特效可以使用名称；外置特效直接使用剪映的资源ID）
+        """
+        _index = index
 
-    def get_draft_duration(self):
+        media = MediaEffect(effect_name_or_resource_id=effect_name_or_resource_id, start=start, duration=duration,
+                            **kwargs)
+
+        # 将媒体信息添加到draft的素材库
+        self.__add_media_to_content_materials(media)
+
+        # 将媒体信息添加到draft的轨道库
+        self.__add_media_to_content_tracks(media, start=start)
+
+        # # 效果的媒体信息不需要添加到draft的元数据库
+        # self.__add_media_to_meta_info(media)
+
+    def calc_draft_duration(self):
         """
         获取（通过计算）草稿的时长
         """
-        self.__get_track_duration("video")
+        return self.__get_track_duration("video")
 
     def save(self):
         """
         保存草稿
         """
         # 校准时长信息
         self.__calc_duration()
@@ -119,15 +140,15 @@
             if _key.startswith("X."):
                 continue
             pass
 
             self._materials_in_draft_content[_key].append(_value)
         pass
 
-    def __add_media_to_content_tracks(self, media: Media):
+    def __add_media_to_content_tracks(self, media: Media, start=0):
         """
         添加媒体信息到素材内容库的轨道部分：
         """
 
         all_tracks = self._tracks_in_draft_content
         target_track = None
         for _track in all_tracks:
@@ -139,20 +160,22 @@
 
         if target_track is None:
             target_track = template.get_track()
             target_track["type"] = media.category_type
             self._tracks_in_draft_content.append(target_track)
         pass
 
-        # 添加新片段之前轨道总时长
-        track_duration = self.__get_track_duration(media.category_type)
+        if not start:
+            # 添加新片段之前轨道总时长
+            start = self.__get_track_duration(media.category_type)
+        pass
 
         # 设置新segment的在轨道上的开始时间
         segment_source_timerange = media.segment_data_for_content["target_timerange"]
-        segment_source_timerange["start"] = track_duration
+        segment_source_timerange["start"] = start
         target_track["segments"].append(media.segment_data_for_content)
 
     def __add_media_to_meta_info(self, media: Media):
         """
         添加媒体信息到元数据库：
         """
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/media.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/media.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,74 +43,123 @@
 
     media_category_type_mapping = {
         "image": "video"
     }
 
     def __init__(self, **kwargs):
         """
-        初始化
+        初始化数据
+        初始化数据分为两个阶段：
+        1. 初始化基础属性（media本身的属性，比如width等）
+        2. 初始化业务属性（media为组成草稿准备的属性，比如轨道的segment等）
+        针对这2个阶段，设置4个钩子，派生类可以根据情况调用：
+        1. _init_basic_info_before
+        2. _init_basic_info_after
+        3. _init_biz_info_before
+        4. _init_biz_info_after
         :param kwargs:
         """
-        # 10. 定义基础属性
+        # 00. 保存传递进来的kwargs，供后续灵活使用
+        self.kwargs = kwargs
+
+        # A.1. 定义基础属性
         self.id = tools.generate_id()  # 在mete_info和content中都使用同一个guid
 
         self.media_type = ''  # 这是媒体文件真实的类型
         self.material_type = ''  # 这是媒体添加到草稿里面，对应的素材类型（比如图片媒体文件image，对应的素材类型就是photo）
         self.category_type = ''  # 这是媒体添加到草稿里面，素材所属类目（比如图片对应的类目就是Video）
 
         self.width = 0
         self.height = 0
         self.duration = 0
 
         self.material_name = ''
         self.file_Path = ''
         self.extra_info = ''
 
-        # 20. 定义最后暴露给草稿文件的属性
-        ## 20.1. 定义暴露给draft_meta_info文件的属性
+        # A.2 初始化基础属性
+        ## A.2.00. 为初始化基础属性前加载逻辑
+        self._init_basic_info_before()
+
+        ## A.2.10. 加载各种资源的文件名称等基础信息
+        media_file_full_name = kwargs.get("mediaFileFullName", "")
+        media_base_name_no_extension = FileHelper.get_base_name_no_extension(media_file_full_name)
+        self.extra_info = media_base_name_no_extension  # media_file_full_name.split("/")[-1]
+        self.material_name = media_base_name_no_extension
+        self.file_Path = media_file_full_name
+
+        ## A.2.20. 加载各种媒体公共的信息
+        media_info = kwargs.get("mediaInfo")
+        self.__load_property_from_media_info(media_info)
+        self.__set_type_info()
+
+        ## A.2.30. 加载媒体的自定义设置
+        duration = kwargs.get("duration", 0)
+        if duration:
+            self.duration = duration
+        pass
+
+        ## A.2.99. 为初始化基础属性后加载逻辑
+        self._init_basic_info_after()
+
+        # B.1. 定义业务属性（最后暴露给草稿文件使用）
+
+        ## B.1.10. 定义暴露给draft_meta_info文件的属性
         self.data_for_meta_info = template.get_material_for_meta_info(self.id)
-        ## 20.2. 定义暴露给draft_content文件的属性
+
+        ## B.1.20. 定义暴露给draft_content文件的属性
         ## 内部有各种属性分为两组，并分别为两个组设置别名：material_for_content,track_for_content
         # 第1组. material组（speed、sound_channel_mapping等，当然最重要的是video（或者audio））
         # 这些属性最后都会最成为materials各种数组属性的元素（比如此处的speed会保存为materials.speeds数组的一个元素：
         # materials.speeds = [speed1, speed2, speed3, ...]。此处的其他各属性亦然。）
         # 第2组. track组（segments等）
         # 具体内容在派生类中实现
         self.data_for_content = {
             "material": {},
             "segment": {},
         }
         self.material_data_for_content = self.data_for_content["material"]
         self.segment_data_for_content = self.data_for_content["segment"]
 
-        # 30. 加载各种资源的文件名称等信息
-        media_file_full_name = kwargs.get("mediaFileFullName", "")
-        media_base_name_no_extension = FileHelper.get_base_name_no_extension(media_file_full_name)
-        self.extra_info = media_base_name_no_extension  # media_file_full_name.split("/")[-1]
-        self.material_name = media_base_name_no_extension
-        self.file_Path = media_file_full_name
-
-        # 40. 加载各种媒体公共的信息
-        media_info = kwargs.get("mediaInfo")
-        self._load_property_from_media(media_info)
-
-        # 50. 加载素材的自定义设置
-        duration = kwargs.get("duration", 0)
-        if duration:
-            self.duration = duration
-        pass
+        # B.2.00. 为初始化业务属性前加载逻辑
+        self._init_biz_info_before()
 
-        # 60.1. 设置草稿文件的meta_info部分
+        ## B.2.10. 设置草稿文件的meta_info部分
         self.__set_data_for_meta_info()
 
-        # 60.2. 设置草稿文件的content部分
+        ## B.2.20. 设置草稿文件的content部分
         # 此部分功能在派生类中实现
         self.__set_data_for_content()
 
-    pass
+        ## B.2.99. 为初始化业务属性后加载逻辑
+        self._init_biz_info_after()
+
+    def _init_basic_info_before(self):
+        """
+        在初始化基础属性前加载逻辑（供派生类使用）
+        """
+        _self = self
+
+    def _init_basic_info_after(self):
+        """
+        在初始化基础属性后加载逻辑（供派生类使用）
+        """
+        _self = self
+
+    def _init_biz_info_before(self):
+        """
+        在初始化业务属性前加载逻辑（供派生类使用）
+        """
+        _self = self
+
+    def _init_biz_info_after(self):
+        """
+        在初始化业务属性后加载逻辑（供派生类使用）
+        """
+        _self = self
 
     def __set_data_for_content(self):
         """
         为草稿文件draft_content准备信息
         """
         self._set_material_data_for_content()
         self._set_segment_data_for_content()
@@ -148,33 +197,43 @@
         self.data_for_meta_info['metetype'] = self.material_type
         self.data_for_meta_info['width'] = self.width
         self.data_for_meta_info['height'] = self.height
         self.data_for_meta_info['duration'] = self.duration
         self.data_for_meta_info['extra_info'] = self.extra_info
         self.data_for_meta_info['file_Path'] = self.file_Path
 
-    def _load_property_from_media(self, media_info: MediaInfo):
+    def __load_property_from_media_info(self, media_info: MediaInfo):
         """
         从媒体信息中加载素材信息
         """
+        if not media_info:
+            return
+        pass
+
         self.media_type = media_info['track_type'].lower()
 
+        if "width" in media_info:
+            self.width = media_info['width']
+            self.height = media_info['height']
+        pass
+
+        if "duration" in media_info:
+            self.duration = media_info['duration'] * 1000
+        pass
+
+    def __set_type_info(self):
+        _type = self.kwargs.get("media_type", "")
+        if _type:
+            self.media_type = _type
+        pass
+
         if self.media_type in self.media_material_type_mapping:
             self.material_type = self.media_material_type_mapping[self.media_type]
         else:
             self.material_type = self.media_type
         pass
 
         if self.media_type in self.media_category_type_mapping:
             self.category_type = self.media_category_type_mapping[self.media_type]
         else:
             self.category_type = self.media_type
         pass
-
-        if "width" in media_info:
-            self.width = media_info['width']
-            self.height = media_info['height']
-        pass
-
-        if "duration" in media_info:
-            self.duration = media_info['duration'] * 1000
-        pass
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaFactory.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaFactory.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 
 
 class MediaFactory:
     """
     媒体工厂
     """
 
-    # media_type_mapping = {
-    #     # "video": "video",
-    #     # "audio": "audio",
-    #     # "image": "photo",
-    # }
-
     @staticmethod
     def create(media_full_name: str, **kwargs):
         """
         根据素材来信创建素材实体
         :param media_full_name:
         :return:
         """
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaImage.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaAudio.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,35 +7,47 @@
  * @company: HiLand & RainyTop
 """
 from JianYingDraft.core import template
 from JianYingDraft.core.media import Media
 from JianYingDraft.utils import tools
 
 
-# TODO:xiedali@2024/03/27 功能需要实现
-
-class MediaImage(Media):
+class MediaAudio(Media):
 
     def _set_material_data_for_content(self):
         speed_id = tools.generate_id()
         scm_id = tools.generate_id()
-        canvas_id = tools.generate_id()
+        beat_id = tools.generate_id()
 
-        self.material_data_for_content["speeds"] = template.get_speed(speed_id)
-        self.material_data_for_content["sound_channel_mappings"] = template.get_sound_channel_mapping(scm_id)
-        self.material_data_for_content["canvases"] = template.get_canvas(canvas_id)
+        self.material_data_for_content['speeds'] = template.get_speed(speed_id)
+        self.material_data_for_content['sound_channel_mappings'] = template.get_sound_channel_mapping(scm_id)
+        self.material_data_for_content['beats'] = template.get_beat(beat_id)
 
-        self.material_data_for_content["videos"] = self.__gen_photo()
+        self.material_data_for_content["audios"] = self.__generate_main_data()
         # 将素材的各种业务信息，暂时保存起来，后续供track下的segment使用
-        self.material_data_for_content["X.extra_material_refs"] = [speed_id, scm_id, canvas_id]
+        self.material_data_for_content["X.extra_material_refs"] = [speed_id, scm_id, beat_id]
+
+        # 以下为音频淡入淡出的效果
+        fade_in_duration = self.kwargs.get("fade_in_duration", 0)
+        fade_out_duration = self.kwargs.get("fade_out_duration", 0)
+        if fade_in_duration > 0 or fade_out_duration > 0:
+            audio_fade_id = tools.generate_id()
+            self.material_data_for_content['audio_fades'] = template.get_audio_fade(
+                audio_fade_id,
+                fade_in_duration,
+                fade_out_duration
+            )
+
+            self.material_data_for_content["X.extra_material_refs"].append(audio_fade_id)
+        pass
 
-    def __gen_photo(self):
-        entity = template.get_video(self.id)
+    def __generate_main_data(self):
+        entity = template.get_audio(self.id)
         entity["duration"] = self.duration
-        entity["height"] = self.height
-        entity["local_material_id"] = self.id  # 暂时跟素材设置为相同的id
-        entity["material_name"] = self.material_name
+        entity["local_material_id"] = self.id
+        entity["name"] = self.material_name
         entity["path"] = self.file_Path
-        entity["type"] = self.material_type
-        entity["width"] = self.width
+        entity["type"] = "extract_" + self.material_type  # "extract_"??什么时候不加这个前缀
         return entity
+
+
 pass
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/mediaVideo.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaText.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,43 +2,47 @@
  * @file   : materialVideo.py
  * @time   : 15:23
  * @date   : 2024/3/23
  * @mail   : 9727005@qq.com
  * @creator: ShanDong Xiedali
  * @company: HiLand & RainyTop
 """
-from JianYingDraft.core.media import Media
 from JianYingDraft.core import template
+from JianYingDraft.core.media import Media
 from JianYingDraft.utils import tools
 
 
-class MediaVideo(Media):
+class MediaText(Media):
+    def __init__(self):
+        super().__init__()
+
+    pass
 
     def _set_material_data_for_content(self):
-        """
-        设置草稿文件的content部分
-        """
-        speed_id = tools.generate_id()
-        scm_id = tools.generate_id()
-        canvas_id = tools.generate_id()
-
-        self.material_data_for_content["speeds"] = template.get_speed(speed_id)
-        self.material_data_for_content["sound_channel_mappings"] = template.get_sound_channel_mapping(scm_id)
-        self.material_data_for_content["canvases"] = template.get_canvas(canvas_id)
+        ma_id = tools.generate_id()
 
-        self.material_data_for_content["videos"] = self.__gen_video()
+        self.material_data_for_content['material_animations'] = template.get_speed(ma_id)
+
+        self.material_data_for_content["texts"] = self.__generate_text()
         # 将素材的各种业务信息，暂时保存起来，后续供track下的segment使用
-        self.material_data_for_content["X.extra_material_refs"] = [speed_id, scm_id, canvas_id]
+        self.material_data_for_content["X.extra_material_refs"] = [ma_id, ]
 
-    def __gen_video(self):
-        entity = template.get_video(self.id)
-        entity["duration"] = self.duration
-        entity["height"] = self.height
-        entity["local_material_id"] = self.id  # 暂时跟素材设置为相同的id
-        entity["material_name"] = self.material_name
-        entity["path"] = self.file_Path
-        entity["type"] = self.material_type
-        entity["width"] = self.width
+    def __generate_text(self):
+        _self = self
+        entity = template.get_text(self.id)
         return entity
 
+    def change_color(self, color):
+        """
+        改变文字颜色
+        :param color: 以“#”开头后跟6位的颜色值
+        """
+        self.material_data_for_content['text_color'] = color
+        r = int(color[1:3], 16)
+        g = int(color[3:5], 16)
+        b = int(color[5:7], 16)
+        color1 = "<color=(1.000000, 1.000000, 1.000000, 1.000000)>"
+        color2 = F'<color=({round(r / 255, 6):.6f}, {round(g / 255, 6):.6f}, {round(b / 255, 6):.6f}, 1.000000)>'
+        self.material_data_for_content['content'] = self.material_data_for_content['content'].replace(color1, color2)
+
 
 pass
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/core/template.py` & `jianyingdraft_py-1.0.1/JianYingDraft/core/template.py`

 * *Files 17% similar despite different names*

```diff
@@ -72,33 +72,33 @@
         "extra_info": "",
         "file_Path": "",
         "height": 0,
         "id": guid,
         "import_time": int(time.time()),
         "import_time_ms": int(time.time()) * 10 ^ 6,
         "md5": "",
-        "metetype": "",  # meta?? 估计剪映开发人员最初拼写错误，以后大家就将错就错了。
+        "metetype": "",  # meta or mate?? 估计剪映开发人员最初拼写错误，以后大家就以讹传讹将错就错了。
         "roughcut_time_range": {"duration": 0, "start": 0},
         "sub_time_range": {"duration": -1, "start": -1},
         "type": 0,
         "width": 0
     }
 
 
-def get_track(guid: str = None):
+def get_track(guid: str = None, track_type: str = ""):
     if guid is None:
         guid = tools.generate_id()
     pass
 
     return {
-        "attribute": 0,
+        "attribute": 0,  # 0表示正常；1表示关闭本轨道
         "flag": 0,
         "id": guid,
         "segments": [],
-        "type": ""
+        "type": track_type
     }
 
 
 def get_segment(guid: str = None):
     if guid is None:
         guid = tools.generate_id()
     pass
@@ -186,15 +186,15 @@
             "upper_left_y": 0.0,
             "upper_right_x": 1.0,
             "upper_right_y": 0.0
         },
         "crop_ratio": "free",
         "crop_scale": 1.0,
         "duration": 0,
-        "extra_type_option": 0,
+        "extra_type_option": 0,  # 是否播放视频素材的本身的背景音。0：播放；1：不播放
         "formula_id": "",
         "freeze": None,
         "gameplay": None,
         "has_audio": True,
         "height": 0,
         "id": guid,
         "intensifies_audio_path": "",
@@ -361,7 +361,109 @@
     pass
 
     return {
         "animations": [],
         "id": guid,
         "type": "sticker_animation"
     }
+
+
+def get_audio_fade(guid: str = None, fade_in_duration: int = 0, fade_out_duration: int = 0):
+    """
+    添加音频的淡入淡出效果
+    @param guid:
+    @param fade_in_duration: 淡入时间（单位微秒）
+    @param fade_out_duration: 淡出时间（单位微秒）
+    @return:
+    """
+    if guid is None:
+        guid = tools.generate_id()
+    pass
+
+    return {
+        "fade_in_duration": fade_in_duration,
+        "fade_out_duration": fade_out_duration,
+        "fade_type": 0,
+        "id": guid,
+        "type": "audio_fade"
+    }
+
+
+def get_video_effect(guid: str = None, resource_id: str = "", name=""):
+    """
+    添加视频特效
+
+    @param guid: 特效的资源id
+    @param name: 特效的名称
+    @param resource_id: 特效资源在剪映的资源库中的id（非常重要，剪映通过这个id来自动获取特效的各种资源）
+    @return:
+    """
+    if guid is None:
+        guid = tools.generate_id()
+    pass
+
+    return {
+        "adjust_params": [
+            {
+                "default_value": 0.33,
+                "name": "effects_adjust_speed",
+                "value": 0.33
+            },
+            {
+                "default_value": 1.0,
+                "name": "effects_adjust_background_animation",
+                "value": 1.0
+            }
+        ],
+        "algorithm_artifact_path": "",
+        "apply_target_type": 2,
+        "apply_time_range": {"duration": 0, "start": 0},
+        "category_id": "1039448",
+        "category_name": "热门",
+        "common_keyframes": [],
+        "disable_effect_faces": [],
+        "effect_id": "1039448",
+        "formula_id": "",
+        "id": guid,
+        "name": name,
+        "path": "",
+        "platform": "all",
+        "render_index": 0,
+        "request_id": "",
+        "resource_id": resource_id,  # 特效的资源id（剪映通过这个id来自动获取特效的各种资源）
+        "source_platform": 0,
+        "time_range": {"duration": 0, "start": 0},
+        "track_render_index": 0,
+        "type": "video_effect",
+        "value": 1.0,
+        "version": ""
+    }
+
+
+def get_transition(guid: str = None, resource_id: str = "", name="", duration: int = 500_000):
+    """
+    添加视频特效
+
+    @param duration: 转场的持续时间（单位微秒）
+    @param guid: 转场的资源id
+    @param name: 转场的名称
+    @param resource_id: 转场资源在剪映的资源库中的id（非常重要，剪映通过这个id来自动获取转场的各种资源）
+    @return:
+    """
+    if guid is None:
+        guid = tools.generate_id()
+    pass
+
+    return {
+        "category_id": "39862",
+        "category_name": "叠化",
+        "duration": duration,
+        "effect_id": "321493",
+        "id": guid,
+        "is_overlap": False,
+        "name": name,
+        "path": "",
+        "platform": "all",
+        "request_id": "202404100726237F33ED27AE329CF48C4E",
+        "resource_id": resource_id,
+        "type": "transition"
+    }
```

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/template/draft_content.json` & `jianyingdraft_py-1.0.1/JianYingDraft/template/draft_content.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.9/JianYingDraft/template/draft_meta_info.json` & `jianyingdraft_py-1.0.1/JianYingDraft/template/draft_meta_info.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.9/LICENSE` & `jianyingdraft_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-0.1.9/pyproject.toml` & `jianyingdraft_py-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JianYingDraft.PY"
-version = "0.1.9"
+version = "1.0.1"
 description = "帮助剪映快速生成草稿的方案"
 authors = ["解大劦 <develope@163.com>"]
 readme = "README.md"
 packages = [{ include = "JianYingDraft" }]
 include = ["README.md", "LICENSE"]
 license = "MIT"
```

### Comparing `jianyingdraft_py-0.1.9/README.md` & `jianyingdraft_py-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 ▌参考资料：
 剪映草稿文件的说明，另外可以参考文章：https://blog.csdn.net/a820206256/article/details/134428639
 
 ## 剪映的草稿原理说明
 
 1. 实现原理 : 剪映的草稿文件是 `json` 的形式存储的。我们只需要创建`draft_content.json`和`draft_mate_info.json`
-   ，其他文件则会在打开剪映软件后会自动补全。
-   `draft_mate_info.json`内的素材信息会出现在剪映左侧的素材库中；两个文件内都记录了素材信息，`draft_content.json`
-   的素材信息会出现在剪映下侧的时间线上。
+   （其他文件则会在打开剪映软件后会自动补全）。两个文件内都记录了素材信息，其中：`draft_mate_info.json`
+   内的素材信息会出现在剪映左侧的素材库中；`draft_content.json`的素材信息会出现在剪映下侧的时间线上。
 2. 添加一个媒体素材到剪映软件，剪映会将其数据记录进入“草稿元数据库” 和 “草稿内容库”（包括素材部分和轨道部分）
 
 ## 本软件的实现原理说明
 
 1. `add_media` 会识别媒体类型，加入到对应轨道。
 2. 当没有视频轨道时，创建音频轨道会先创建视频轨道。
```

### Comparing `jianyingdraft_py-0.1.9/PKG-INFO` & `jianyingdraft_py-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianYingDraft.PY
-Version: 0.1.9
+Version: 1.0.1
 Summary: 帮助剪映快速生成草稿的方案
 License: MIT
 Author: 解大劦
 Author-email: develope@163.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,17 +24,16 @@
 
 ▌参考资料：
 剪映草稿文件的说明，另外可以参考文章：https://blog.csdn.net/a820206256/article/details/134428639
 
 ## 剪映的草稿原理说明
 
 1. 实现原理 : 剪映的草稿文件是 `json` 的形式存储的。我们只需要创建`draft_content.json`和`draft_mate_info.json`
-   ，其他文件则会在打开剪映软件后会自动补全。
-   `draft_mate_info.json`内的素材信息会出现在剪映左侧的素材库中；两个文件内都记录了素材信息，`draft_content.json`
-   的素材信息会出现在剪映下侧的时间线上。
+   （其他文件则会在打开剪映软件后会自动补全）。两个文件内都记录了素材信息，其中：`draft_mate_info.json`
+   内的素材信息会出现在剪映左侧的素材库中；`draft_content.json`的素材信息会出现在剪映下侧的时间线上。
 2. 添加一个媒体素材到剪映软件，剪映会将其数据记录进入“草稿元数据库” 和 “草稿内容库”（包括素材部分和轨道部分）
 
 ## 本软件的实现原理说明
 
 1. `add_media` 会识别媒体类型，加入到对应轨道。
 2. 当没有视频轨道时，创建音频轨道会先创建视频轨道。
```

