# Comparing `tmp/ivycheck-0.9.3.tar.gz` & `tmp/ivycheck-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivycheck-0.9.3.tar", last modified: Tue Apr  9 00:43:44 2024, max compression
+gzip compressed data, was "ivycheck-0.9.4.tar", last modified: Thu Mar 21 13:36:57 2024, max compression
```

## Comparing `ivycheck-0.9.3.tar` & `ivycheck-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 00:43:33.000000 ivycheck-0.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-09 00:43:44.134417 ivycheck-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-09 00:43:33.000000 ivycheck-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:43:44.134417 ivycheck-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 00:43:33.000000 ivycheck-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.130417 ivycheck-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/src/ivycheck/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/src/ivycheck/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/src/ivycheck/models/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/checkresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/entitymatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/hallucinationop.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/httpvalidationerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/piiop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/prompt_injectionop.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/models/validationerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/src/ivycheck/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32082 2024-04-09 00:43:33.000000 ivycheck-0.9.3/src/ivycheck/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:43:44.134417 ivycheck-0.9.3/src/ivycheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-09 00:43:43.000000 ivycheck-0.9.3/src/ivycheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 00:43:44.000000 ivycheck-0.9.3/src/ivycheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:43:43.000000 ivycheck-0.9.3/src/ivycheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 00:43:43.000000 ivycheck-0.9.3/src/ivycheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 00:43:43.000000 ivycheck-0.9.3/src/ivycheck.egg-info/top_level.txt
+drwxr-xr-x   0 tammo      (501) staff       (20)        0 2024-03-21 13:36:57.924314 ivycheck-0.9.4/
+-rw-r--r--   0 tammo      (501) staff       (20)     2751 2024-03-21 13:36:57.923972 ivycheck-0.9.4/PKG-INFO
+-rw-r--r--   0 tammo      (501) staff       (20)     2480 2024-03-21 13:25:38.000000 ivycheck-0.9.4/README.md
+-rw-r--r--   0 tammo      (501) staff       (20)       38 2024-03-21 13:36:57.924375 ivycheck-0.9.4/setup.cfg
+-rw-r--r--   0 tammo      (501) staff       (20)      657 2024-03-21 13:36:52.000000 ivycheck-0.9.4/setup.py
+drwxr-xr-x   0 tammo      (501) staff       (20)        0 2024-03-21 13:36:57.922003 ivycheck-0.9.4/src/
+drwxr-xr-x   0 tammo      (501) staff       (20)        0 2024-03-21 13:36:57.922672 ivycheck-0.9.4/src/ivycheck/
+-rw-r--r--   0 tammo      (501) staff       (20)       29 2024-03-21 13:33:04.000000 ivycheck-0.9.4/src/ivycheck/__init__.py
+-rw-r--r--   0 tammo      (501) staff       (20)     3804 2024-03-21 13:07:59.000000 ivycheck-0.9.4/src/ivycheck/client.py
+drwxr-xr-x   0 tammo      (501) staff       (20)        0 2024-03-21 13:36:57.923572 ivycheck-0.9.4/src/ivycheck.egg-info/
+-rw-r--r--   0 tammo      (501) staff       (20)     2751 2024-03-21 13:36:57.000000 ivycheck-0.9.4/src/ivycheck.egg-info/PKG-INFO
+-rw-r--r--   0 tammo      (501) staff       (20)      245 2024-03-21 13:36:57.000000 ivycheck-0.9.4/src/ivycheck.egg-info/SOURCES.txt
+-rw-r--r--   0 tammo      (501) staff       (20)        1 2024-03-21 13:36:57.000000 ivycheck-0.9.4/src/ivycheck.egg-info/dependency_links.txt
+-rw-r--r--   0 tammo      (501) staff       (20)       22 2024-03-21 13:36:57.000000 ivycheck-0.9.4/src/ivycheck.egg-info/requires.txt
+-rw-r--r--   0 tammo      (501) staff       (20)        9 2024-03-21 13:36:57.000000 ivycheck-0.9.4/src/ivycheck.egg-info/top_level.txt
```

