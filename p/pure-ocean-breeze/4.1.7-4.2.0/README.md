# Comparing `tmp/pure_ocean_breeze-4.1.7.tar.gz` & `tmp/pure_ocean_breeze-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.1.7.tar", last modified: Fri Mar 29 05:46:15 2024, max compression
+gzip compressed data, was "pure_ocean_breeze-4.2.0.tar", last modified: Tue Apr  9 04:24:24 2024, max compression
```

## Comparing `pure_ocean_breeze-4.1.7.tar` & `pure_ocean_breeze-4.2.0.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.323238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.323238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31927 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    66752 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.323238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.323238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.323238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    36390 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    98155 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   273197 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.327238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   192825 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.331238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    85655 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.331238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   314704 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.331238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.331238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    43178 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.331238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   138094 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.335238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29805 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    29153 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   193541 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.339238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-03-29 05:46:15.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-03-29 05:46:15.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 05:46:15.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-29 05:46:15.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-29 05:46:15.000000 pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 05:46:15.343238 pure_ocean_breeze-4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-29 05:46:11.000000 pure_ocean_breeze-4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.305228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31927 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66752 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36390 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.309228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98533 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   273197 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192825 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85655 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   314704 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.313228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43178 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138094 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.317228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29805 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29153 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193541 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.321228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 04:24:24.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-09 04:24:24.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:24:24.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 04:24:24.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 04:24:24.000000 pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:24:24.325228 pure_ocean_breeze-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-09 04:24:20.000000 pure_ocean_breeze-4.2.0/setup.py
```

### Comparing `pure_ocean_breeze-4.1.7/LICENSE` & `pure_ocean_breeze-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/PKG-INFO` & `pure_ocean_breeze-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.1.7
+Version: 4.2.0
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
@@ -29,15 +29,15 @@
 Requires-Dist: texttable
 Requires-Dist: numpy_ext
 Requires-Dist: xpinyin
 Requires-Dist: cufflinks
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: tradetime
 Requires-Dist: deprecation
-Requires-Dist: questdb
+Requires-Dist: questdb==1.1.0
 Requires-Dist: mpire
 Requires-Dist: py7zr
 Requires-Dist: unrar
 Requires-Dist: rarfile
 Requires-Dist: chardet
 Requires-Dist: psycopg2-binary
 Provides-Extra: windows
```

### Comparing `pure_ocean_breeze-4.1.7/README.md` & `pure_ocean_breeze-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
 __updated__ = "2023-07-18 14:49:23"
-__version__ = "4.1.7"
+__version__ = "4.2.0"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/__init__.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,17 +121,19 @@
 
 from pure_ocean_breeze.jason.state.homeplace import *
 from pure_ocean_breeze.jason.state.decorators import *
 
 from pure_ocean_breeze.jason.data.dicts import *
 from pure_ocean_breeze.jason.data.read_data import *
 from pure_ocean_breeze.jason.data.tools import *
+from pure_ocean_breeze.jason.data.database import *
 
 from pure_ocean_breeze.jason.labor.process import *
 from pure_ocean_breeze.jason.labor.comment import *
 
-
+import sys
+sys.path.append('/home/chenzongwei/pythoncode')
```

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/dicts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/read_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/data/tools.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/comment.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/labor/process.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/labor/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import numpy as np
 import pandas as pd
 import os
 import tqdm.auto
 import scipy.stats as ss
 from scipy.optimize import linprog
 import statsmodels.formula.api as smf
-import matplotlib as mpl
+# import matplotlib as mpl
 
-mpl.rcParams.update(mpl.rcParamsDefault)
+# mpl.rcParams.update(mpl.rcParamsDefault)
 import matplotlib.pyplot as plt
 
 plt.rcParams["axes.unicode_minus"] = False
 
 from functools import reduce, lru_cache, partial
 from dateutil.relativedelta import relativedelta
 from loguru import logger
@@ -950,22 +950,23 @@
         industry_codes = list(df.columns)
         industry_codes = [i for i in industry_codes if i.startswith("w")]
         industry_codes_str = "+".join(industry_codes)
         if len(industry_codes_str) > 0:
             ols_result = smf.ols("fac~cap_size+" + industry_codes_str, data=df).fit()
         else:
             ols_result = smf.ols("fac~cap_size", data=df).fit()
-        ols_w = ols_result.params["cap_size"]
-        ols_b = ols_result.params["Intercept"]
-        ols_bs = {}
-        for ind in industry_codes:
-            ols_bs[ind] = ols_result.params[ind]
-        df.fac = df.fac - ols_w * df.cap_size - ols_b
-        for k, v in ols_bs.items():
-            df.fac = df.fac - v * df[k]
+        # ols_w = ols_result.params["cap_size"]
+        # ols_b = ols_result.params["Intercept"]
+        # ols_bs = {}
+        # for ind in industry_codes:
+        #     ols_bs[ind] = ols_result.params[ind]
+        # df.fac = df.fac - ols_w * df.cap_size - ols_b
+        # for k, v in ols_bs.items():
+        #     df.fac = df.fac - v * df[k]
+        df.fac=ols_result.resid
         df = df[["fac"]]
         return df
 
     @classmethod
     @lru_cache(maxsize=None)
     def get_log_cap(cls):
         """获得对数市值"""
@@ -982,15 +983,15 @@
         )
         if not only_cap:
             self.factors = pd.merge(
                 self.factors, self.swindustry_dummy, on=["date", "code"]
             )
 
         self.factors = self.factors.set_index(["date", "code"])
-        self.factors = self.factors.groupby(["date"]).apply(self.neutralize_factors)
+        self.factors = self.factors.groupby(["date"],as_index=False).apply(self.neutralize_factors)
         self.factors = self.factors.reset_index()
         self.factors = self.factors.pivot(index="date", columns="code", values="fac")
 
     def get_ic_rankic(cls, df):
         """计算IC和RankIC"""
         df1 = df[["ret", "fac"]]
         ic = df1.corr(method="pearson").iloc[0, 1]
@@ -2353,19 +2354,22 @@
         df = df.rename(columns={"snow_fac": "fac"})
         return df
 
     def get_snow_fac(self):
         """获得纯净因子"""
         self.snow_fac = (
             self.corr_pri.set_index(["date", "code"])
-            .groupby(["date"])
+            .groupby(["date"],as_index=False)
             .apply(self.ols_in_group)
         )
-        self.snow_fac = self.snow_fac.unstack()
-        self.snow_fac.columns = list(map(lambda x: x[1], list(self.snow_fac.columns)))
+        if 'date' in self.snow_fac.columns:
+            self.snow_fac=self.snow_fac.rename(columns={'date':'old_date'})
+        # self.snow_fac = self.snow_fac.unstack()
+        # self.snow_fac.columns = list(map(lambda x: x[1], list(self.snow_fac.columns)))
+        self.snow_fac=self.snow_fac.reset_index().pivot(index='date',columns='code',values='fac')
 
 
 @do_on_dfs
 class pure_snowtrain(object):
     """直接返回纯净因子"""
 
     def __init__(
@@ -2645,13 +2649,14 @@
     for i in tqdm.auto.tqdm(ddss):
         ds.append(pd.concat(i))
     return ds
 
 
 @do_on_dfs
 def sun(factor:pd.DataFrame,rolling_5:int=1):
+    '''先单因子测试，再测试其与常用风格之间的关系'''
     if rolling_5:
         factor=boom_one(factor)
     shen=pure_moonnight(factor)
     pfi=pure_snowtrain(factor)
     shen=pure_moonnight(pfi,neutralize=1)
     display(pfi.show_corr())
```

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/decorators.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/homeplace.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/state/states.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/jason/withs/requires.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/jason/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.1.7
+Version: 4.2.0
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
@@ -29,15 +29,15 @@
 Requires-Dist: texttable
 Requires-Dist: numpy_ext
 Requires-Dist: xpinyin
 Requires-Dist: cufflinks
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: tradetime
 Requires-Dist: deprecation
-Requires-Dist: questdb
+Requires-Dist: questdb==1.1.0
 Requires-Dist: mpire
 Requires-Dist: py7zr
 Requires-Dist: unrar
 Requires-Dist: rarfile
 Requires-Dist: chardet
 Requires-Dist: psycopg2-binary
 Provides-Extra: windows
```

### Comparing `pure_ocean_breeze-4.1.7/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.2.0/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pure_ocean_breeze/future_version/__init__.py
 pure_ocean_breeze/future_version/half_way.py
 pure_ocean_breeze/future_version/in_thoughts.py
 pure_ocean_breeze/initialize/__init__.py
 pure_ocean_breeze/initialize/initialize.py
 pure_ocean_breeze/jason/__init__.py
 pure_ocean_breeze/jason/data/__init__.py
+pure_ocean_breeze/jason/data/database.py
 pure_ocean_breeze/jason/data/dicts.py
 pure_ocean_breeze/jason/data/read_data.py
 pure_ocean_breeze/jason/data/tools.py
 pure_ocean_breeze/jason/labor/__init__.py
 pure_ocean_breeze/jason/labor/comment.py
 pure_ocean_breeze/jason/labor/process.py
 pure_ocean_breeze/jason/state/__init__.py
```

### Comparing `pure_ocean_breeze-4.1.7/setup.py` & `pure_ocean_breeze-4.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "texttable",
     "numpy_ext",
     "xpinyin",
     "cufflinks",
     "clickhouse_sqlalchemy",
     "tradetime",
     "deprecation",
-    "questdb",
+    "questdb==1.1.0",
     "mpire",
     "py7zr",
     "unrar",
     "rarfile",
     # "zipfile",
     "chardet",
 ]
```

