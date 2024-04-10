# Comparing `tmp/draive-0.9.2.tar.gz` & `tmp/draive-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draive-0.9.2.tar", last modified: Fri Apr  5 14:01:19 2024, max compression
+gzip compressed data, was "draive-0.9.3.tar", last modified: Wed Apr 10 08:09:57 2024, max compression
```

## Comparing `draive-0.9.2.tar` & `draive-0.9.3.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.296897 draive-0.9.2/
--rw-r--r--   0 miquido    (501) staff       (20)     1063 2024-02-19 11:52:11.000000 draive-0.9.2/LICENSE
--rw-r--r--   0 miquido    (501) staff       (20)     3415 2024-04-05 14:01:19.296635 draive-0.9.2/PKG-INFO
--rw-r--r--   0 miquido    (501) staff       (20)     1135 2024-02-21 15:32:19.000000 draive-0.9.2/README.md
--rw-r--r--   0 miquido    (501) staff       (20)     1540 2024-04-05 13:59:48.000000 draive-0.9.2/pyproject.toml
--rw-r--r--   0 miquido    (501) staff       (20)       38 2024-04-05 14:01:19.296943 draive-0.9.2/setup.cfg
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.280512 draive-0.9.2/src/
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.282483 draive-0.9.2/src/draive/
--rw-r--r--   0 miquido    (501) staff       (20)     4029 2024-04-05 12:31:51.000000 draive-0.9.2/src/draive/__init__.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.283959 draive-0.9.2/src/draive/conversation/
--rw-r--r--   0 miquido    (501) staff       (20)      601 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/conversation/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     2630 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/conversation/call.py
--rw-r--r--   0 miquido    (501) staff       (20)     1950 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/conversation/completion.py
--rw-r--r--   0 miquido    (501) staff       (20)     4811 2024-04-03 11:11:38.000000 draive-0.9.2/src/draive/conversation/lmm.py
--rw-r--r--   0 miquido    (501) staff       (20)      432 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/conversation/message.py
--rw-r--r--   0 miquido    (501) staff       (20)      502 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/conversation/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.284635 draive-0.9.2/src/draive/embedding/
--rw-r--r--   0 miquido    (501) staff       (20)      266 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/embedding/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      333 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/embedding/call.py
--rw-r--r--   0 miquido    (501) staff       (20)      255 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/embedding/embedded.py
--rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/embedding/embedder.py
--rw-r--r--   0 miquido    (501) staff       (20)      166 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/embedding/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.284761 draive-0.9.2/src/draive/generation/
--rw-r--r--   0 miquido    (501) staff       (20)      461 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/generation/__init__.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.285259 draive-0.9.2/src/draive/generation/image/
--rw-r--r--   0 miquido    (501) staff       (20)      257 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/generation/image/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      331 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/generation/image/call.py
--rw-r--r--   0 miquido    (501) staff       (20)      286 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/generation/image/generator.py
--rw-r--r--   0 miquido    (501) staff       (20)      191 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/generation/image/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.285922 draive-0.9.2/src/draive/generation/model/
--rw-r--r--   0 miquido    (501) staff       (20)      257 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/model/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      849 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/model/call.py
--rw-r--r--   0 miquido    (501) staff       (20)      652 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/model/generator.py
--rw-r--r--   0 miquido    (501) staff       (20)     2055 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/generation/model/lmm.py
--rw-r--r--   0 miquido    (501) staff       (20)      337 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/model/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.286544 draive-0.9.2/src/draive/generation/text/
--rw-r--r--   0 miquido    (501) staff       (20)      248 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/text/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      688 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/text/call.py
--rw-r--r--   0 miquido    (501) staff       (20)      509 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/text/generator.py
--rw-r--r--   0 miquido    (501) staff       (20)     1567 2024-04-03 11:11:38.000000 draive-0.9.2/src/draive/generation/text/lmm.py
--rw-r--r--   0 miquido    (501) staff       (20)      329 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/generation/text/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.287049 draive-0.9.2/src/draive/helpers/
--rw-r--r--   0 miquido    (501) staff       (20)      343 2024-03-07 13:44:53.000000 draive-0.9.2/src/draive/helpers/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     3011 2024-03-25 15:25:45.000000 draive-0.9.2/src/draive/helpers/env.py
--rw-r--r--   0 miquido    (501) staff       (20)     1657 2024-03-25 15:25:45.000000 draive-0.9.2/src/draive/helpers/logs.py
--rw-r--r--   0 miquido    (501) staff       (20)      446 2024-03-25 09:58:05.000000 draive-0.9.2/src/draive/helpers/split_sequence.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.287801 draive-0.9.2/src/draive/lmm/
--rw-r--r--   0 miquido    (501) staff       (20)      454 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/lmm/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     1777 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/lmm/call.py
--rw-r--r--   0 miquido    (501) staff       (20)     1540 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/lmm/completion.py
--rw-r--r--   0 miquido    (501) staff       (20)     1492 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/lmm/message.py
--rw-r--r--   0 miquido    (501) staff       (20)      166 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/lmm/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.288806 draive-0.9.2/src/draive/mistral/
--rw-r--r--   0 miquido    (501) staff       (20)      320 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/mistral/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     2809 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/mistral/chat_response.py
--rw-r--r--   0 miquido    (501) staff       (20)     4681 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/mistral/chat_stream.py
--rw-r--r--   0 miquido    (501) staff       (20)     3134 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/mistral/chat_tools.py
--rw-r--r--   0 miquido    (501) staff       (20)     3281 2024-04-05 10:49:51.000000 draive-0.9.2/src/draive/mistral/client.py
--rw-r--r--   0 miquido    (501) staff       (20)     1752 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/mistral/config.py
--rw-r--r--   0 miquido    (501) staff       (20)       84 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/mistral/errors.py
--rw-r--r--   0 miquido    (501) staff       (20)     7713 2024-04-03 11:11:38.000000 draive-0.9.2/src/draive/mistral/lmm.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.290257 draive-0.9.2/src/draive/openai/
--rw-r--r--   0 miquido    (501) staff       (20)      692 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/openai/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     2857 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/openai/chat_response.py
--rw-r--r--   0 miquido    (501) staff       (20)     4483 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/openai/chat_stream.py
--rw-r--r--   0 miquido    (501) staff       (20)     4109 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/openai/chat_tools.py
--rw-r--r--   0 miquido    (501) staff       (20)     7165 2024-04-05 10:49:51.000000 draive-0.9.2/src/draive/openai/client.py
--rw-r--r--   0 miquido    (501) staff       (20)     3929 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/openai/config.py
--rw-r--r--   0 miquido    (501) staff       (20)      939 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/openai/embedding.py
--rw-r--r--   0 miquido    (501) staff       (20)       82 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/openai/errors.py
--rw-r--r--   0 miquido    (501) staff       (20)     1018 2024-04-02 10:34:03.000000 draive-0.9.2/src/draive/openai/images.py
--rw-r--r--   0 miquido    (501) staff       (20)     8460 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/openai/lmm.py
--rw-r--r--   0 miquido    (501) staff       (20)      478 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/openai/tokenization.py
--rw-r--r--   0 miquido    (501) staff       (20)        0 2024-02-22 12:12:34.000000 draive-0.9.2/src/draive/py.typed
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.291027 draive-0.9.2/src/draive/scope/
--rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/scope/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)    11066 2024-04-05 13:02:00.000000 draive-0.9.2/src/draive/scope/access.py
--rw-r--r--   0 miquido    (501) staff       (20)     1687 2024-03-27 10:16:01.000000 draive-0.9.2/src/draive/scope/dependencies.py
--rw-r--r--   0 miquido    (501) staff       (20)      244 2024-02-19 11:44:30.000000 draive-0.9.2/src/draive/scope/errors.py
--rw-r--r--   0 miquido    (501) staff       (20)    13451 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/scope/metrics.py
--rw-r--r--   0 miquido    (501) staff       (20)     1537 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/scope/state.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.291559 draive-0.9.2/src/draive/similarity/
--rw-r--r--   0 miquido    (501) staff       (20)      156 2024-02-21 14:35:24.000000 draive-0.9.2/src/draive/similarity/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      816 2024-02-19 15:31:53.000000 draive-0.9.2/src/draive/similarity/cosine.py
--rw-r--r--   0 miquido    (501) staff       (20)     2211 2024-03-04 10:44:43.000000 draive-0.9.2/src/draive/similarity/mmr.py
--rw-r--r--   0 miquido    (501) staff       (20)      999 2024-03-04 10:44:43.000000 draive-0.9.2/src/draive/similarity/similarity.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.291823 draive-0.9.2/src/draive/splitters/
--rw-r--r--   0 miquido    (501) staff       (20)       79 2024-02-21 14:35:24.000000 draive-0.9.2/src/draive/splitters/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     4152 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/splitters/basic.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.292305 draive-0.9.2/src/draive/tokenization/
--rw-r--r--   0 miquido    (501) staff       (20)      274 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/tokenization/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      347 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/tokenization/call.py
--rw-r--r--   0 miquido    (501) staff       (20)      179 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/tokenization/state.py
--rw-r--r--   0 miquido    (501) staff       (20)      218 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/tokenization/text.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.293209 draive-0.9.2/src/draive/tools/
--rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/tools/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)       78 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/tools/errors.py
--rw-r--r--   0 miquido    (501) staff       (20)      735 2024-04-05 12:31:44.000000 draive-0.9.2/src/draive/tools/state.py
--rw-r--r--   0 miquido    (501) staff       (20)     5081 2024-04-05 12:31:45.000000 draive-0.9.2/src/draive/tools/tool.py
--rw-r--r--   0 miquido    (501) staff       (20)     1414 2024-04-04 12:45:04.000000 draive-0.9.2/src/draive/tools/toolbox.py
--rw-r--r--   0 miquido    (501) staff       (20)      310 2024-04-05 12:31:46.000000 draive-0.9.2/src/draive/tools/update.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.294643 draive-0.9.2/src/draive/types/
--rw-r--r--   0 miquido    (501) staff       (20)     1121 2024-04-05 12:31:48.000000 draive-0.9.2/src/draive/types/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)      271 2024-03-20 13:44:10.000000 draive-0.9.2/src/draive/types/images.py
--rw-r--r--   0 miquido    (501) staff       (20)     1300 2024-04-05 13:02:01.000000 draive-0.9.2/src/draive/types/memory.py
--rw-r--r--   0 miquido    (501) staff       (20)      485 2024-03-27 09:57:51.000000 draive-0.9.2/src/draive/types/missing.py
--rw-r--r--   0 miquido    (501) staff       (20)     1265 2024-04-05 13:38:20.000000 draive-0.9.2/src/draive/types/model.py
--rw-r--r--   0 miquido    (501) staff       (20)      201 2024-04-04 07:45:35.000000 draive-0.9.2/src/draive/types/multimodal.py
--rw-r--r--   0 miquido    (501) staff       (20)    29172 2024-04-05 13:02:01.000000 draive-0.9.2/src/draive/types/parameters.py
--rw-r--r--   0 miquido    (501) staff       (20)    12036 2024-04-05 12:31:48.000000 draive-0.9.2/src/draive/types/specification.py
--rw-r--r--   0 miquido    (501) staff       (20)      358 2024-03-27 11:38:48.000000 draive-0.9.2/src/draive/types/state.py
--rw-r--r--   0 miquido    (501) staff       (20)      354 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/types/updates.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.295364 draive-0.9.2/src/draive/utils/
--rw-r--r--   0 miquido    (501) staff       (20)      351 2024-03-25 15:25:45.000000 draive-0.9.2/src/draive/utils/__init__.py
--rw-r--r--   0 miquido    (501) staff       (20)     5142 2024-04-05 13:02:03.000000 draive-0.9.2/src/draive/utils/cache.py
--rw-r--r--   0 miquido    (501) staff       (20)     3451 2024-04-05 13:02:03.000000 draive-0.9.2/src/draive/utils/early_exit.py
--rw-r--r--   0 miquido    (501) staff       (20)     4633 2024-04-05 13:02:03.000000 draive-0.9.2/src/draive/utils/retry.py
--rw-r--r--   0 miquido    (501) staff       (20)     3082 2024-04-02 08:57:56.000000 draive-0.9.2/src/draive/utils/stream.py
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.295945 draive-0.9.2/src/draive.egg-info/
--rw-r--r--   0 miquido    (501) staff       (20)     3415 2024-04-05 14:01:19.000000 draive-0.9.2/src/draive.egg-info/PKG-INFO
--rw-r--r--   0 miquido    (501) staff       (20)     3144 2024-04-05 14:01:19.000000 draive-0.9.2/src/draive.egg-info/SOURCES.txt
--rw-r--r--   0 miquido    (501) staff       (20)        1 2024-04-05 14:01:19.000000 draive-0.9.2/src/draive.egg-info/dependency_links.txt
--rw-r--r--   0 miquido    (501) staff       (20)      210 2024-04-05 14:01:19.000000 draive-0.9.2/src/draive.egg-info/requires.txt
--rw-r--r--   0 miquido    (501) staff       (20)        7 2024-04-05 14:01:19.000000 draive-0.9.2/src/draive.egg-info/top_level.txt
-drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-05 14:01:19.295737 draive-0.9.2/tests/
--rw-r--r--   0 miquido    (501) staff       (20)     1669 2024-03-27 10:16:01.000000 draive-0.9.2/tests/test_metrics.py
--rw-r--r--   0 miquido    (501) staff       (20)     1329 2024-03-27 09:57:51.000000 draive-0.9.2/tests/test_model.py
--rw-r--r--   0 miquido    (501) staff       (20)     1501 2024-04-04 06:59:25.000000 draive-0.9.2/tests/test_state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.953258 draive-0.9.3/
+-rw-r--r--   0 miquido    (501) staff       (20)     1063 2024-02-19 11:52:11.000000 draive-0.9.3/LICENSE
+-rw-r--r--   0 miquido    (501) staff       (20)     3349 2024-04-10 08:09:57.952994 draive-0.9.3/PKG-INFO
+-rw-r--r--   0 miquido    (501) staff       (20)     1135 2024-02-21 15:32:19.000000 draive-0.9.3/README.md
+-rw-r--r--   0 miquido    (501) staff       (20)     1498 2024-04-10 08:09:36.000000 draive-0.9.3/pyproject.toml
+-rw-r--r--   0 miquido    (501) staff       (20)       38 2024-04-10 08:09:57.953305 draive-0.9.3/setup.cfg
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.936288 draive-0.9.3/src/
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.938037 draive-0.9.3/src/draive/
+-rw-r--r--   0 miquido    (501) staff       (20)     4137 2024-04-10 08:09:36.000000 draive-0.9.3/src/draive/__init__.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.939405 draive-0.9.3/src/draive/conversation/
+-rw-r--r--   0 miquido    (501) staff       (20)      601 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/conversation/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2630 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/conversation/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1950 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/conversation/completion.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4811 2024-04-03 11:11:38.000000 draive-0.9.3/src/draive/conversation/lmm.py
+-rw-r--r--   0 miquido    (501) staff       (20)      432 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/conversation/message.py
+-rw-r--r--   0 miquido    (501) staff       (20)      502 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/conversation/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.940024 draive-0.9.3/src/draive/embedding/
+-rw-r--r--   0 miquido    (501) staff       (20)      266 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/embedding/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      333 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/embedding/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)      255 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/embedding/embedded.py
+-rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/embedding/embedder.py
+-rw-r--r--   0 miquido    (501) staff       (20)      166 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/embedding/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.940146 draive-0.9.3/src/draive/generation/
+-rw-r--r--   0 miquido    (501) staff       (20)      461 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/generation/__init__.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.940665 draive-0.9.3/src/draive/generation/image/
+-rw-r--r--   0 miquido    (501) staff       (20)      257 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/generation/image/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      331 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/generation/image/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)      286 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/generation/image/generator.py
+-rw-r--r--   0 miquido    (501) staff       (20)      191 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/generation/image/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.941335 draive-0.9.3/src/draive/generation/model/
+-rw-r--r--   0 miquido    (501) staff       (20)      257 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/model/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      849 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/model/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)      652 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/model/generator.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2055 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/generation/model/lmm.py
+-rw-r--r--   0 miquido    (501) staff       (20)      337 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/model/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.942031 draive-0.9.3/src/draive/generation/text/
+-rw-r--r--   0 miquido    (501) staff       (20)      248 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/text/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      688 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/text/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)      509 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/text/generator.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1567 2024-04-03 11:11:38.000000 draive-0.9.3/src/draive/generation/text/lmm.py
+-rw-r--r--   0 miquido    (501) staff       (20)      329 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/generation/text/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.942553 draive-0.9.3/src/draive/helpers/
+-rw-r--r--   0 miquido    (501) staff       (20)      343 2024-03-07 13:44:53.000000 draive-0.9.3/src/draive/helpers/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     3011 2024-03-25 15:25:45.000000 draive-0.9.3/src/draive/helpers/env.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1657 2024-03-25 15:25:45.000000 draive-0.9.3/src/draive/helpers/logs.py
+-rw-r--r--   0 miquido    (501) staff       (20)      446 2024-03-25 09:58:05.000000 draive-0.9.3/src/draive/helpers/split_sequence.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.943169 draive-0.9.3/src/draive/lmm/
+-rw-r--r--   0 miquido    (501) staff       (20)      454 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/lmm/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1777 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/lmm/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1540 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/lmm/completion.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1492 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/lmm/message.py
+-rw-r--r--   0 miquido    (501) staff       (20)      166 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/lmm/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.944858 draive-0.9.3/src/draive/mistral/
+-rw-r--r--   0 miquido    (501) staff       (20)      456 2024-04-10 08:09:36.000000 draive-0.9.3/src/draive/mistral/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2809 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/mistral/chat_response.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4681 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/mistral/chat_stream.py
+-rw-r--r--   0 miquido    (501) staff       (20)     3134 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/mistral/chat_tools.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4389 2024-04-10 08:09:36.000000 draive-0.9.3/src/draive/mistral/client.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2149 2024-04-10 08:09:36.000000 draive-0.9.3/src/draive/mistral/config.py
+-rw-r--r--   0 miquido    (501) staff       (20)      948 2024-04-10 08:09:36.000000 draive-0.9.3/src/draive/mistral/embedding.py
+-rw-r--r--   0 miquido    (501) staff       (20)       84 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/mistral/errors.py
+-rw-r--r--   0 miquido    (501) staff       (20)     7713 2024-04-03 11:11:38.000000 draive-0.9.3/src/draive/mistral/lmm.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.946357 draive-0.9.3/src/draive/openai/
+-rw-r--r--   0 miquido    (501) staff       (20)      692 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/openai/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2857 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/openai/chat_response.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4483 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/openai/chat_stream.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4109 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/openai/chat_tools.py
+-rw-r--r--   0 miquido    (501) staff       (20)     7165 2024-04-05 10:49:51.000000 draive-0.9.3/src/draive/openai/client.py
+-rw-r--r--   0 miquido    (501) staff       (20)     3929 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/openai/config.py
+-rw-r--r--   0 miquido    (501) staff       (20)      939 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/openai/embedding.py
+-rw-r--r--   0 miquido    (501) staff       (20)       82 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/openai/errors.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1018 2024-04-02 10:34:03.000000 draive-0.9.3/src/draive/openai/images.py
+-rw-r--r--   0 miquido    (501) staff       (20)     8460 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/openai/lmm.py
+-rw-r--r--   0 miquido    (501) staff       (20)      478 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/openai/tokenization.py
+-rw-r--r--   0 miquido    (501) staff       (20)        0 2024-02-22 12:12:34.000000 draive-0.9.3/src/draive/py.typed
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.947192 draive-0.9.3/src/draive/scope/
+-rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/scope/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)    11066 2024-04-05 13:02:00.000000 draive-0.9.3/src/draive/scope/access.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1687 2024-03-27 10:16:01.000000 draive-0.9.3/src/draive/scope/dependencies.py
+-rw-r--r--   0 miquido    (501) staff       (20)      244 2024-02-19 11:44:30.000000 draive-0.9.3/src/draive/scope/errors.py
+-rw-r--r--   0 miquido    (501) staff       (20)    13451 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/scope/metrics.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1537 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/scope/state.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.947719 draive-0.9.3/src/draive/similarity/
+-rw-r--r--   0 miquido    (501) staff       (20)      156 2024-02-21 14:35:24.000000 draive-0.9.3/src/draive/similarity/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      816 2024-02-19 15:31:53.000000 draive-0.9.3/src/draive/similarity/cosine.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2211 2024-03-04 10:44:43.000000 draive-0.9.3/src/draive/similarity/mmr.py
+-rw-r--r--   0 miquido    (501) staff       (20)      999 2024-03-04 10:44:43.000000 draive-0.9.3/src/draive/similarity/similarity.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.947947 draive-0.9.3/src/draive/splitters/
+-rw-r--r--   0 miquido    (501) staff       (20)       79 2024-02-21 14:35:24.000000 draive-0.9.3/src/draive/splitters/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4152 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/splitters/basic.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.948479 draive-0.9.3/src/draive/tokenization/
+-rw-r--r--   0 miquido    (501) staff       (20)      274 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/tokenization/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      347 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/tokenization/call.py
+-rw-r--r--   0 miquido    (501) staff       (20)      179 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/tokenization/state.py
+-rw-r--r--   0 miquido    (501) staff       (20)      218 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/tokenization/text.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.949205 draive-0.9.3/src/draive/tools/
+-rw-r--r--   0 miquido    (501) staff       (20)      441 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/tools/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)       78 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/tools/errors.py
+-rw-r--r--   0 miquido    (501) staff       (20)      735 2024-04-05 12:31:44.000000 draive-0.9.3/src/draive/tools/state.py
+-rw-r--r--   0 miquido    (501) staff       (20)     5081 2024-04-05 12:31:45.000000 draive-0.9.3/src/draive/tools/tool.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1414 2024-04-04 12:45:04.000000 draive-0.9.3/src/draive/tools/toolbox.py
+-rw-r--r--   0 miquido    (501) staff       (20)      310 2024-04-05 12:31:46.000000 draive-0.9.3/src/draive/tools/update.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.950426 draive-0.9.3/src/draive/types/
+-rw-r--r--   0 miquido    (501) staff       (20)     1121 2024-04-05 12:31:48.000000 draive-0.9.3/src/draive/types/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)      271 2024-03-20 13:44:10.000000 draive-0.9.3/src/draive/types/images.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1300 2024-04-05 13:02:01.000000 draive-0.9.3/src/draive/types/memory.py
+-rw-r--r--   0 miquido    (501) staff       (20)      485 2024-03-27 09:57:51.000000 draive-0.9.3/src/draive/types/missing.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1772 2024-04-09 07:26:23.000000 draive-0.9.3/src/draive/types/model.py
+-rw-r--r--   0 miquido    (501) staff       (20)      201 2024-04-04 07:45:35.000000 draive-0.9.3/src/draive/types/multimodal.py
+-rw-r--r--   0 miquido    (501) staff       (20)    32096 2024-04-09 07:26:23.000000 draive-0.9.3/src/draive/types/parameters.py
+-rw-r--r--   0 miquido    (501) staff       (20)    12454 2024-04-09 07:26:23.000000 draive-0.9.3/src/draive/types/specification.py
+-rw-r--r--   0 miquido    (501) staff       (20)      358 2024-03-27 11:38:48.000000 draive-0.9.3/src/draive/types/state.py
+-rw-r--r--   0 miquido    (501) staff       (20)      354 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/types/updates.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.951026 draive-0.9.3/src/draive/utils/
+-rw-r--r--   0 miquido    (501) staff       (20)      351 2024-03-25 15:25:45.000000 draive-0.9.3/src/draive/utils/__init__.py
+-rw-r--r--   0 miquido    (501) staff       (20)     5142 2024-04-05 13:02:03.000000 draive-0.9.3/src/draive/utils/cache.py
+-rw-r--r--   0 miquido    (501) staff       (20)     3451 2024-04-05 13:02:03.000000 draive-0.9.3/src/draive/utils/early_exit.py
+-rw-r--r--   0 miquido    (501) staff       (20)     4633 2024-04-05 13:02:03.000000 draive-0.9.3/src/draive/utils/retry.py
+-rw-r--r--   0 miquido    (501) staff       (20)     3082 2024-04-02 08:57:56.000000 draive-0.9.3/src/draive/utils/stream.py
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.952349 draive-0.9.3/src/draive.egg-info/
+-rw-r--r--   0 miquido    (501) staff       (20)     3349 2024-04-10 08:09:57.000000 draive-0.9.3/src/draive.egg-info/PKG-INFO
+-rw-r--r--   0 miquido    (501) staff       (20)     3176 2024-04-10 08:09:57.000000 draive-0.9.3/src/draive.egg-info/SOURCES.txt
+-rw-r--r--   0 miquido    (501) staff       (20)        1 2024-04-10 08:09:57.000000 draive-0.9.3/src/draive.egg-info/dependency_links.txt
+-rw-r--r--   0 miquido    (501) staff       (20)      175 2024-04-10 08:09:57.000000 draive-0.9.3/src/draive.egg-info/requires.txt
+-rw-r--r--   0 miquido    (501) staff       (20)        7 2024-04-10 08:09:57.000000 draive-0.9.3/src/draive.egg-info/top_level.txt
+drwxr-xr-x   0 miquido    (501) staff       (20)        0 2024-04-10 08:09:57.951918 draive-0.9.3/tests/
+-rw-r--r--   0 miquido    (501) staff       (20)     1669 2024-03-27 10:16:01.000000 draive-0.9.3/tests/test_metrics.py
+-rw-r--r--   0 miquido    (501) staff       (20)     2233 2024-04-09 07:26:23.000000 draive-0.9.3/tests/test_model.py
+-rw-r--r--   0 miquido    (501) staff       (20)     1501 2024-04-04 06:59:25.000000 draive-0.9.3/tests/test_state.py
```

### Comparing `draive-0.9.2/LICENSE` & `draive-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/PKG-INFO` & `draive-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draive
-Version: 0.9.2
+Version: 0.9.3
 Maintainer-email: Kacper Kaliński <kacper.kalinski@miquido.com>
 License: MIT License
         
         Copyright (c) 2024 Miquido
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,28 +29,27 @@
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.14
-Requires-Dist: mistralai~=0.1.3
+Requires-Dist: openai~=1.16
+Requires-Dist: mistralai~=0.1
 Requires-Dist: numpy~=1.26
-Requires-Dist: tiktoken~=0.6.0
+Requires-Dist: tiktoken~=0.6
 Requires-Dist: pydantic~=2.6
-Requires-Dist: httpx~=0.25.0
+Requires-Dist: httpx~=0.25
 Provides-Extra: dev
-Requires-Dist: ruff~=0.2.0; extra == "dev"
-Requires-Dist: pyright~=1.1.0; extra == "dev"
-Requires-Dist: bandit~=1.7.0; extra == "dev"
-Requires-Dist: pytest~=7.4.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: ruff~=0.3.0; extra == "dev"
+Requires-Dist: pyright~=1.1; extra == "dev"
+Requires-Dist: bandit~=1.7; extra == "dev"
+Requires-Dist: pytest~=7.4; extra == "dev"
+Requires-Dist: pytest-cov~=4.1; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
-Requires-Dist: python-dotenv~=1.0.0; extra == "dev"
 
 # draive
 
 Framework for building AI oriented applications.
 
 ## License
```

### Comparing `draive-0.9.2/README.md` & `draive-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/pyproject.toml` & `draive-0.9.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "draive"
-version = "0.9.2"
+version = "0.9.3"
 readme = "README.md"
 maintainers = [
   {name = "Kacper Kaliński", email = "kacper.kalinski@miquido.com"}
 ]
 requires-python = ">=3.11"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 license = {file = "LICENSE"}
 dependencies = [
-    "openai~=1.14",
-    "mistralai~=0.1.3",
+    "openai~=1.16",
+    "mistralai~=0.1",
     "numpy~=1.26",
-    "tiktoken~=0.6.0",
+    "tiktoken~=0.6",
     "pydantic~=2.6",
-    "httpx~=0.25.0",
+    "httpx~=0.25",
 ]
 
 [project.urls]
 Homepage = "https://miquido.com"
 Repository = "https://github.com/miquido/draive.git"
 
 [project.optional-dependencies]
 dev = [
-    "ruff~=0.2.0",
-    "pyright~=1.1.0",
-    "bandit~=1.7.0",
-    "pytest~=7.4.0",
-    "pytest-cov~=4.1.0",
+    "ruff~=0.3.0",
+    "pyright~=1.1",
+    "bandit~=1.7",
+    "pytest~=7.4",
+    "pytest-cov~=4.1",
     "pytest-asyncio~=0.23.0",
-    "python-dotenv~=1.0.0",
 ]
 
 [tool.ruff]
 target-version = "py311"
 line-length = 100
 extend-exclude = [".venv", ".git", ".cache"]
 lint.select = ["E", "F", "A", "I", "B", "PL", "W", "C", "RUF", "UP"]
```

### Comparing `draive-0.9.2/src/draive/__init__.py` & `draive-0.9.3/src/draive/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     LMMCompletionStream,
     LMMCompletionStreamingUpdate,
     lmm_completion,
 )
 from draive.mistral import (
     MistralChatConfig,
     MistralClient,
+    MistralEmbeddingConfig,
     MistralException,
+    mistral_embed_text,
     mistral_lmm_completion,
 )
 from draive.openai import (
     OpenAIChatConfig,
     OpenAIClient,
     OpenAIEmbeddingConfig,
     OpenAIException,
@@ -178,9 +180,11 @@
     "openai_tokenize_text",
     "openai_embed_text",
     "openai_lmm_completion",
     "openai_generate_image",
     "MistralException",
     "MistralClient",
     "MistralChatConfig",
+    "MistralEmbeddingConfig",
     "mistral_lmm_completion",
+    "mistral_embed_text",
 ]
```

### Comparing `draive-0.9.2/src/draive/conversation/__init__.py` & `draive-0.9.3/src/draive/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/conversation/call.py` & `draive-0.9.3/src/draive/conversation/call.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/conversation/completion.py` & `draive-0.9.3/src/draive/conversation/completion.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/conversation/lmm.py` & `draive-0.9.3/src/draive/conversation/lmm.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/generation/model/call.py` & `draive-0.9.3/src/draive/generation/model/call.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/generation/model/generator.py` & `draive-0.9.3/src/draive/generation/model/generator.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/generation/model/lmm.py` & `draive-0.9.3/src/draive/generation/model/lmm.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/generation/text/call.py` & `draive-0.9.3/src/draive/generation/text/call.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/generation/text/lmm.py` & `draive-0.9.3/src/draive/generation/text/lmm.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/helpers/env.py` & `draive-0.9.3/src/draive/helpers/env.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/helpers/logs.py` & `draive-0.9.3/src/draive/helpers/logs.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/lmm/call.py` & `draive-0.9.3/src/draive/lmm/call.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/lmm/completion.py` & `draive-0.9.3/src/draive/lmm/completion.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/lmm/message.py` & `draive-0.9.3/src/draive/lmm/message.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/mistral/chat_response.py` & `draive-0.9.3/src/draive/mistral/chat_response.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/mistral/chat_stream.py` & `draive-0.9.3/src/draive/mistral/chat_stream.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/mistral/chat_tools.py` & `draive-0.9.3/src/draive/mistral/chat_tools.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/mistral/config.py` & `draive-0.9.3/src/draive/mistral/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Literal, TypedDict
 
 from draive.helpers import getenv_float, getenv_int, getenv_str
 from draive.types import State
 
 __all__ = [
     "MistralChatConfig",
+    "MistralEmbeddingConfig",
 ]
 
 
 class ResponseFormat(TypedDict):
     type: Literal["text", "json_object"]
 
 
@@ -50,7 +51,21 @@
         if self.response_format:
             result += f"\n+ response_format: {self.response_format.get('type', 'text')}"
         if self.timeout:
             result += f"\n+ timeout: {self.timeout}"
         result += f"\n+ recursion_limit: {self.recursion_limit}"
 
         return result.replace("\n", "\n|   ")
+
+
+class MistralEmbeddingConfig(State):
+    model: (Literal["mistral-embed"] | str) = "mistral-embed"
+    batch_size: int = 32
+
+    def metric_summary(
+        self,
+        trimmed: bool,
+    ) -> str:
+        result: str = f"mistral config\n+ model: {self.model}"
+        result += f"\n+ batch_size: {self.batch_size}"
+
+        return result.replace("\n", "\n|   ")
```

### Comparing `draive-0.9.2/src/draive/mistral/lmm.py` & `draive-0.9.3/src/draive/mistral/lmm.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/__init__.py` & `draive-0.9.3/src/draive/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/chat_response.py` & `draive-0.9.3/src/draive/openai/chat_response.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/chat_stream.py` & `draive-0.9.3/src/draive/openai/chat_stream.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/chat_tools.py` & `draive-0.9.3/src/draive/openai/chat_tools.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/client.py` & `draive-0.9.3/src/draive/openai/client.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/config.py` & `draive-0.9.3/src/draive/openai/config.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/embedding.py` & `draive-0.9.3/src/draive/openai/embedding.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/images.py` & `draive-0.9.3/src/draive/openai/images.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/openai/lmm.py` & `draive-0.9.3/src/draive/openai/lmm.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/scope/access.py` & `draive-0.9.3/src/draive/scope/access.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/scope/dependencies.py` & `draive-0.9.3/src/draive/scope/dependencies.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/scope/metrics.py` & `draive-0.9.3/src/draive/scope/metrics.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/scope/state.py` & `draive-0.9.3/src/draive/scope/state.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/similarity/cosine.py` & `draive-0.9.3/src/draive/similarity/cosine.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/similarity/mmr.py` & `draive-0.9.3/src/draive/similarity/mmr.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/similarity/similarity.py` & `draive-0.9.3/src/draive/similarity/similarity.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/splitters/basic.py` & `draive-0.9.3/src/draive/splitters/basic.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/tools/state.py` & `draive-0.9.3/src/draive/tools/state.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/tools/tool.py` & `draive-0.9.3/src/draive/tools/tool.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/tools/toolbox.py` & `draive-0.9.3/src/draive/tools/toolbox.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/types/__init__.py` & `draive-0.9.3/src/draive/types/__init__.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/types/memory.py` & `draive-0.9.3/src/draive/types/memory.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/types/parameters.py` & `draive-0.9.3/src/draive/types/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import builtins
+import datetime
 import inspect
 import types
 import typing
+import uuid
 from collections import abc as collections_abc
 from collections.abc import Callable, Iterable, Iterator
 from dataclasses import (
     _MISSING_TYPE as DATACLASS_MISSING_TYPE,  # pyright: ignore[reportPrivateUsage]
 )
 from dataclasses import MISSING as DATACLASS_MISSING
 from dataclasses import Field as DataclassField
@@ -663,14 +665,82 @@
                     if value in options:
                         return value
                     else:
                         raise TypeError("Invalid value", annotation, value)
 
             return validated_literal
 
+        case uuid.UUID:
+            if validate := additional:
+
+                def validated_uuid(value: Any) -> Any:
+                    if isinstance(value, uuid.UUID):
+                        validate(value)
+                        return value
+                    elif isinstance(value, str):
+                        uuid_value: uuid.UUID = uuid.UUID(hex=value)
+                        validate(uuid_value)
+                        return uuid_value
+                    elif isinstance(value, bytes):
+                        uuid_value: uuid.UUID = uuid.UUID(bytes=value)
+                        validate(uuid_value)
+                        return uuid_value
+                    else:
+                        raise TypeError("Invalid value", annotation, value)
+            else:
+
+                def validated_uuid(value: Any) -> Any:
+                    if isinstance(value, uuid.UUID):
+                        return value
+                    elif isinstance(value, str):
+                        return uuid.UUID(hex=value)
+                    elif isinstance(value, bytes):
+                        return uuid.UUID(bytes=value)
+                    else:
+                        raise TypeError("Invalid value", annotation, value)
+
+            return validated_uuid
+
+        case datetime.datetime:
+            if validate := additional:
+
+                def validated_datetime(value: Any) -> Any:
+                    if isinstance(value, datetime.datetime):
+                        validate(value)
+                        return value
+                    elif isinstance(value, str):
+                        datetime_value: datetime.datetime = datetime.datetime.fromisoformat(value)
+                        validate(datetime_value)
+                        return datetime_value
+                    elif isinstance(value, float | int):
+                        datetime_value: datetime.datetime = datetime.datetime.fromtimestamp(
+                            value,
+                            datetime.UTC,
+                        )
+                        validate(datetime_value)
+                        return datetime_value
+                    else:
+                        raise TypeError("Invalid value", annotation, value)
+            else:
+
+                def validated_datetime(value: Any) -> Any:
+                    if isinstance(value, datetime.datetime):
+                        return value
+                    elif isinstance(value, str):
+                        return datetime.datetime.fromisoformat(value)
+                    elif isinstance(value, float | int):
+                        return datetime.datetime.fromtimestamp(
+                            value,
+                            datetime.UTC,
+                        )
+                    else:
+                        raise TypeError("Invalid value", annotation, value)
+
+            return validated_datetime
+
         case parametrized if issubclass(parametrized, ParametrizedState):
             if validate := additional:
 
                 def validated(value: Any) -> Any:
                     if isinstance(value, parametrized):
                         validate(value)
                         return value
```

### Comparing `draive-0.9.2/src/draive/types/specification.py` & `draive-0.9.3/src/draive/types/specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import builtins
+import datetime
 import inspect
 import types
 import typing
+import uuid
 from collections.abc import Callable
 from dataclasses import is_dataclass
 from typing import (
     Any,
     Literal,
     NotRequired,
     ParamSpec,
@@ -53,14 +55,20 @@
     description: NotRequired[str]
 
 
 @final
 class ParameterStringSpecification(TypedDict, total=False):
     type: Required[Literal["string"]]
     description: NotRequired[str]
+    format: NotRequired[
+        Literal[
+            "uuid",
+            "date-time",
+        ]
+    ]
 
 
 @final
 class ParameterStringEnumSpecification(TypedDict, total=False):
     type: Required[Literal["string"]]
     enum: Required[list[str]]
     description: NotRequired[str]
@@ -266,14 +274,26 @@
                     "type": "number",
                     "enum": list(options),
                 }
 
             else:
                 raise TypeError("Unsupported literal type annotation", annotation)
 
+        case datetime.datetime:
+            specification = {
+                "type": "string",
+                "format": "date-time",
+            }
+
+        case uuid.UUID:
+            specification = {
+                "type": "string",
+                "format": "uuid",
+            }
+
         case parametrized if issubclass(parametrized, ParametrizedModel):
             specification = parametrized.specification()
 
         case typed_dict if typing.is_typeddict(typed_dict) or typing_extensions.is_typeddict(
             typed_dict
         ):
             specification = _annotations_specification(typed_dict.__annotations__)
```

### Comparing `draive-0.9.2/src/draive/utils/cache.py` & `draive-0.9.3/src/draive/utils/cache.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/utils/early_exit.py` & `draive-0.9.3/src/draive/utils/early_exit.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/utils/retry.py` & `draive-0.9.3/src/draive/utils/retry.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive/utils/stream.py` & `draive-0.9.3/src/draive/utils/stream.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/src/draive.egg-info/PKG-INFO` & `draive-0.9.3/src/draive.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draive
-Version: 0.9.2
+Version: 0.9.3
 Maintainer-email: Kacper Kaliński <kacper.kalinski@miquido.com>
 License: MIT License
         
         Copyright (c) 2024 Miquido
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,28 +29,27 @@
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.14
-Requires-Dist: mistralai~=0.1.3
+Requires-Dist: openai~=1.16
+Requires-Dist: mistralai~=0.1
 Requires-Dist: numpy~=1.26
-Requires-Dist: tiktoken~=0.6.0
+Requires-Dist: tiktoken~=0.6
 Requires-Dist: pydantic~=2.6
-Requires-Dist: httpx~=0.25.0
+Requires-Dist: httpx~=0.25
 Provides-Extra: dev
-Requires-Dist: ruff~=0.2.0; extra == "dev"
-Requires-Dist: pyright~=1.1.0; extra == "dev"
-Requires-Dist: bandit~=1.7.0; extra == "dev"
-Requires-Dist: pytest~=7.4.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: ruff~=0.3.0; extra == "dev"
+Requires-Dist: pyright~=1.1; extra == "dev"
+Requires-Dist: bandit~=1.7; extra == "dev"
+Requires-Dist: pytest~=7.4; extra == "dev"
+Requires-Dist: pytest-cov~=4.1; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
-Requires-Dist: python-dotenv~=1.0.0; extra == "dev"
 
 # draive
 
 Framework for building AI oriented applications.
 
 ## License
```

### Comparing `draive-0.9.2/src/draive.egg-info/SOURCES.txt` & `draive-0.9.3/src/draive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 src/draive/lmm/state.py
 src/draive/mistral/__init__.py
 src/draive/mistral/chat_response.py
 src/draive/mistral/chat_stream.py
 src/draive/mistral/chat_tools.py
 src/draive/mistral/client.py
 src/draive/mistral/config.py
+src/draive/mistral/embedding.py
 src/draive/mistral/errors.py
 src/draive/mistral/lmm.py
 src/draive/openai/__init__.py
 src/draive/openai/chat_response.py
 src/draive/openai/chat_stream.py
 src/draive/openai/chat_tools.py
 src/draive/openai/client.py
```

### Comparing `draive-0.9.2/tests/test_metrics.py` & `draive-0.9.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `draive-0.9.2/tests/test_model.py` & `draive-0.9.3/tests/test_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,54 @@
-import json
+from collections.abc import Callable
 from typing import Any, Literal
 
-from draive import Field, Model
+from draive import Field, State
 
 
 def invalid(value: str) -> None:
     if value != "valid":
         raise ValueError()
 
 
-class ExampleNestedModel(Model):
+class ExampleNestedState(State):
     string: str = "default"
     more: list[int] | None = None
 
 
-class ExampleModel(Model):
+def dummy_callable() -> None:
+    pass
+
+
+class ExampleState(State):
     string: str = "default"
     number: int = Field(alias="alias", description="description", default=1)
     none_default: int | None = Field(default=None)
     value_default: int = Field(default=9)
     invalid: str = Field(validator=invalid, default="valid")
-    nested: ExampleNestedModel = Field(alias="answer", default=ExampleNestedModel())
+    nested: ExampleNestedState = Field(alias="answer", default=ExampleNestedState())
     full: Literal["A", "B"] | list[int] | str | bool | None = Field(
         alias="all",
         description="complex",
         default="",
         validator=lambda value: None,
     )
+    function: Callable[..., Any] = dummy_callable
 
 
 # TODO: prepare extensive tests
 def test_validated_passes_with_valid_values() -> None:
     values_dict: dict[str, Any] = {
         "string": "value",
         "alias": 42,
         "none_default": 1,
         "value_default": 8,
         "invalid": "valid",
         "answer": {"string": "value", "more": None},
         "all": True,
+        "function": dummy_callable,
     }
-    assert json.loads(ExampleModel.validated(**values_dict).as_json()) == values_dict
+    model: ExampleState = ExampleState.validated(**values_dict)
+    assert model.as_dict() == values_dict
 
 
 def test_validated_passes_with_default_values() -> None:
-    ExampleModel.validated()
+    ExampleState.validated()
```

### Comparing `draive-0.9.2/tests/test_state.py` & `draive-0.9.3/tests/test_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,85 @@
-from collections.abc import Callable
+import json
+from datetime import UTC, datetime
 from typing import Any, Literal
+from uuid import UUID
 
-from draive import Field, State
+from draive import Field, Model
 
 
 def invalid(value: str) -> None:
     if value != "valid":
         raise ValueError()
 
 
-class ExampleNestedState(State):
+class ExampleNestedModel(Model):
     string: str = "default"
     more: list[int] | None = None
 
 
-def dummy_callable() -> None:
-    pass
-
-
-class ExampleState(State):
+class ExampleModel(Model):
     string: str = "default"
     number: int = Field(alias="alias", description="description", default=1)
     none_default: int | None = Field(default=None)
     value_default: int = Field(default=9)
     invalid: str = Field(validator=invalid, default="valid")
-    nested: ExampleNestedState = Field(alias="answer", default=ExampleNestedState())
+    nested: ExampleNestedModel = Field(alias="answer", default=ExampleNestedModel())
     full: Literal["A", "B"] | list[int] | str | bool | None = Field(
         alias="all",
         description="complex",
         default="",
         validator=lambda value: None,
     )
-    function: Callable[..., Any] = dummy_callable
 
 
 # TODO: prepare extensive tests
 def test_validated_passes_with_valid_values() -> None:
     values_dict: dict[str, Any] = {
         "string": "value",
         "alias": 42,
         "none_default": 1,
         "value_default": 8,
         "invalid": "valid",
         "answer": {"string": "value", "more": None},
         "all": True,
-        "function": dummy_callable,
     }
-    model: ExampleState = ExampleState.validated(**values_dict)
-    assert model.as_dict() == values_dict
+    assert json.loads(ExampleModel.validated(**values_dict).as_json()) == values_dict
 
 
 def test_validated_passes_with_default_values() -> None:
-    ExampleState.validated()
+    ExampleModel.validated()
+
+
+class DatetimeModel(Model):
+    value: datetime
+
+
+datetimeModelInstance: DatetimeModel = DatetimeModel(
+    value=datetime.fromtimestamp(0, UTC),
+)
+datetimeModelJSON: str = '{"value": "1970-01-01T00:00:00+00:00"}'
+
+
+def test_datetime_encoding() -> None:
+    assert datetimeModelInstance.as_json() == datetimeModelJSON
+
+
+def test_datetime_decoding() -> None:
+    assert DatetimeModel.from_json(datetimeModelJSON) == datetimeModelInstance
+
+
+class UUIDModel(Model):
+    value: UUID
+
+
+uuidModelInstance: UUIDModel = UUIDModel(
+    value=UUID(hex="0cf728c0369348e78552e8d86d35e8b0"),
+)
+uuidModelJSON: str = '{"value": "0cf728c0369348e78552e8d86d35e8b0"}'
+
+
+def test_uuid_encoding() -> None:
+    assert uuidModelInstance.as_json() == uuidModelJSON
+
+
+def test_uuid_decoding() -> None:
+    assert UUIDModel.from_json(uuidModelJSON) == uuidModelInstance
```

