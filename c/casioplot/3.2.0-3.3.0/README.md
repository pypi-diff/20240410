# Comparing `tmp/casioplot-3.2.0.tar.gz` & `tmp/casioplot-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casioplot-3.2.0.tar", last modified: Mon Apr  8 13:56:11 2024, max compression
+gzip compressed data, was "casioplot-3.3.0.tar", last modified: Wed Apr 10 14:41:09 2024, max compression
```

## Comparing `casioplot-3.2.0.tar` & `casioplot-3.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:56:05.000000 casioplot-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 13:56:05.000000 casioplot-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-08 13:56:11.547819 casioplot-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 13:56:05.000000 casioplot-3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-08 13:56:05.000000 casioplot-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:56:11.547819 casioplot-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.543819 casioplot-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.543819 casioplot-3.2.0/src/casioplot/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot/bg_images/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/bg_images/blanck.png
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/bg_images/calculator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/casioplot.py
--rw-r--r--   0 runner    (1001) docker     (127)   127342 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/characters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot/presets/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/default.toml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/fx-CG50.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/fx-CG50_AU.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/presets/graph_90+e.toml
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 13:56:05.000000 casioplot-3.2.0/src/casioplot/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:56:11.547819 casioplot-3.2.0/src/casioplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 13:56:11.000000 casioplot-3.2.0/src/casioplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.614899 casioplot-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 14:41:03.000000 casioplot-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 14:41:03.000000 casioplot-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-10 14:41:09.614899 casioplot-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-10 14:41:03.000000 casioplot-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 14:41:03.000000 casioplot-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:41:09.614899 casioplot-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.610898 casioplot-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.610898 casioplot-3.3.0/src/casioplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.610898 casioplot-3.3.0/src/casioplot/bg_images/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/bg_images/blanck.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/bg_images/calculator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/casioplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127342 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.614899 casioplot-3.3.0/src/casioplot/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/presets/default.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/presets/fx-CG50.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/presets/fx-CG50_AU.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/presets/graph_90+e.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-10 14:41:03.000000 casioplot-3.3.0/src/casioplot/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:41:09.614899 casioplot-3.3.0/src/casioplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-10 14:41:09.000000 casioplot-3.3.0/src/casioplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 14:41:09.000000 casioplot-3.3.0/src/casioplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:41:09.000000 casioplot-3.3.0/src/casioplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:41:09.000000 casioplot-3.3.0/src/casioplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 14:41:09.000000 casioplot-3.3.0/src/casioplot.egg-info/top_level.txt
```

### Comparing `casioplot-3.2.0/LICENSE` & `casioplot-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casioplot-3.2.0/PKG-INFO` & `casioplot-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.2.0
+Version: 3.3.0
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,22 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Pillow
 
 Casioplot for computers
 =======================
 
+.. image:: https://readthedocs.org/projects/casioplot/badge/?version=latest
+    :target: https://casioplot.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://badge.fury.io/py/casioplot.svg
+    :target: https://badge.fury.io/py/casioplot
+    :alt: PyPI Status
+
 Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
@@ -124,8 +132,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.2.0 - Uniwix - MiguelTorrinhaPereira
+v 3.3.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.2.0/README.rst` & `casioplot-3.3.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Casioplot for computers
 =======================
 
+.. image:: https://readthedocs.org/projects/casioplot/badge/?version=latest
+    :target: https://casioplot.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://badge.fury.io/py/casioplot.svg
+    :target: https://badge.fury.io/py/casioplot
+    :alt: PyPI Status
+
 Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
@@ -83,8 +91,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.2.0 - Uniwix - MiguelTorrinhaPereira
+v 3.3.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.2.0/pyproject.toml` & `casioplot-3.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Pillow"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "casioplot"
-version = "3.2.0"
+version = "3.3.0"
 description = "Use casioplot module on a computer"
 readme = "README.rst"
 authors = [
     { name = "Uniwix", email = "uniwixu@gmail.com" },
     { name = "Miguel Torrinha Pereira", email = "miguel.torrinha.pereira+pypi@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `casioplot-3.2.0/src/casioplot/bg_images/calculator.png` & `casioplot-3.3.0/src/casioplot/bg_images/calculator.png`

 * *Files identical despite different names*

### Comparing `casioplot-3.2.0/src/casioplot/casioplot.py` & `casioplot-3.3.0/src/casioplot/casioplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,21 @@
     Using a try statement is faster than checking if the coordinates are in bounds.
 
     :param x: x coordinate (from the left)
     :param y: y coordinate (from the top)
     :param color: The pixel color. A tuple that contain 3 integers from 0 to 255
     """
     try:
+        if _settings["correct_colors"] is True:  # corrects the colors to match the behavior of the casio calculators
+            color = (  # there may be a faster way
+                color[0] - color[0] % 8,
+                color[1] - color[1] % 4,
+                color[2] - color[2] % 8
+            )
+
         _canvas.put(
             "#%02x%02x%02x" % color,  # convert the color (RGB tuple) to a hexadecimal string '#RRGGBB'
             to=(x, y)
         )
     except tk.TclError:  # the pixel is out of the canvas
         pass
 
@@ -215,21 +222,19 @@
     _background_display.place(x=0, y=0)
     _canvas_display = tk.Label(master=_window, image=_canvas, border=0)
     """The tkinter label that shows the canvas
 
     :meta hide-value:
     """
     _canvas_display.place(x=_settings["left_margin"], y=_settings["top_margin"])
+
 except tk.TclError:
     print("The tkinter window couldn't be created. The screen won't be shown.")
 
 
 @atexit.register
-def run_at_exit() -> None:
+def _run_at_exit() -> None:
     """This function should be called at the end of the program to close the tkinter window"""
     if _settings["save_screen"] is True:  # saves the thes screen as it was before the program ended
         _save_screen()
-    if _settings["show_screen"] is True:  # keeps the tkinter window open after the program ends
-        if _settings["close_window"] is True:
-            _window.destroy()
-        else:
-            _window.mainloop()
+    if _settings["show_screen"] is True and _settings["close_window"] is False:  # keeps the tkinter window open after the program ends
+        _window.mainloop()
```

### Comparing `casioplot-3.2.0/src/casioplot/characters.py` & `casioplot-3.3.0/src/casioplot/characters.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.2.0/src/casioplot/presets/default.toml` & `casioplot-3.3.0/src/casioplot/presets/default.toml`

 * *Files 6% similar despite different names*

```diff
@@ -59,7 +59,12 @@
 # where number is the number of the save.
 [saving_screen]
 save_screen = false
 image_name = "casioplot"
 image_format = "png"
 save_multiple = false
 save_rate = 1
+
+# the casio calculators don't have the same precission for colors as the computer
+# the option `correct_colors` makes the set_pixel function correct the colors to match what would happen in the calculators
+[colors]
+correct_colors = false
```

### Comparing `casioplot-3.2.0/src/casioplot/settings.py` & `casioplot-3.3.0/src/casioplot/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,18 @@
         ),
         "saving_screen": (
             "save_screen",
             "image_name",
             "image_format",
             "save_multiple",
             "save_rate"
-        )
+        ),
+        "colors": (
+            "correct_colors",
+        ),
     }
 
     def _check_toml(toml: dict) -> None:
         """Checks for wrong settings and section in the toml
 
         :py:func:`_check_settings` doesn't notice this type of error because:py:func:`_get_configuration_from_file`
         doesn't read them, so they aren't part of the config return by :py:func:`_get_configuration_from_file`
```

### Comparing `casioplot-3.2.0/src/casioplot/types.py` & `casioplot-3.3.0/src/casioplot/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This file contains the types :py:class:`Configuration`, :py:class:`Color` and :py:class:`Text_size`"""
 
 from typing import TypedDict, Literal
 
 
 class Configuration(TypedDict, total=False):
-    """The type :py:class:`Configuration` makes it possible to representing all settings and configs in a dictionary but still
-    have type annotations for every setting.
+    """The type :py:class:`Configuration` makes it possible to representing all settings and configs in a dictionary
+    but still have type annotations for every setting.
     The option :python:`total=False` makes it possible for a configuration to not have a value for all settings"""
 
     # canvas size
     width: int  # canvas width in pixels
     height: int  # canvas height in pixels
 
     # margins
@@ -31,14 +31,16 @@
     save_screen: bool  # Save the screen as an image
     image_name: str
     image_format: str  # should be one of the following image formats: jpeg, jpg, png, gif, bmp, tiff or tif
     save_multiple: bool  # save multiple images so that the user can examine better the virtual screen
     save_rate: int  # if `save_multiple is True a new image will be saved`
     # every `save_rate` times show_screen is called
 
+    correct_colors: bool  # the casio calculators don't have the same precission for colors as the computer
+    # this options makes the set_pixel function correct the colors to match what would happen in the calculators
 
 Color = tuple[int, int, int]
 """A color is represented as a tuple of three integers, each integer is in the range [0, 255] and represents the
 intensity of the color in the red, green and blue channels respectively."""
 
 
 Text_size = Literal["small", "medium", "large"]
```

### Comparing `casioplot-3.2.0/src/casioplot.egg-info/PKG-INFO` & `casioplot-3.3.0/src/casioplot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.2.0
+Version: 3.3.0
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,22 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Pillow
 
 Casioplot for computers
 =======================
 
+.. image:: https://readthedocs.org/projects/casioplot/badge/?version=latest
+    :target: https://casioplot.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://badge.fury.io/py/casioplot.svg
+    :target: https://badge.fury.io/py/casioplot
+    :alt: PyPI Status
+
 Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
@@ -124,8 +132,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.2.0 - Uniwix - MiguelTorrinhaPereira
+v 3.3.0 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.2.0/src/casioplot.egg-info/SOURCES.txt` & `casioplot-3.3.0/src/casioplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

