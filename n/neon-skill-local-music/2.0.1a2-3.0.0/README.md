# Comparing `tmp/neon-skill-local_music-2.0.1a2.tar.gz` & `tmp/neon-skill-local_music-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-local_music-2.0.1a2.tar", last modified: Wed Apr  3 00:02:13 2024, max compression
+gzip compressed data, was "neon-skill-local_music-3.0.0.tar", last modified: Tue Apr  9 23:12:37 2024, max compression
```

## Comparing `neon-skill-local_music-2.0.1a2.tar` & `neon-skill-local_music-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/locale/en-us/vocab/local.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 00:02:13.000000 neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:02:13.960772 neon-skill-local_music-2.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 00:02:09.000000 neon-skill-local_music-2.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/ui/music-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:13.956771 neon-skill-local_music-2.0.1a2/util/
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 00:02:10.000000 neon-skill-local_music-2.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.227141 neon-skill-local_music-3.0.0/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.227141 neon-skill-local_music-3.0.0/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/locale/en-us/vocab/local.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/ui/music-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/version.py
```

### Comparing `neon-skill-local_music-2.0.1a2/LICENSE.md` & `neon-skill-local_music-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/PKG-INFO` & `neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-local_music
-Version: 2.0.1a2
+Name: neon-skill-local-music
+Version: 3.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-2.0.1a2/README.md` & `neon-skill-local_music-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/__init__.py` & `neon-skill-local_music-3.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/neon_skill_local_music.egg-info/PKG-INFO` & `neon-skill-local_music-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-local-music
-Version: 2.0.1a2
+Name: neon-skill-local_music
+Version: 3.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-2.0.1a2/setup.py` & `neon-skill-local_music-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/skill.json` & `neon-skill-local_music-3.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/test/test_skill.py` & `neon-skill-local_music-3.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/util/__init__.py` & `neon-skill-local_music-3.0.0/util/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-2.0.1a2/version.py` & `neon-skill-local_music-3.0.0/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a2"
+__version__ = "3.0.0"
```

