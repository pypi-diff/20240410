# Comparing `tmp/zeroset-0.0.1.tar.gz` & `tmp/zeroset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroset-0.0.1.tar", last modified: Wed Jun 21 20:17:56 2023, max compression
+gzip compressed data, was "zeroset-0.0.2.tar", last modified: Wed Apr 10 08:46:43 2024, max compression
```

## Comparing `zeroset-0.0.1.tar` & `zeroset-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:17:56.640928 zeroset-0.0.1/
--rw-rw-rw-   0        0        0      456 2023-06-21 20:17:56.639937 zeroset-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-21 18:10:26.000000 zeroset-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 20:17:56.640928 zeroset-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-21 19:38:15.000000 zeroset-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:17:56.628049 zeroset-0.0.1/zeroset/
--rw-rw-rw-   0        0        0      373 2023-06-21 20:15:40.000000 zeroset-0.0.1/zeroset/__init__.py
--rw-rw-rw-   0        0        0     7289 2023-06-21 20:13:52.000000 zeroset-0.0.1/zeroset/cv0.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:17:56.639937 zeroset-0.0.1/zeroset.egg-info/
--rw-rw-rw-   0        0        0      456 2023-06-21 20:17:56.000000 zeroset-0.0.1/zeroset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-21 20:17:56.000000 zeroset-0.0.1/zeroset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:17:56.000000 zeroset-0.0.1/zeroset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-21 20:17:56.000000 zeroset-0.0.1/zeroset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:17:56.000000 zeroset-0.0.1/zeroset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.747323 zeroset-0.0.2/
+-rw-rw-rw-   0        0        0      821 2024-04-10 08:46:43.747323 zeroset-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-12-14 09:12:56.000000 zeroset-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 08:46:43.747323 zeroset-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-04-10 08:06:37.000000 zeroset-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.708570 zeroset-0.0.2/test/
+-rw-rw-rw-   0        0        0      170 2024-04-10 07:45:29.000000 zeroset-0.0.2/test/test_cv0.py
+-rw-rw-rw-   0        0        0      231 2023-07-23 05:21:32.000000 zeroset-0.0.2/test/test_glob.py
+-rw-rw-rw-   0        0        0     1070 2023-12-17 10:16:05.000000 zeroset-0.0.2/test/test_script.py
+-rw-rw-rw-   0        0        0     3666 2023-12-14 11:18:25.000000 zeroset-0.0.2/test/test_tabulate.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.732263 zeroset-0.0.2/zeroset/
+-rw-rw-rw-   0        0        0      373 2024-04-03 06:30:00.000000 zeroset-0.0.2/zeroset/__init__.py
+-rw-rw-rw-   0        0        0     8067 2024-04-10 07:48:24.000000 zeroset-0.0.2/zeroset/cv0.py
+-rw-rw-rw-   0        0        0      844 2023-08-31 14:08:59.000000 zeroset-0.0.2/zeroset/fmt0.py
+-rw-rw-rw-   0        0        0     5888 2024-04-10 08:02:20.000000 zeroset-0.0.2/zeroset/l0.py
+-rw-rw-rw-   0        0        0     2160 2023-12-14 11:32:37.000000 zeroset-0.0.2/zeroset/py0.py
+-rw-rw-rw-   0        0        0     3760 2024-02-15 14:22:09.000000 zeroset-0.0.2/zeroset/s0.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.746216 zeroset-0.0.2/zeroset.egg-info/
+-rw-rw-rw-   0        0        0      821 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/top_level.txt
```

### Comparing `zeroset-0.0.1/setup.py` & `zeroset-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="zeroset",
-    version="0.0.1",
-    author="Bomm Kim",
-    author_email="springnode@gmail.com",
-    description="Useful collection of features.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/springkim/zeroset",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'natsort>=8.0.0',
-        'Pillow>=8.0.0',
-        'opencv-python>=3.2.0',
-        'screeninfo>=0.8.0',
-    ],
-)
+        name="zeroset",
+        version="0.0.2",
+        author="Bomm Kim",
+        author_email="springnode@gmail.com",
+        description="Useful collection of features.",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        url="https://github.com/springkim/zeroset",
+        packages=setuptools.find_packages(),
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+        ],
+        python_requires='>=3.6',
+        install_requires=[
+            'natsort>=8.0.0',
+            'Pillow>=8.0.0',
+            'opencv-python>=3.2.0',
+            'screeninfo>=0.8.0',
+            'tabulate>=0.9.0',
+            'pytz',
+            'selenium>=4.0.0',
+            'webdriver-manager>=4.0.0',
+            'screeninfo',
+        ],
+)
```

### Comparing `zeroset-0.0.1/zeroset/cv0.py` & `zeroset-0.0.2/zeroset/cv0.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     r, eimg = cv2.imencode(os.path.splitext(filename)[1], img, params)
     if r:
         with open(filename, mode="wb") as f:
             eimg.tofile(f)
     return r
 
 
+def imreads(filepaths: str, flags=cv2.IMREAD_COLOR):
+    return [imread(filepath, flags) for filepath in filepaths]
+
+
 def waitKey(delay=0):
     return cv2.waitKey(delay)
 
 
 def waitESC(delay=1):
     return cv2.waitKey(delay) == 27
 
@@ -111,14 +115,15 @@
         else:
             _, _, cw, ch = cv2.getWindowImageRect(winname)
             window_ratio = cv2.getWindowProperty(winname, cv2.WND_PROP_ASPECT_RATIO)
             image_ratio = img.shape[1] / img.shape[0]
             if abs(image_ratio - window_ratio) > 0.1:
                 nw, nh = resize(img, width=cw, return_size=True)
                 cv2.resizeWindow(winname, nw, nh)
+
     elif mode == IMSHOW_AUTOSIZE:
         cv2.namedWindow(winname, cv2.WINDOW_AUTOSIZE)
     elif mode == IMSHOW_FULLSCREEN:
         cv2.namedWindow(winname, cv2.WINDOW_NORMAL)
         cv2.setWindowProperty(winname, cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN)
         _, _, cw, ch = cv2.getWindowImageRect(winname)
         img = resize(img, width=cw, height=ch, return_size=False)
@@ -210,7 +215,33 @@
         value = tuple([value] * channel)
     N = max(img.shape[:2])
     dst = np.zeros((N, N, img.shape[2]), dtype=np.uint8) + np.array(value, dtype=np.uint8)
     dx = (N - img.shape[1]) // 2
     dy = (N - img.shape[0]) // 2
     dst[dy:dy + img.shape[0], dx:dx + img.shape[1]] = img
     return dst
+
+
+def _to_image_list(args):
+    imgs = []
+    for arg in args:
+        if isinstance(arg, list):
+            imgs += arg
+        elif isinstance(arg, np.ndarray):
+            imgs.append(arg)
+        else:
+            pass
+    return imgs
+
+
+def hconcat(*args):
+    imgs = _to_image_list(args)
+    max_height = max(img.shape[0] for img in imgs)
+    rimgs = [resize(img, height=max_height) for img in imgs]
+    return cv2.hconcat(rimgs)
+
+
+def vconcat(*args):
+    imgs = _to_image_list(args)
+    max_width = max(img.shape[1] for img in imgs)
+    rimgs = [resize(img, width=max_width) for img in imgs]
+    return cv2.vconcat(rimgs)
```

