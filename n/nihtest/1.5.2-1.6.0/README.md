# Comparing `tmp/nihtest-1.5.2.tar.gz` & `tmp/nihtest-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nihtest-1.5.2.tar", last modified: Wed Mar 20 09:17:43 2024, max compression
+gzip compressed data, was "nihtest-1.6.0.tar", last modified: Wed Apr 10 09:27:50 2024, max compression
```

## Comparing `nihtest-1.5.2.tar` & `nihtest-1.6.0.tar`

### file list

```diff
@@ -1,157 +1,160 @@
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-03-20 09:17:43.540363 nihtest-1.5.2/
--rw-r--r--   0 dillo      (501) staff       (20)      993 2024-03-20 09:15:51.000000 nihtest-1.5.2/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.5.2/LICENSE
--rw-r--r--   0 dillo      (501) staff       (20)      168 2023-06-27 09:50:58.000000 nihtest-1.5.2/MANIFEST.in
--rw-r--r--   0 dillo      (501) staff       (20)      787 2024-03-20 09:17:36.000000 nihtest-1.5.2/NEWS.md
--rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-03-20 09:17:43.540291 nihtest-1.5.2/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)      969 2023-07-01 07:17:52.000000 nihtest-1.5.2/README.md
--rw-r--r--   0 dillo      (501) staff       (20)      145 2024-01-03 16:10:59.000000 nihtest-1.5.2/TODO.md
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-03-20 09:17:43.522293 nihtest-1.5.2/manpages/
--rw-r--r--   0 dillo      (501) staff       (20)      576 2023-06-09 14:53:27.000000 nihtest-1.5.2/manpages/Makefile
--rw-r--r--   0 dillo      (501) staff       (20)    11161 2024-01-17 10:41:49.000000 nihtest-1.5.2/manpages/nihtest-case.html
--rw-r--r--   0 dillo      (501) staff       (20)     6559 2024-01-17 10:41:49.000000 nihtest-1.5.2/manpages/nihtest-case.man
--rw-r--r--   0 dillo      (501) staff       (20)     6427 2024-03-15 10:00:51.000000 nihtest-1.5.2/manpages/nihtest-case.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)    13046 2024-01-17 10:41:49.000000 nihtest-1.5.2/manpages/nihtest.conf.html
--rw-r--r--   0 dillo      (501) staff       (20)     7613 2024-01-17 10:41:49.000000 nihtest-1.5.2/manpages/nihtest.conf.man
--rw-r--r--   0 dillo      (501) staff       (20)     7262 2024-01-03 16:08:10.000000 nihtest-1.5.2/manpages/nihtest.conf.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)     7738 2024-01-17 10:41:15.000000 nihtest-1.5.2/manpages/nihtest.html
--rw-r--r--   0 dillo      (501) staff       (20)     4599 2024-01-17 10:41:15.000000 nihtest-1.5.2/manpages/nihtest.man
--rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.5.2/manpages/nihtest.mdoc
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-03-20 09:17:43.524072 nihtest-1.5.2/nihtest/
--rw-r--r--   0 dillo      (501) staff       (20)     1361 2023-11-20 16:45:16.000000 nihtest-1.5.2/nihtest/Command.py
--rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.5.2/nihtest/CompareArrays.py
--rw-r--r--   0 dillo      (501) staff       (20)     5831 2024-01-03 10:20:32.000000 nihtest-1.5.2/nihtest/Configuration.py
--rw-r--r--   0 dillo      (501) staff       (20)     1059 2023-06-28 11:07:23.000000 nihtest-1.5.2/nihtest/Environment.py
--rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.5.2/nihtest/Features.py
--rw-r--r--   0 dillo      (501) staff       (20)     5360 2024-03-20 09:08:41.000000 nihtest-1.5.2/nihtest/File.py
--rw-r--r--   0 dillo      (501) staff       (20)     1291 2023-12-27 15:18:23.000000 nihtest-1.5.2/nihtest/Sandbox.py
--rw-r--r--   0 dillo      (501) staff       (20)     6544 2024-01-04 15:06:40.000000 nihtest-1.5.2/nihtest/Test.py
--rw-r--r--   0 dillo      (501) staff       (20)    11150 2024-01-03 14:32:25.000000 nihtest-1.5.2/nihtest/TestCase.py
--rw-r--r--   0 dillo      (501) staff       (20)      677 2023-06-27 09:50:58.000000 nihtest-1.5.2/nihtest/Utility.py
--rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.5.2/nihtest/__init__.py
--rw-r--r--   0 dillo      (501) staff       (20)     1361 2024-03-20 09:15:51.000000 nihtest-1.5.2/nihtest/__main__.py
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-03-20 09:17:43.540063 nihtest-1.5.2/nihtest.egg-info/
--rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)     3686 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/SOURCES.txt
--rw-r--r--   0 dillo      (501) staff       (20)        1 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/dependency_links.txt
--rw-r--r--   0 dillo      (501) staff       (20)       50 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/entry_points.txt
--rw-r--r--   0 dillo      (501) staff       (20)       16 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/requires.txt
--rw-r--r--   0 dillo      (501) staff       (20)        8 2024-03-20 09:17:43.000000 nihtest-1.5.2/nihtest.egg-info/top_level.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1018 2024-03-20 09:15:51.000000 nihtest-1.5.2/pyproject.toml
--rw-r--r--   0 dillo      (501) staff       (20)       76 2024-03-20 09:17:43.540583 nihtest-1.5.2/setup.cfg
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-03-20 09:17:43.539864 nihtest-1.5.2/tests/
--rw-r--r--   0 dillo      (501) staff       (20)     2216 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/argument-escaped.input
--rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/argument-escaped.test
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/binary-1
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/binary-2
--rw-r--r--   0 dillo      (501) staff       (20)     1808 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/can-preload.c
--rw-r--r--   0 dillo      (501) staff       (20)     2539 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/cat.c
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.5.2/tests/comparator-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.5.2/tests/comparator-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.5.2/tests/comparator-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.5.2/tests/comparator-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-06-27 10:06:35.000000 nihtest-1.5.2/tests/comparator-preprocess.input
--rw-r--r--   0 dillo      (501) staff       (20)      290 2023-06-28 10:48:16.000000 nihtest-1.5.2/tests/comparator-preprocess.test
--rw-r--r--   0 dillo      (501) staff       (20)     1590 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/comparator.c
--rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/compare-binary-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      249 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/compare-binary-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/compare-binary-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/compare-binary-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/config.h
--rw-r--r--   0 dillo      (501) staff       (20)      104 2024-01-03 10:11:30.000000 nihtest-1.5.2/tests/copier.input
--rw-r--r--   0 dillo      (501) staff       (20)      160 2024-01-03 10:12:56.000000 nihtest-1.5.2/tests/copier.test
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/default-stderr-replace.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.5.2/tests/default-stderr-replace.test
--rw-r--r--   0 dillo      (501) staff       (20)     1755 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/delete.c
--rw-r--r--   0 dillo      (501) staff       (20)     1651 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/delete.h
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/description-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/diff-1.input
--rw-r--r--   0 dillo      (501) staff       (20)      218 2023-04-17 17:35:49.000000 nihtest-1.5.2/tests/diff-1.test
--rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/diff-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      188 2023-04-17 17:36:44.000000 nihtest-1.5.2/tests/diff-2.test
--rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/echo.c
--rw-r--r--   0 dillo      (501) staff       (20)       82 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/empty-lines.txt
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-clear-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-clear-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-28 11:05:36.000000 nihtest-1.5.2/tests/environment-not-passed-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-not-passed-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-28 11:07:43.000000 nihtest-1.5.2/tests/environment-passthrough-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-passthrough-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-set-config-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-set-config-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-set-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-set-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-unset-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/environment-unset-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/failure.txt
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/false-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      201 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/false-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/false-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/false-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/false.c
--rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/features-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      236 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/features-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/features-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/features-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/features-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/features-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/file-del-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      246 2023-04-12 10:14:06.000000 nihtest-1.5.2/tests/file-del-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      131 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/file-del-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/file-del-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/file-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      254 2023-04-15 15:28:11.000000 nihtest-1.5.2/tests/file-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.5.2/tests/file-inline-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      320 2023-04-15 15:28:58.000000 nihtest-1.5.2/tests/file-inline-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      280 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/file-inline-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/file-inline-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/file-new-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      217 2023-04-12 10:14:06.000000 nihtest-1.5.2/tests/file-new-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.5.2/tests/file-new-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/file-new-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.5.2/tests/file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.5.2/tests/file-subdirectory-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/file-subdirectory-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     3310 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/file.c
--rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/getenv.c
--rw-r--r--   0 dillo      (501) staff       (20)     1756 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/ineffective-delete.c
--rw-r--r--   0 dillo      (501) staff       (20)      508 2024-01-03 10:08:16.000000 nihtest-1.5.2/tests/nihtest-conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      236 2023-06-27 09:50:58.000000 nihtest-1.5.2/tests/nihtest.conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 13:24:22.000000 nihtest-1.5.2/tests/parameter-tests-1.input
--rw-r--r--   0 dillo      (501) staff       (20)     1696 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/parameter-tests-1.test
--rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/parameter-tests-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      389 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/parameter-tests-2.test
--rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/precheck-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      213 2023-04-12 12:29:19.000000 nihtest-1.5.2/tests/precheck-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/precheck-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/precheck-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/precheck-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.5.2/tests/precheck-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      174 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/preload-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.5.2/tests/preload-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.5.2/tests/preload-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stderr-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      265 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stderr-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stderr-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stderr-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.5.2/tests/stderr-replace-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stderr-replace-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stdin-file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stdin-file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stdin-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stdin-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stdout-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      253 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stdout-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/stdout-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/stdout-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/success.txt
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/true-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      197 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/true-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.5.2/tests/true-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.5.2/tests/true-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1785 2023-06-28 09:11:26.000000 nihtest-1.5.2/tests/true.c
--rw-r--r--   0 dillo      (501) staff       (20)     2546 2024-03-15 10:00:51.000000 nihtest-1.5.2/tests/uppercase.c
--rw-r--r--   0 dillo      (501) staff       (20)      251 2023-12-27 15:28:23.000000 nihtest-1.5.2/tests/working-directory.input
--rw-r--r--   0 dillo      (501) staff       (20)      115 2023-12-27 15:21:44.000000 nihtest-1.5.2/tests/working-directory.test
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.195079 nihtest-1.6.0/
+-rw-r--r--   0 dillo      (501) staff       (20)      993 2024-04-10 09:25:50.000000 nihtest-1.6.0/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.6.0/LICENSE
+-rw-r--r--   0 dillo      (501) staff       (20)      168 2023-06-27 09:50:58.000000 nihtest-1.6.0/MANIFEST.in
+-rw-r--r--   0 dillo      (501) staff       (20)      927 2024-04-10 09:25:07.000000 nihtest-1.6.0/NEWS.md
+-rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-10 09:27:50.195007 nihtest-1.6.0/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)      969 2023-07-01 07:17:52.000000 nihtest-1.6.0/README.md
+-rw-r--r--   0 dillo      (501) staff       (20)      145 2024-01-03 16:10:59.000000 nihtest-1.6.0/TODO.md
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.172517 nihtest-1.6.0/manpages/
+-rw-r--r--   0 dillo      (501) staff       (20)      576 2023-06-09 14:53:27.000000 nihtest-1.6.0/manpages/Makefile
+-rw-r--r--   0 dillo      (501) staff       (20)    11543 2024-04-10 09:27:24.000000 nihtest-1.6.0/manpages/nihtest-case.html
+-rw-r--r--   0 dillo      (501) staff       (20)     6783 2024-04-10 09:27:24.000000 nihtest-1.6.0/manpages/nihtest-case.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6638 2024-04-10 09:25:07.000000 nihtest-1.6.0/manpages/nihtest-case.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)    13046 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.conf.html
+-rw-r--r--   0 dillo      (501) staff       (20)     7613 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.conf.man
+-rw-r--r--   0 dillo      (501) staff       (20)     7262 2024-01-03 16:08:10.000000 nihtest-1.6.0/manpages/nihtest.conf.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)     7738 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.html
+-rw-r--r--   0 dillo      (501) staff       (20)     4599 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.man
+-rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.6.0/manpages/nihtest.mdoc
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.174515 nihtest-1.6.0/nihtest/
+-rw-r--r--   0 dillo      (501) staff       (20)     1361 2023-11-20 16:45:16.000000 nihtest-1.6.0/nihtest/Command.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.6.0/nihtest/CompareArrays.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5831 2024-01-03 10:20:32.000000 nihtest-1.6.0/nihtest/Configuration.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1059 2023-06-28 11:07:23.000000 nihtest-1.6.0/nihtest/Environment.py
+-rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.6.0/nihtest/Features.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5236 2024-04-10 09:02:06.000000 nihtest-1.6.0/nihtest/File.py
+-rw-r--r--   0 dillo      (501) staff       (20)      359 2024-03-27 16:58:56.000000 nihtest-1.6.0/nihtest/Output.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1291 2023-12-27 15:18:23.000000 nihtest-1.6.0/nihtest/Sandbox.py
+-rw-r--r--   0 dillo      (501) staff       (20)     6922 2024-04-10 09:17:51.000000 nihtest-1.6.0/nihtest/Test.py
+-rw-r--r--   0 dillo      (501) staff       (20)    11504 2024-04-10 09:17:27.000000 nihtest-1.6.0/nihtest/TestCase.py
+-rw-r--r--   0 dillo      (501) staff       (20)      690 2024-04-10 09:02:06.000000 nihtest-1.6.0/nihtest/Utility.py
+-rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.6.0/nihtest/__init__.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1361 2024-04-10 09:25:50.000000 nihtest-1.6.0/nihtest/__main__.py
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.194741 nihtest-1.6.0/nihtest.egg-info/
+-rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)     3767 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/SOURCES.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        1 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/dependency_links.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       50 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/entry_points.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       16 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/requires.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        8 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/top_level.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1018 2024-04-10 09:25:50.000000 nihtest-1.6.0/pyproject.toml
+-rw-r--r--   0 dillo      (501) staff       (20)       76 2024-04-10 09:27:50.195308 nihtest-1.6.0/setup.cfg
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.194534 nihtest-1.6.0/tests/
+-rw-r--r--   0 dillo      (501) staff       (20)     2216 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/argument-escaped.input
+-rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/argument-escaped.test
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/binary-1
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/binary-2
+-rw-r--r--   0 dillo      (501) staff       (20)     1808 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/can-preload.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2539 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/cat.c
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.6.0/tests/comparator-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.6.0/tests/comparator-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.6.0/tests/comparator-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.6.0/tests/comparator-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-06-27 10:06:35.000000 nihtest-1.6.0/tests/comparator-preprocess.input
+-rw-r--r--   0 dillo      (501) staff       (20)      290 2023-06-28 10:48:16.000000 nihtest-1.6.0/tests/comparator-preprocess.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1590 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/comparator.c
+-rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      279 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/compare-binary-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/config.h
+-rw-r--r--   0 dillo      (501) staff       (20)      104 2024-01-03 10:11:30.000000 nihtest-1.6.0/tests/copier.input
+-rw-r--r--   0 dillo      (501) staff       (20)      160 2024-01-03 10:12:56.000000 nihtest-1.6.0/tests/copier.test
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/default-stderr-replace.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/default-stderr-replace.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1755 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/delete.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1651 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/delete.h
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/description-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/diff-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)      250 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/diff-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/diff-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      220 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/diff-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/echo.c
+-rw-r--r--   0 dillo      (501) staff       (20)       82 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/empty-lines.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-clear-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-clear-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-28 11:05:36.000000 nihtest-1.6.0/tests/environment-not-passed-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-not-passed-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-28 11:07:43.000000 nihtest-1.6.0/tests/environment-passthrough-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-passthrough-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-config-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-config-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-unset-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-unset-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/failure.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      237 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/false-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/false-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false.c
+-rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      275 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/features-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/features-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/features-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-del-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      285 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-del-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      131 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/file-del-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-del-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      289 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.6.0/tests/file-inline-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      362 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-inline-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      280 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/file-inline-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/file-inline-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-new-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      256 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-new-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.6.0/tests/file-new-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-new-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.6.0/tests/file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.6.0/tests/file-subdirectory-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-subdirectory-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     3310 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/file.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/getenv.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1756 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/ineffective-delete.c
+-rw-r--r--   0 dillo      (501) staff       (20)      508 2024-01-03 10:08:16.000000 nihtest-1.6.0/tests/nihtest-conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      236 2023-06-27 09:50:58.000000 nihtest-1.6.0/tests/nihtest.conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/parameter-tests-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)     1696 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/parameter-tests-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/parameter-tests-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      389 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/parameter-tests-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      252 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/precheck-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/precheck-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.6.0/tests/precheck-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      174 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/preload-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.6.0/tests/preload-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.6.0/tests/preload-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stderr-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      302 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/stderr-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stderr-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stderr-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.6.0/tests/stderr-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stderr-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdin-file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdin-file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdin-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdin-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdout-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      290 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/stdout-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdout-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdout-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      208 2024-04-10 09:19:57.000000 nihtest-1.6.0/tests/stdout-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2024-04-10 09:19:57.000000 nihtest-1.6.0/tests/stdout-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/success.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/true-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      232 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/true-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/true-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/true-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1785 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/true.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2546 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/uppercase.c
+-rw-r--r--   0 dillo      (501) staff       (20)      251 2023-12-27 15:28:23.000000 nihtest-1.6.0/tests/working-directory.input
+-rw-r--r--   0 dillo      (501) staff       (20)      115 2023-12-27 15:21:44.000000 nihtest-1.6.0/tests/working-directory.test
```

### Comparing `nihtest-1.5.2/CMakeLists.txt` & `nihtest-1.6.0/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.12)
 
 # Also update version in nihtest/__main__.py and pyproject.toml
 project(nihtest
-        VERSION 1.5.2
+        VERSION 1.6.0
         DESCRIPTION "NiH testing framework"
         HOMEPAGE_URL "https://github.com/nih-at/nihtest"
         LANGUAGES C)
 
 enable_testing()
 
 find_package(Python3 REQUIRED COMPONENTS Interpreter)
```

### Comparing `nihtest-1.5.2/LICENSE` & `nihtest-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/NEWS.md` & `nihtest-1.6.0/NEWS.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# 1.6.0 [2024-04-10]
+
+- Print command line for `--verbose --setup-only`.
+- Add `stdout-replace` directive.
+- Better integration with IDEs.
+
 # 1.5.2 [2024-03-20]
 
 - Fix @SANDBOX@ substitution in file names on Windows.
 
 # 1.5.1 [2024-03-15]
 
 - Fix preload test with newer glibc.
```

### Comparing `nihtest-1.5.2/PKG-INFO` & `nihtest-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.5.2
+Version: 1.6.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.5.2/README.md` & `nihtest-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/Makefile` & `nihtest-1.6.0/manpages/Makefile`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest-case.html` & `nihtest-1.6.0/manpages/nihtest-case.html`

 * *Files 5% similar despite different names*

```diff
@@ -107,17 +107,15 @@
         &#x201C;end-of-inline-data&#x201D;. If both <var class="Ar">in</var> and
         <var class="Ar">out</var> are &#x201C;&lt;inline&gt;&#x201D;, the input
         data comes first. Otherwise the argument specifies the name of the file
         to copy or compare againts.</p>
   </dd>
   <dt><a class="permalink" href="#mkdir"><code class="Ic" id="mkdir">mkdir</code></a>
     <var class="Ar">name</var></dt>
-  <dd>Create directory <var class="Ar">name</var>
-    <br/>
-     in the test directory.</dd>
+  <dd>Create directory <var class="Ar">name</var> in the test directory.</dd>
   <dt><a class="permalink" href="#precheck"><code class="Ic" id="precheck">precheck</code></a>
     <var class="Ar">command</var> [<var class="Ar">argument ...</var>]</dt>
   <dd>If <var class="Ar">command</var> exits with non-zero status, skip the
       test.</dd>
   <dt><a class="permalink" href="#preload"><code class="Ic" id="preload">preload</code></a>
     <var class="Ar">object</var></dt>
   <dd>Pre-load the shared object <var class="Ar">object</var> before running the
@@ -172,14 +170,20 @@
   </dd>
   <dt><a class="permalink" href="#stdout"><code class="Ic" id="stdout">stdout</code></a>
     [<var class="Ar">file</var>]</dt>
   <dd>Specify the expect standard output (stdout). If <var class="Ar">file</var>
       is given, the output is compared with that file, otherwise the expected
       text is taken from the following lines of the test case, up to a line
       consisting of &#x201C;end-of-inline-data&#x201D;.</dd>
+  <dt><a class="permalink" href="#stdout-replace"><code class="Ic" id="stdout-replace">stdout-replace</code></a>
+    <var class="Ar">pattern replacement</var></dt>
+  <dd>Run regular expression replacement over the standard output and the
+      expected output as provided by <code class="Ic">stdout</code> before
+      comparing them. See <code class="Ic">stderr-replace</code> for
+    details.</dd>
   <dt><a class="permalink" href="#working-directory"><code class="Ic" id="working-directory">working-directory</code></a>
     <var class="Ar">directory</var></dt>
   <dd>Run the program in the subdirectory <var class="Ar">directory</var> inside
       the sandbox. The directory will be created if it doesn't exist.</dd>
 </dl>
 </section>
 <section class="Sh">
@@ -187,13 +191,13 @@
   ALSO</a></h1>
 <a class="Xr" href="nihtest.html">nihtest(1)</a>,
   <a class="Xr" href="nihtest-config.html">nihtest-config(5)</a>
 </section>
 </div>
 <table class="foot">
   <tr>
-    <td class="foot-date">November 20, 2023</td>
+    <td class="foot-date">April 10, 2024</td>
     <td class="foot-os">NiH</td>
   </tr>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -36,16 +36,15 @@
       “{}” specifies that the file does not exist (i. e. that it is created or
       deleted by the program).
       For “<inline>” the contents of the file are taken from the test case, up
       to a line consisting of “end-of-inline-data”. If both in and out are
       “<inline>”, the input data comes first. Otherwise the argument specifies
       the name of the file to copy or compare againts.
   _m_k_d_i_r name
-      Create directory name
-      in the test directory.
+      Create directory name in the test directory.
   _p_r_e_c_h_e_c_k command [argument ...]
       If command exits with non-zero status, skip the test.
   _p_r_e_l_o_a_d object
       Pre-load the shared object object before running the program.
       This is not supported on macOS and Windows, where tests with preload will
       be skipped.
   _p_r_o_g_r_a_m name
@@ -77,13 +76,17 @@
       Otherwise the text provided to the program via a pipe is taken from the
       test case, up to a line consisting of “end-of-inline-data”.
   _s_t_d_o_u_t [file]
       Specify the expect standard output (stdout). If file is given, the output
       is compared with that file, otherwise the expected text is taken from the
       following lines of the test case, up to a line consisting of “end-of-
       inline-data”.
+  _s_t_d_o_u_t_-_r_e_p_l_a_c_e pattern replacement
+      Run regular expression replacement over the standard output and the
+      expected output as provided by stdout before comparing them. See stderr-
+      replace for details.
   _w_o_r_k_i_n_g_-_d_i_r_e_c_t_o_r_y directory
       Run the program in the subdirectory directory inside the sandbox. The
       directory will be created if it doesn't exist.
 ************ _SS_EE_EE_ _AA_LL_SS_OO ************
 _n_i_h_t_e_s_t_(_1_), _n_i_h_t_e_s_t_-_c_o_n_f_i_g_(_5_)
-November 20, 2023 NiH
+April 10, 2024 NiH
```

### Comparing `nihtest-1.5.2/manpages/nihtest-case.man` & `nihtest-1.6.0/manpages/nihtest-case.man`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.TH "NIHTEST-CASE" "5" "November 20, 2023" "NiH" "File Formats Manual"
+.TH "NIHTEST-CASE" "5" "April 10, 2024" "NiH" "File Formats Manual"
 .nh
 .if n .ad l
 .SH "NAME"
 \fBnihtest-case\fR
 \- test case format for nihtest
 .SH "DESCRIPTION"
 nihtest(1)
@@ -124,15 +124,15 @@
 \(lq<inline>\(rq,
 the input data comes first.
 Otherwise the argument specifies the name of the file to copy or compare againts.
 .TP 22n
 \fBmkdir\fR \fIname\fR
 Create directory
 \fIname\fR
- in the test directory.
+in the test directory.
 .TP 22n
 \fBprecheck\fR \fIcommand\fR [\fIargument ...\fR]
 If
 \fIcommand\fR
 exits with non-zero status, skip the test.
 .TP 22n
 \fBpreload\fR \fIobject\fR
@@ -213,14 +213,23 @@
 Specify the expect standard output (stdout).
 If
 \fIfile\fR
 is given, the output is compared with that file,
 otherwise the expected text is taken from the following lines of the test case, up to a line consisting of
 \(lqend-of-inline-data\(rq.
 .TP 22n
+\fBstdout-replace\fR \fIpattern replacement\fR
+Run regular expression replacement over the standard output
+and the expected output as provided by
+\fBstdout\fR
+before comparing them.
+See
+\fBstderr-replace\fR
+for details.
+.TP 22n
 \fBworking-directory\fR \fIdirectory\fR
 Run the program in the subdirectory
 \fIdirectory\fR
 inside the sandbox.
 The directory will be created if it doesn't exist.
 .SH "SEE ALSO"
 nihtest(1),
```

### Comparing `nihtest-1.5.2/manpages/nihtest-case.mdoc` & `nihtest-1.6.0/manpages/nihtest-case.mdoc`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.Dd November 20, 2023
+.Dd April 10, 2024
 .Dt NIHTEST-CASE 5
 .Os
 .Sh NAME
 .Nm nihtest-case
 .Nd test case format for nihtest
 .Sh DESCRIPTION
 .Xr nihtest 1
@@ -193,14 +193,22 @@
 .It Ic stdout Op Ar file
 Specify the expect standard output (stdout).
 If
 .Ar file
 is given, the output is compared with that file,
 otherwise the expected text is taken from the following lines of the test case, up to a line consisting of
 .Dq end-of-inline-data .
+.It Ic stdout-replace Ar pattern replacement
+Run regular expression replacement over the standard output
+and the expected output as provided by
+.Ic stdout
+before comparing them.
+See
+.Ic stderr-replace
+for details.
 .\" .It Ic ulimit Ar C VALUE
 .\" Set
 .\" .Xr ulimit 1
 .\" flag
 .\" .Fl Ar C
 .\" to
 .\" .Ar VALUE
```

### Comparing `nihtest-1.5.2/manpages/nihtest.conf.html` & `nihtest-1.6.0/manpages/nihtest.conf.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest.conf.man` & `nihtest-1.6.0/manpages/nihtest.conf.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest.conf.mdoc` & `nihtest-1.6.0/manpages/nihtest.conf.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest.html` & `nihtest-1.6.0/manpages/nihtest.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest.man` & `nihtest-1.6.0/manpages/nihtest.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/manpages/nihtest.mdoc` & `nihtest-1.6.0/manpages/nihtest.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/Command.py` & `nihtest-1.6.0/nihtest/Command.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/CompareArrays.py` & `nihtest-1.6.0/nihtest/CompareArrays.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/Configuration.py` & `nihtest-1.6.0/nihtest/Configuration.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/Environment.py` & `nihtest-1.6.0/nihtest/Environment.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/Features.py` & `nihtest-1.6.0/nihtest/Features.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/File.py` & `nihtest-1.6.0/nihtest/File.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.name = name
         self.input = input
         self.result = result
 
     def file_name(self, directory):
         return self.name.replace("@SANDBOX@", os.path.abspath(directory))
 
-    def compare(self, configuration, directory):
+    def compare(self, output, configuration, directory):
         if not self.result:
             return True
 
         input_file_name = os.path.join(directory, self.file_name(directory))
         output_is_binary = False
 
         file_extension = pathlib.Path(self.name).suffix[1:]
@@ -58,40 +58,39 @@
                 command = Command.Command(configuration.find_program(comparator[0]), arguments, stdin=self.result.data, environment=Environment.Environment(configuration).environment)
                 command.run()
                 if command.exit_code != 0:
                     if command.stderr:
                         print(f"comparing {self.name} failed:")
                         print("\n".join(command.stderr))
                     else:
-                        print(f"{self.name} differs:")
-                        print("\n".join(command.stdout))
+                        output.print(f"{self.name} differs:")
+                        output.print("\n".join(command.stdout))
                 return command.exit_code == 0
             output_data = self.result.data
 
         if key in configuration.comparator_preprocessors:
             preprocessor = configuration.comparator_preprocessors[key]
             arguments = preprocessor[1:] + [input_file_name]
             # TODO: allow binary data
             command = Command.Command(configuration.find_program(preprocessor[0]), arguments, environment=Environment.Environment(configuration).environment)
             command.run()
-            return Utility.compare_lines(self.name, output_data, command.stdout, configuration.verbose != Configuration.When.NEVER)
+            return Utility.compare_lines(output, self.name, output_data, command.stdout)
 
         if not output_is_binary:
             try:
                 input_data = Utility.read_lines(input_file_name)
-                return Utility.compare_lines(self.name, output_data, input_data, configuration.verbose != Configuration.When.NEVER)
+                return Utility.compare_lines(output, self.name, output_data, input_data)
             except UnicodeDecodeError:
                 output_data = "\n".join(output_data)
 
         with open(input_file_name, "rb") as file:
             input_data = file.read()
         if input_data != output_data:
-            if configuration.verbose != Configuration.When.NEVER:
-                print(f"{self.name} differs:")
-                print("Binary files differ.")
+            output.print(f"{self.name} differs:")
+            output.print("Binary files differ.")
             return False
         return True
 
     def prepare(self, configuration, directory):
         if self.input:
             output_file_name = os.path.join(directory, self.file_name(directory))
             os.makedirs(os.path.dirname(output_file_name), 0o777, True)
```

### Comparing `nihtest-1.5.2/nihtest/Sandbox.py` & `nihtest-1.6.0/nihtest/Sandbox.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/nihtest/Test.py` & `nihtest-1.6.0/nihtest/Test.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import stat
 import sys
 
 from nihtest import Command
 from nihtest import Configuration
 from nihtest import Environment
 from nihtest import Features
+from nihtest import Output
 from nihtest import TestCase
 from nihtest import Sandbox
 from nihtest import Utility
 
 
-def process_stderr_line(line, replacements):
+def process_output_line(line, replacements):
     for replacement in replacements:
         line = re.sub(replacement[0], replacement[1], line)
     return line
 
 
 class TestResult(enum.Enum):
     OK = 0
@@ -67,14 +68,16 @@
             except Exception as e:
                 self.error(f"can't set modification time for '{file}': {e}")
 
         if not self.ok:
             return TestResult.ERROR
 
         if not self.case.configuration.run_test:
+            if self.case.configuration.verbose == Configuration.When.ALWAYS:
+                print(self.case.program + " " + " ".join(self.case.arguments))
             return TestResult.OK
 
         for file in self.case.read_only:
             full_file = os.path.join(self.sandbox.directory, file)
             st = os.stat(full_file)
             os.chmod(full_file, st.st_mode & ~(stat.S_IWUSR))
 
@@ -95,28 +98,30 @@
 
         for file in self.case.read_only:
             full_file = os.path.join(self.sandbox.directory, file)
             if os.path.exists(full_file):
                 st = os.stat(full_file)
                 os.chmod(full_file, st.st_mode | stat.S_IWRITE)
 
-        self.compare("exit code", [str(self.case.exit_code)], [str(command.exit_code)])
-        self.compare("output", self.case.stdout, command.stdout)
-        self.compare("error output", self.case.stderr, self.process_stderr(command.stderr))
+        output = Output.Output(self.case.file_name + ":1: test case failed", self.case.configuration.verbose != Configuration.When.NEVER)
+
+        self.compare(output, "exit code", [str(self.case.exit_code)], [str(command.exit_code)])
+        self.compare(output,"output", self.case.stdout, self.process_output_replace(command.stdout, self.case.stdout_replace))
+        self.compare(output, "error output", self.case.stderr, self.process_output_replace(command.stderr, self.case.stderr_replace))
 
         files_expected = []
         for file in self.case.files:
             if file.result:
                 files_expected.append(file.file_name(self.sandbox.directory))
 
-        self.compare("file list", sorted(files_expected), sorted(files_got))
+        self.compare(output, "file list", sorted(files_expected), sorted(files_got))
 
         file_content_ok = True
         for file in self.case.files:
-            if file.name in files_got and not file.compare(self.case.configuration, self.sandbox.directory):
+            if file.name in files_got and not file.compare(output, self.case.configuration, self.sandbox.directory):
                 file_content_ok = False
         if not file_content_ok:
             self.failed.append("file contents")
 
         if self.case.configuration.keep_sandbox == Configuration.When.NEVER or (
                 self.case.configuration.keep_sandbox == Configuration.When.FAILED and not self.failed):
             self.sandbox.cleanup()
@@ -124,17 +129,16 @@
         if self.failed:
             if self.case.configuration.verbose != Configuration.When.NEVER:
                 print(self.case.name + " -- FAIL: " + ", ".join(self.failed))
                 return TestResult.FAILED
         else:
             return TestResult.OK
 
-    def compare(self, description, expected, got):
-        if not Utility.compare_lines(description, expected, got,
-                                     self.case.configuration.verbose != Configuration.When.NEVER):
+    def compare(self, output, description, expected, got):
+        if not Utility.compare_lines(output, description, expected, got):
             self.failed.append(description)
 
     def list_files(self):
         skip_directories = []
         files = []
         for directory, sub_directories, sub_files in os.walk("."):
             skip = False
@@ -168,9 +172,9 @@
         if not self.case.precheck:
             return True
         program = self.case.configuration.find_program(self.case.precheck[0])
         command = Command.Command(program, self.case.precheck[1:])
         command.run()
         return command.exit_code == 0
 
-    def process_stderr(self, lines):
-        return list(map(lambda line: process_stderr_line(line, self.case.stderr_replace), lines))
+    def process_output_replace(self, lines, replacements):
+        return list(map(lambda line: process_output_line(line, replacements), lines))
```

### Comparing `nihtest-1.5.2/nihtest/TestCase.py` & `nihtest-1.6.0/nihtest/TestCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.program = configuration.default_program
         self.exit_code = 0
         self.read_only = []
         self.stderr = []
         self.stderr_replace = []
         self.stdin = []
         self.stdout = []
+        self.stdout_replace = []
         self.ok = True
         self.directories = []
         self.modification_times = {}
         self.working_directory = configuration.default_working_directory
         self.parse_case()
         if not self.ok:
             raise RuntimeError("invalid test case")
@@ -199,14 +200,17 @@
             self.stdin = self.configuration.find_input_file(arguments[0])
         else:
             self.stdin = self.get_inline_data()
 
     def directive_stdout(self, arguments):
         self.stdout = self.io_data(arguments)
 
+    def directive_stdout_replace(self, arguments):
+        self.stdout_replace.append((re.compile(arguments[0]), arguments[1]))
+
     def directive_working_directory(self, arguments):
         self.working_directory = arguments[0]
 
     directives = {
         "arguments": Directive(method=directive_arguments,
                                usage="[argument ...]",
                                minimum_arguments=0, maximum_arguments=-1),
@@ -266,14 +270,17 @@
                            usage="[file]",
                            minimum_arguments=0, maximum_arguments=1,
                            only_once=True),
         "stdout": Directive(method=directive_stdout,
                             usage="[file]",
                             minimum_arguments=0, maximum_arguments=1,
                             only_once=True),
+        "stdout-replace": Directive(method=directive_stdout_replace,
+                                    usage="pattern replacement",
+                                    minimum_arguments=2),
         "working-directory": Directive(method=directive_working_directory,
                                        usage="directory",
                                        minimum_arguments=1,
                                        only_once=True)
     }
 
     def get_program_directories(self):
```

### Comparing `nihtest-1.5.2/nihtest/Utility.py` & `nihtest-1.6.0/nihtest/Utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import sys
 
 from nihtest import CompareArrays
 
 
-def compare_lines(description, expected, got, verbose):
-    if not verbose:
+def compare_lines(output, description, expected, got):
+    if not output.verbose:
         return expected == got
 
     compare = CompareArrays.CompareArrays(expected, got)
     diff = compare.get_diff()
     if diff:
-        print(f"{description} differs:")
+        output.print(f"{description} differs:")
         write_lines(sys.stdout, diff)
         return False
     return True
 
 
 def read_lines(file_name):
     lines = []
```

### Comparing `nihtest-1.5.2/nihtest/__main__.py` & `nihtest-1.6.0/nihtest/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import sys
 
 from nihtest import Test
 from nihtest import Configuration
 
-VERSION = "1.5.2"
+VERSION = "1.6.0"
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='nihtest',
         description="nihtest " + VERSION + "\nCopyright (C) 2023 Dieter Baron and Thomas Klausner")
     parser.add_argument('testcase', help='Testcase to run')
```

### Comparing `nihtest-1.5.2/nihtest.egg-info/PKG-INFO` & `nihtest-1.6.0/nihtest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.5.2
+Version: 1.6.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.5.2/nihtest.egg-info/SOURCES.txt` & `nihtest-1.6.0/nihtest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 manpages/nihtest.mdoc
 nihtest/Command.py
 nihtest/CompareArrays.py
 nihtest/Configuration.py
 nihtest/Environment.py
 nihtest/Features.py
 nihtest/File.py
+nihtest/Output.py
 nihtest/Sandbox.py
 nihtest/Test.py
 nihtest/TestCase.py
 nihtest/Utility.py
 nihtest/__init__.py
 nihtest/__main__.py
 nihtest.egg-info/PKG-INFO
@@ -136,14 +137,16 @@
 tests/stdin-file-pass.test
 tests/stdin-pass.input
 tests/stdin-pass.test
 tests/stdout-fail.input
 tests/stdout-fail.test
 tests/stdout-pass.input
 tests/stdout-pass.test
+tests/stdout-replace-pass.input
+tests/stdout-replace-pass.test
 tests/success.txt
 tests/true-fail.input
 tests/true-fail.test
 tests/true-pass.input
 tests/true-pass.test
 tests/true.c
 tests/uppercase.c
```

### Comparing `nihtest-1.5.2/pyproject.toml` & `nihtest-1.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nihtest"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
     { name="Dieter Baron", email="dillo@nih.at" },
     { name="Thomas Klausner", email="wiz@gatalith.at"}
 ]
 description = "A testing tool for command line utilities."
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
@@ -26,15 +26,15 @@
 "Homepage" = "https://github.com/nih-at/nihtest"
 "Bug Tracker" = "https://github.com/nih-at/nihtest/issues"
 
 [project.scripts]
 nihtest = "nihtest.__main__:main"
 
 [tool.bumpver]
-current_version = "1.5.2"
+current_version = "1.6.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [tool.bumpver.file_patterns]
 "nihtest/__main__.py" = [
     'VERSION = "{version}"'
 ]
 "pyproject.toml" = [
```

### Comparing `nihtest-1.5.2/tests/CMakeLists.txt` & `nihtest-1.6.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/can-preload.c` & `nihtest-1.6.0/tests/can-preload.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/cat.c` & `nihtest-1.6.0/tests/cat.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/comparator.c` & `nihtest-1.6.0/tests/comparator.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/delete.c` & `nihtest-1.6.0/tests/delete.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/delete.h` & `nihtest-1.6.0/tests/delete.h`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/echo.c` & `nihtest-1.6.0/tests/echo.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/false.c` & `nihtest-1.6.0/tests/false.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/file.c` & `nihtest-1.6.0/tests/file.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/getenv.c` & `nihtest-1.6.0/tests/getenv.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/ineffective-delete.c` & `nihtest-1.6.0/tests/ineffective-delete.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/parameter-tests-1.test` & `nihtest-1.6.0/tests/parameter-tests-1.test`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/true.c` & `nihtest-1.6.0/tests/true.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.5.2/tests/uppercase.c` & `nihtest-1.6.0/tests/uppercase.c`

 * *Files identical despite different names*

