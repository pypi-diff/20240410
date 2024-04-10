# Comparing `tmp/xrframes-0.0.1.tar.gz` & `tmp/xrframes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrframes-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xrframes-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xrframes-0.0.1.tar` & `xrframes-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2024-04-08 15:12:20.359310 xrframes-0.0.1/LICENSE
--rw-r--r--   0        0        0     2490 2024-04-09 21:55:29.028989 xrframes-0.0.1/README.md
--rw-r--r--   0        0        0      774 2024-04-09 21:13:14.906424 xrframes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      200 2024-04-09 21:57:18.171845 xrframes-0.0.1/xrframes/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-09 21:09:20.586622 xrframes-0.0.1/xrframes/_rich_dask.py
--rw-r--r--   0        0        0     1364 2024-04-09 21:09:21.332911 xrframes-0.0.1/xrframes/_rich_joblib.py
--rw-r--r--   0        0        0    11299 2024-04-09 21:04:41.280076 xrframes-0.0.1/xrframes/core.py
--rw-r--r--   0        0        0        0 2024-04-09 04:38:57.565418 xrframes-0.0.1/xrframes/py.typed
--rw-r--r--   0        0        0      280 2024-04-09 20:32:09.325438 xrframes-0.0.1/xrframes/util.py
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 xrframes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-08 15:12:20.359310 xrframes-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2490 2024-04-09 21:55:29.028989 xrframes-0.0.2/README.md
+-rw-r--r--   0        0        0      774 2024-04-09 21:13:14.906424 xrframes-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-10 18:00:30.234646 xrframes-0.0.2/xrframes/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-09 21:09:20.586622 xrframes-0.0.2/xrframes/_rich_dask.py
+-rw-r--r--   0        0        0     1364 2024-04-09 21:09:21.332911 xrframes-0.0.2/xrframes/_rich_joblib.py
+-rw-r--r--   0        0        0    11622 2024-04-10 17:56:16.076107 xrframes-0.0.2/xrframes/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:38:57.565418 xrframes-0.0.2/xrframes/py.typed
+-rw-r--r--   0        0        0      280 2024-04-09 20:32:09.325438 xrframes-0.0.2/xrframes/util.py
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 xrframes-0.0.2/PKG-INFO
```

### Comparing `xrframes-0.0.1/LICENSE` & `xrframes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.1/README.md` & `xrframes-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.1/pyproject.toml` & `xrframes-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.1/xrframes/_rich_dask.py` & `xrframes-0.0.2/xrframes/_rich_dask.py`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.1/xrframes/_rich_joblib.py` & `xrframes-0.0.2/xrframes/_rich_joblib.py`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.1/xrframes/core.py` & `xrframes-0.0.2/xrframes/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,37 +215,42 @@
 
     def to_mp4(
         self,
         out: str | Path = "./movie.mp4",
         *,
         fps: int = 10,
         crf: int = 17,
+        exe: str | Path = "ffmpeg",
     ) -> None:
         """Make an MP4 movie from the PNG frames with FFmpeg.
 
         Parameters
         ----------
         fps
             Frame rate (per second).
         crf
             Constant rate factor (0--51, lower is better quality, 23 is FFmpeg's default).
             https://trac.ffmpeg.org/wiki/Encode/H.264#a1.ChooseaCRFvalue
+        exe
+            Path to ``ffmpeg``.
         """
         import subprocess
 
         from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
         if self._frame_pattern is None:
             raise RuntimeError("call `write_frames` first")
 
         out = Path(out).expanduser()
 
+        exe = Path(exe)
+
         # fmt: off
         cmd = [
-            "ffmpeg",
+            exe.as_posix(),
             "-y",
             "-r", str(fps),
             "-i", self._frame_pattern,
             "-vf", "pad=ceil(iw/2)*2:ceil(ih/2)*2",
             "-c:v", "libx264",
             "-pix_fmt", "yuv420p",
             "-preset", "veryslow",
@@ -277,14 +282,15 @@
     def to_gif(
         self,
         out: str | Path = "./movie.gif",
         *,
         fps: int = 10,
         scale: str = "100%",
         magick: bool = True,
+        exe: str | Path = "convert",
     ) -> None:
         """Make a GIF from the PNG frames with ImageMagick.
 
         Parameters
         ----------
         fps
             Frame rate (per second).
@@ -292,41 +298,46 @@
             Scaling applied when generating the output.
             For example
             ``'480x380'`` (maximum width and height in pixels, preserves original aspect ratio)
             or ``'50%'``.
         magick
             Use ``magick`` base command (new CLI for ImageMagick 7),
             i.e. ``magick convert`` instead of just ``convert``.
+            Ignored if a custom `exe` is provived.
+        exe
+            Path to ``convert`` or ``magick``.
         """
         import subprocess
 
         from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
         out = Path(out).expanduser()
 
+        exe = Path(exe)
+
         if not self.paths:
             raise RuntimeError("call `write_frames` first")
 
         files = [f.as_posix() for f in self.paths]
 
         # fmt: off
         cmd = [
-            "convert",
+            exe.as_posix(),
             "-scale", scale,
             # "-unsharp", "0x6+0.5+0",
             "-dispose", "previous",
             "-delay", str(round(100 / fps)),
             "-loop", "0",
             "-layers", "optimizeframe",
             *files,
             out.as_posix(),
         ]
         # fmt: on
 
-        if magick:
+        if magick and cmd[0] == "convert":
             cmd.insert(0, "magick")
 
         try:
             with Progress(
                 SpinnerColumn(finished_text="✔"),
                 r" [progress.description]{task.description}",
                 TimeElapsedColumn(),
```

### Comparing `xrframes-0.0.1/PKG-INFO` & `xrframes-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrframes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Similar to ``xmovie``, make animations from xarray objects.
 Author-email: zmoon <zmoon92@gmail.com>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: rich
 Project-URL: Home, https://github.com/zmoon/xrframes
```

