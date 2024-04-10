# Comparing `tmp/musicAlgLib-1.1.6.tar.gz` & `tmp/musicAlgLib-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.1.6.tar", last modified: Mon Apr  8 02:21:36 2024, max compression
+gzip compressed data, was "musicAlgLib-1.1.8.tar", last modified: Wed Apr 10 03:09:18 2024, max compression
```

## Comparing `musicAlgLib-1.1.6.tar` & `musicAlgLib-1.1.8.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.209596 musicAlgLib-1.1.6/
--rw-rw-rw-   0        0        0     4676 2024-04-08 02:21:36.209100 musicAlgLib-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.176364 musicAlgLib-1.1.6/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.180333 musicAlgLib-1.1.6/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.180828 musicAlgLib-1.1.6/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.191740 musicAlgLib-1.1.6/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.192237 musicAlgLib-1.1.6/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.6/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.192732 musicAlgLib-1.1.6/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19719 2024-04-08 02:18:42.000000 musicAlgLib-1.1.6/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.193228 musicAlgLib-1.1.6/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.6/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.194220 musicAlgLib-1.1.6/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.195212 musicAlgLib-1.1.6/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.195709 musicAlgLib-1.1.6/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.197197 musicAlgLib-1.1.6/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.197692 musicAlgLib-1.1.6/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.6/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.200199 musicAlgLib-1.1.6/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.201660 musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.203148 musicAlgLib-1.1.6/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.203644 musicAlgLib-1.1.6/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.6/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.6/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.204141 musicAlgLib-1.1.6/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.6/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     5038 2024-04-08 02:21:22.000000 musicAlgLib-1.1.6/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    15970 2024-04-08 02:18:42.000000 musicAlgLib-1.1.6/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.205132 musicAlgLib-1.1.6/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0    12316 2024-04-08 02:18:42.000000 musicAlgLib-1.1.6/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.206124 musicAlgLib-1.1.6/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     6338 2024-04-08 02:21:22.000000 musicAlgLib-1.1.6/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.207116 musicAlgLib-1.1.6/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.208108 musicAlgLib-1.1.6/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.6/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.208604 musicAlgLib-1.1.6/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.6/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.6/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:21:36.179341 musicAlgLib-1.1.6/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-08 02:21:36.000000 musicAlgLib-1.1.6/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-08 02:21:36.000000 musicAlgLib-1.1.6/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:21:36.000000 musicAlgLib-1.1.6/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-08 02:21:36.000000 musicAlgLib-1.1.6/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 02:21:36.000000 musicAlgLib-1.1.6/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 02:21:36.209596 musicAlgLib-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     5839 2024-04-08 02:21:29.000000 musicAlgLib-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.335065 musicAlgLib-1.1.8/
+-rw-rw-rw-   0        0        0     4676 2024-04-10 03:09:18.335065 musicAlgLib-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.109391 musicAlgLib-1.1.8/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.121294 musicAlgLib-1.1.8/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.122286 musicAlgLib-1.1.8/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4990 2024-04-10 02:54:19.000000 musicAlgLib-1.1.8/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.268602 musicAlgLib-1.1.8/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.so
+-rw-rw-rw-   0        0        0   443512 2024-04-10 02:47:29.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/peaqb
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.269098 musicAlgLib-1.1.8/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.8/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.269594 musicAlgLib-1.1.8/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    18008 2024-04-10 02:35:19.000000 musicAlgLib-1.1.8/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.270586 musicAlgLib-1.1.8/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.8/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.271082 musicAlgLib-1.1.8/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.289434 musicAlgLib-1.1.8/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.289930 musicAlgLib-1.1.8/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.291418 musicAlgLib-1.1.8/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.291914 musicAlgLib-1.1.8/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.8/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.310761 musicAlgLib-1.1.8/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.321673 musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-09 08:00:44.000000 musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.323161 musicAlgLib-1.1.8/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.324153 musicAlgLib-1.1.8/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.8/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.8/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.324649 musicAlgLib-1.1.8/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.8/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4957 2024-04-09 06:04:47.000000 musicAlgLib-1.1.8/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    16458 2024-04-09 07:55:19.000000 musicAlgLib-1.1.8/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.325641 musicAlgLib-1.1.8/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0     8648 2024-04-10 02:54:19.000000 musicAlgLib-1.1.8/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.326137 musicAlgLib-1.1.8/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     4187 2024-04-10 02:54:19.000000 musicAlgLib-1.1.8/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.332585 musicAlgLib-1.1.8/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.333577 musicAlgLib-1.1.8/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.8/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.334569 musicAlgLib-1.1.8/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.8/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.8/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:09:18.111870 musicAlgLib-1.1.8/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-10 03:09:17.000000 musicAlgLib-1.1.8/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2250 2024-04-10 03:09:18.000000 musicAlgLib-1.1.8/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:09:17.000000 musicAlgLib-1.1.8/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-10 03:09:18.000000 musicAlgLib-1.1.8/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 03:09:18.000000 musicAlgLib-1.1.8/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:09:18.335561 musicAlgLib-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     5900 2024-04-10 03:09:08.000000 musicAlgLib-1.1.8/setup.py
```

### Comparing `musicAlgLib-1.1.6/PKG-INFO` & `musicAlgLib-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.6
+Version: 1.1.8
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.6/README.md` & `musicAlgLib-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.1.8/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.1.8/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # coding=utf-8
 import numpy as np
-
-import librosa
-import soundfile as sf
-
 import math
 
 
 def histogram_calculation(x=None, N=None, K=None):
     '''
     x:   audio samples
     N:   number of audio sample
@@ -171,23 +167,28 @@
 
     clipping_ratio = np.zeros(shape=[len(audio_data), ], dtype=np.float32)
     clipping_detect_flag = np.zeros(shape=[len(audio_data), ], dtype=np.float32)
     for i in range(audio_piece):
         clipping_ratio[i * N:(i + 1) * N] = Rcl_list[i] * 10000 / 32768
         clipping_detect_flag[i * N:(i + 1) * N] = clipping_flag_list[i] * 10000 / 32768
     return sum(clipping_flag_list)/len(clipping_flag_list)
-def cal_clip_index(testFile=None):
+def cal_clip_index(testdata,samplerate=48000):
     """
     Parameters
     ----------
     testFile
     Returns
     -------
 
     """
-    audio_data, sr = librosa.load(testFile, sr=None)  # float [-1,1)
-    return clip_detect(audio_data=audio_data, sr=sr)
+    channel = len(testdata[0])
+    clip_list = []
+    for i in range(channel):
+        curdata = testdata[:, i]
+        clip_list.append(clip_detect(audio_data=curdata, sr=samplerate))
+
+    return clip_list
 
 if __name__ == '__main__':
 
     clipindex = cal_clip_index('mixDstFile.wav')
     print(clipindex)
```

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.1.8/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.1.8/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 import librosa
 from PCC.Pearson_CC import get_max_cc_by_dll
 import ctypes,os,platform
 from ctypes import *
 from timeAligment.time_align import cal_fine_delay_of_specific_section
 from VAD_NN.hubconf import silero_vad
 
+
+
+
+
 def get_my_dll():
     """
     :return:
     """
     mydll = None
     cur_paltform = platform.platform().split('-')[0]
     if cur_paltform == 'Windows':
@@ -110,67 +114,38 @@
         raise TypeError('wrong format! not wav/mp4 file!' + str(suffix))
     if suffix == '.mp4':
         wavFileName = get_wav_from_mp4(wavFileName)
     wavf = wave.open(wavFileName, 'rb')
     refChannel,refsamWidth,refsamplerate,refframeCount = wavf.getnchannels(),wavf.getsampwidth(),wavf.getframerate(),wavf.getnframes()
     return refChannel,refsamWidth*8,refsamplerate,refframeCount
 
-def get_rms_level(wavFileName=None,rmsMode='total',section=None,speechOnly=False,frameDuration=0.05,shiftduration=0.05):
+def get_rms_level_by_float(data,samplerate=48000,frameDuration=0.05,shiftduration=0.05):
     """
-    wavFileName：输入文件 wav，mp4
+    data：float 类型数据
+    samplerate： 采样率
+    section：计算范围
+    frameDuration：帧长，默认50ms
+    shiftduration：帧移，默认50ms
     Returns
     -------
-    refChannel:通道数
-    refsamWidth：比特位 2代表16bit
-    refsamplerate：采样率
-    refframeCount：样点数
+    RMS
     """
-    suffix = os.path.splitext(wavFileName)[-1]
-    if suffix != '.wav':
-        raise TypeError('wrong format! not wav file!' + str(suffix))
-
-    lenth,fs = get_file_duration(wavFileName)
-    data = get_one_channel_data(wavFileName)
-    if section == None:
-        startTime = 0
-        endTime = lenth
-    else:
-        startTime = section[0]
-        endTime = section[1]
-    if startTime > lenth or startTime > endTime:
-        raise TypeError('start point is larger than the file lenth :' + str(suffix))
-    if endTime > lenth:
-        endTime = lenth
-    curdata = data[int(startTime*fs):int(endTime*fs)]
-    if section == None and speechOnly:
-        speechSection = silero_vad(wavFileName)
-        # TODO 选取最小的地方计算有效频谱
-        testdata, fs, ch = get_data_array(wavFileName)
-        curdata = np.array([])
-        for eachSection in speechSection:
-            curdata = np.concatenate(
-                (curdata, testdata[int(fs * eachSection[0]):int(fs * eachSection[1])]))
-
-    if rmsMode == 'total':
-        return get_rms(curdata)
-    if rmsMode == 'average':
-        return get_ave_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    if rmsMode == 'peak':
-        return  get_peak_rms(curdata)
-    if rmsMode == 'std':
-        return  get_std_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    if rmsMode == 'max':
-        return  get_max_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    if rmsMode == 'min':
-        return  get_min_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    if rmsMode == 'dynmic':
-        return  get_max_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration) - get_min_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    if rmsMode == 'duration':
-        return  get_duration_above_specific_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
-    return None
+    channel = len(data[0])
+    result = {'total': [], 'average': [], 'peak': [], 'max': [], 'min': [], 'dymic': [], 'std': []}
+    for i in range(channel):
+        curdata = data[:, i]
+        result['total'].append(get_rms(curdata))
+        ave,max,minn,dymic,std =get_ave_rms(curdata,samplerate,frameDuration,shiftduration)
+        result['average'].append(ave)
+        result['max'].append(max)
+        result['min'].append(minn)
+        result['dymic'].append(dymic)
+        result['std'].append(std)
+        result['peak'].append(get_peak_rms(curdata))
+    return result
 
 
 
 def calculate_band_energy(audio_signal, sample_rate, num_bands,freq_mode='upper'):
     # Perform FFT on audio signal
     fmin,fmax = 100,sample_rate/2 - 100
     freq_points = np.linspace(0, sample_rate/2, num_bands+1)
@@ -239,46 +214,38 @@
             return i
     return -1
 
 
 
 
 
-def get_effective_spectral(audiofile):
-
-    speechSection = silero_vad(audiofile)
+def get_effective_spectral(testdata,fs):
 
     #TODO 选取最小的地方计算有效频谱
-    testdata,fs,ch = get_data_array(audiofile)
-
-
-    testallarray = np.array([])
-    for eachSection in speechSection:
-        testallarray= np.concatenate((testallarray,testdata[int(fs*eachSection[0]):int(fs*eachSection[1])]))
 
     #audio_data, sample_rate, ch = get_data_array(audiofile)
     FRAME_LEN = 960
     frame_shift = 480
 
-    n_sengen = (len(testallarray) - FRAME_LEN) // frame_shift
+    n_sengen = (len(testdata) - FRAME_LEN) // frame_shift
     max_level,min_level = -99,99
     for a in range(n_sengen):
-        cursrcLevel = get_rms(testallarray[a * frame_shift:a * frame_shift + FRAME_LEN])
+        cursrcLevel = get_rms(testdata[a * frame_shift:a * frame_shift + FRAME_LEN])
         if cursrcLevel >max_level:
             max_level = cursrcLevel
         if cursrcLevel < min_level:
             min_level = cursrcLevel
     print(max_level,min_level,'++++')
     thirdduration = (max_level-min_level) / 3
     max_level = min_level + thirdduration
     min_level = min_level - thirdduration
     # Calculate energy for each frequency
     sumlist = []
     for a in range(n_sengen):
-        curdata = testallarray[a * frame_shift:a * frame_shift + FRAME_LEN]
+        curdata = testdata[a * frame_shift:a * frame_shift + FRAME_LEN]
         cursrcLevel = get_rms(curdata)
         if cursrcLevel > min_level and cursrcLevel < max_level:
 
         #if cursrcLevel
             test_energy, upper_freqs = calculate_band_energy(curdata, fs, 40)
             # for i in range(len(test_energy)):
             #     print(upper_freqs[i],test_energy[i])
```

### Comparing `musicAlgLib-1.1.6/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.1.8/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.1.8/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.1.8/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.1.8/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.1.8/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.1.8/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.1.8/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.1.8/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.1.8/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.1.8/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/STI/sti.py` & `musicAlgLib-1.1.8/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.1.8/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/__init__.py` & `musicAlgLib-1.1.8/musicAlgLib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from .VAD_NN.hubconf import silero_vad
 from operator import methodcaller
 from .computeAudioQuality.mainProcess import computeAudioQuality
 
 from ctypes import  *
 
 def compute_music_quality(metrics,testFile=None,refFile=None,outFile=None,audioType=1,
-                         rmsCalsection=None,polqaMode=0,pitchLogMode=1,fineDelaySection=None,rmsSpeechOnly=False,rmsFrameDuration=0.05,rmsShiftDuration=0.05):
+                         calSection=None,polqaMode=0,pitchLogMode=1,fineDelaySection=None,rmsSpeechOnly=False,rmsFrameDuration=0.05,rmsShiftDuration=0.05):
     """
-    :param metrics: ['ALL','POLQA','PEAQ','LOUDNESS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','TOTALRMS','AVERMS','PEAKRMS','STDRMS','MAXRMS','MINRMS','DYNMIC','LRATE','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
+    :param metrics: ['ALL','POLQA','PEAQ','LUFS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','RMS','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
 
     #
     # POLQA 窄带模式  8k  超宽带模式 48k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
     # PEAQ 无采样率限制；WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
     # MATCH 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
     # MUSIC 无采样率限制;WAV/PCM输入;双端输入：ref、test；无时间长度要求；
     # MUSICSTA 无采样率限制,WAV/PCM输入;双端输入：ref、test；无时间长度要求；
@@ -58,15 +58,15 @@
     """
     paraDicts = {
         'metrics':metrics,
         'testFile':testFile,
         'refFile':refFile,
         'outFile':outFile,
         "audioType":audioType,
-        'rmsCalsection':rmsCalsection,
+        'calSection':calSection,
         'polqaMode':polqaMode,
         "pitchLogMode":pitchLogMode,
         "fineDelaySection":fineDelaySection,
         "rmsSpeechOnly":rmsSpeechOnly,
         'rmsFrameDuration' : rmsFrameDuration,
         'rmsShiftDuration' : rmsShiftDuration
     }
```

### Comparing `musicAlgLib-1.1.6/musicAlgLib/commFunction.py` & `musicAlgLib-1.1.8/musicAlgLib/commFunction.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 import numpy as np
 import math
 import librosa
 
 
 import numpy as np
 
+import  soundfile as sf
+
+def get_data_by_sf(file):
+    """
+    """
+    data, rate = sf.read(file)
+    return data,rate,len(data[0])
+
+
+
+
 windowLen = 0.05
 
 class emxArray_real_T(Structure):
  _fields_ = [
           ("pdata", POINTER(c_double)),  # c_byte
           ("psize", POINTER(c_int)),  # c_byte
           ("allocSize", c_int),  #  c_byte
@@ -77,16 +88,16 @@
 
 
 
 def get_data_of_ctypes_(inWaveFile=None,int2float=False,datatype=np.int16):
     wavf = wave.open(inWaveFile, 'rb')
     refChannel,refsamWidth,refsamplerate,refframeCount = wavf.getnchannels(),wavf.getsampwidth(),wavf.getframerate(),wavf.getnframes()
 
-    if (refChannel,refsamWidth) != (1,2):
-        raise TypeError('Different format of ref and test files!')
+    # if (refChannel,refsamWidth) != (1,2):
+    #     raise TypeError('Different format of ref and test files!')
     pcmdata = wavf.readframes(refframeCount)
 
     ref = np.frombuffer(pcmdata,dtype=datatype)
 
     ref = ref.astype(np.float64)
     if int2float:
         ref = ref/32768
@@ -345,20 +356,24 @@
 
     root_path = project_path[:project_path.find("{}\\".format(PROJECT_NAME)) + len("{}\\".format(PROJECT_NAME))]
 
     #print('当前项目名称：{}\r\n当前项目根路径：{}'.format(PROJECT_NAME, root_path))
 
     return root_path
 
+def make_out_file_sf(tarFile,data,fs,datatpye='PCM_16'):
+    """
 
+    """
+    sf.write(tarFile,data,fs,datatpye)
 def make_out_file(tarFile,data,fs,channel,datatpye=np.int16,databitnum=2):
     """
 
     """
-    outData = data.astype(datatpye)
+    outData =np.ndarray([int(num*32767) for num in data])
     wavfile = wave.open(tarFile, 'wb')
     wavfile.setnchannels(channel)
     wavfile.setsampwidth(databitnum)
     wavfile.setframerate(fs)
     wavfile.writeframes(outData.tobytes())
     wavfile.close()
 
@@ -371,18 +386,26 @@
     Returns
     -------
     '''
     frameLen = frameDuration * fs
     frameshift = shiftduration * fs
     nFrames = int((len(data)-frameLen)//frameshift)
     totalRms,cnt = 0,0
+    maxRms,minRms = -199,199
+    rms_list = []
     for a in range(nFrames):
-        totalRms += get_rms(data[int(a*frameshift):int(a*frameshift+frameLen)])
+        curRms = get_rms(data[int(a*frameshift):int(a*frameshift+frameLen)])
+        if curRms > maxRms:
+            maxRms = curRms
+        if curRms < minRms:
+            minRms = curRms
+        totalRms += curRms
         cnt += 1
-    return totalRms/cnt
+        rms_list.append(curRms)
+    return totalRms/cnt,maxRms,minRms,maxRms-minRms,np.std(rms_list, ddof=1)
 
 def get_std_rms(data,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     data
 
@@ -416,28 +439,29 @@
         maxcnt += 1
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         if curRms > threshold:
             validcnt += 1
 
     return validcnt/maxcnt
 
+
+
 def get_rms(records):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    data = records.astype(np.float32).tolist()
-    if len(data) == 0:
+    if len(records) == 0:
         return -99.9
-    rms = math.sqrt(sum([(x/32767) * (x/32767) for x in data])/len(data))
+    rms = math.sqrt(sum([(x) * (x) for x in records])/len(records))
     dBrmsValue = 20*math.log10(rms + 1.0E-6)
     return dBrmsValue
 
 
 def get_peak_rms(records):
     '''
     Parameters
@@ -446,15 +470,15 @@
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
 
     maxdata = max(records)
-    maxRms = 20 * math.log10(maxdata/32767 + 1.0E-6)
+    maxRms = 20 * math.log10(maxdata + 1.0E-6)
     return maxRms
 
 def get_max_rms(records,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     records
```

### Comparing `musicAlgLib-1.1.6/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.1.8/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.1.8/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.1.8/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.1.8/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.6/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.1.8/musicAlgLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.6
+Version: 1.1.8
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.6/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.1.8/musicAlgLib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 musicAlgLib/DLLS/matchsig.so
 musicAlgLib/DLLS/musicStability.dll
 musicAlgLib/DLLS/musicStability.dylib
 musicAlgLib/DLLS/musicStability.so
 musicAlgLib/DLLS/pcc.dll
 musicAlgLib/DLLS/pcc.dylib
 musicAlgLib/DLLS/pcc.so
+musicAlgLib/DLLS/peaqb
 musicAlgLib/DLLS/peaqb.exe
 musicAlgLib/DLLS/silero_vad.jit
 musicAlgLib/DLLS/snr_music.dll
 musicAlgLib/DLLS/snr_music.dylib
 musicAlgLib/DLLS/snr_music.so
 musicAlgLib/DLLs/__init__.py
 musicAlgLib/DynmicRange/__init__.py
```

### Comparing `musicAlgLib-1.1.6/setup.py` & `musicAlgLib-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.1.6',
+    version='1.1.8',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
@@ -91,29 +91,31 @@
     'numpy',
     'wave',
     'matplotlib',
     'datetime',
     'scipy',
     'pystoi',
     'paramiko',
-    'moviepy',
+    'pyloudnorm',
+    'soundfile'
     'torch',
     'torchaudio',
     'librosa',
     'requests',
     'pandas',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     data_files=[
         ('', ['musicAlgLib/DLLS/cygwin1.dll']),
         ('', ['musicAlgLib/DLLS/peaqb.exe']),
+        ('', ['musicAlgLib/DLLS/peaqb']),
         ('', ['musicAlgLib/DLLS/matchsig.dll']),
         ('', ['musicAlgLib/DLLS/snr_music.dll']),
         ('', ['musicAlgLib/DLLS/musicStability.dll']),
         ('', ['musicAlgLib/DLLS/pcc.dll']),
         ('', ['musicAlgLib/DLLS/matchsig.dylib']),
         ('', ['musicAlgLib/DLLS/snr_music.dylib']),
         ('', ['musicAlgLib/DLLS/musicStability.dylib']),
```

