# Comparing `tmp/pyMV2H-1.0.1.tar.gz` & `tmp/pyMV2H-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyMV2H-1.0.1.tar", last modified: Sat Jan 30 21:57:49 2021, max compression
+gzip compressed data, was "pyMV2H-1.1.0.tar", last modified: Wed Apr 10 01:53:01 2024, max compression
```

## Comparing `pyMV2H-1.0.1.tar` & `pyMV2H-1.1.0.tar`

### file list

```diff
@@ -1,78 +1,88 @@
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/
--rw-r--r--   0 lucaspaim   (501) staff       (20)      167 2020-12-21 12:41:48.000000 pyMV2H-1.0.1/MANIFEST.in
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3967 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/PKG-INFO
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2811 2021-01-30 21:56:20.000000 pyMV2H-1.0.1/README.md
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H/
--rw-r--r--   0 lucaspaim   (501) staff       (20)       22 2021-01-30 21:54:27.000000 pyMV2H-1.0.1/pyMV2H/__init__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)       29 2020-12-21 12:40:47.000000 pyMV2H-1.0.1/pyMV2H/__main__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1578 2021-01-30 21:56:20.000000 pyMV2H-1.0.1/pyMV2H/cli.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H/commands/
--rw-r--r--   0 lucaspaim   (501) staff       (20)       59 2020-12-23 21:05:45.000000 pyMV2H-1.0.1/pyMV2H/commands/__init__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      303 2020-12-21 13:01:16.000000 pyMV2H-1.0.1/pyMV2H/commands/base.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      804 2021-01-30 14:16:19.000000 pyMV2H-1.0.1/pyMV2H/commands/compare_files.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      347 2020-12-21 19:26:08.000000 pyMV2H-1.0.1/pyMV2H/commands/midi_converter.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H/converter/
--rw-r--r--   0 lucaspaim   (501) staff       (20)        0 2020-12-21 13:15:56.000000 pyMV2H-1.0.1/pyMV2H/converter/__init__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2044 2021-01-02 13:49:59.000000 pyMV2H-1.0.1/pyMV2H/converter/base.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3720 2020-12-22 14:09:47.000000 pyMV2H-1.0.1/pyMV2H/converter/midi_converter.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H/metrics/
--rw-r--r--   0 lucaspaim   (501) staff       (20)        0 2020-12-21 19:51:30.000000 pyMV2H-1.0.1/pyMV2H/metrics/__init__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      386 2020-12-23 00:04:36.000000 pyMV2H-1.0.1/pyMV2H/metrics/f1.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2881 2020-12-23 20:45:22.000000 pyMV2H-1.0.1/pyMV2H/metrics/harmony.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3639 2021-01-01 22:00:18.000000 pyMV2H-1.0.1/pyMV2H/metrics/meter.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      723 2021-01-01 14:57:39.000000 pyMV2H-1.0.1/pyMV2H/metrics/multi_pitch.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      983 2021-01-01 15:34:27.000000 pyMV2H-1.0.1/pyMV2H/metrics/mv2h.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1040 2021-01-01 22:06:52.000000 pyMV2H-1.0.1/pyMV2H/metrics/note_value.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     4467 2021-01-02 14:19:46.000000 pyMV2H-1.0.1/pyMV2H/metrics/voice.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H/utils/
--rw-r--r--   0 lucaspaim   (501) staff       (20)        0 2020-12-21 13:48:44.000000 pyMV2H-1.0.1/pyMV2H/utils/__init__.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      721 2020-12-23 19:53:59.000000 pyMV2H-1.0.1/pyMV2H/utils/algorithm_config.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     6081 2021-01-30 20:24:50.000000 pyMV2H-1.0.1/pyMV2H/utils/align_files.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      717 2021-01-30 21:22:12.000000 pyMV2H-1.0.1/pyMV2H/utils/alignment_node.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1066 2021-01-02 13:56:15.000000 pyMV2H-1.0.1/pyMV2H/utils/comparators.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3827 2020-12-23 23:01:58.000000 pyMV2H-1.0.1/pyMV2H/utils/convert_time.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1799 2021-01-01 14:55:47.000000 pyMV2H-1.0.1/pyMV2H/utils/matches.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      708 2020-12-21 19:45:50.000000 pyMV2H-1.0.1/pyMV2H/utils/midi_meta_tonic_map.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     5912 2021-01-30 20:29:40.000000 pyMV2H-1.0.1/pyMV2H/utils/music.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3113 2020-12-23 22:05:10.000000 pyMV2H-1.0.1/pyMV2H/utils/mv2h.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      497 2020-12-23 17:36:57.000000 pyMV2H-1.0.1/pyMV2H/utils/normalize_list_size.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)      546 2020-12-23 20:18:23.000000 pyMV2H-1.0.1/pyMV2H/utils/pojos.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1552 2020-12-23 20:45:22.000000 pyMV2H-1.0.1/pyMV2H/utils/remove_duplicates.py
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3150 2021-01-02 14:06:42.000000 pyMV2H-1.0.1/pyMV2H/utils/voice.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/
--rw-r--r--   0 lucaspaim   (501) staff       (20)     3967 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/PKG-INFO
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2027 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/SOURCES.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)        1 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/dependency_links.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)       44 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/entry_points.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)       65 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/requires.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)        7 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/pyMV2H.egg-info/top_level.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)       67 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/setup.cfg
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1450 2021-01-02 14:34:29.000000 pyMV2H-1.0.1/setup.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/
--rw-r--r--   0 lucaspaim   (501) staff       (20)     6148 2021-01-30 13:48:20.000000 pyMV2H-1.0.1/tests/.DS_Store
--rw-r--r--   0 lucaspaim   (501) staff       (20)        0 2020-12-21 12:50:55.000000 pyMV2H-1.0.1/tests/__init__.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/__pycache__/
--rw-r--r--   0 lucaspaim   (501) staff       (20)      144 2021-01-30 16:54:38.000000 pyMV2H-1.0.1/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1373 2021-01-30 16:54:38.000000 pyMV2H-1.0.1/tests/__pycache__/test_cli.cpython-37-pytest-6.2.1.pyc
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/commands/
--rw-r--r--   0 lucaspaim   (501) staff       (20)        0 2020-12-21 12:50:55.000000 pyMV2H-1.0.1/tests/commands/__init__.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/commands/__pycache__/
--rw-r--r--   0 lucaspaim   (501) staff       (20)      153 2021-01-30 16:54:38.000000 pyMV2H-1.0.1/tests/commands/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1155 2021-01-30 16:54:38.000000 pyMV2H-1.0.1/tests/commands/__pycache__/test_hello.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2635 2021-01-30 21:44:45.000000 pyMV2H-1.0.1/tests/commands/__pycache__/test_mv2h_metrics.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 lucaspaim   (501) staff       (20)     2682 2021-01-30 21:44:38.000000 pyMV2H-1.0.1/tests/commands/test_mv2h_metrics.py
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/input_files/
--rw-r--r--   0 lucaspaim   (501) staff       (20)     6148 2021-01-30 14:37:19.000000 pyMV2H-1.0.1/tests/input_files/.DS_Store
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/input_files/midi/
--rw-rw-r--   0 lucaspaim   (501) staff       (20)     3526 2021-01-04 21:32:04.000000 pyMV2H-1.0.1/tests/input_files/midi/Bach-846p-edited.mid
--rw-rw-r--   0 lucaspaim   (501) staff       (20)     3544 2021-01-04 21:31:32.000000 pyMV2H-1.0.1/tests/input_files/midi/Bach-846p-orig.mid
--rw-rw-r--   0 lucaspaim   (501) staff       (20)     7107 2021-01-04 21:22:28.000000 pyMV2H-1.0.1/tests/input_files/midi/Bach-italian-concerto-edited.mid
--rw-rw-r--   0 lucaspaim   (501) staff       (20)     7151 2021-01-04 21:23:02.000000 pyMV2H-1.0.1/tests/input_files/midi/Bach-italian-concerto-orig.mid
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/input_files/output_java/
--rw-r--r--   0 lucaspaim   (501) staff       (20)     1658 2021-01-30 21:37:23.000000 pyMV2H-1.0.1/tests/input_files/output_java/output_test_cases.txt
-drwxr-xr-x   0 lucaspaim   (501) staff       (20)        0 2021-01-30 21:57:49.000000 pyMV2H-1.0.1/tests/input_files/transcription_files/
--rw-rw-r--   0 lucaspaim   (501) staff       (20)    18389 2021-01-04 21:33:18.000000 pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-846p-edited.mid.txt
--rw-rw-r--   0 lucaspaim   (501) staff       (20)    18464 2021-01-04 21:33:18.000000 pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-846p-orig.mid.txt
--rw-rw-r--   0 lucaspaim   (501) staff       (20)    35617 2021-01-04 21:33:18.000000 pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-italian-concerto-edited.mid.txt
--rw-rw-r--   0 lucaspaim   (501) staff       (20)    35828 2021-01-04 21:33:18.000000 pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-italian-concerto-orig.mid.txt
--rw-r--r--   0 lucaspaim   (501) staff       (20)      705 2020-12-21 13:00:35.000000 pyMV2H-1.0.1/tests/test_cli.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.540720 pyMV2H-1.1.0/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      167 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/MANIFEST.in
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3340 2024-04-10 01:53:01.540612 pyMV2H-1.1.0/PKG-INFO
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2811 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/README.md
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.516685 pyMV2H-1.1.0/pyMV2H/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       22 2024-04-10 01:46:04.000000 pyMV2H-1.1.0/pyMV2H/__init__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       29 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/__main__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1578 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/cli.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.519120 pyMV2H-1.1.0/pyMV2H/commands/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       59 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/commands/__init__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      303 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/commands/base.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      804 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/commands/compare_files.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      347 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/commands/midi_converter.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.519703 pyMV2H-1.1.0/pyMV2H/converter/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/converter/__init__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2044 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/converter/base.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3720 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/converter/midi_converter.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.521572 pyMV2H-1.1.0/pyMV2H/metrics/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/__init__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      554 2024-04-10 00:37:51.000000 pyMV2H-1.1.0/pyMV2H/metrics/f1.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2881 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/harmony.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3639 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/meter.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1768 2024-04-10 01:39:54.000000 pyMV2H-1.1.0/pyMV2H/metrics/multi_pitch.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1088 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/mv2h.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1242 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/note_value.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     4500 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/metrics/voice.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.530109 pyMV2H-1.1.0/pyMV2H/utils/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/__init__.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      721 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/algorithm_config.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     6241 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/align_files.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      717 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/alignment_node.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1066 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/comparators.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3812 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/convert_time.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      724 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/freeze_args.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2719 2024-04-10 01:43:31.000000 pyMV2H-1.1.0/pyMV2H/utils/matches.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      708 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/midi_meta_tonic_map.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     5937 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/music.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3113 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/mv2h.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      497 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/normalize_list_size.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      546 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/pojos.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1552 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/remove_duplicates.py
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3292 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/pyMV2H/utils/voice.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.518103 pyMV2H-1.1.0/pyMV2H.egg-info/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3340 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/PKG-INFO
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2521 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/SOURCES.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        1 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/dependency_links.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       43 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/entry_points.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       64 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/requires.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        7 2024-04-10 01:53:01.000000 pyMV2H-1.1.0/pyMV2H.egg-info/top_level.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)       67 2024-04-10 01:53:01.541035 pyMV2H-1.1.0/setup.cfg
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1449 2024-04-10 01:44:38.000000 pyMV2H-1.1.0/setup.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.530480 pyMV2H-1.1.0/tests/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/__init__.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.530820 pyMV2H-1.1.0/tests/__pycache__/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     1272 2024-04-10 01:05:45.000000 pyMV2H-1.1.0/tests/__pycache__/test_cli.cpython-39.pyc
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.531347 pyMV2H-1.1.0/tests/commands/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/commands/__init__.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.531812 pyMV2H-1.1.0/tests/commands/__pycache__/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     4082 2024-04-10 01:42:20.000000 pyMV2H-1.1.0/tests/commands/__pycache__/test_mv2h_metrics.cpython-39.pyc
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     4233 2024-04-10 01:42:18.000000 pyMV2H-1.1.0/tests/commands/test_mv2h_metrics.py
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.515124 pyMV2H-1.1.0/tests/input_files/
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.535180 pyMV2H-1.1.0/tests/input_files/midi/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3526 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/Bach-846p-edited.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     3544 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/Bach-846p-orig.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     7107 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/Bach-italian-concerto-edited.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     7151 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/Bach-italian-concerto-orig.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    14002 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/output.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    13039 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/reference.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    15227 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/target.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    12850 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/transcription_01.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    13076 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/transcription_02.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    12988 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/transcription_03.mid
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    12726 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/midi/transcription_04.mid
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.535555 pyMV2H-1.1.0/tests/input_files/output_java/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)     2321 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/output_java/output_test_cases.txt
+drwxr-xr-x   0 lucasmpaim   (501) staff       (20)        0 2024-04-10 01:53:01.539835 pyMV2H-1.1.0/tests/input_files/transcription_files/
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    18389 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-846p-edited.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    18464 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-846p-orig.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    35617 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-italian-concerto-edited.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    35828 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-italian-concerto-orig.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    53502 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/output.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    46716 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/reference.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    59615 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/target.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    46268 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/transcription_01.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    46787 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/transcription_02.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    46743 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/transcription_03.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)    45690 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/input_files/transcription_files/transcription_04.mid.txt
+-rw-r--r--   0 lucasmpaim   (501) staff       (20)      705 2024-04-10 00:35:03.000000 pyMV2H-1.1.0/tests/test_cli.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyMV2H-1.0.1/README.md` & `pyMV2H-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/cli.py` & `pyMV2H-1.1.0/pyMV2H/cli.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/commands/compare_files.py` & `pyMV2H-1.1.0/pyMV2H/commands/compare_files.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/converter/base.py` & `pyMV2H-1.1.0/pyMV2H/converter/base.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/converter/midi_converter.py` & `pyMV2H-1.1.0/pyMV2H/converter/midi_converter.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/metrics/harmony.py` & `pyMV2H-1.1.0/pyMV2H/metrics/harmony.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/metrics/meter.py` & `pyMV2H-1.1.0/pyMV2H/metrics/meter.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/metrics/mv2h.py` & `pyMV2H-1.1.0/pyMV2H/metrics/mv2h.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,19 @@
         p_music: Music,
         t_music: Music,
         weights: MV2H_WEIGHTS = MV2H_WEIGHTS()
 ):
     p_music.read_if_needed()
     t_music.read_if_needed()
 
-    multi_pitch = multi_pitch_accuracy(p_music.__notes__, t_music.__notes__) * weights.multi_pitch
-    voice = voice_score(p_music, t_music) * weights.voice
+    multi_pitch, multi_pitch_match = multi_pitch_accuracy(p_music.__notes__, t_music.__notes__, True)
+    multi_pitch *= weights.multi_pitch
+
+    voice, voice_match = voice_score(p_music, t_music, True)
+    voice *= weights.voice
     harmony = harmony_score(p_music, t_music) * weights.harmonic
     meter = meter_score(p_music, t_music) * weights.metrical
-    note_value = note_value_score(p_music, t_music) * weights.note_value
+    note_value = note_value_score(p_music, t_music, multi_pitch_match, voice_match) * weights.note_value
 
     return MV2H(
         multi_pitch, voice, harmony, meter, note_value, weights
     )
```

### Comparing `pyMV2H-1.0.1/pyMV2H/metrics/note_value.py` & `pyMV2H-1.1.0/pyMV2H/metrics/note_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from pyMV2H.metrics.multi_pitch import multi_pitch_accuracy
 from pyMV2H.metrics.voice import voice_score
 from pyMV2H.utils.music import Music
 from pyMV2H.utils.algorithm_config import DURATION_DELTA
 from pyMV2H.utils.pojos import NOTE
 
 
-def note_value_score(p_music: Music, t_music: Music) -> float:
+def note_value_score(p_music: Music, t_music: Music, multi_pitch_match=None, voice_match=None) -> float:
     p_music.read_if_needed()
     t_music.read_if_needed()
 
-    _, notes_check = voice_score(p_music, t_music, return_match_mapping=True)
-    _, multi_pinch_check = multi_pitch_accuracy(
-        p_music.__notes__,
-        t_music.__notes__,
-        return_match_notes=True
-    )
+    notes_check = voice_match
+    multi_pinch_check = multi_pitch_match
+
+    if notes_check is None:
+        _, notes_check = voice_score(p_music, t_music, return_match_mapping=True)
+
+    if multi_pinch_check is None:
+        _, multi_pinch_check = multi_pitch_accuracy(
+            p_music.__notes__,
+            t_music.__notes__,
+            return_match_notes=True
+        )
     score_sum = 0.
     for t_note in notes_check:
         score_sum += _get_note_score(multi_pinch_check[t_note], t_note)
     return score_sum / len(notes_check)
 
 
 def _get_note_score(p_note: NOTE, t_note: NOTE) -> float:
```

### Comparing `pyMV2H-1.0.1/pyMV2H/metrics/voice.py` & `pyMV2H-1.1.0/pyMV2H/metrics/voice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from functools import lru_cache
+
 from .f1 import f1_score
 from pyMV2H.utils.music import Music
 from ..utils.align_files import create_list_of_size
 from ..utils.matches import note_match, match_note_list
 from ..utils.voice import Voice
 
 
+@lru_cache(maxsize=128)
 def voice_score(p_music: Music, t_music: Music, return_match_mapping=False):
     p_music.read_if_needed()
     t_music.read_if_needed()
 
-    provided_voices = create_list_of_size(len(p_music.__voices__), lambda: Voice())
-    transcription_voices = create_list_of_size(len(t_music.__voices__), lambda: Voice())
+    provided_voices = [Voice() for _ in range(len(p_music.__voices__))]
+    transcription_voices = [Voice() for _ in range(len(t_music.__voices__))]
     p_note_mapping = match_note_list(p_music.__notes__, t_music.__notes__)
 
     match_mapping = list()
 
     for t_note in p_note_mapping.keys():
         p_note = p_note_mapping[t_note]
         provided_voices[p_note.voice].add_note(note=p_note)
```

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/algorithm_config.py` & `pyMV2H-1.1.0/pyMV2H/utils/algorithm_config.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/align_files.py` & `pyMV2H-1.1.0/pyMV2H/utils/align_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+import math
 from functools import reduce
 
-import numpy as np
+from tqdm import tqdm
 
 from pyMV2H.metrics import f1
 from pyMV2H.utils.music import Music
 from pyMV2H.utils.algorithm_config import NON_ALIGNMENT_PENALTY
 from pyMV2H.utils.alignment_node import AlignmentNode
 from pyMV2H.utils.mv2h import MV2H
 
 
 def align_files(provided_file: Music, transcription_file: Music):
     """
     Align based on DTW algorithm
     """
+
     from pyMV2H.metrics.mv2h import mv2h
 
     provided_file.read_if_needed()
     transcription_file.read_if_needed()
 
     alignment_nodes = _get_possible_alignments(provided_file, transcription_file)
     total = 0
     best = MV2H(0., 0., 0., 0., 0.)
     best_music = None
 
     for node in alignment_nodes:
         total += node.count
 
-    for node_aligment in alignment_nodes:
-        for j in range(node_aligment.count):
-            alignment = node_aligment.get_alignment(j)
-            shifted_music = transcription_file.align(provided_file, alignment)
-            candidate: MV2H = mv2h(provided_file, shifted_music)
-            if candidate > best:
-                best = candidate
-                best_music = shifted_music
+    with tqdm(total=total) as pbar:
+        for node_alignment in alignment_nodes:
+            for j in range(node_alignment.count):
+                alignment = node_alignment.get_alignment(j)
+                shifted_music = transcription_file.align(provided_file, alignment)
+                candidate: MV2H = mv2h(provided_file, shifted_music)
+                if candidate > best:
+                    best = candidate
+                    best_music = shifted_music
+                pbar.update()
+
     return best_music, best
 
 
 def _get_possible_alignments(provided_file: Music, transcription_file: Music):
     previous_cells = _get_align_matrix(provided_file, transcription_file)
     ARRAY_SIZE = len(previous_cells)
     cache_matrix = create_list_of_size(ARRAY_SIZE, lambda: create_list_of_size(len(previous_cells[0]), list))
@@ -82,20 +87,20 @@
 
     p_notes_map = _get_note_pitch_maps(provided_notes)
     t_notes_map = _get_note_pitch_maps(transcription_notes)
 
     ARRAY_SIZE = (len(provided_notes) + 1, len(transcription_notes) + 1)
 
     previous_cells = create_list_of_size(ARRAY_SIZE[0], lambda: create_list_of_size(ARRAY_SIZE[1], list))
-    distances = np.zeros(ARRAY_SIZE)
-    distances[0] = np.full(ARRAY_SIZE[1], np.Inf)
+    distances = [[0 for _ in range(ARRAY_SIZE[1])] for _ in range(ARRAY_SIZE[0])] # create_list_of_size(ARRAY_SIZE[0], lambda: create_list_of_size(ARRAY_SIZE[1], 0))
+    distances[0] = [math.inf] * ARRAY_SIZE[1]
     distances[0][0] = 0.
 
     for i in range(1, ARRAY_SIZE[0]):
-        distances[i][0] = np.Inf
+        distances[i][0] = math.inf
 
     for j in range(1, ARRAY_SIZE[1]):
         for i in range(1, ARRAY_SIZE[0]):
             distance = get_distance(p_notes_map[i - 1], t_notes_map[j - 1])
 
             distance_i_1 = distances[i - 1][j] + NON_ALIGNMENT_PENALTY
             distance_j_1 = distances[i][j - 1] + NON_ALIGNMENT_PENALTY
@@ -133,38 +138,36 @@
     :param p_note_map: The pitch map of a ground truth note set.
     :param t_note_map: he pitch map of a possible transcription note set.
     :return: The alignment score. 1 - its F-measure.
     """
     true_positives = 0
     false_positives = 0
 
-    for t_key in t_note_map.keys():
-        count = t_note_map[t_key]
+    for t_key, count in t_note_map.items():
         if t_key in p_note_map:
             p_count = p_note_map[t_key]
             true_positives += min(count, p_count)
             if count > p_count:
                 false_positives += count - p_count
         else:
             false_positives += count
 
     if true_positives == 0:
         return 1.0
 
-    p_count = reduce(lambda a, b: a + b, p_note_map.values(), 0)
+    p_count = sum(p_note_map.values())
     false_negatives = p_count - true_positives
     return 1 - f1.f1_score(true_positives, false_positives, false_negatives)
 
 
 def create_list_of_size(size: int, value) -> list:
     """
     Helper function to create an list of size x with initial value
     Use this method only for dynamic lists, make preference for numpy arrays initializers like:
     np.zeros(SHAPE) etc.
     :param size: size of the list
     :param value: lambda function to initialize the value
     :return: the list of size x with all elements equal to return of value
     """
-    list_to_return = list()
-    for _ in range(size):
-        list_to_return.append(value())
-    return list_to_return
+    return [
+        value() if callable(value) else value for _ in range(size)
+    ]
```

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/alignment_node.py` & `pyMV2H-1.1.0/pyMV2H/utils/alignment_node.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/comparators.py` & `pyMV2H-1.1.0/pyMV2H/utils/comparators.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/convert_time.py` & `pyMV2H-1.1.0/pyMV2H/utils/convert_time.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 
 def convert_time(time: int, p_music, t_music, alignment, alignment_times) -> int:
 
-    alignment_time = None
-
-    if time in alignment_times:
-        alignment_time = alignment_times[time]
-
+    alignment_time = alignment_times.get(time, None)
     if alignment_time is not None:
         return alignment_time
 
     t_index = -1
     t_notes = t_music.get_notes_grouped_by_onset()
 
     # Find the correct transcription anchor index to start with
@@ -26,31 +22,32 @@
 
     p_notes = p_music.get_notes_grouped_by_onset()
     p_previous_anchor = -1
     p_previous_previous_anchor = -1
     p_next_anchor = len(p_notes)
     p_next_next_anchor = len(p_notes)
 
-    for index, _ in enumerate(alignment):
-        if alignment[index] != -1:
-            if alignment[index] == t_index:
+    for index, current_alignment in enumerate(alignment):
+        if current_alignment != -1:
+            if current_alignment == t_index:
                 # This is the correct time, exactly on the index
                 return p_notes[index][0].on
-            elif alignment[index] < t_index:
+            elif current_alignment < t_index:
                 # The time is past this anchor
                 p_previous_previous_anchor = p_previous_anchor
                 p_previous_anchor = index
             else:
                 #  We are past the time
                 if p_next_anchor == len(p_notes):
                     # This is the first anchor for which we are past the time
                     p_next_anchor = index
                 else:
                     # This is the 2nd anchor for which we are past the time
                     p_next_next_anchor = index
+                    break
 
     if p_previous_anchor == -1 and p_next_anchor == len(p_notes):
         # Nothing was aligned
         alignment_times[time] = time
         return time
 
     if p_previous_anchor == -1:
@@ -68,15 +65,15 @@
             alignment_time = (
                     time -
                     t_notes[alignment[p_next_anchor]][0].on +
                     p_notes[alignment[p_next_anchor]][0].on
             )
     elif p_next_anchor == len(p_notes):
         # Time is after the last anchor. Use the previous rate.
-        if p_next_anchor == len(p_notes):
+        if p_previous_anchor != -1:
             alignment_time = _convert_time(
                 time,
                 p_previous_previous_anchor,
                 p_previous_anchor,
                 p_notes,
                 t_notes,
                 alignment
```

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/midi_meta_tonic_map.py` & `pyMV2H-1.1.0/pyMV2H/utils/midi_meta_tonic_map.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/music.py` & `pyMV2H-1.1.0/pyMV2H/utils/music.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import lru_cache
+
 from pyMV2H.utils.convert_time import convert_time
 from pyMV2H.utils.comparators import note_comparator
 from pyMV2H.utils.pojos import NOTE, TATUM, KEY, HIERARCHY
 from pyMV2H.utils.voice import Voice
 
 
 def need_read(fn):
@@ -28,26 +30,28 @@
         self.__keys__ = keys
         self.__notes__ = notes
         self.__hierarchy__ = hierarchy
         self.__has_read__ = True
         self.__duration__ = 0.
         self.__voices__ = list()
         self.__post_process__()
+        self.__notes_list__ = list()
 
     def read_if_needed(self):
         if not self.__has_read__:
             self.read()
 
     def read(self):
         self.__tatums__ = list()
         self.__keys__ = list()
         self.__notes__ = list()
         self.__hierarchy__ = list()
         self.__voices__ = list()
         self.__duration__ = 0.
+        self.__notes_list__ = list()
 
         with open(self.__file_name__, 'r') as file:
             all_lines = file.readlines()
             for line in all_lines:
                 self.parse_line(line)
         self.__has_read__ = True
         self.__post_process__()
@@ -88,14 +92,18 @@
         if len(args) == 3:
             # time is optional on original description, set it to zero by default
             args.append(0)
         self.__hierarchy__.append(HIERARCHY(*args))
 
     @need_read
     def get_notes_grouped_by_onset(self):
+
+        if len(self.__notes_list__) != 0:
+            return self.__notes_list__
+
         notes = list()
 
         most_recent_list = list()
         most_recent_value_onset_time = self.__notes__[0].on
         most_recent_list.append(self.__notes__[0])
         notes.append(most_recent_list)
 
@@ -103,14 +111,15 @@
             if note.on == most_recent_value_onset_time:
                 most_recent_list.append(note)
             else:
                 most_recent_list = list()
                 most_recent_value_onset_time = note.on
                 most_recent_list.append(note)
                 notes.append(most_recent_list)
+        self.__notes_list__ = notes
         return notes
 
     def __post_process__(self):
         """
         Create music structure
         """
         if self.__notes__ is None:
@@ -121,65 +130,56 @@
             self.__duration__ = max(self.__duration__, note.off_val)
             # Create music voices
             while note.voice >= len(self.__voices__):
                 self.__voices__.append(Voice())
             # add note to voice
             self.__voices__[note.voice].add_note(note)
 
-        for key in self.__keys__:
-            self.__duration__ = max(self.__duration__, key.time)
-
-        for tatum in self.__tatums__:
-            self.__duration__ = max(self.__duration__, tatum.time)
+        if len(self.__keys__) > 0:
+            self.__duration__ = max(self.__duration__, max(self.__keys__, key=lambda item: item.time).time)
+        if len(self.__tatums__) > 0:
+            self.__duration__ = max(self.__duration__, max(self.__tatums__, key=lambda item: item.time).time)
 
         for voice in self.__voices__:
             voice.create_connections()
 
     def align(self, p_music, alignment: list):
-        new_notes = list()
         align_times = dict()
 
         # Convert each note into a new note
-        for note in self.__notes__:
-            new_notes.append(
-                NOTE(
-                    note.pitch,
-                    convert_time(note.on, p_music, self, alignment, align_times),
-                    convert_time(note.on_val, p_music, self, alignment, align_times),
-                    convert_time(note.off_val, p_music, self, alignment, align_times),
-                    note.voice
-                )
-            )
+        new_notes = [
+            NOTE(
+                note.pitch,
+                convert_time(note.on, p_music, self, alignment, align_times),
+                convert_time(note.on_val, p_music, self, alignment, align_times),
+                convert_time(note.off_val, p_music, self, alignment, align_times),
+                note.voice
+            ) for note in self.__notes__
+        ]
 
         # Convert each hierarchy
-        new_hierarchies = list()
-        for hierarchy in self.__hierarchy__:
-            new_hierarchies.append(
-                HIERARCHY(
-                    hierarchy.bpb,
-                    hierarchy.sbpb,
-                    hierarchy.tpsb,
-                    hierarchy.al,
-                    convert_time(hierarchy.time, p_music, self, alignment, align_times),
-                )
-            )
+        new_hierarchies = [
+            HIERARCHY(
+                hierarchy.bpb,
+                hierarchy.sbpb,
+                hierarchy.tpsb,
+                hierarchy.al,
+                convert_time(hierarchy.time, p_music, self, alignment, align_times),
+            ) for hierarchy in self.__hierarchy__
+        ]
 
         # Convert each tatum
-        new_tatums = list()
-        for tatum in self.__tatums__:
-            new_tatums.append(
-                TATUM(
-                    convert_time(tatum.time, p_music, self, alignment, align_times),
-                )
-            )
-
-        new_keys = list()
-        for key in self.__keys__:
-            new_keys.append(
-                KEY(
-                    key.tonic,
-                    key.is_major,
-                    convert_time(key.time, p_music, self, alignment, align_times),
-                )
-            )
+        new_tatums = [
+            TATUM(
+                convert_time(tatum.time, p_music, self, alignment, align_times),
+            ) for tatum in self.__tatums__
+        ]
+
+        new_keys = [
+            KEY(
+                key.tonic,
+                key.is_major,
+                convert_time(key.time, p_music, self, alignment, align_times),
+            ) for key in self.__keys__
+        ]
 
         return Music(new_tatums, new_keys, new_notes, new_hierarchies)
```

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/mv2h.py` & `pyMV2H-1.1.0/pyMV2H/utils/mv2h.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/pojos.py` & `pyMV2H-1.1.0/pyMV2H/utils/pojos.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/remove_duplicates.py` & `pyMV2H-1.1.0/pyMV2H/utils/remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/pyMV2H/utils/voice.py` & `pyMV2H-1.1.0/pyMV2H/utils/voice.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,30 +27,35 @@
 
 
 class Voice:
 
     def __init__(self):
         self.__notes__ = list()
         self.__note_clusters__ = OrderedDict()
+        self.__connection_created__ = False
 
     def create_connections(self):
+
+        if self.__connection_created__:
+            return
+
         # remove all previous connections
         for cluster in self.__note_clusters__.values():
             cluster.next_clusters = list()
 
         _cluster = self.__note_clusters__
         self.__note_clusters__ = OrderedDict(
             sorted(
                 _cluster.items(), key=cluster_comparator()
             )
         )
 
         ordered_notes = list(self.__notes__)
         ordered_notes.sort(key=note_comparator())
-        self.__notes__ = list(ordered_notes)
+        self.__notes__ = ordered_notes
         # create new connections
         for base_key in self.__note_clusters__.keys():
             base_cluster = self.__note_clusters__[base_key]
 
             for next_key in self.__note_clusters__.keys():
                 next_cluster = self.__note_clusters__[next_key]
                 if next_key == base_key:
@@ -64,14 +69,15 @@
                             base_cluster.next_clusters[0].onset_time == next_cluster.onset_time
                     ):
                         # All note clusters at the earliest time after this one's offset time, if no
                         # connections were added from rule
                         base_cluster.next_clusters.append(next_cluster)
                     else:
                         break
+        self.__connection_created__ = True
 
     def get_cluster(self, note: NOTE) -> Optional[NoteCluster]:
         key = (NoteCluster(note.on, note.off_val)).key_string
         cluster = self.__note_clusters__[key]
         if cluster is not None and note in cluster.notes:
             return cluster
         return None
```

### Comparing `pyMV2H-1.0.1/setup.py` & `pyMV2H-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     url='https://github.com/lucasmpaim/pyMV2H',
     author='Lucas Mrowskovsky Paim',
     author_email='lucas.mrowskovsky@pucpr.edu.br',
     license='UNLICENSE',
     classifiers=[],
     keywords='cli',
     packages=find_packages(exclude=['docs', 'tests*']),
-    install_requires=['docopt', 'pretty_midi', 'mido', 'numpy'],
+    install_requires=['docopt', 'pretty_midi', 'mido', 'tqdm'],
     extras_require={
         'test': ['coverage', 'pytest', 'pytest-cov'],
     },
     entry_points={
         'console_scripts': [
             'pyMV2H=pyMV2H.cli:main',
         ],
```

### Comparing `pyMV2H-1.0.1/tests/input_files/midi/Bach-846p-edited.mid` & `pyMV2H-1.1.0/tests/input_files/midi/Bach-846p-edited.mid`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/midi/Bach-846p-orig.mid` & `pyMV2H-1.1.0/tests/input_files/midi/Bach-846p-orig.mid`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/midi/Bach-italian-concerto-edited.mid` & `pyMV2H-1.1.0/tests/input_files/midi/Bach-italian-concerto-edited.mid`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/midi/Bach-italian-concerto-orig.mid` & `pyMV2H-1.1.0/tests/input_files/midi/Bach-italian-concerto-orig.mid`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/output_java/output_test_cases.txt` & `pyMV2H-1.1.0/tests/input_files/output_java/output_test_cases.txt`

 * *Files 10% similar despite different names*

```diff
@@ -58,7 +58,30 @@
 Multi-pitch: 1.0
 Voice: 1.0
 Meter: 1.0
 Value: 1.0
 Harmony: 1.0
 MV2H: 1.0
 
+-g ${TRANSCRIPTION_DIR}/reference.mid.txt -t ${TRANSCRIPTION_DIR}/transcription_04.mid.txt
+Multi-pitch: 0.8424878836833601
+Voice: 0.9833333333333334
+Meter: 1.0
+Value: 0.995855130615959
+Harmony: 1.0
+MV2H: 0.9643352695265305
+
+-g ${TRANSCRIPTION_DIR}/target.mid.txt -t ${TRANSCRIPTION_DIR}/output.mid.txt
+Multi-pitch: 0.7116057233704293
+Voice: 0.9219817767653758
+Meter: 1.0
+Value: 0.9422821071123146
+Harmony: 1.0
+MV2H: 0.9151739214496238
+
+-g ${TRANSCRIPTION_DIR}/target.mid.txt -t ${TRANSCRIPTION_DIR}/output.mid.txt -a
+Multi-pitch: 0.7243243243243244
+Voice: 0.9153788727136992
+Meter: 0.9030769230769231
+Value: 0.941540225997801
+Harmony: 1.0
+MV2H: 0.8968640692225496
```

### Comparing `pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-846p-edited.mid.txt` & `pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-846p-edited.mid.txt`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-846p-orig.mid.txt` & `pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-846p-orig.mid.txt`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-italian-concerto-edited.mid.txt` & `pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-italian-concerto-edited.mid.txt`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/input_files/transcription_files/Bach-italian-concerto-orig.mid.txt` & `pyMV2H-1.1.0/tests/input_files/transcription_files/Bach-italian-concerto-orig.mid.txt`

 * *Files identical despite different names*

### Comparing `pyMV2H-1.0.1/tests/test_cli.py` & `pyMV2H-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

