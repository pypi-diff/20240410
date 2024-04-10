# Comparing `tmp/spotidex-0.0.5.tar.gz` & `tmp/spotidex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.5.tar", max compression
+gzip compressed data, was "spotidex-0.0.6.tar", max compression
```

## Comparing `spotidex-0.0.5.tar` & `spotidex-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      532 2024-04-09 17:06:57.148329 spotidex-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.5/README.md
--rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.5/spotidex/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.5/spotidex/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.5/spotidex/cli/app_screens/__init__.py
--rw-r--r--   0        0        0     6871 2024-04-07 04:25:26.776169 spotidex-0.0.5/spotidex/cli/app_screens/DownloadInterface.py
--rw-r--r--   0        0        0     4675 2024-04-06 10:26:15.321454 spotidex-0.0.5/spotidex/cli/app_screens/MainMenuInterface.py
--rw-r--r--   0        0        0     4576 2024-04-09 17:31:03.911736 spotidex-0.0.5/spotidex/cli/app_screens/SearchInterface.py
--rw-r--r--   0        0        0     4025 2024-04-06 10:25:55.937694 spotidex-0.0.5/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-r--r--   0        0        0     2430 2024-04-06 10:26:19.911279 spotidex-0.0.5/spotidex/cli/app_screens/SettingsInterface.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.5/spotidex/cli/custom_widgets/__init__.py
--rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
--rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
--rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
--rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
--rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
--rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
--rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
--rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
--rw-r--r--   0        0        0     4510 2024-04-06 08:18:54.195763 spotidex-0.0.5/spotidex/cli/custom_widgets/AppInterface.py
--rw-r--r--   0        0        0     1409 2024-04-06 10:25:36.360967 spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-r--r--   0        0        0     1933 2024-03-26 10:25:59.101131 spotidex-0.0.5/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.5/spotidex/cli/popup_screens/__init__.py
--rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
--rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
--rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
--rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
--rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
--rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
--rw-r--r--   0        0        0     4303 2024-04-06 09:28:28.087939 spotidex-0.0.5/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-r--r--   0        0        0     1135 2024-04-09 16:48:01.830808 spotidex-0.0.5/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.5/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.5/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-r--r--   0        0        0      616 2024-04-07 04:09:10.420863 spotidex-0.0.5/spotidex/cli/SpotidexApp.py
--rw-r--r--   0        0        0     4196 2024-04-09 16:52:32.143307 spotidex-0.0.5/spotidex/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.5/spotidex/src/__init__.py
--rw-r--r--   0        0        0     3043 2024-04-07 05:31:37.359930 spotidex-0.0.5/spotidex/src/content.py
--rw-r--r--   0        0        0     6712 2024-04-09 17:18:55.031801 spotidex-0.0.5/spotidex/src/download.py
--rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.5/spotidex/src/static.py
--rw-r--r--   0        0        0     5950 2024-04-09 17:11:57.735948 spotidex-0.0.5/spotidex/src/utils.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 spotidex-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      553 2024-04-10 09:43:59.673109 spotidex-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.6/README.md
+-rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.6/spotidex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.6/spotidex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.6/spotidex/cli/app_screens/__init__.py
+-rw-r--r--   0        0        0     6912 2024-04-10 18:01:30.463082 spotidex-0.0.6/spotidex/cli/app_screens/DownloadInterface.py
+-rw-r--r--   0        0        0     4675 2024-04-10 14:00:34.257827 spotidex-0.0.6/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-r--r--   0        0        0     5137 2024-04-10 14:45:17.645923 spotidex-0.0.6/spotidex/cli/app_screens/SearchInterface.py
+-rw-r--r--   0        0        0     4025 2024-04-06 10:25:55.937694 spotidex-0.0.6/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-r--r--   0        0        0     2450 2024-04-10 18:25:24.740301 spotidex-0.0.6/spotidex/cli/app_screens/SettingsInterface.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.6/spotidex/cli/custom_widgets/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
+-rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
+-rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
+-rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
+-rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
+-rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
+-rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
+-rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
+-rw-r--r--   0        0        0     4510 2024-04-10 14:45:36.699352 spotidex-0.0.6/spotidex/cli/custom_widgets/AppInterface.py
+-rw-r--r--   0        0        0     1467 2024-04-10 18:25:15.239179 spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-r--r--   0        0        0     1933 2024-03-26 10:25:59.101131 spotidex-0.0.6/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.6/spotidex/cli/popup_screens/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
+-rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
+-rw-r--r--   0        0        0     4303 2024-04-10 15:10:02.743220 spotidex-0.0.6/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-r--r--   0        0        0     1135 2024-04-10 14:45:53.954177 spotidex-0.0.6/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.6/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.6/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-r--r--   0        0        0      700 2024-04-10 18:25:42.766710 spotidex-0.0.6/spotidex/cli/SpotidexApp.py
+-rw-r--r--   0        0        0     4196 2024-04-09 16:52:32.143307 spotidex-0.0.6/spotidex/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.6/spotidex/src/__init__.py
+-rw-r--r--   0        0        0     3043 2024-04-07 05:31:37.359930 spotidex-0.0.6/spotidex/src/content.py
+-rw-r--r--   0        0        0     6712 2024-04-09 17:18:55.031801 spotidex-0.0.6/spotidex/src/download.py
+-rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.6/spotidex/src/static.py
+-rw-r--r--   0        0        0     5991 2024-04-10 18:07:50.938740 spotidex-0.0.6/spotidex/src/utils.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 spotidex-0.0.6/PKG-INFO
```

### Comparing `spotidex-0.0.5/pyproject.toml` & `spotidex-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotidex"
-version = "0.0.5"
+version = "0.0.6"
 description = "Spotify Downloader TUI"
 authors = ["Libin Lalu <libinlalu000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,14 +12,15 @@
 requests = "2.31.0"
 rich = "13.7.1"
 spotipy = "2.23.0"
 textual = "0.56.4"
 tqdm = "4.66.1"
 yt-dlp = "2024.3.10"
 ytmusicapi = "1.3.2"
+pyperclip = "^1.8.2"
 
 [tool.poetry.scripts]
-my_script = "spotidex:main"
+spotidex = "spotidex:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spotidex-0.0.5/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-0.0.6/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,16 @@
             track_info = (
                 full_track_info[:57] + "..."
                 if len(full_track_info) > 57
                 else (name[:57] + "..." if len(name) > 40 else full_track_info)
             )
         else:
             track_info = (
-                f"{name[:45]}..."
-                if len(name) > 45
+                f"{name[:43]}... [{len(self.app.selected_tracks)} Tracks]"
+                if len(name) > 43
                 else f"{name} [{len(self.app.selected_tracks)} Tracks]"
             )
 
         download_info = {
             f"{link_type.capitalize()} Info": track_info,
             "Download Path": shorten_path(self.app.saved_settings["download_path"], 57),
             "Download Quality": self.app.saved_settings["download_quality"],
```

### Comparing `spotidex-0.0.5/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-0.0.6/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-0.0.6/spotidex/cli/app_screens/SearchInterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from spotidex.cli.custom_widgets.AppInterface import AppInterface
 from spotidex.cli.app_screens.MainMenuInterface import MainMenuInterface
 from spotidex.cli.utils import input_validator, app_description
 from spotidex.cli.utils import get_link_details
 
 from textual.worker import Worker, get_current_worker
+from textual.binding import Binding
 from textual import work
+import pyperclip
 
 CSS = """
 Search {
     align: center middle;
 }
 
 #search-interface #interface{
@@ -44,28 +46,41 @@
     border:tall black
 }
 """
 
 
 class Search(Screen):
     DEFAULT_CSS = CSS
+    BINDINGS = [
+        Binding("tab", "paste_link", "PASTE SPOTIFY LINK",priority=True),
+        Binding("delete", "clear_input", "CLEAR INPUT",priority=True)
+    ]
 
     def compose(self):
         yield AppInterface(
             Horizontal(
                 Input(
                     id="search-input",
                     placeholder="PASTE YOUR SPOTIFY LINK HERE",
                 ),
                 Button("SEARCH", "success", id="search-button", disabled=True),
             ),
             Label(app_description, id="app-description", shrink=True),
             id="search-interface",
         )
 
+    def action_paste_link(self):
+        if self.query_one("#search-input", Input).value =="":
+            self.query_one("#search-input", Input).value = pyperclip.paste()
+        self.query_one("#search-input", Input).focus()
+    
+    def action_clear_input(self):
+        self.query_one("#search-input", Input).value = ""
+
+
     @work(exclusive=True, thread=True)
     def get_link_info(self):
         self.app.query_one("LoadingIndicator").styles.background = "#1c1c1c"
         try:
             self.app.link_details = get_link_details(self.app.spotify_link)
         except Exception as spotidex_error:
             if spotidex_error.message == "NetworkError":
```

### Comparing `spotidex-0.0.5/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-0.0.6/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-0.0.6/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from textual.widgets import Button
 from textual.containers import Horizontal
 from textual.screen import Screen
 from textual.reactive import reactive
 
 from spotidex.cli.custom_widgets.DownloadPathSelector import DownloadPathSelector
 from spotidex.cli.custom_widgets.MetadataCheckBox import MetadataCheckBox
-from spotidex.cli.custom_widgets.DownloadQualitySelection import DownloadQualitySelection
+from spotidex.cli.custom_widgets.DownloadQualitySelection import (
+    DownloadQualitySelection,
+)
 from spotidex.cli.custom_widgets.AppInterface import AppInterface
-from spotidex.cli.utils import Path
+from spotidex.cli.utils import get_downloads_folder
 
 CSS = """
 Settings{
     align:center middle;
     height:auto;
     width:auto;
 
@@ -52,27 +54,26 @@
             Horizontal(
                 MetadataCheckBox(),
                 DownloadQualitySelection(),
                 id="metadata-download-quality-container",
             ),
             Button("SAVE SETTINGS", "success", id="save-settings-button"),
             Button("RESET SETTINGS", "error", id="reset-settings-button"),
-            id = "settings-interface"
+            id="settings-interface",
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "reset-settings-button":
             self.app.query_one(MetadataCheckBox).value = True
-            self.app.query_one(DownloadPathSelector).value = str(Path.cwd())
+            self.app.query_one(DownloadPathSelector).value = str(get_downloads_folder())
             self.app.query_one(DownloadQualitySelection).value = "high"
         elif event.button.id == "save-settings-button":
             self.app.notify("SETTINGS SAVED SUCCESSFULLY", title="Spotidex")
             self.app.saved_settings = {
-                "add_metadata":self.app.query_one(MetadataCheckBox).value ,
+                "add_metadata": self.app.query_one(MetadataCheckBox).value,
                 "download_path": self.app.query_one(DownloadPathSelector).value,
                 "download_quality": self.app.query_one(DownloadQualitySelection).value,
-                }
+            }
             self.app.pop_screen()
-            
-    def on_mount(self):
-        self.app.query_one("#nav-label").update('[bold]SETTINGS')
 
+    def on_mount(self):
+        self.app.query_one("#nav-label").update("[bold]SETTINGS")
```

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-0.0.6/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-
 from textual.widgets import Button, Static
 from textual.containers import Container
 from textual.widget import Widget
 
 from spotidex.cli.popup_screens.DownloadPathPopup import DownloadPathScreen
-from spotidex.cli.utils import Path, shorten_path
+from spotidex.cli.utils import Path, shorten_path, get_downloads_folder
 from textual.reactive import reactive
 
 CSS = """
 DownloadPathSelector{
     width:auto;
     height:auto;
 
@@ -37,23 +36,25 @@
 }
 
 """
 
 
 class DownloadPathSelector(Widget):
     DEFAULT_CSS = CSS
-    value = reactive(str(Path.cwd()))
+    value = reactive(str(get_downloads_folder()))
 
     def compose(self):
         with Container(id="download-path-container"):
             yield Static(id="download-path-label")
             yield Button("CHANGE", id="download-path-button", variant="primary")
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         def change_value(value):
             self.value = value
 
         if event.button.id == "download-path-button":
             self.app.push_screen(DownloadPathScreen(), change_value)
 
     def watch_value(self, value):
-        self.query_one("#download-path-label").update("[bold]"+shorten_path(value, 65))
+        self.query_one("#download-path-label").update(
+            "[bold]" + shorten_path(value, 65)
+        )
```

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-0.0.6/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc` & `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-0.0.6/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-0.0.6/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-0.0.6/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-0.0.6/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/cli/SpotidexApp.py` & `spotidex-0.0.6/spotidex/cli/SpotidexApp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from textual.app import App
 from spotidex.cli.app_screens.SearchInterface import Search
 from spotidex.cli.app_screens.SettingsInterface import Settings
-from spotidex.cli.utils import Path
+from spotidex.cli.utils import get_downloads_folder
+from spotidex.src.utils import get_ffmpeg
 
 
 class SpotidexApp(App):
     TITLE = "SPOTIDEX"
     SUB_TITLE = "SPOTIFY DOWNLOADER"
     SCREENS = {"SettingsScreen": Settings}
 
     def on_ready(self) -> None:
         self.app.saved_settings = {
             "add_metadata": True,
-            "download_path": str(Path.cwd()),
+            "download_path": str(get_downloads_folder()),
             "download_quality": "high",
         }
         self.push_screen(Search())
- 
-def main():
-    SpotidexApp().run()
-
 
 
+def main():
+    get_ffmpeg()
+    SpotidexApp().run()
```

### Comparing `spotidex-0.0.5/spotidex/cli/utils.py` & `spotidex-0.0.6/spotidex/cli/utils.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/src/content.py` & `spotidex-0.0.6/spotidex/src/content.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/src/download.py` & `spotidex-0.0.6/spotidex/src/download.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/src/static.py` & `spotidex-0.0.6/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.5/spotidex/src/utils.py` & `spotidex-0.0.6/spotidex/src/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os,re,stat,platform,requests,subprocess
 from mutagen.id3 import ID3, APIC, TPE1, TIT2, TALB
 import concurrent.futures
 from pathlib import Path
 from tqdm import tqdm
+from rich.progress import Progress, SpinnerColumn
+from rich.console import Console
 
 from spotidex.src.static import FFMPEG_URLS
 
 progress_dict = {}
 class SpotidexError(Exception):
     def __init__(self,message):
         self.message = message
@@ -117,15 +119,16 @@
     os_name = platform.system().lower()
     os_arch = platform.machine().lower()
 
     ffmpeg_url = FFMPEG_URLS.get(os_name, {}).get(os_arch)
     ffmpeg_path = get_ffmpeg_path(os_name)
 
     if ffmpeg_path.exists():
-        run_ffmpeg(ffmpeg_path)
+        if not run_ffmpeg(ffmpeg_path) :
+            download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name)
         return ffmpeg_path
 
     download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name)
     return ffmpeg_path
 
 def get_ffmpeg_path(os_name):
     executable_extension = ".exe" if os_name == "windows" else ""
@@ -135,50 +138,41 @@
     current_path = Path().cwd()
     os.chdir(get_spotidex_data_directory())
     try:
         subprocess.run(
             [ffmpeg_path], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
     except Exception:
-        print("Network Error: Please check your internet connection and try later")
-        exit()
-    finally:
-        os.chdir(current_path)
-
+        return False
+    os.chdir(current_path)
+    return True
 
 def download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name):
     try:
         ffmpeg_binary = requests.get(ffmpeg_url, stream=True, timeout=10)
     except Exception:
         print("Network Error: Please check your internet connection and try later")
         exit()
-
-    with open(ffmpeg_path, "wb") as ffmpeg_file, tqdm(
-        total=100,
-        unit="%",
-        unit_scale=True,
-        unit_divisor=1024,
-        dynamic_ncols=True,
-        bar_format="Initializing : |{bar:50}| {percentage:.0f}% ",
-    ) as progress_bar:
+    with open(ffmpeg_path, "wb") as ffmpeg_file:
         try:
-            for data in ffmpeg_binary.iter_content(chunk_size=1024):
-                ffmpeg_file.write(data)
-                progress_bar.update(
-                    len(data)
-                    * 100
-                    / int(ffmpeg_binary.headers.get("content-length", 0))
-                )
-        except Exception:
-            progress_bar.close()
+            total_length = int(ffmpeg_binary.headers.get("content-length", 0))
+            with Progress(
+                SpinnerColumn('arc'),
+                " INITIALIZING{task.percentage:>3.0f}%",
+            ) as progress:
+                task = progress.add_task("Downloading", total=total_length)
+                for data in ffmpeg_binary.iter_content(chunk_size=1024):
+                    ffmpeg_file.write(data)
+                    progress.update(task, advance=len(data), total_bytes=total_length)
+        except Exception as e:
             print("Network Error: Please check your internet connection and try later")
             exit()
 
     if os_name in ["linux", "darwin"]:
         ffmpeg_path.chmod(ffmpeg_path.stat().st_mode | stat.S_IEXEC)
 
 def get_valid_name(path, name):
     name, i = re.sub(r"[^\w\d(),.\-\[\] ]", "", name), 1
     add_mp3 = ".mp3" if ".mp3" in name else ""
     while Path(path, name).exists():
-        name, i = name.replace('.mp3',"").split(" (")[0] + f" ({i})" + add_mp3, i + 1
+        name, i = name.replace('.mp3',"").split(" (")[-1] + f" ({i})" + add_mp3, i + 1
     return name.replace('.mp3',"")
```

### Comparing `spotidex-0.0.5/PKG-INFO` & `spotidex-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spotify Downloader TUI
 License: MIT
 Author: Libin Lalu
 Author-email: libinlalu000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mutagen (==1.47.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.1)
 Requires-Dist: spotipy (==2.23.0)
 Requires-Dist: textual (==0.56.4)
 Requires-Dist: tqdm (==4.66.1)
 Requires-Dist: yt-dlp (==2024.3.10)
 Requires-Dist: ytmusicapi (==1.3.2)
```

