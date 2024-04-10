# Comparing `tmp/tbc_video_export-0.1.0b8.tar.gz` & `tmp/tbc_video_export-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbc_video_export-0.1.0b8.tar", max compression
+gzip compressed data, was "tbc_video_export-0.1.0b9.tar", max compression
```

## Comparing `tbc_video_export-0.1.0b8.tar` & `tbc_video_export-0.1.0b9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    35149 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/LICENSE
--rw-r--r--   0        0        0     3170 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/README.md
--rw-r--r--   0        0        0     3159 2024-02-08 10:56:32.479028 tbc_video_export-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/__init__.py
--rw-r--r--   0        0        0     1735 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/__main__.py
--rw-r--r--   0        0        0      204 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/__init__.py
--rw-r--r--   0        0        0     2235 2024-02-08 10:56:32.479028 tbc_video_export-0.1.0b8/src/tbc_video_export/common/consts.py
--rw-r--r--   0        0        0     3951 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/enums.py
--rw-r--r--   0        0        0     3093 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/exceptions.py
--rw-r--r--   0        0        0     9721 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/file_helper.py
--rw-r--r--   0        0        0     4293 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/tbc_json_helper.py
--rw-r--r--   0        0        0      120 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/__init__.py
--rw-r--r--   0        0        0     5529 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/ansi.py
--rw-r--r--   0        0        0     1112 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/files.py
--rw-r--r--   0        0        0     1305 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/flatlist.py
--rw-r--r--   0        0        0     1624 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/interrupts.py
--rw-r--r--   0        0        0     3440 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/log.py
--rw-r--r--   0        0        0      821 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/strings.py
--rw-r--r--   0        0        0     5142 2024-02-08 10:55:32.291144 tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/win32.py
--rw-r--r--   0        0        0      197 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/config/__init__.py
--rw-r--r--   0        0        0    10176 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/config/config.py
--rw-r--r--   0        0        0     9905 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/config/default.py
--rw-r--r--   0        0        0     1152 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/config/json.py
--rw-r--r--   0        0        0     4760 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/config/profile.py
--rw-r--r--   0        0        0      100 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/opts/__init__.py
--rw-r--r--   0        0        0     3120 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts.py
--rw-r--r--   0        0        0    13610 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_ffmpeg.py
--rw-r--r--   0        0        0     7819 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_ldtools.py
--rw-r--r--   0        0        0    11522 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_parser.py
--rw-r--r--   0        0        0      134 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/__init__.py
--rw-r--r--   0        0        0      290 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/__init__.py
--rw-r--r--   0        0        0     1784 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/export_state.py
--rw-r--r--   0        0        0     3216 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser.py
--rw-r--r--   0        0        0     1773 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_factory.py
--rw-r--r--   0        0        0     1888 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ffmpeg.py
--rw-r--r--   0        0        0     2198 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_chroma_decoder.py
--rw-r--r--   0        0        0     2108 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_dropout_correct.py
--rw-r--r--   0        0        0     1101 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_export_metadata.py
--rw-r--r--   0        0        0     1395 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_process_efm.py
--rw-r--r--   0        0        0     1933 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_process_vbi.py
--rw-r--r--   0        0        0     6322 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/process.py
--rw-r--r--   0        0        0     9976 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/process_handler.py
--rw-r--r--   0        0        0     2115 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/process_state.py
--rw-r--r--   0        0        0     8631 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/progress_handler.py
--rw-r--r--   0        0        0      308 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/__init__.py
--rw-r--r--   0        0        0      419 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/__init__.py
--rw-r--r--   0        0        0     2369 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe.py
--rw-r--r--   0        0        0     1400 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_dummy.py
--rw-r--r--   0        0        0     2588 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_factory.py
--rw-r--r--   0        0        0     9619 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt.py
--rw-r--r--   0        0        0    21062 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt_async.py
--rw-r--r--   0        0        0     3208 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_posix.py
--rw-r--r--   0        0        0     1944 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_os.py
--rw-r--r--   0        0        0     3935 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper.py
--rw-r--r--   0        0        0      530 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_config.py
--rw-r--r--   0        0        0    20040 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ffmpeg.py
--rw-r--r--   0        0        0     8421 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_group.py
--rw-r--r--   0        0        0     9154 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_chroma_decoder.py
--rw-r--r--   0        0        0     3164 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_dropout_correct.py
--rw-r--r--   0        0        0     2177 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_export_metadata.py
--rw-r--r--   0        0        0     2695 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_process_efm.py
--rw-r--r--   0        0        0     2912 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_process_vbi.py
--rw-r--r--   0        0        0     9169 2024-02-08 10:55:32.295144 tbc_video_export-0.1.0b8/src/tbc_video_export/program_state.py
--rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 tbc_video_export-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-08 17:52:18.579122 tbc_video_export-0.1.0b9/LICENSE
+-rw-r--r--   0        0        0     3170 2024-02-08 17:52:18.579122 tbc_video_export-0.1.0b9/README.md
+-rw-r--r--   0        0        0     3159 2024-02-08 17:53:17.855841 tbc_video_export-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/__init__.py
+-rw-r--r--   0        0        0     1735 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/__main__.py
+-rw-r--r--   0        0        0      204 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/__init__.py
+-rw-r--r--   0        0        0     2235 2024-02-08 17:53:17.859841 tbc_video_export-0.1.0b9/src/tbc_video_export/common/consts.py
+-rw-r--r--   0        0        0     3951 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/enums.py
+-rw-r--r--   0        0        0     3093 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/exceptions.py
+-rw-r--r--   0        0        0     9721 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/file_helper.py
+-rw-r--r--   0        0        0     4293 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/tbc_json_helper.py
+-rw-r--r--   0        0        0      120 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/__init__.py
+-rw-r--r--   0        0        0     5529 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/ansi.py
+-rw-r--r--   0        0        0     1112 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/files.py
+-rw-r--r--   0        0        0     1305 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/flatlist.py
+-rw-r--r--   0        0        0     1624 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/interrupts.py
+-rw-r--r--   0        0        0     3440 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/log.py
+-rw-r--r--   0        0        0      821 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/strings.py
+-rw-r--r--   0        0        0     5142 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/win32.py
+-rw-r--r--   0        0        0      197 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/config/__init__.py
+-rw-r--r--   0        0        0    10176 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/config/config.py
+-rw-r--r--   0        0        0     9905 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/config/default.py
+-rw-r--r--   0        0        0     1152 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/config/json.py
+-rw-r--r--   0        0        0     4760 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/config/profile.py
+-rw-r--r--   0        0        0      100 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/opts/__init__.py
+-rw-r--r--   0        0        0     3120 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts.py
+-rw-r--r--   0        0        0    13610 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_ffmpeg.py
+-rw-r--r--   0        0        0     7819 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_ldtools.py
+-rw-r--r--   0        0        0    11522 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_parser.py
+-rw-r--r--   0        0        0      134 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/__init__.py
+-rw-r--r--   0        0        0      290 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/__init__.py
+-rw-r--r--   0        0        0     1784 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/export_state.py
+-rw-r--r--   0        0        0     3216 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser.py
+-rw-r--r--   0        0        0     1773 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_factory.py
+-rw-r--r--   0        0        0     1888 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ffmpeg.py
+-rw-r--r--   0        0        0     2198 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_chroma_decoder.py
+-rw-r--r--   0        0        0     2108 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_dropout_correct.py
+-rw-r--r--   0        0        0     1101 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_export_metadata.py
+-rw-r--r--   0        0        0     1395 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_process_efm.py
+-rw-r--r--   0        0        0     1933 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_process_vbi.py
+-rw-r--r--   0        0        0     6322 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/process.py
+-rw-r--r--   0        0        0     9976 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/process_handler.py
+-rw-r--r--   0        0        0     2115 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/process_state.py
+-rw-r--r--   0        0        0     8631 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/progress_handler.py
+-rw-r--r--   0        0        0      308 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/__init__.py
+-rw-r--r--   0        0        0      419 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/__init__.py
+-rw-r--r--   0        0        0     2369 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe.py
+-rw-r--r--   0        0        0     1400 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_dummy.py
+-rw-r--r--   0        0        0     2588 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_factory.py
+-rw-r--r--   0        0        0     9619 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt.py
+-rw-r--r--   0        0        0    21062 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt_async.py
+-rw-r--r--   0        0        0     3208 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_posix.py
+-rw-r--r--   0        0        0     1944 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_os.py
+-rw-r--r--   0        0        0     3935 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper.py
+-rw-r--r--   0        0        0      530 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_config.py
+-rw-r--r--   0        0        0    20064 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ffmpeg.py
+-rw-r--r--   0        0        0     8421 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_group.py
+-rw-r--r--   0        0        0     9154 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_chroma_decoder.py
+-rw-r--r--   0        0        0     3164 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_dropout_correct.py
+-rw-r--r--   0        0        0     2177 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_export_metadata.py
+-rw-r--r--   0        0        0     2695 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_process_efm.py
+-rw-r--r--   0        0        0     2912 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_process_vbi.py
+-rw-r--r--   0        0        0     9169 2024-02-08 17:52:18.583123 tbc_video_export-0.1.0b9/src/tbc_video_export/program_state.py
+-rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 tbc_video_export-0.1.0b9/PKG-INFO
```

### Comparing `tbc_video_export-0.1.0b8/LICENSE` & `tbc_video_export-0.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/README.md` & `tbc_video_export-0.1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/pyproject.toml` & `tbc_video_export-0.1.0b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tbc-video-export"
-version = "0.1.0b8"
+version = "0.1.0b9"
 description = "Cross-platform tool for exporting S-Video and CVBS-type TBC files to standard video files."
 authors = ["Jitterbug <3130448+JuniorIsAJitterbug@users.noreply.github.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/JuniorIsAJitterbug/tbc-video-export"
 keywords = ["vhs-decode", "ld-decode", "cvbs-decode", "tbc", "rf capture"]
```

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/__main__.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/__main__.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/consts.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if TYPE_CHECKING:
     from typing import Final
 
 _metadata = importlib.metadata.metadata("tbc-video-export")
 
 # substituted by poetry-dynamic-versioning when doing pyinstaller builds
-__version__ = "0.1.0b8"
+__version__ = "0.1.0b9"
 
 APPLICATION_NAME: Final = _metadata["Name"]
 PROJECT_VERSION: Final = _metadata["Version"] if __version__ == "0.0.0" else __version__
 PROJECT_SUMMARY: Final = _metadata["Summary"]
 PROJECT_URL: Final = _metadata["Home-Page"]
 PROJECT_URL_ISSUES: Final = next(
     (
```

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/enums.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/enums.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/exceptions.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/file_helper.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/file_helper.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/tbc_json_helper.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/tbc_json_helper.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/ansi.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/files.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/files.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/flatlist.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/flatlist.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/interrupts.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/log.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/log.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/strings.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/strings.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/common/utils/win32.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/common/utils/win32.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/config/config.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/config/config.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/config/default.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/config/default.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/config/json.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/config/json.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/config/profile.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/config/profile.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_ffmpeg.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_ldtools.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_ldtools.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/opts/opts_parser.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/opts/opts_parser.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/export_state.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/export_state.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_factory.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ffmpeg.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_chroma_decoder.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_chroma_decoder.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_dropout_correct.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_dropout_correct.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_export_metadata.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_export_metadata.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_process_efm.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_process_efm.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/parser/parser_ld_process_vbi.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/parser/parser_ld_process_vbi.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/process.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/process.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/process_handler.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/process_handler.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/process_state.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/process_state.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/progress_handler.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/progress_handler.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_dummy.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_dummy.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_factory.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_factory.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt_async.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_nt_async.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_named_posix.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_named_posix.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/pipe/pipe_os.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/pipe/pipe_os.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_config.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_config.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ffmpeg.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
                 "auto",
                 self._get_color_range_opt(),
                 self._get_input_opts(),
                 self._get_filter_complex_opts(),
                 self._get_map_opts(),
                 self._get_timecode_opt(),
                 self._get_framerate_opt(),
-                self._get_aspect_ratio_opt(),
                 self._get_color_range_opt(),
                 self._get_color_opts(),
                 self._get_format_opts(),
                 self._get_codec_opts(),
                 self._get_metadata_opts(),
                 self._get_output_opt(),
             )
@@ -224,14 +223,17 @@
                 for of in (profile.other_filter for profile in filter_profiles)
                 if of is not None
             )
             if (filter_profiles := self._get_profile().filter_profiles) is not None
             else ""
         )
 
+        if self._state.opts.force_anamorphic or self._state.opts.letterbox:
+            common_filters.append(self._get_widescreen_aspect_ratio_filter())
+
         # override profile colorlevels if set with opt
         if self._state.opts.force_black_level is not None:
             common_filters.append(
                 "colorlevels="
                 f"rimin={self._state.opts.force_black_level[0]}/255:"
                 f"gimin={self._state.opts.force_black_level[1]}/255:"
                 f"bimin={self._state.opts.force_black_level[2]}/255"
@@ -359,25 +361,22 @@
         return FlatList(
             (
                 "-framerate",
                 self._get_framerate(),
             )
         )
 
-    def _get_aspect_ratio_opt(self) -> FlatList | None:
-        """Return opts for aspect ratio."""
-        # do not add AR flag to file, as it must match the rawvideo from chroma on merge
-        if self._is_two_step_luma_mode():
-            return None
-
-        return (
-            FlatList(("-aspect", "16:9"))
-            if (self._state.opts.force_anamorphic or self._state.opts.letterbox)
-            else None
-        )
+    def _get_widescreen_aspect_ratio_filter(self) -> str:
+        """Return filter for widescreen aspect ratio."""
+        match self._state.video_system:
+            case VideoSystem.PAL:
+                return "setsar=512/461:max=1000"
+
+            case VideoSystem.NTSC | VideoSystem.PAL_M:
+                return "setsar=194/171:max=1000"
 
     def _get_color_opts(self) -> FlatList | None:
         """Return opts for color settings."""
         match self._state.video_system:
             case VideoSystem.PAL | VideoSystem.PAL_M:
                 return FlatList(
                     (
```

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_group.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_group.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_chroma_decoder.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_chroma_decoder.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_dropout_correct.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_dropout_correct.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_export_metadata.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_export_metadata.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_process_efm.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_process_efm.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/process/wrapper/wrapper_ld_process_vbi.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/process/wrapper/wrapper_ld_process_vbi.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/src/tbc_video_export/program_state.py` & `tbc_video_export-0.1.0b9/src/tbc_video_export/program_state.py`

 * *Files identical despite different names*

### Comparing `tbc_video_export-0.1.0b8/PKG-INFO` & `tbc_video_export-0.1.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbc-video-export
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: Cross-platform tool for exporting S-Video and CVBS-type TBC files to standard video files.
 Home-page: https://github.com/JuniorIsAJitterbug/tbc-video-export
 License: GPL-3.0-or-later
 Keywords: vhs-decode,ld-decode,cvbs-decode,tbc,rf capture
 Author: Jitterbug
 Author-email: 3130448+JuniorIsAJitterbug@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
```

