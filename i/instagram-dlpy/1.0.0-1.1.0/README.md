# Comparing `tmp/instagram-dlpy-1.0.0.tar.gz` & `tmp/instagram-dlpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-dlpy-1.0.0.tar", last modified: Thu Mar 28 00:51:47 2024, max compression
+gzip compressed data, was "instagram-dlpy-1.1.0.tar", last modified: Tue Apr  9 22:16:57 2024, max compression
```

## Comparing `instagram-dlpy-1.0.0.tar` & `instagram-dlpy-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-28 00:51:47.831031 instagram-dlpy-1.0.0/
--rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-28 00:29:28.000000 instagram-dlpy-1.0.0/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)     1335 2024-03-28 00:51:47.830961 instagram-dlpy-1.0.0/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      605 2024-03-28 00:35:14.000000 instagram-dlpy-1.0.0/README.md
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-28 00:51:47.830772 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)     1335 2024-03-28 00:51:47.000000 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      331 2024-03-28 00:51:47.000000 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2024-03-28 00:51:47.000000 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2024-03-28 00:51:47.000000 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)       12 2024-03-28 00:51:47.000000 instagram-dlpy-1.0.0/instagram_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-28 00:51:47.830130 instagram-dlpy-1.0.0/instagramdl/
--rw-r--r--   0 becky      (501) staff       (20)        0 2023-06-21 12:21:02.000000 instagram-dlpy-1.0.0/instagramdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)     2473 2024-03-28 00:03:26.000000 instagram-dlpy-1.0.0/instagramdl/api.py
--rw-r--r--   0 becky      (501) staff       (20)     3318 2024-03-28 00:12:21.000000 instagram-dlpy-1.0.0/instagramdl/models.py
--rw-r--r--   0 becky      (501) staff       (20)     6974 2024-03-27 23:25:59.000000 instagram-dlpy-1.0.0/instagramdl/parser.py
--rw-r--r--   0 becky      (501) staff       (20)       79 2024-03-28 00:51:47.831255 instagram-dlpy-1.0.0/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)     1022 2024-03-28 00:39:44.000000 instagram-dlpy-1.0.0/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-03-28 00:51:47.830430 instagram-dlpy-1.0.0/tests/
--rw-r--r--   0 becky      (501) staff       (20)     3740 2024-03-28 00:27:41.000000 instagram-dlpy-1.0.0/tests/test_urls.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180484 instagram-dlpy-1.1.0/
+-rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)     1347 2024-04-09 22:16:57.180411 instagram-dlpy-1.1.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      617 2024-03-28 00:54:03.000000 instagram-dlpy-1.1.0/README.md
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180229 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)     1347 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      331 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)       12 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.179922 instagram-dlpy-1.1.0/instagramdl/
+-rw-r--r--   0 becky      (501) staff       (20)        0 2023-06-21 12:21:02.000000 instagram-dlpy-1.1.0/instagramdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)     2473 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/instagramdl/api.py
+-rw-r--r--   0 becky      (501) staff       (20)     3723 2024-04-09 22:14:48.000000 instagram-dlpy-1.1.0/instagramdl/models.py
+-rw-r--r--   0 becky      (501) staff       (20)     6974 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/instagramdl/parser.py
+-rw-r--r--   0 becky      (501) staff       (20)       79 2024-04-09 22:16:57.180662 instagram-dlpy-1.1.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)     1022 2024-04-09 22:15:34.000000 instagram-dlpy-1.1.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180053 instagram-dlpy-1.1.0/tests/
+-rw-r--r--   0 becky      (501) staff       (20)     3740 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/tests/test_urls.py
```

### Comparing `instagram-dlpy-1.0.0/LICENSE` & `instagram-dlpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-dlpy-1.0.0/PKG-INFO` & `instagram-dlpy-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: instagram-dlpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python package to download Instagram posts by URL without needing to login
 Home-page: https://github.com/Fluxticks/InstagramDL
-Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.0.0.tar.gz
+Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz
 Author: Fluxticks
 Keywords: instagram,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/instagram-dlpy)
+
 # InstagramDL
 
 A python package to download Instagram posts by URL without needing to login.
 
-## TODO
-
-- Upload package to PyPI
-
 ## Usage
 
 1. Install the package
 
 ```bash
-$ pip install git+https://github.com/Fluxticks/InstagramDL.git
+$ pip install instagram-dlpy
 ```
 
 2. Import the package
 
 ```python
 from instagramdl.api import get_post_data
 from instagramdl.parser import parse_api_response
```

### Comparing `instagram-dlpy-1.0.0/instagram_dlpy.egg-info/PKG-INFO` & `instagram-dlpy-1.1.0/instagram_dlpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: instagram-dlpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python package to download Instagram posts by URL without needing to login
 Home-page: https://github.com/Fluxticks/InstagramDL
-Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.0.0.tar.gz
+Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz
 Author: Fluxticks
 Keywords: instagram,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/instagram-dlpy)
+
 # InstagramDL
 
 A python package to download Instagram posts by URL without needing to login.
 
-## TODO
-
-- Upload package to PyPI
-
 ## Usage
 
 1. Install the package
 
 ```bash
-$ pip install git+https://github.com/Fluxticks/InstagramDL.git
+$ pip install instagram-dlpy
 ```
 
 2. Import the package
 
 ```python
 from instagramdl.api import get_post_data
 from instagramdl.parser import parse_api_response
```

### Comparing `instagram-dlpy-1.0.0/instagramdl/api.py` & `instagram-dlpy-1.1.0/instagramdl/api.py`

 * *Files identical despite different names*

### Comparing `instagram-dlpy-1.0.0/instagramdl/models.py` & `instagram-dlpy-1.1.0/instagramdl/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,23 @@
     profile_pic_url: str
     full_name: str
     is_private: bool
     follower_count: int
     post_count: int
     related_profiles: Optional[List["User"]] = None
 
+    @property
+    def url(self) -> str:
+        """The users actual URL.
+
+        Returns:
+            str: The URL of the user.
+        """
+        return f"https://www.instagram.com/{self.username}"
+
 
 class PostKind(StrEnum):
     """A string enum to store the Instagram string representations of the different post types."""
 
     VIDEO = "XDTGraphVideo"
     IMAGE = "XDTGraphImage"
     MULTI = "XDTGraphSidecar"
@@ -53,14 +62,23 @@
     height: int
     user: User
     caption: str
     timestamp: int
     like_count: int
     comment_count: int
 
+    @property
+    def url(self) -> str:
+        """The actual URL of the post.
+
+        Returns:
+            str: The post URL
+        """
+        return f"https://www.instagram.com/p/{self.shortcode}"
+
     def download(
         self, download_path: str, max_chunk_size: int = 8192
     ) -> Union[str, List[str]]:
         """Downloads any media related to a post. Cannot be used on the generic `Post` class as it has no associated media.
 
         Args:
             download_path (str): The path to download the files to.
```

### Comparing `instagram-dlpy-1.0.0/instagramdl/parser.py` & `instagram-dlpy-1.1.0/instagramdl/parser.py`

 * *Files identical despite different names*

### Comparing `instagram-dlpy-1.0.0/setup.py` & `instagram-dlpy-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="instagram-dlpy",
-    version="1.0.0",
+    version="1.1.0",
     url="https://github.com/Fluxticks/InstagramDL",
-    download_url="https://github.com/Fluxticks/InstagramDL/archive/v1.0.0.tar.gz",
+    download_url="https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=["requests"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A python package to download Instagram posts by URL without needing to login",
     classifiers=[
```

### Comparing `instagram-dlpy-1.0.0/tests/test_urls.py` & `instagram-dlpy-1.1.0/tests/test_urls.py`

 * *Files identical despite different names*

