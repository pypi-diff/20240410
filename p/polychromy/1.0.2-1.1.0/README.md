# Comparing `tmp/polychromy-1.0.2.tar.gz` & `tmp/polychromy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polychromy-1.0.2.tar", last modified: Fri Dec 29 14:32:03 2023, max compression
+gzip compressed data, was "polychromy-1.1.0.tar", last modified: Wed Apr 10 14:24:09 2024, max compression
```

## Comparing `polychromy-1.0.2.tar` & `polychromy-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-12-29 14:32:03.081889 polychromy-1.0.2/
--rw-r--r--   0 simon     (1000) simon     (1000)     1073 2023-12-01 16:50:16.000000 polychromy-1.0.2/LICENSE.md
--rw-r--r--   0 simon     (1000) simon     (1000)       25 2023-12-16 23:59:44.000000 polychromy-1.0.2/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     5187 2023-12-29 14:32:03.081889 polychromy-1.0.2/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     4346 2023-12-29 14:25:28.000000 polychromy-1.0.2/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-12-29 14:32:03.081889 polychromy-1.0.2/polychromy/
--rw-r--r--   0 simon     (1000) simon     (1000)       80 2023-12-29 12:02:04.000000 polychromy-1.0.2/polychromy/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-12-29 14:32:03.081889 polychromy-1.0.2/polychromy/data/
--rw-r--r--   0 simon     (1000) simon     (1000)    62454 2023-12-29 13:56:02.000000 polychromy-1.0.2/polychromy/data/colors.json
--rw-r--r--   0 simon     (1000) simon     (1000)      927 2023-12-27 16:15:27.000000 polychromy-1.0.2/polychromy/data/jsoncreator.py
--rw-r--r--   0 simon     (1000) simon     (1000)    10406 2023-12-29 12:01:56.000000 polychromy-1.0.2/polychromy/polychromy.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-12-29 14:32:03.081889 polychromy-1.0.2/polychromy.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     5187 2023-12-29 14:32:03.000000 polychromy-1.0.2/polychromy.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      332 2023-12-29 14:32:03.000000 polychromy-1.0.2/polychromy.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-12-29 14:32:03.000000 polychromy-1.0.2/polychromy.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       23 2023-12-29 14:32:03.000000 polychromy-1.0.2/polychromy.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       11 2023-12-29 14:32:03.000000 polychromy-1.0.2/polychromy.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)      948 2023-12-29 12:02:39.000000 polychromy-1.0.2/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-12-29 14:32:03.081889 polychromy-1.0.2/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)      599 2023-12-29 12:03:13.000000 polychromy-1.0.2/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-10 14:24:09.071574 polychromy-1.1.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1073 2024-01-04 19:24:21.000000 polychromy-1.1.0/LICENSE.md
+-rw-r--r--   0 simon     (1000) simon     (1000)       61 2024-01-10 18:59:46.000000 polychromy-1.1.0/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)     5265 2024-04-10 14:24:09.071574 polychromy-1.1.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     4380 2024-04-10 12:00:25.000000 polychromy-1.1.0/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-10 14:24:09.067574 polychromy-1.1.0/polychromy/
+-rw-r--r--   0 simon     (1000) simon     (1000)       80 2024-01-04 19:24:21.000000 polychromy-1.1.0/polychromy/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-10 14:24:09.071574 polychromy-1.1.0/polychromy/data/
+-rw-r--r--   0 simon     (1000) simon     (1000)    62992 2024-04-10 12:30:16.000000 polychromy-1.1.0/polychromy/data/colors.json
+-rw-r--r--   0 simon     (1000) simon     (1000)    12297 2024-04-10 14:20:22.000000 polychromy-1.1.0/polychromy/polychromy.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-10 14:24:09.071574 polychromy-1.1.0/polychromy.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     5265 2024-04-10 14:24:09.000000 polychromy-1.1.0/polychromy.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-10 14:24:09.000000 polychromy-1.1.0/polychromy.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-10 14:24:09.000000 polychromy-1.1.0/polychromy.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       32 2024-04-10 14:24:09.000000 polychromy-1.1.0/polychromy.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       11 2024-04-10 14:24:09.000000 polychromy-1.1.0/polychromy.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)      988 2024-04-10 11:51:55.000000 polychromy-1.1.0/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-10 14:24:09.071574 polychromy-1.1.0/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)      611 2024-04-10 11:55:31.000000 polychromy-1.1.0/setup.py
```

### Comparing `polychromy-1.0.2/LICENSE.md` & `polychromy-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polychromy-1.0.2/PKG-INFO` & `polychromy-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: polychromy
-Version: 1.0.2
+Version: 1.1.0
 Summary: A module to print a strings in a given colour, with a given colour background
 Author-email: scalvaruso <calvaruso.simone@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://pypi.org/project/polychromy
 Project-URL: Repository, https://github.com/scalvaruso/polychromy
-Keywords: ansi,background,color,colour,format,foreground,Hex,RGB,sRGB,text
+Keywords: ansi,background,color,colour,colorate,font,format,foreground,Hex,paint,RGB,sRGB,text
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: textlinebreaker>=0.1.0
+Requires-Dist: requests
 
 # Polychromy
 
 [<img src="https://img.shields.io/badge/polychromy-py-blue?style=flat&logo=python&logoWidth=20.svg/"></a>](https://github.com/scalvaruso/polychromy/)
 [![PyPI - Version](https://img.shields.io/pypi/v/polychromy?logo=pypi&logoColor=white&color=blue)](https://pypi.org/project/polychromy/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polychromy?logo=python)](https://pypi.org/project/polychromy/)
 [![Downloads](https://static.pepy.tech/badge/polychromy)](https://pepy.tech/project/polychromy)
@@ -36,15 +37,15 @@
 Polychromy is a Python script to manipulate the colors of a text.
 
 ## Features
 
 - Function ```colorate``` prints text of a specified colour in a specified colour background.
 - Function ```show``` prints out color details such as Hex and RGB values of a given colour in a square of the given colour.
 
-## Latest Version 1.0.2
+## Latest Version 1.1.0
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -53,15 +54,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Getting Started
 
 ### Prerequisites
 
-This script relies on the Python standard library and ```textlinebreaker```.
+This script relies on the Python standard library, and the libraries ```requests``` and ```textlinebreaker```.
 
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install polychromy
```

### Comparing `polychromy-1.0.2/README.md` & `polychromy-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Polychromy is a Python script to manipulate the colors of a text.
 
 ## Features
 
 - Function ```colorate``` prints text of a specified colour in a specified colour background.
 - Function ```show``` prints out color details such as Hex and RGB values of a given colour in a square of the given colour.
 
-## Latest Version 1.0.2
+## Latest Version 1.1.0
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -33,15 +33,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Getting Started
 
 ### Prerequisites
 
-This script relies on the Python standard library and ```textlinebreaker```.
+This script relies on the Python standard library, and the libraries ```requests``` and ```textlinebreaker```.
 
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install polychromy
```

### Comparing `polychromy-1.0.2/polychromy/data/colors.json` & `polychromy-1.1.0/polychromy/data/colors.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923857868020305%*

 * *Differences: {"'Live Test'": "OrderedDict([('hex', '#61D6D6'), ('rgb', '97;214;214'), ('xterm', '14'), ('fg', "*

 * *                "'96'), ('bg', '106'), ('alt', 'Cyan From Local')])",*

 * * "'Sensaimidori'": "OrderedDict([('hex', '#374231'), ('rgb', '55;66;49'), ('xterm', ''), ('fg', "*

 * *                   "''), ('bg', ''), ('alt', 'Thousand Year Old Green')])",*

 * * "'Thousand Year Old Green'": "OrderedDict([('hex', '#374231'), ('rgb', '55;66;49'), ('xterm', "*

 * *                              "''), ('fg', ''), ('bg', ''), ('alt', 'Sen […]*

```diff
@@ -1883,14 +1883,22 @@
         "alt": "",
         "bg": "",
         "fg": "",
         "hex": "#FAF0E6",
         "rgb": "250;240;230",
         "xterm": ""
     },
+    "Live Test": {
+        "alt": "Cyan From Local",
+        "bg": "106",
+        "fg": "96",
+        "hex": "#61D6D6",
+        "rgb": "97;214;214",
+        "xterm": "14"
+    },
     "Magenta": {
         "alt": "Fuchsia",
         "bg": "",
         "fg": "",
         "hex": "#FF00FF",
         "rgb": "255;0;255",
         "xterm": "201"
@@ -2723,14 +2731,22 @@
         "alt": "",
         "bg": "",
         "fg": "",
         "hex": "#FFF5EE",
         "rgb": "255;245;238",
         "xterm": ""
     },
+    "Sensaimidori": {
+        "alt": "Thousand Year Old Green",
+        "bg": "",
+        "fg": "",
+        "hex": "#374231",
+        "rgb": "55;66;49",
+        "xterm": ""
+    },
     "Sienna": {
         "alt": "",
         "bg": "",
         "fg": "",
         "hex": "#A0522D",
         "rgb": "160;82;45",
         "xterm": ""
@@ -2963,14 +2979,22 @@
         "alt": "",
         "bg": "",
         "fg": "",
         "hex": "#D7AFD7",
         "rgb": "215;175;215",
         "xterm": "182"
     },
+    "Thousand Year Old Green": {
+        "alt": "Sensaimidori",
+        "bg": "",
+        "fg": "",
+        "hex": "#374231",
+        "rgb": "55;66;49",
+        "xterm": ""
+    },
     "Tomato": {
         "alt": "",
         "bg": "",
         "fg": "",
         "hex": "#FF6347",
         "rgb": "255;99;71",
         "xterm": ""
```

### Comparing `polychromy-1.0.2/polychromy/polychromy.py` & `polychromy-1.1.0/polychromy/polychromy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import json
 import os
 import re
+import requests
+from requests.exceptions import RequestException
 import sys
-import json
 from textlinebreaker import split_line
 
+
 # Create a class for color
 class Color:
     def __init__(self, name, hex, rgb, xterm, fg, bg, alt):
 
         self.name = name
         self.hex = hex
         self.rgb = rgb
@@ -15,23 +18,30 @@
         self.fg = fg
         self.bg = bg
         self.alt = alt
 
 
 # Show example of color
 def main():
+
     show()
 
 
 # Import colors from json file
 def _import_colors():
 
-    data_path = os.path.join(os.path.dirname(__file__), 'data', 'colors.json')
-    with open(data_path, 'r') as file:
-        json_colors = json.load(file)
+    url = 'https://raw.githubusercontent.com/scalvaruso/polychromy/main/dynamic_data/livecolors.json'
+    try:
+        response = requests.get(url)
+        json_colors = response.json()
+
+    except RequestException:
+        data_path = os.path.join(os.path.dirname(__file__), 'data', 'colors.json')
+        with open(data_path, 'r') as file:
+            json_colors = json.load(file)
 
     # Create instances of Color class for each color
     colors = {}
     for color_name, color_details in json_colors.items():
         colors[color_name] = Color(
             name=color_name,
             hex=color_details["hex"],
@@ -43,15 +53,15 @@
         )
 
     return colors
 
 
 # Print a square in the given color with
 # name, xterm, hex, and rgb values of the given color 
-def show(color_in="", colors = _import_colors()):
+def show(color_in="", colors=_import_colors()):
 
     # Check if any argument is passed to the function
     if color_in != "":
         pass
     
     # If no argument is passed to the function it checks if any argument was given launching the program
     # If no argument was given then it uses a random color
@@ -104,17 +114,18 @@
     text = []
     l = 0
     for line in split_line(f"{color_name}",30,"centre"):
         text.append(line)
         l += 1
     text.append("{:^30}".format(""))
     if alt_names:
-        text.append("{:<30}".format(f"Other names: "+ "{:.>17}".format(f" {alt_names}")))
-        text.append("{:^30}".format(""))
-        l += 2
+        alt_line = ("{:>30}".format(f"Other names: "+ "{:.>17}".format(f" {alt_names}")))
+        for line in split_line(f"{alt_line}",30,"right"):
+            text.append(line)
+            l += 1
     if color_fg:
         text.append("{:^30}".format(f"ANSI Color Codes"))
         text.append("{:^30}".format("Foreground: " + "{:.>18}".format(f" {color_fg}")))
         text.append("{:^30}".format("Background: " + "{:.>18}".format(f" {color_bg}")))
         l += 3
     for i in range(7-l):
         text.append("{:^30}".format(""))
@@ -131,129 +142,185 @@
     side_space = " " * 4
 
     syscol = f"x{color_x}"
     if color_in == syscol:
         color_rgb = syscol
 
     # Print color details
-    display_menu  = "\n" + adjustment + colorate(f"╔{or_line}╗", text_color, color_rgb) + "\n"
-    display_menu  += adjustment + colorate(f"║{filling}║", text_color, color_rgb) + "\n"
+    display_color  = "\n" + adjustment + colorate(f"╔{or_line}╗", text_color, color_rgb) + "\n"
+    display_color  += adjustment + colorate(f"║{filling}║", text_color, color_rgb) + "\n"
     for item in text:
-        display_menu  += adjustment + colorate(f"║{side_space + item + side_space}║", text_color, color_rgb) + "\n"
-    display_menu  += adjustment + colorate(f"║{filling}║", text_color, color_rgb) + "\n"
-    display_menu  += adjustment + colorate(f"╚{or_line}╝", text_color, color_rgb) + "\n"
+        display_color  += adjustment + colorate(f"║{side_space + item + side_space}║", text_color, color_rgb) + "\n"
+    display_color  += adjustment + colorate(f"║{filling}║", text_color, color_rgb) + "\n"
+    display_color  += adjustment + colorate(f"╚{or_line}╝", text_color, color_rgb) + "\n"
 
-    print(display_menu)
+    print(display_color)
 
 
 # This function return a given string with escape codes
 # to print it in the given foreground and background colors.
-def colorate(txt,fg_col=37,bg_col=0):
+def colorate(txt, fg_col=37, bg_col=0):
     
     # Check validity of the given colors
-    fg_color = _valid_color(fg_col)
-    bg_color = _valid_color(bg_col, False)
+    fg_color = _valid_color(str(fg_col))
+    if bg_col == 0:
+        bg_color = "\033[0m"
+    else:
+        bg_color = _valid_color(str(bg_col), False)
     
     # If foreground color is equal to the reset code
     # Remove foreground color code
     if (fg_color == "\033[0m") and (fg_color != bg_color):
         fg_color = ""
 
     # Return string with color codes and reset code at the end
     return f"{bg_color}{fg_color}{txt}\033[0m"
 
 
 # Check validity of color
-def _valid_color(color, text=True):
-    
-    palette = _get_color(color) # [0]=name, [1]=alt_name, [2]=color_x, [3]=color_hex, [4]=color_rgb, [5]=color_fg, [6]=color_bg, [7]=unknown
+def _valid_color(color, text=True, all_colors = _import_colors()):
 
-    if isinstance(color,int):
-        color = str(color)
-    
-    if palette[7]:
+    if color.title() in all_colors.keys():  #Color Name
+        color_rgb = all_colors[color.title()].rgb
         if text:
-            return "\033[37m"
+            return f"\033[38;2;{color_rgb}m"
         else:
-            return "\033[0m"
-    elif color==palette[5] or color==palette[6]:
+            return f"\033[48;2;{color_rgb}m"
+
+    elif _check_ansi(color):  #ANSI Color
+        if text:
+            return f"\033[{color}m"
+        else:
+            return f"\033[{color}m"
+
+    elif _check_Xterm(color):   #Xterm Color
         if text:
-            return f"\033[{palette[5]}m"
+            return f"\033[38;5;{color[1:]}m"
         else:
-            return f"\033[{palette[6]}m"
-    elif color[1:] == palette[2]:
+            return f"\033[48;5;{color[1:]}m"
+
+    elif _check_RGB(color): #RGB Color
+        if text:
+            return f"\033[38;2;{color}m"
+        else:
+            return f"\033[48;2;{color}m"
+    
+    elif rgb := _check_HEX(color): #HEX Color
         if text:
-            return f"\033[38;5;{palette[2]}m"
+            return f"\033[38;2;{rgb}m"
         else:
-            return f"\033[48;5;{palette[2]}m"
+            return f"\033[48;2;{rgb}m"
+    
     else:
         if text:
-            return f"\033[38;2;{palette[4]}m"
+            return "\033[37m"
         else:
-            return f"\033[48;2;{palette[4]}m"
-
-
-# Get and return details about a given color
-def _get_color(color, all_colors = _import_colors()):
+            return "\033[0m"
 
-    unknown = False
 
-    # Check if the input is a valid ANSI color code.
+# Check if the input is a valid ANSI color code.
+def _check_ansi(color):
+    
     if matches := re.search("^([0-9]{1,3})$", str(color)):
+        if int(color) in [0, 30, 31, 32, 33, 34, 35, 36, 37, 40, 41, 42, 43, 44, 45, 46, 47, 90, 91, 92, 93, 94, 95, 96, 97, 100, 101, 102, 103, 104, 105, 106, 107]:
+            return True
+        else:
+            return None
+    else:
+        return False
+            
 
-        try:
-            color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.fg == str(color)))
-        except:
-            try:
-                color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.bg == str(color)))
-            except:
-                return _invalid_range()
-             
-    # Check if the color name is in the list of colors
-    elif color.title() in all_colors.keys():
-        color_name = color.title()
-
-    # Check if the Xterm Number is valid
-    elif matches := re.search("^[xX]([0-9]{1,3})$", color):
+# Check if the Xterm Number is valid
+def _check_Xterm(color):
+        
+    if matches := re.search("^[xX]([0-9]{1,3})$", color):
         color = int(matches.group(1))
         if 0 <= color < 256:
-            color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.xterm == str(color)))
+            return True
         else:
-            return _invalid_range()
+            return None
+    else:
+        return False
+    
 
+def _check_RGB(color):
     # Check if the RGB color code is valid and in the list of colors
-    elif matches := re.search("^([0-9]*;[0-9]*;[0-9]*)$", color):
+    if re.search("^([0-9]*;[0-9]*;[0-9]*)$", color):
 
         r,g,b = color.split(";")
 
         if (0<=int(r)<=255) and (0<=int(g)<=255) and (0<=int(b)<=255):
+            return True
+        else:
+            return None
+    else:
+        return False   
 
-            try:
-                #color_name = list(all_colors.keys())[list(map(lambda x: x['rgb'], all_colors.values())).index(matches.group(1))]
-                color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.rgb == matches.group(1)))#, None)
-            except:
-                return _no_name(matches.group(1))
-            
-        # Return an error message for an invalid color code
+
+def _check_HEX(color):
+    # Check if the HEX color code is valid and in the list of colors
+    if re.search("^(#[0-9A-Za-z]{6})$", color):
+        if matches := re.search("^#([0-9A-Fa-f]{2})([0-9A-Fa-f]{2})([0-9A-Fa-f]{2})$", color):
+            #Return hex values coverted to dec for r, g, b
+            #group(1): hex value for "r"; group(2): hex value for "g"; group(3): hex value for "b";
+            return f"{int(matches.group(1), 16)};{int(matches.group(2), 16)};{int(matches.group(3), 16)}"
         else:
-            return _invalid_range()
-                
+            return None
+    else:
+        return False
+
+
+# Get and return details about a given color
+def _get_color(color, all_colors = _import_colors()):
+
+    unknown = False
+
+    # If the input is a valid ANSI color code find name.
+    if _check_ansi(color):
+        try:
+            color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.fg == str(color)))
+        except:
+            color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.bg == str(color)))
+    # Return error message if ANSI value is out of range
+    elif _check_ansi(color) == None:
+        return _invalid_range()
+
+    # Check if the Xterm Number is valid
+    elif _check_Xterm(color):
+        color = color[1:]
+        color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.xterm == str(color)))
+    # Return error message if Xterm value is out of range
+    elif _check_Xterm(color) == None:
+        return _invalid_range()
+
+    # Check if the RGB color code is valid and in the list of colors
+    elif _check_RGB(color):
+        try:
+            #color_name = list(all_colors.keys())[list(map(lambda x: x['rgb'], all_colors.values())).index(matches.group(1))]
+            color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.rgb == color))#, None)
+        except:
+            # Return an error message for an invalid color code
+            return _no_name(color)
+    elif _check_RGB(color) == None:
+        return _invalid_range()
+
     # Check if the HEX color code is valid and in the list of colors
-    elif matches := re.search("^(#[0-9A-Za-z]{6})$", color):
-        color = matches.group(1).upper()
+    elif _check_HEX(color):
+        color = color.upper()
         try:
             #color_name = list(all_colors.keys())[list(map(lambda x: x['hex'], all_colors.values(color))).index()]
             color_name = next((col_name for col_name, color_obj in all_colors.items() if color_obj.hex == color))#, None)
         except:
-            if matches := re.search("^(#[0-9A-F]{6})$", color):
-                return _no_name(matches.group(1))
-            
-            # Return an error message for an invalid color range
-            else:
-                return _invalid_range()
+            return _no_name(color)
+    elif _check_HEX(color) == None:
+        return _invalid_range()
+
+    # Check if the color name is in the list of colors
+    elif color.title() in all_colors.keys():
+        color_name = color.title()
 
     # Return an error message for an unknown color name
     else:
         name = f"Color '{color.title()}' Unknown"
         alt_name = ""
         color_x = "???"
         color_hex = "#??????"
```

### Comparing `polychromy-1.0.2/polychromy.egg-info/PKG-INFO` & `polychromy-1.1.0/polychromy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: polychromy
-Version: 1.0.2
+Version: 1.1.0
 Summary: A module to print a strings in a given colour, with a given colour background
 Author-email: scalvaruso <calvaruso.simone@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://pypi.org/project/polychromy
 Project-URL: Repository, https://github.com/scalvaruso/polychromy
-Keywords: ansi,background,color,colour,format,foreground,Hex,RGB,sRGB,text
+Keywords: ansi,background,color,colour,colorate,font,format,foreground,Hex,paint,RGB,sRGB,text
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: textlinebreaker>=0.1.0
+Requires-Dist: requests
 
 # Polychromy
 
 [<img src="https://img.shields.io/badge/polychromy-py-blue?style=flat&logo=python&logoWidth=20.svg/"></a>](https://github.com/scalvaruso/polychromy/)
 [![PyPI - Version](https://img.shields.io/pypi/v/polychromy?logo=pypi&logoColor=white&color=blue)](https://pypi.org/project/polychromy/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polychromy?logo=python)](https://pypi.org/project/polychromy/)
 [![Downloads](https://static.pepy.tech/badge/polychromy)](https://pepy.tech/project/polychromy)
@@ -36,15 +37,15 @@
 Polychromy is a Python script to manipulate the colors of a text.
 
 ## Features
 
 - Function ```colorate``` prints text of a specified colour in a specified colour background.
 - Function ```show``` prints out color details such as Hex and RGB values of a given colour in a square of the given colour.
 
-## Latest Version 1.0.2
+## Latest Version 1.1.0
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -53,15 +54,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Getting Started
 
 ### Prerequisites
 
-This script relies on the Python standard library and ```textlinebreaker```.
+This script relies on the Python standard library, and the libraries ```requests``` and ```textlinebreaker```.
 
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install polychromy
```

### Comparing `polychromy-1.0.2/pyproject.toml` & `polychromy-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "polychromy"
-version = "1.0.2"
-dependencies = ["textlinebreaker >= 0.1.0 "]
+version = "1.1.0"
+dependencies = ["textlinebreaker >= 0.1.0 ","requests"]
 requires-python = ">=3.9"
 authors = [
     { name="scalvaruso", email="calvaruso.simone@gmail.com" },
 ]
 description = "A module to print a strings in a given colour, with a given colour background"
 readme = "README.md"
 license = {text = "MIT License"}
-keywords = ["ansi", "background", "color", "colour", "format", "foreground", "Hex", "RGB", "sRGB", "text"]
+keywords = ["ansi", "background", "color", "colour", "colorate", "font", "format", "foreground", "Hex", "paint", "RGB", "sRGB", "text"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `polychromy-1.0.2/setup.py` & `polychromy-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="polychromy",
-    version="1.0.2",
+    version="1.1.0",
     packages=find_namespace_packages(include=['polychromy', 'polychromy.*'], exclude=['images']),
     # Use find_packages and exclude the folder
     include_package_data=True,
-    install_requires=["textlinebreaker >= 0.1.0 "],  # Add any dependencies here
+    install_requires=["textlinebreaker >= 0.1.0 ", "requests"],  # Add any dependencies here
     
     # other setup configurations...
 
     # Explicitly include 'polychromy.data' package
     package_data={
         "polychromy": ["data/colors.json"],
         "polychromy.data": [],  # Add specific data files if necessary
```

