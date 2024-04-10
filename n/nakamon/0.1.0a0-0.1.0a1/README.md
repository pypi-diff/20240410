# Comparing `tmp/nakamon-0.1.0a0.tar.gz` & `tmp/nakamon-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakamon-0.1.0a0.tar", max compression
+gzip compressed data, was "nakamon-0.1.0a1.tar", max compression
```

## Comparing `nakamon-0.1.0a0.tar` & `nakamon-0.1.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a0/LICENSE
--rw-r--r--   0        0        0       89 2024-04-09 04:57:56.950211 nakamon-0.1.0a0/README.md
--rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a0/nakamon/__init__.py
--rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a0/nakamon/damage.py
--rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a0/nakamon/nakamon.py
--rw-r--r--   0        0        0      335 2024-04-10 04:06:04.440971 nakamon-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 nakamon-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a1/README.md
+-rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a1/nakamon/__init__.py
+-rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a1/nakamon/damage.py
+-rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a1/nakamon/nakamon.py
+-rw-r--r--   0        0        0      379 2024-04-10 04:56:03.077632 nakamon-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 nakamon-0.1.0a1/PKG-INFO
```

### Comparing `nakamon-0.1.0a0/LICENSE` & `nakamon-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a0/nakamon/damage.py` & `nakamon-0.1.0a1/nakamon/damage.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a0/nakamon/nakamon.py` & `nakamon-0.1.0a1/nakamon/nakamon.py`

 * *Files identical despite different names*

