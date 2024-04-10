# Comparing `tmp/noobstuffs-2.0.3.tar.gz` & `tmp/noobstuffs-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noobstuffs-2.0.3.tar", max compression
+gzip compressed data, was "noobstuffs-2.0.4.tar", max compression
```

## Comparing `noobstuffs-2.0.3.tar` & `noobstuffs-2.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      797 2024-04-07 14:36:55.084895 noobstuffs-2.0.3/NoobStuffs/__init__.py
--rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.3/NoobStuffs/libandroid/__init__.py
--rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.3/NoobStuffs/libdatetime/__init__.py
--rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.3/NoobStuffs/libformatter/__init__.py
--rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.3/NoobStuffs/libformatter/escape.py
--rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.3/NoobStuffs/libgithub/__init__.py
--rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.3/NoobStuffs/liblogging/__init__.py
--rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.3/NoobStuffs/libpasty/__init__.py
--rwxr-xr-x   0        0        0     1696 2024-04-07 14:37:17.247443 noobstuffs-2.0.3/NoobStuffs/libtelegrambot/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.3/NoobStuffs/libtelegraph/__init__.py
--rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.3/README.md
--rw-r--r--   0        0        0      805 2024-04-07 14:36:00.749090 noobstuffs-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-04-10 11:33:17.152746 noobstuffs-2.0.4/NoobStuffs/__init__.py
+-rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.4/NoobStuffs/libandroid/__init__.py
+-rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.4/NoobStuffs/libdatetime/__init__.py
+-rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.4/NoobStuffs/libformatter/__init__.py
+-rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.4/NoobStuffs/libformatter/escape.py
+-rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.4/NoobStuffs/libgithub/__init__.py
+-rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.4/NoobStuffs/liblogging/__init__.py
+-rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.4/NoobStuffs/libpasty/__init__.py
+-rwxr-xr-x   0        0        0     1991 2024-04-09 12:36:20.032841 noobstuffs-2.0.4/NoobStuffs/libtelegrambot/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.4/NoobStuffs/libtelegraph/__init__.py
+-rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.4/README.md
+-rw-r--r--   0        0        0      805 2024-04-10 11:33:32.586248 noobstuffs-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.4/PKG-INFO
```

### Comparing `noobstuffs-2.0.3/NoobStuffs/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
```

### Comparing `noobstuffs-2.0.3/NoobStuffs/libandroid/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libdatetime/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libdatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libformatter/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libformatter/escape.py` & `noobstuffs-2.0.4/NoobStuffs/libformatter/escape.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libgithub/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libgithub/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/liblogging/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/liblogging/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libpasty/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libpasty/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/NoobStuffs/libtelegrambot/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libtelegrambot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 
 from telegram import InlineKeyboardButton, InlineKeyboardMarkup
 from telegram.constants import ParseMode
 from telegram.ext import ApplicationBuilder
 
 
 class TelegramLogBot:
-    def __init__(self, token: str, chat_id: int, parse_mode: ParseMode):
+    def __init__(
+        self,
+        token: str,
+        chat_id: int,
+        parse_mode: ParseMode,
+        disable_web_page_preview: bool,
+    ):
         self.__app = ApplicationBuilder().token(token).build()
         self.__chat_id = chat_id
         self.__parse_mode = parse_mode
+        self.__disable_web_page_preview = disable_web_page_preview
         self.__buttons = []
         self.__button_index = -1
 
     def build_button(self, text: str, link: str, newline: bool = False):
         button = InlineKeyboardButton(text=text, url=link)
         if newline or len(self.__buttons) == 0:
             self.__button_index += 1
@@ -28,18 +35,20 @@
     async def log_msg(self, message: str, use_buttons: bool = False):
         reply_markup = InlineKeyboardMarkup(self.__buttons) if use_buttons else None
         await self.__app.bot.send_message(
             text=message,
             chat_id=self.__chat_id,
             reply_markup=reply_markup,
             parse_mode=self.__parse_mode,
+            disable_web_page_preview=self.__disable_web_page_preview,
         )
 
     async def log_img(self, image: BinaryIO, caption: str, use_buttons: bool = False):
         reply_markup = InlineKeyboardMarkup(self.__buttons) if use_buttons else None
         await self.__app.bot.send_photo(
             photo=image,
             chat_id=self.__chat_id,
             caption=caption,
             reply_markup=reply_markup,
             parse_mode=self.__parse_mode,
+            disable_web_page_preview=self.__disable_web_page_preview,
         )
```

### Comparing `noobstuffs-2.0.3/NoobStuffs/libtelegraph/__init__.py` & `noobstuffs-2.0.4/NoobStuffs/libtelegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/README.md` & `noobstuffs-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.3/pyproject.toml` & `noobstuffs-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NoobStuffs"
-version = "2.0.3"
+version = "2.0.4"
 description = "Python Library for PrajjuS Projects"
 license = "GPL-3.0"
 authors = ["PrajjuS <theprajjus@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PrajjuS/NoobStuffs"
 keywords = ["noobstuffs", "libs", "noob", "lazy"]
 classifiers = [
```

### Comparing `noobstuffs-2.0.3/PKG-INFO` & `noobstuffs-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NoobStuffs
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python Library for PrajjuS Projects
 Home-page: https://github.com/PrajjuS/NoobStuffs
 License: GPL-3.0
 Keywords: noobstuffs,libs,noob,lazy
 Author: PrajjuS
 Author-email: theprajjus@gmail.com
 Requires-Python: >=3.8,<4.0
```

