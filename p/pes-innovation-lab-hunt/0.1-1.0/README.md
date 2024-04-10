# Comparing `tmp/pes-innovation-lab-hunt-0.1.tar.gz` & `tmp/pes-innovation-lab-hunt-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pes-innovation-lab-hunt-0.1.tar", last modified: Wed Apr 10 20:24:38 2024, max compression
+gzip compressed data, was "pes-innovation-lab-hunt-1.0.tar", last modified: Wed Apr 10 20:24:54 2024, max compression
```

## Comparing `pes-innovation-lab-hunt-0.1.tar` & `pes-innovation-lab-hunt-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:38.810561 pes-innovation-lab-hunt-0.1/
--rw-r--r--   0 monish    (1000) monish    (1000)      150 2024-04-10 20:24:38.810561 pes-innovation-lab-hunt-0.1/PKG-INFO
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:38.809560 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt/
--rw-r--r--   0 monish    (1000) monish    (1000)      120 2024-04-09 14:34:01.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt/__init__.py
--rw-r--r--   0 monish    (1000) monish    (1000)     5234 2024-04-10 20:07:39.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt/hunt.py
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:38.810561 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt.egg-info/
--rw-r--r--   0 monish    (1000) monish    (1000)      150 2024-04-10 20:24:38.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt.egg-info/PKG-INFO
--rw-r--r--   0 monish    (1000) monish    (1000)      264 2024-04-10 20:24:38.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt.egg-info/SOURCES.txt
--rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-10 20:24:38.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt.egg-info/dependency_links.txt
--rw-r--r--   0 monish    (1000) monish    (1000)       24 2024-04-10 20:24:38.000000 pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt.egg-info/top_level.txt
--rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-10 20:24:38.810561 pes-innovation-lab-hunt-0.1/setup.cfg
--rw-r--r--   0 monish    (1000) monish    (1000)      339 2024-04-10 20:24:33.000000 pes-innovation-lab-hunt-0.1/setup.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:54.761109 pes-innovation-lab-hunt-1.0/
+-rw-r--r--   0 monish    (1000) monish    (1000)      150 2024-04-10 20:24:54.761109 pes-innovation-lab-hunt-1.0/PKG-INFO
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:54.760109 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt/
+-rw-r--r--   0 monish    (1000) monish    (1000)      120 2024-04-09 14:34:01.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt/__init__.py
+-rw-r--r--   0 monish    (1000) monish    (1000)     5234 2024-04-10 20:07:39.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt/hunt.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-10 20:24:54.760109 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt.egg-info/
+-rw-r--r--   0 monish    (1000) monish    (1000)      150 2024-04-10 20:24:54.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt.egg-info/PKG-INFO
+-rw-r--r--   0 monish    (1000) monish    (1000)      264 2024-04-10 20:24:54.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt.egg-info/SOURCES.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-10 20:24:54.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt.egg-info/dependency_links.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)       24 2024-04-10 20:24:54.000000 pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt.egg-info/top_level.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-10 20:24:54.761109 pes-innovation-lab-hunt-1.0/setup.cfg
+-rw-r--r--   0 monish    (1000) monish    (1000)      339 2024-04-10 20:24:51.000000 pes-innovation-lab-hunt-1.0/setup.py
```

### Comparing `pes-innovation-lab-hunt-0.1/pes_innovation_lab_hunt/hunt.py` & `pes-innovation-lab-hunt-1.0/pes_innovation_lab_hunt/hunt.py`

 * *Files identical despite different names*

