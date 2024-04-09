# Comparing `tmp/supamodel-0.2.0.tar.gz` & `tmp/supamodel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.2.0.tar", max compression
+gzip compressed data, was "supamodel-0.3.0.tar", max compression
```

## Comparing `supamodel-0.2.0.tar` & `supamodel-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,22 @@
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633617 supamodel-0.2.0/README.md
--rw-r--r--   0        0        0      265 2024-04-09 16:24:15.805034 supamodel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.2.0/supamodel/__init__.py
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 supamodel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.3.0/README.md
+-rw-r--r--   0        0        0      523 2024-04-09 22:47:45.369423 supamodel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.3.0/supamodel/__init__.py
+-rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.3.0/supamodel/_abc.py
+-rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.3.0/supamodel/_client.py
+-rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.3.0/supamodel/_core.py
+-rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.3.0/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.3.0/supamodel/_types.py
+-rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.3.0/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.3.0/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.3.0/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.3.0/supamodel/exceptions.py
+-rw-r--r--   0        0        0     7911 2024-04-09 21:41:30.442305 supamodel-0.3.0/supamodel/supa_model.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.3.0/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.3.0/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.3.0/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.3.0/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.3.0/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.3.0/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.3.0/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.3.0/supamodel/utils.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 supamodel-0.3.0/PKG-INFO
```

