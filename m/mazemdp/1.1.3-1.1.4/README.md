# Comparing `tmp/mazemdp-1.1.3.tar.gz` & `tmp/mazemdp-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazemdp-1.1.3.tar", last modified: Thu Feb 29 09:47:52 2024, max compression
+gzip compressed data, was "mazemdp-1.1.4.tar", last modified: Wed Apr 10 17:23:53 2024, max compression
```

## Comparing `mazemdp-1.1.3.tar` & `mazemdp-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.816881 mazemdp-1.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-02-29 09:47:42.000000 mazemdp-1.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.812881 mazemdp-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.816881 mazemdp-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-29 09:47:42.000000 mazemdp-1.1.3/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1866 2024-02-29 09:47:42.000000 mazemdp-1.1.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-02-29 09:47:42.000000 mazemdp-1.1.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-02-29 09:47:42.000000 mazemdp-1.1.3/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)     1366 2024-02-29 09:47:42.000000 mazemdp-1.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-02-29 09:47:52.816881 mazemdp-1.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4212 2024-02-29 09:47:42.000000 mazemdp-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-29 09:47:42.000000 mazemdp-1.1.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-02-29 09:47:42.000000 mazemdp-1.1.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      677 2024-02-29 09:47:52.816881 mazemdp-1.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-02-29 09:47:42.000000 mazemdp-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.812881 mazemdp-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.816881 mazemdp-1.1.3/src/mazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9408 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16737 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6129 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-02-29 09:47:42.000000 mazemdp-1.1.3/src/mazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.816881 mazemdp-1.1.3/src/mazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 09:47:52.000000 mazemdp-1.1.3/src/mazemdp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:52.816881 mazemdp-1.1.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:47:42.000000 mazemdp-1.1.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-02-29 09:47:42.000000 mazemdp-1.1.3/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.414032 mazemdp-1.1.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-04-10 17:23:48.000000 mazemdp-1.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.410032 mazemdp-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.410032 mazemdp-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 17:23:48.000000 mazemdp-1.1.4/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1866 2024-04-10 17:23:48.000000 mazemdp-1.1.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-04-10 17:23:48.000000 mazemdp-1.1.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-04-10 17:23:48.000000 mazemdp-1.1.4/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1366 2024-04-10 17:23:48.000000 mazemdp-1.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-10 17:23:53.414032 mazemdp-1.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4212 2024-04-10 17:23:48.000000 mazemdp-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 17:23:48.000000 mazemdp-1.1.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-10 17:23:48.000000 mazemdp-1.1.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      677 2024-04-10 17:23:53.414032 mazemdp-1.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-10 17:23:48.000000 mazemdp-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.410032 mazemdp-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.410032 mazemdp-1.1.4/src/mazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9374 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16737 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6129 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3332 2024-04-10 17:23:48.000000 mazemdp-1.1.4/src/mazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.414032 mazemdp-1.1.4/src/mazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 17:23:53.000000 mazemdp-1.1.4/src/mazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:53.414032 mazemdp-1.1.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:48.000000 mazemdp-1.1.4/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-04-10 17:23:48.000000 mazemdp-1.1.4/tests/test_mdp.py
```

### Comparing `mazemdp-1.1.3/.github/workflows/python-publish.yml` & `mazemdp-1.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/.gitignore` & `mazemdp-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/LICENSE` & `mazemdp-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/Makefile` & `mazemdp-1.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/PKG-INFO` & `mazemdp-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 1.1.3
+Version: 1.1.4
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>
 Project-URL: homepage, https://github.com/osigaud/SimpleMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
```

### Comparing `mazemdp-1.1.3/README.md` & `mazemdp-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/pyproject.toml` & `mazemdp-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/setup.cfg` & `mazemdp-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/src/mazemdp/chrono.py` & `mazemdp-1.1.4/src/mazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/src/mazemdp/maze.py` & `mazemdp-1.1.4/src/mazemdp/maze.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,23 +95,21 @@
         self.init_states(width, height, walls)
 
         # ##################### Action Space ######################
         self.nb_actions = nb_actions
 
         # ##################### Distribution Over Initial States ######################
 
-        start_distribution = np.zeros(
-            self.nb_states
-        )  # distribution over initial states
+        start_distribution = np.zeros(self.nb_states)
 
         if start_states is None:
-            for state in start_distribution:
+            for state in range(len(start_distribution)):
                 start_distribution[state] = 1.0 / len(start_distribution)
         else:
-            for state in start_states:
+            for state in range(len(start_states)):
                 start_distribution[state] = 1.0 / len(start_states)
 
         # ##################### Transition Matrix ######################
         transition_matrix = self.init_transitions(hit)
 
         if hit:
             reward_matrix = self.reward_hit_walls(transition_matrix)
```

### Comparing `mazemdp-1.1.3/src/mazemdp/maze_plotter.py` & `mazemdp-1.1.4/src/mazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/src/mazemdp/mdp.py` & `mazemdp-1.1.4/src/mazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/src/mazemdp/simple_action_space.py` & `mazemdp-1.1.4/src/mazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/src/mazemdp/toolbox.py` & `mazemdp-1.1.4/src/mazemdp/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
     # - Q : a Q-function represented as a nX times nU matrix
     # - x : the state for which we want the soft-max distribution
     # - temperature : temperature parameter of the soft-max distribution
     # Note that temperature can be set to 0 because numpy can deal with the division by 0
     # Output :
     # - p : probability of each action according to the soft-max distribution
 
-    p = np.zeros((len(q[x])))
+    nb_options = len(q[x])
+    p = np.zeros(nb_options)
     sump = 0
-    for i in range(len(p)):
+    for i in range(nb_options):
         p[i] = np.exp((q[x, i] / temperature).round(5))
         sump += p[i]
 
     p = p / sump
     return p
```

### Comparing `mazemdp-1.1.3/src/mazemdp.egg-info/PKG-INFO` & `mazemdp-1.1.4/src/mazemdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazemdp
-Version: 1.1.3
+Version: 1.1.4
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>
 Project-URL: homepage, https://github.com/osigaud/SimpleMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
```

### Comparing `mazemdp-1.1.3/src/mazemdp.egg-info/SOURCES.txt` & `mazemdp-1.1.4/src/mazemdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mazemdp-1.1.3/tests/test_mdp.py` & `mazemdp-1.1.4/tests/test_mdp.py`

 * *Files identical despite different names*

