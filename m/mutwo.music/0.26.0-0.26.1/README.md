# Comparing `tmp/mutwo.music-0.26.0.tar.gz` & `tmp/mutwo.music-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.music-0.26.0.tar", last modified: Wed Dec 27 20:46:08 2023, max compression
+gzip compressed data, was "mutwo.music-0.26.1.tar", last modified: Tue Apr  9 22:04:01 2024, max compression
```

## Comparing `mutwo.music-0.26.0.tar` & `mutwo.music-0.26.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2102 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.766778 mutwo.music-0.26.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.770778 mutwo.music-0.26.0/mutwo/music_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/grace_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1139 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/metricities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12039 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26267 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_converters/spectrals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.770778 mutwo.music-0.26.0/mutwo/music_events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_events/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10563 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_events/music.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.770778 mutwo.music-0.26.0/mutwo/music_generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_generators/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.774778 mutwo.music-0.26.0/mutwo/music_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1587 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36923 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/ambituses.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2154 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/commas.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.774778 mutwo.music-0.26.0/mutwo/music_parameters/configurations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/configurations/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.774778 mutwo.music-0.26.0/mutwo/music_parameters/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4464 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7580 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/constants/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.774778 mutwo.music-0.26.0/mutwo/music_parameters/instruments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/Bassoon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/BfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      427 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/CelticHarp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/EfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/Flute.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/Oboe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/Piccolo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22802 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/instruments/general.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.774778 mutwo.music-0.26.0/mutwo/music_parameters/lyrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/lyrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/lyrics/text_based_lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3462 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/notation_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23404 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitch_intervals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/mutwo/music_parameters/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/CommonHarmonic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/DirectPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9091 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42947 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/JustIntonationPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1669 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/MidiPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2341 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/ScalePitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24609 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/WesternPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9075 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15358 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/scales.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8424 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_parameters/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/mutwo/music_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_utilities/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_utilities/indicator_collection_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_utilities/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/mutwo/music_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/mutwo/music_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/mutwo.music.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2102 2023-12-27 20:46:08.000000 mutwo.music-0.26.0/mutwo.music.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2759 2023-12-27 20:46:08.000000 mutwo.music-0.26.0/mutwo.music.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-12-27 20:46:08.000000 mutwo.music-0.26.0/mutwo.music.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-12-27 20:46:08.000000 mutwo.music-0.26.0/mutwo.music.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-12-27 20:46:08.000000 mutwo.music-0.26.0/mutwo.music.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-12-27 20:46:08.778778 mutwo.music-0.26.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1844 2023-12-27 20:45:57.000000 mutwo.music-0.26.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.720684 mutwo.music-0.26.1/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/grace_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1139 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/metricities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12039 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26267 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/spectrals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10563 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/music.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_generators/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1587 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36923 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/ambituses.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2154 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/commas.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_parameters/configurations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/diatonic_pitch_classes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4464 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7580 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/instruments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Bassoon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/BfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      427 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/CelticHarp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/EfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Flute.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Oboe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Piccolo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22802 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/general.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/text_based_lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/notation_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23404 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitch_intervals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/CommonHarmonic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/DirectPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9091 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42947 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/JustIntonationPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1669 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/MidiPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2341 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/ScalePitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24609 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/WesternPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9134 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15358 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/scales.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8424 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo/music_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/indicator_collection_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo/music_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo.music.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2759 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1843 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/setup.py
```

### Comparing `mutwo.music-0.26.0/LICENSE` & `mutwo.music-0.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/PKG-INFO` & `mutwo.music-0.26.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.26.0
+Version: 0.26.1
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mutwo.core<2.0.0,>=1.3.0
-Requires-Dist: epitran<2.0.0,>=1.23
+Requires-Dist: epitran<1.25,>=1.23
 Requires-Dist: sympy<2.0.0,>=1.10.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.music
```

### Comparing `mutwo.music-0.26.0/README.md` & `mutwo.music-0.26.1/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/__init__.py` & `mutwo.music-0.26.1/mutwo/music_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/configurations.py` & `mutwo.music-0.26.1/mutwo/music_converters/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/grace_notes.py` & `mutwo.music-0.26.1/mutwo/music_converters/grace_notes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/instruments.py` & `mutwo.music-0.26.1/mutwo/music_converters/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/metricities.py` & `mutwo.music-0.26.1/mutwo/music_converters/metricities.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/parsers.py` & `mutwo.music-0.26.1/mutwo/music_converters/parsers.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/playing_indicators.py` & `mutwo.music-0.26.1/mutwo/music_converters/playing_indicators.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_converters/spectrals.py` & `mutwo.music-0.26.1/mutwo/music_converters/spectrals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_events/configurations.py` & `mutwo.music-0.26.1/mutwo/music_events/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_events/music.py` & `mutwo.music-0.26.1/mutwo/music_events/music.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_generators/constants.py` & `mutwo.music-0.26.1/mutwo/music_generators/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/__init__.py` & `mutwo.music-0.26.1/mutwo/music_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/abc.py` & `mutwo.music-0.26.1/mutwo/music_parameters/abc.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/commas.py` & `mutwo.music-0.26.1/mutwo/music_parameters/commas.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/configurations/instruments.py` & `mutwo.music-0.26.1/mutwo/music_parameters/configurations/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/configurations/pitch_intervals.py` & `mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/configurations/pitches.py` & `mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/diatonic_pitch_classes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/instruments.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/pitch_intervals.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/pitches.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/playing_indicators.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/playing_indicators.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/constants/volumes.py` & `mutwo.music-0.26.1/mutwo/music_parameters/constants/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/instruments/__init__.py` & `mutwo.music-0.26.1/mutwo/music_parameters/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/instruments/general.py` & `mutwo.music-0.26.1/mutwo/music_parameters/instruments/general.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/lyrics/__init__.py` & `mutwo.music-0.26.1/mutwo/music_parameters/lyrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/lyrics/text_based_lyrics.py` & `mutwo.music-0.26.1/mutwo/music_parameters/lyrics/text_based_lyrics.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/notation_indicators.py` & `mutwo.music-0.26.1/mutwo/music_parameters/notation_indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Define notation indicators for simple events.
 
 This submodules provides several classes to express notation
 specifications for :class:`mutwo.core_events.SimpleEvent` objects.
 They mostly derive from traditional Western notation.
-Unlike indicators of the :mod:`mutwo.music_parameters.notation_indicators`
+Unlike playing indicators (see 'mutwo/music_parameters/playing_indicators.py')
 module, notation indicators shouldn't have an effect on the played music
 and are merely specifications of representation. The proper way to handle
 notation indicators should be via a :class:`NotationIndicatorCollection`
 object that should be attached to the respective :class:`SimpleEvent`.
 The collection contains all possible notation indicators which are defined
 in this module. :class:`mutwo.music_events.NoteLike` contain by default
 a notation indicator collection.
@@ -87,14 +87,14 @@
             raise dataclasses.FrozenInstanceError(
                 f"Can't override frozen property (notation indicator) '{notation_indicator}'!"
             )
         else:
             super().__setattr__(parameter_name, value)
 
 
-# Dynamically define __all__ in order to catch all PlayingIndicator classes
+# Dynamically define __all__ in order to catch all NotationIndicator classes
 __all__ = tuple(
     name
     for name, cls in globals().items()
     if inspect.isclass(cls)
     and music_parameters.abc.NotationIndicator in inspect.getmro(cls)
 ) + ("NotationIndicatorCollection",)
```

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitch_intervals.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/CommonHarmonic.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/CommonHarmonic.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/DirectPitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/DirectPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/JustIntonationPitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/JustIntonationPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/MidiPitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/MidiPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/ScalePitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/ScalePitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/WesternPitch.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/WesternPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/pitches/__init__.py` & `mutwo.music-0.26.1/mutwo/music_parameters/pitches/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/playing_indicators.py` & `mutwo.music-0.26.1/mutwo/music_parameters/playing_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     bartok_pizzicato: music_parameters.abc.PlayingIndicator = f()
     bend_after: BendAfter = f(BendAfter)
     breath_mark: music_parameters.abc.PlayingIndicator = f()
     cue: Cue = f(Cue)
     duration_line_dashed: music_parameters.abc.PlayingIndicator = f()
     duration_line_triller: music_parameters.abc.PlayingIndicator = f()
     fermata: Fermata = f(Fermata)
+    flageolet: music_parameters.abc.PlayingIndicator = f()
     glissando: music_parameters.abc.PlayingIndicator = f()
     hairpin: Hairpin = f(Hairpin)
     natural_harmonic_node_list: NaturalHarmonicNodeList = f(NaturalHarmonicNodeList)
     laissez_vibrer: music_parameters.abc.PlayingIndicator = f()
     optional: music_parameters.abc.PlayingIndicator = f()
     ornamentation: Ornamentation = f(Ornamentation)
     pedal: Pedal = f(Pedal)
```

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/scales.py` & `mutwo.music-0.26.1/mutwo/music_parameters/scales.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_parameters/volumes.py` & `mutwo.music-0.26.1/mutwo/music_parameters/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_utilities/exceptions.py` & `mutwo.music-0.26.1/mutwo/music_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_utilities/indicator_collection_parsers.py` & `mutwo.music-0.26.1/mutwo/music_utilities/indicator_collection_parsers.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo/music_utilities/tools.py` & `mutwo.music-0.26.1/mutwo/music_utilities/tools.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/mutwo.music.egg-info/PKG-INFO` & `mutwo.music-0.26.1/mutwo.music.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.26.0
+Version: 0.26.1
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mutwo.core<2.0.0,>=1.3.0
-Requires-Dist: epitran<2.0.0,>=1.23
+Requires-Dist: epitran<1.25,>=1.23
 Requires-Dist: sympy<2.0.0,>=1.10.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.music
```

### Comparing `mutwo.music-0.26.0/mutwo.music.egg-info/SOURCES.txt` & `mutwo.music-0.26.1/mutwo.music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.0/setup.py` & `mutwo.music-0.26.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             include=["mutwo.*"]
         )
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
         "mutwo.core>=1.3.0, <2.0.0",
-        "epitran>=1.23, <2.0.0",
+        "epitran>=1.23, <1.25",
         "sympy>=1.10.1, <2.0.0",
         "python-ranges>=1.2.0, <2.0.0",
     ],
     extras_require=extras_require,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

