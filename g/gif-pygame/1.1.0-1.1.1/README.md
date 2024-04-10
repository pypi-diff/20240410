# Comparing `tmp/gif_pygame-1.1.0.tar.gz` & `tmp/gif_pygame-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-1.1.0.tar", last modified: Fri Oct  6 09:52:09 2023, max compression
+gzip compressed data, was "gif_pygame-1.1.1.tar", last modified: Wed Apr 10 13:26:05 2024, max compression
```

## Comparing `gif_pygame-1.1.0.tar` & `gif_pygame-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-10-06 09:52:09.809275 gif_pygame-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5216 2023-10-06 09:52:09.807272 gif_pygame-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2023-10-06 09:51:49.000000 gif_pygame-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-06 09:52:09.797224 gif_pygame-1.1.0/gif_pygame/
--rw-rw-rw-   0        0        0      111 2023-10-06 08:19:03.000000 gif_pygame-1.1.0/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0      397 2023-10-05 18:17:43.000000 gif_pygame-1.1.0/gif_pygame/_common.py
--rw-rw-rw-   0        0        0    16349 2023-10-06 08:27:13.000000 gif_pygame-1.1.0/gif_pygame/gif_pygame.py
--rw-rw-rw-   0        0        0    18523 2023-10-06 08:21:00.000000 gif_pygame-1.1.0/gif_pygame/transform.py
-drwxrwxrwx   0        0        0        0 2023-10-06 09:52:09.806262 gif_pygame-1.1.0/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     5216 2023-10-06 09:52:09.000000 gif_pygame-1.1.0/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-10-06 09:52:09.000000 gif_pygame-1.1.0/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-06 09:52:09.000000 gif_pygame-1.1.0/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-10-06 09:52:09.000000 gif_pygame-1.1.0/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-06 09:52:09.000000 gif_pygame-1.1.0/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-06 09:52:09.809275 gif_pygame-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-10-06 08:19:51.000000 gif_pygame-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:26:05.161520 gif_pygame-1.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4760 2024-04-10 13:26:05.160521 gif_pygame-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3727 2024-04-10 13:23:11.000000 gif_pygame-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 13:26:05.149581 gif_pygame-1.1.1/gif_pygame/
+-rw-rw-rw-   0        0        0      100 2024-04-10 13:14:14.000000 gif_pygame-1.1.1/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-10-05 18:17:43.000000 gif_pygame-1.1.1/gif_pygame/_common.py
+-rw-rw-rw-   0        0        0     8566 2024-04-10 13:24:58.000000 gif_pygame-1.1.1/gif_pygame/gif_pygame.py
+-rw-rw-rw-   0        0        0    18517 2024-04-10 13:25:43.000000 gif_pygame-1.1.1/gif_pygame/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:26:05.159520 gif_pygame-1.1.1/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     4760 2024-04-10 13:26:05.000000 gif_pygame-1.1.1/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-10 13:26:05.000000 gif_pygame-1.1.1/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:26:05.000000 gif_pygame-1.1.1/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 13:26:05.000000 gif_pygame-1.1.1/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 13:26:05.000000 gif_pygame-1.1.1/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:26:05.161520 gif_pygame-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2024-04-10 05:13:40.000000 gif_pygame-1.1.1/setup.py
```

### Comparing `gif_pygame-1.1.0/LICENSE` & `gif_pygame-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-1.1.0/PKG-INFO` & `gif_pygame-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif_pygame
-Version: 1.1.0
+Version: 1.1.1
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,18 @@
 s3 = pygame.Surface((66, 66))
 s1.fill((255, 0, 0))
 s2.fill((0, 255, 0))
 s3.fill((0, 0, 255))
 
 example_surfs = gif_pygame.GIFPygame([(s1, 1), (s2, 1), (s3, 1)])
 
+clock = pygame.Clock()
+
 while True:
+    clock.tick(60)
     win.fill((0, 0, 0))
     
     # There are 2 ways of rendering the animated img file, the first method is doing "gif.render(surface, (x, y))", the other method is doing "surface.blit(gif.blit_ready(), (x, y))". THE ".blit_ready()" FUNCTION MUST BE CALLED WHEN DOING THE SECOND METHOD
     example_gif.render(win, (128-example_gif.get_width()*0.5, 256-example_gif.get_height()*0.5))
     example_png.render(win, (256-example_png.get_width()*0.5, 256-example_png.get_height()*0.5))
     win.blit(example_surfs.blit_ready(), (384-example_surfs.get_width()*0.5, 256-example_surfs.get_height()*0.5))
 
@@ -71,15 +74,15 @@
                     example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
 
                 if example_surfs.paused: # Check whether `example_surfs` is paused or not
                     example_surfs.unpause() # unpauses `example_surfs` if it was paused
                 else:
                     example_surfs.pause() # pauses `example_surfs` if it was unpaused
                     
-    pygame.display.update()
+    pygame.display.flip()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
 
 To render the image you've got 2 options:
@@ -92,16 +95,12 @@
 - `GIFPygame.get_width()`, returns the width of the image
 - `GIFPygame.get_height()`, returns the height of the image
 - `GIFPygame.get_size()`, returns the size of the image
 - `GIFPygame.get_rect()`, returns the rect of the image
 - `GIFPygame.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `GIFPygame.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
 - `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
-- `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
-- `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
-- `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
+- `gif_pygame.transform()`, a sublibrary for editing the surfaces.
 
 Please use python's `help()` function for more in-depth explanation
 
 (A documentation will be added soon)
```

### Comparing `gif_pygame-1.1.0/README.md` & `gif_pygame-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 s3 = pygame.Surface((66, 66))
 s1.fill((255, 0, 0))
 s2.fill((0, 255, 0))
 s3.fill((0, 0, 255))
 
 example_surfs = gif_pygame.GIFPygame([(s1, 1), (s2, 1), (s3, 1)])
 
+clock = pygame.Clock()
+
 while True:
+    clock.tick(60)
     win.fill((0, 0, 0))
     
     # There are 2 ways of rendering the animated img file, the first method is doing "gif.render(surface, (x, y))", the other method is doing "surface.blit(gif.blit_ready(), (x, y))". THE ".blit_ready()" FUNCTION MUST BE CALLED WHEN DOING THE SECOND METHOD
     example_gif.render(win, (128-example_gif.get_width()*0.5, 256-example_gif.get_height()*0.5))
     example_png.render(win, (256-example_png.get_width()*0.5, 256-example_png.get_height()*0.5))
     win.blit(example_surfs.blit_ready(), (384-example_surfs.get_width()*0.5, 256-example_surfs.get_height()*0.5))
 
@@ -46,15 +49,15 @@
                     example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
 
                 if example_surfs.paused: # Check whether `example_surfs` is paused or not
                     example_surfs.unpause() # unpauses `example_surfs` if it was paused
                 else:
                     example_surfs.pause() # pauses `example_surfs` if it was unpaused
                     
-    pygame.display.update()
+    pygame.display.flip()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
 
 To render the image you've got 2 options:
@@ -67,16 +70,12 @@
 - `GIFPygame.get_width()`, returns the width of the image
 - `GIFPygame.get_height()`, returns the height of the image
 - `GIFPygame.get_size()`, returns the size of the image
 - `GIFPygame.get_rect()`, returns the rect of the image
 - `GIFPygame.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `GIFPygame.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
 - `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
-- `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
-- `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
-- `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
+- `gif_pygame.transform()`, a sublibrary for editing the surfaces.
 
 Please use python's `help()` function for more in-depth explanation
 
 (A documentation will be added soon)
```

### Comparing `gif_pygame-1.1.0/gif_pygame/transform.py` & `gif_pygame-1.1.1/gif_pygame/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: UTF-8 -*-
 
 """
-allows for easy gif tranformation
+allows for easy gif editing
 """
 
 import pygame, warnings
 
 from typing import Union, Tuple, Sequence, Iterable, Optional
 from gif_pygame.gif_pygame import GIFPygame, is_ce
```

### Comparing `gif_pygame-1.1.0/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-1.1.1/gif_pygame.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gif-pygame
-Version: 1.1.0
+Name: gif_pygame
+Version: 1.1.1
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,18 @@
 s3 = pygame.Surface((66, 66))
 s1.fill((255, 0, 0))
 s2.fill((0, 255, 0))
 s3.fill((0, 0, 255))
 
 example_surfs = gif_pygame.GIFPygame([(s1, 1), (s2, 1), (s3, 1)])
 
+clock = pygame.Clock()
+
 while True:
+    clock.tick(60)
     win.fill((0, 0, 0))
     
     # There are 2 ways of rendering the animated img file, the first method is doing "gif.render(surface, (x, y))", the other method is doing "surface.blit(gif.blit_ready(), (x, y))". THE ".blit_ready()" FUNCTION MUST BE CALLED WHEN DOING THE SECOND METHOD
     example_gif.render(win, (128-example_gif.get_width()*0.5, 256-example_gif.get_height()*0.5))
     example_png.render(win, (256-example_png.get_width()*0.5, 256-example_png.get_height()*0.5))
     win.blit(example_surfs.blit_ready(), (384-example_surfs.get_width()*0.5, 256-example_surfs.get_height()*0.5))
 
@@ -71,15 +74,15 @@
                     example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
 
                 if example_surfs.paused: # Check whether `example_surfs` is paused or not
                     example_surfs.unpause() # unpauses `example_surfs` if it was paused
                 else:
                     example_surfs.pause() # pauses `example_surfs` if it was unpaused
                     
-    pygame.display.update()
+    pygame.display.flip()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
 
 To render the image you've got 2 options:
@@ -92,16 +95,12 @@
 - `GIFPygame.get_width()`, returns the width of the image
 - `GIFPygame.get_height()`, returns the height of the image
 - `GIFPygame.get_size()`, returns the size of the image
 - `GIFPygame.get_rect()`, returns the rect of the image
 - `GIFPygame.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `GIFPygame.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
 - `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
-- `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
-- `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
-- `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
+- `gif_pygame.transform()`, a sublibrary for editing the surfaces.
 
 Please use python's `help()` function for more in-depth explanation
 
 (A documentation will be added soon)
```

### Comparing `gif_pygame-1.1.0/setup.py` & `gif_pygame-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="1.1.0",
+    version="1.1.1",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pygame-ce", "pillow"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
```

