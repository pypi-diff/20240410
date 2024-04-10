# Comparing `tmp/alipcs_py-0.7.0.tar.gz` & `tmp/alipcs_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alipcs_py-0.7.0.tar", max compression
+gzip compressed data, was "alipcs_py-0.8.0.tar", max compression
```

## Comparing `alipcs_py-0.7.0.tar` & `alipcs_py-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1054 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/LICENSE
--rw-r--r--   0        0        0    43930 2024-04-03 04:31:01.213811 alipcs_py-0.7.0/README.md
--rw-r--r--   0        0        0      106 2024-04-03 03:26:20.780775 alipcs_py-0.7.0/alipcs_py/__init__.py
--rw-r--r--   0        0        0      240 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/alipcs/__init__.py
--rw-r--r--   0        0        0    40588 2024-04-03 04:39:24.951253 alipcs_py-0.7.0/alipcs_py/alipcs/api.py
--rw-r--r--   0        0        0     2051 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/alipcs/errors.py
--rw-r--r--   0        0        0    19386 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/alipcs/inner.py
--rw-r--r--   0        0        0    44545 2024-04-03 04:39:24.951253 alipcs_py-0.7.0/alipcs_py/alipcs/pcs.py
--rw-r--r--   0        0        0    12095 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/alipcs/phone.py
--rw-r--r--   0        0        0     1446 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/alipcs/tree.py
--rw-r--r--   0        0        0      122 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/app/__init__.py
--rw-r--r--   0        0        0     8026 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/app/account.py
--rw-r--r--   0        0        0    50253 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/app/app.py
--rw-r--r--   0        0        0      825 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/app/config.py
--rw-r--r--   0        0        0        0 2024-03-30 15:28:24.848594 alipcs_py-0.7.0/alipcs_py/commands/__init__.py
--rw-r--r--   0        0        0      788 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/cat.py
--rw-r--r--   0        0        0      653 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/crypto.py
--rw-r--r--   0        0        0    14746 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/display.py
--rw-r--r--   0        0        0    12989 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/commands/download.py
--rw-r--r--   0        0        0      494 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/env.py
--rw-r--r--   0        0        0       40 2024-04-02 03:48:14.826887 alipcs_py-0.7.0/alipcs_py/commands/errors.py
--rw-r--r--   0        0        0     2557 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/file_operators.py
--rw-r--r--   0        0        0    20271 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/index.html
--rw-r--r--   0        0        0     5938 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/list_files.py
--rw-r--r--   0        0        0      508 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/log.py
--rw-r--r--   0        0        0     1250 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/login.py
--rw-r--r--   0        0        0     9366 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/commands/play.py
--rw-r--r--   0        0        0      805 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/search.py
--rw-r--r--   0        0        0     7031 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/commands/server.py
--rw-r--r--   0        0        0     9314 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/share.py
--rw-r--r--   0        0        0     2670 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/sifter.py
--rw-r--r--   0        0        0     2900 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/sync.py
--rw-r--r--   0        0        0    23198 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/commands/upload.py
--rw-r--r--   0        0        0      199 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/commands/user.py
--rw-r--r--   0        0        0     1317 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/common/cache.py
--rw-r--r--   0        0        0     2014 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/common/concurrent.py
--rw-r--r--   0        0        0      188 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/common/constant.py
--rw-r--r--   0        0        0     8745 2024-03-30 15:26:17.162178 alipcs_py-0.7.0/alipcs_py/common/crypto.py
--rw-r--r--   0        0        0      655 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/common/date.py
--rw-r--r--   0        0        0     2123 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/common/downloader.py
--rw-r--r--   0        0        0     1160 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/event.py
--rw-r--r--   0        0        0     3179 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/file_type.py
--rw-r--r--   0        0        0    34044 2024-04-02 13:11:34.629254 alipcs_py-0.7.0/alipcs_py/common/io.py
--rw-r--r--   0        0        0     2810 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/keyboard.py
--rw-r--r--   0        0        0     1087 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/log.py
--rw-r--r--   0        0        0      700 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/net.py
--rw-r--r--   0        0        0      165 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/number.py
--rw-r--r--   0        0        0     1554 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/path.py
--rw-r--r--   0        0        0      143 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/platform.py
--rw-r--r--   0        0        0     1222 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/progress_bar.py
--rw-r--r--   0        0        0     1322 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/simple_cipher.pyx
--rw-r--r--   0        0        0       73 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/url.py
--rw-r--r--   0        0        0      451 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/common/util.py
--rw-r--r--   0        0        0     1208 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/config/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 15:28:25.920615 alipcs_py-0.7.0/alipcs_py/storage/__init__.py
--rw-r--r--   0        0        0     6121 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/storage/store.py
--rw-r--r--   0        0        0     5188 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/storage/tables.py
--rw-r--r--   0        0        0     1424 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/alipcs_py/utils.py
--rw-r--r--   0        0        0      735 2024-03-30 15:26:17.166178 alipcs_py-0.7.0/build.py
--rw-r--r--   0        0        0     1587 2024-04-03 03:26:20.768775 alipcs_py-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    46320 1970-01-01 00:00:00.000000 alipcs_py-0.7.0/setup.py
--rw-r--r--   0        0        0    45379 1970-01-01 00:00:00.000000 alipcs_py-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/LICENSE
+-rw-r--r--   0        0        0    43247 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/README.md
+-rw-r--r--   0        0        0      106 2024-04-09 14:35:54.653213 alipcs_py-0.8.0/alipcs_py/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-07 09:50:59.163603 alipcs_py-0.8.0/alipcs_py/alipcs/__init__.py
+-rw-r--r--   0        0        0    51371 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/alipcs/api.py
+-rw-r--r--   0        0        0     3869 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/alipcs/errors.py
+-rw-r--r--   0        0        0    20929 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/alipcs/inner.py
+-rw-r--r--   0        0        0    52549 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/alipcs/pcs.py
+-rw-r--r--   0        0        0    12095 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/alipcs/phone.py
+-rw-r--r--   0        0        0     1446 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/alipcs/tree.py
+-rw-r--r--   0        0        0      122 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/app/__init__.py
+-rw-r--r--   0        0        0     8041 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/app/account.py
+-rw-r--r--   0        0        0    49674 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/app/app.py
+-rw-r--r--   0        0        0      825 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/app/config.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:28:24.848594 alipcs_py-0.8.0/alipcs_py/commands/__init__.py
+-rw-r--r--   0        0        0      802 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/cat.py
+-rw-r--r--   0        0        0      668 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/crypto.py
+-rw-r--r--   0        0        0    14728 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/display.py
+-rw-r--r--   0        0        0    19413 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/download.py
+-rw-r--r--   0        0        0      494 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/env.py
+-rw-r--r--   0        0        0       40 2024-04-02 03:48:14.826887 alipcs_py-0.8.0/alipcs_py/commands/errors.py
+-rw-r--r--   0        0        0     3257 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/file_operators.py
+-rw-r--r--   0        0        0    20271 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/index.html
+-rw-r--r--   0        0        0     5922 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/list_files.py
+-rw-r--r--   0        0        0      508 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/log.py
+-rw-r--r--   0        0        0     1250 2024-04-07 09:50:59.227605 alipcs_py-0.8.0/alipcs_py/commands/login.py
+-rw-r--r--   0        0        0     9158 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/play.py
+-rw-r--r--   0        0        0      805 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/search.py
+-rw-r--r--   0        0        0     7051 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/server.py
+-rw-r--r--   0        0        0    10328 2024-04-09 14:35:32.116762 alipcs_py-0.8.0/alipcs_py/commands/share.py
+-rw-r--r--   0        0        0     2670 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/sifter.py
+-rw-r--r--   0        0        0     2905 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/commands/sync.py
+-rw-r--r--   0        0        0    18489 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/commands/upload.py
+-rw-r--r--   0        0        0      199 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/commands/user.py
+-rw-r--r--   0        0        0     1317 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/common/cache.py
+-rw-r--r--   0        0        0     1003 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/concurrent.py
+-rw-r--r--   0        0        0      188 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/common/constant.py
+-rw-r--r--   0        0        0     8745 2024-03-30 15:26:17.162178 alipcs_py-0.8.0/alipcs_py/common/crypto.py
+-rw-r--r--   0        0        0      655 2024-04-02 13:11:34.629254 alipcs_py-0.8.0/alipcs_py/common/date.py
+-rw-r--r--   0        0        0     2220 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/downloader.py
+-rw-r--r--   0        0        0     1160 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/event.py
+-rw-r--r--   0        0        0     3179 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/file_type.py
+-rw-r--r--   0        0        0    34576 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/io.py
+-rw-r--r--   0        0        0     2810 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/keyboard.py
+-rw-r--r--   0        0        0     1114 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/log.py
+-rw-r--r--   0        0        0     1321 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/net.py
+-rw-r--r--   0        0        0      165 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/number.py
+-rw-r--r--   0        0        0     1397 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/common/path.py
+-rw-r--r--   0        0        0      143 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/platform.py
+-rw-r--r--   0        0        0     1222 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/progress_bar.py
+-rw-r--r--   0        0        0     1322 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/simple_cipher.pyx
+-rw-r--r--   0        0        0       73 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/url.py
+-rw-r--r--   0        0        0      451 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/common/util.py
+-rw-r--r--   0        0        0     1208 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:28:25.920615 alipcs_py-0.8.0/alipcs_py/storage/__init__.py
+-rw-r--r--   0        0        0     6146 2024-04-09 14:35:32.120762 alipcs_py-0.8.0/alipcs_py/storage/store.py
+-rw-r--r--   0        0        0     5188 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/storage/tables.py
+-rw-r--r--   0        0        0     1424 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/alipcs_py/utils.py
+-rw-r--r--   0        0        0      735 2024-03-30 15:26:17.166178 alipcs_py-0.8.0/build.py
+-rw-r--r--   0        0        0     1623 2024-04-09 14:35:54.653213 alipcs_py-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    45615 1970-01-01 00:00:00.000000 alipcs_py-0.8.0/setup.py
+-rw-r--r--   0        0        0    44696 1970-01-01 00:00:00.000000 alipcs_py-0.8.0/PKG-INFO
```

### Comparing `alipcs_py-0.7.0/LICENSE` & `alipcs_py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/README.md` & `alipcs_py-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -718,34 +718,14 @@
 
 上传过程中，按 “p” 可以暂停或继续上传。
 
 ```
 AliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR
 ```
 
-指定上传方式：
-
-`--upload-type Many`: 同时上传多个文件。
-
-适合大多数文件长度小于 100M 以下的情况。
-
-```
-AliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR
-```
-
-<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>
-
-<del>适合大多数文件长度大于 1G 以上的情况。</del>
-
-**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**
-
-```
-AliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR
-```
-
 指定同时上传连接数量:
 
 `--max-workers` 默认为 CPU 核数。
 
 ```
 AliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR
 ```
@@ -754,22 +734,21 @@
 
 比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。
 
 如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`
 
 ### 选项
 
-| Option                                                     | Description                             |
-| ---------------------------------------------------------- | --------------------------------------- |
-| -t, --upload-type [One \| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |
-| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |
-| -e, --encrypt-type [No \| Simple \| ChaCha20 \| AES256CBC] | 文件加密方法，默认为 No 不加密          |
-| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |
-| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |
-| --no-show-progress, --NP                                   | 不显示上传进度                          |
+| Option                                                     | Description                           |
+| ---------------------------------------------------------- | ------------------------------------- |
+| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的          |
+| -e, --encrypt-type [No \| Simple \| ChaCha20 \| AES256CBC] | 文件加密方法，默认为 No 不加密        |
+| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数 |
+| --no-ignore-existing, --NI                                 | 上传已经存在的文件                    |
+| --no-show-progress, --NP                                   | 不显示上传进度                        |
 
 ## 同步本地目录到远端
 
 同步本地目录到远端。
 
 如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。
```

### Comparing `alipcs_py-0.7.0/alipcs_py/alipcs/api.py` & `alipcs_py-0.8.0/alipcs_py/alipcs/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Optional, List, Tuple, Dict, Union, DefaultDict, Iterable, Iterator, Callable, IO
+from typing import Any, Optional, List, Tuple, Dict, Union, DefaultDict, Iterable, Callable, IO
 from threading import Lock
 from collections import defaultdict
 from copy import deepcopy
 from functools import partial
 import logging
+import warnings
 
 from alipcs_py.alipcs.errors import AliPCSError
 from alipcs_py.common.io import RangeRequestIO, DEFAULT_MAX_CHUNK_SIZE
 from alipcs_py.alipcs.pcs import AliPCS, AliOpenPCS, CheckNameMode
 from alipcs_py.alipcs.inner import PcsFile, PcsPreparedFile, PcsSharedLink, PcsSharedLinkInfo, PcsUser, PcsDownloadUrl
 from alipcs_py.common.path import split_posix_path, join_path, posix_path_dirname
 
@@ -16,18 +17,36 @@
 logger = logging.getLogger(__name__)
 
 
 _ALI_PCS_API_LOCK = Lock()
 
 
 class AliPCSApi:
-    """Aliyundrive PCS Api
+    """Alipan Drive Personal Cloud Service API
 
-    This is the wrapper of `AliPCS`. It parses the content of response of raw
-    AliPCS requests to some inner data structions.
+    This is the wrapper of `AliPCS` class. It parses the raw content of response of
+    AliPCS request into the inner data structions.
+
+    Args:
+        refresh_token (str): The refresh token of the user.
+        access_token (str, optional): The access token of the user.
+        token_type (str): The token type. Default is "Bearer".
+        expire_time (int, optional): The expire time of the token.
+        user_id (str, optional): The user id of the user.
+        user_name (str, optional): The user name of the user.
+        nick_name (str, optional): The nick name of the user.
+        device_id (str, optional): The device id of the user.
+        default_drive_id (str, optional): The default drive id of the user.
+        role (str, optional): The role of the user.
+        status (str, optional): The status of the user.
+        error_max_retries (int): The max retries when a client request error occurs. Default is 2.
+        max_keepalive_connections (int): The max keepalive connections. Default is 50.
+        max_connections (int): The max number of connections in the pool. Default is 50.
+        keepalive_expiry (float): The keepalive expiry. Default is 10 * 60 seconds.
+        connection_max_retries (int): The max retries when a connection error occurs. Default is 2.
     """
 
     def __init__(
         self,
         refresh_token: str,
         access_token: str = "",
         token_type: str = "",
@@ -35,27 +54,37 @@
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
         device_id: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
+        error_max_retries: int = 2,
+        max_keepalive_connections: int = 50,
+        max_connections: int = 50,
+        keepalive_expiry: float = 10 * 60,
+        connection_max_retries: int = 2,
     ):
         self._alipcs = AliPCS(
             refresh_token,
             access_token=access_token,
             token_type=token_type,
             expire_time=expire_time,
             user_id=user_id,
             user_name=user_name,
             nick_name=nick_name,
             device_id=device_id,
             default_drive_id=default_drive_id,
             role=role,
             status=status,
+            error_max_retries=error_max_retries,
+            max_keepalive_connections=max_keepalive_connections,
+            max_connections=max_connections,
+            keepalive_expiry=keepalive_expiry,
+            connection_max_retries=connection_max_retries,
         )
 
         # The path tree is for user's own files
         self._path_tree = PathTree(self)
 
         # Map `share_id` to a `PathTree` for that shared link
         self._shared_path_tree: DefaultDict[str, PathTree] = defaultdict(partial(PathTree, self))
@@ -100,64 +129,164 @@
     def role(self) -> str:
         return self._alipcs.role
 
     @property
     def status(self) -> str:
         return self._alipcs.status
 
-    def meta(self, *file_ids: str, share_id: str = None) -> List[PcsFile]:
-        """Meta data of `remotepaths`"""
+    def path_traceback(self, file_id: str, share_id: Optional[str] = None) -> List[PcsFile]:
+        """Traceback the path of the file
+
+        Return the list of all `PcsFile`s from the file to the top level directory.
+
+        Important:
+            The `path` property of the returned `PcsFile` has absolute path.
+        """
+
+        try:
+            info = self._alipcs.path_traceback(file_id, share_id=share_id)
+        except AliPCSError as err:
+            if err.error_code == "NotFound.File":
+                return []
+            raise
+
+        pcs_files = []
+        for item_info in info["items"][::-1]:
+            pcs_file = PcsFile.from_(item_info)
+            pcs_file.path = join_path(pcs_files[-1].path if pcs_files else "/", pcs_file.name)
+            pcs_files.append(pcs_file)
+
+        pcs_files.reverse()
+        return pcs_files
+
+    def meta_by_path(self, remotepath: str) -> Optional[PcsFile]:
+        """Get the meta of the the path
+
+        Can not get the shared files' meta info by their paths.
+
+        Important:
+            The `path` property of the returned `PcsFile` is the argument `remotepath`.
+        """
+
+        assert remotepath.startswith("/"), "Path should start with '/'"
+
+        if remotepath == "/":
+            return PcsFile.root()
 
-        pcs_files = [PcsFile.root() if fid == "root" else None for fid in file_ids]
-        fids = [fid for fid in file_ids if fid != "root"]
+        try:
+            info = self._alipcs.meta_by_path(remotepath)
+        except AliPCSError as err:
+            if err.error_code == "NotFound.File":
+                return None
+            raise
+
+        pcs_file = PcsFile.from_(info)
+        pcs_file.path = remotepath
+        return pcs_file
+
+    def meta(self, file_id: str, share_id: Optional[str] = None) -> Optional[PcsFile]:
+        """Get meta info of the file
+
+        Important:
+            The `path` property of the returned `PcsFile` is only the name of the file.
+        """
+
+        try:
+            info = self._alipcs.meta(file_id, share_id=share_id)
+        except AliPCSError as err:
+            if err.error_code == "NotFound.File":
+                return None
+            raise
+
+        return PcsFile.from_(info)
 
-        if fids:
-            info = self._alipcs.meta(*fids, share_id=share_id)
-            pfs = [PcsFile.from_(v.get("body")) for v in info["responses"]]
-            j = 0
-            for i in range(len(pcs_files)):
-                if pcs_files[i] is None:
-                    pcs_files[i] = pfs[j]
-                    j += 1
+    def get_file(
+        self, *, remotepath: str = "", file_id: str = "", share_id: Optional[str] = None
+    ) -> Optional[PcsFile]:
+        """Get the file's info by the given `remotepath` or `file_id`
+
+        If the `remotepath` is given, the `file_id` will be ignored.
+
+        Important:
+            If the `remotepath` is given, the `path` property of the returned `PcsFile` is the `remotepath`.
+            If the `file_id` is given, the `path` property of the returned `PcsFile` is only the name of the file.
+        """
 
-        return [pf for pf in pcs_files if pf is not None]
+        if remotepath:
+            if share_id:
+                return self.path(remotepath, share_id=share_id)
+            else:
+                return self.meta_by_path(remotepath)
+        elif file_id:
+            return self.meta(file_id, share_id=share_id)
+        else:
+            raise ValueError("One of `remotepath` and `file_id` must be given")
 
     def exists(self, file_id: str) -> bool:
-        """Check whether `remotepath` exists"""
+        """Check whether the file exists
+
+        Return True if the file exists and does not in the trash else False.
+        """
 
         return self._alipcs.exists(file_id)
 
+    def exists_in_trash(self, file_id: str) -> bool:
+        """Check whether the file exists in the trash
+
+        Return True if the file exists in the trash else False.
+        """
+
+        return self._alipcs.exists_in_trash(file_id)
+
     def is_file(self, file_id: str) -> bool:
-        """Check whether `remotepath` is a file"""
+        """Check whether `file_id` is a file"""
 
         return self._alipcs.is_file(file_id)
 
     def is_dir(self, file_id: str) -> bool:
-        """Check whether `remotepath` is a directory"""
+        """Check whether `file_id` is a directory"""
 
         return self._alipcs.is_dir(file_id)
 
     def list(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
         next_marker: str = "",
     ) -> Tuple[List[PcsFile], str]:
         """List the directory's contents
 
         List files and directories in the given directory (which has the `file_id`).
         The return items size is limited by the `limit` parameter. If you want to list
         more, using the returned `next_marker` parameter for next `list` call.
+
+        Args:
+            file_id (str): The directory's file id.
+            share_id (str): The share id if the file_id is in shared link.
+            desc (bool): Descending order by time.
+            name (bool): Order by name.
+            time (bool): Order by time.
+            size (bool): Order by size.
+            all (bool): Unknown, just for the request.
+            limit (int): The number of items to return.
+            url_expire_sec (int): The download url's expire time.
+            next_marker (str): The next marker for next list call.
+
+        Returns:
+            Tuple[List[PcsFile], str]: The list of `PcsFile` and the next marker.
+
+        Important:
+            These PcsFile instances' path property is only the name of the file.
         """
 
         info = self._alipcs.list(
             file_id=file_id,
             share_id=share_id,
             desc=desc,
             name=name,
@@ -165,160 +294,179 @@
             size=size,
             all=all,
             limit=limit,
             url_expire_sec=url_expire_sec,
             next_marker=next_marker,
         )
         next_marker = info["next_marker"]
-        return [PcsFile.from_(v) for v in info.get("items", [])], next_marker
+        pcs_files = []
+        for v in info.get("items", []):
+            pcs_files.append(PcsFile.from_(v))
+        return pcs_files, next_marker
 
     def list_iter(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
         recursive: bool = False,
         include_dir: bool = True,
-    ) -> Iterator[PcsFile]:
+    ) -> Iterable[PcsFile]:
         """Iterate the directory by its `file_id`
 
         Iterate all files and directories at the directory (which has the `file_id`).
+
+        Args:
+            file_id (str): The directory's file id.
+            share_id (str): The share id if the file_id is in shared link.
+            desc (bool): Descending order by time.
+            name (bool): Order by name.
+            time (bool): Order by time.
+            size (bool): Order by size.
+            all (bool): Unknown, just for the request.
+            limit (int): The number of one request queries.
+            url_expire_sec (int): The download url's expire time.
+            recursive (bool): Recursively iterate the directory.
+            include_dir (bool): Include directory in the result.
+
+        Returns:
+            Iterable[PcsFile]: The iterator of `PcsFile`.
+
+        Important:
+            These PcsFile instances' path property is the path from the first sub-directory of the `file_id` to the file name.
+            e.g.
+                If the directory (owned `file_id`) has path `level0/`, a sub-directory which of path is
+                `level0/level1/level2` then its corresponding PcsFile.path is `level1/level2`.
         """
 
         next_marker = ""
-        pcs_file = self.meta(file_id, share_id=share_id)[0]
-        dirname = pcs_file.name
         while True:
             pcs_files, next_marker = self.list(
                 file_id,
                 share_id=share_id,
                 desc=desc,
                 name=name,
                 time=time,
                 size=size,
                 all=all,
                 limit=limit,
                 url_expire_sec=url_expire_sec,
                 next_marker=next_marker,
             )
             for pf in pcs_files:
-                pf.path = join_path(dirname, pf.name)
-
-                if pf.is_dir:
+                if pf.is_file:
+                    yield pf
+                else:
                     if include_dir:
-                        yield pf
+                        # The upper recursive call will change the `pf.path`.
+                        # So, we need to deepcopy it.
+                        yield deepcopy(pf)
                     if recursive:
                         for sub_pf in self.list_iter(
                             pf.file_id,
                             share_id=share_id,
                             desc=desc,
                             name=name,
                             time=time,
                             size=size,
                             all=all,
                             limit=limit,
                             url_expire_sec=url_expire_sec,
                             recursive=recursive,
                             include_dir=include_dir,
                         ):
-                            sub_pf.path = join_path(dirname, sub_pf.path)
-                            yield sub_pf
-                else:
-                    yield pf
+                            sub_pf.path = join_path(pf.path, sub_pf.path)
+                            if sub_pf.is_file:
+                                yield sub_pf
+                            else:
+                                # The upper recursive call will change the `pf.path`.
+                                # So, we need to deepcopy it.
+                                yield deepcopy(sub_pf)
 
             if not next_marker:
                 return
 
-    def path(self, remotepath: str, share_id: str = None) -> Optional[PcsFile]:
-        """Get the pcs file's info by the given absolute `remotepath`"""
+    def path(self, remotepath: str, share_id: Optional[str] = None) -> Optional[PcsFile]:
+        """Get the pcs file's info by the given absolute `remotepath`
+
+        Important:
+            The `path` property of the returned `PcsFile` is the argument `remotepath`.
+        """
+
+        assert remotepath.startswith("/"), "`remotepath` should start with '/'"
 
         if share_id:
             return self._shared_path_tree[share_id].search(remotepath=remotepath, share_id=share_id)
         else:
             return self._path_tree.search(remotepath=remotepath)
 
-    def paths(self, *remotepaths: str, share_id: str = None) -> List[Optional[PcsFile]]:
-        """Get the pcs files' info by the given absolute `remotepaths`"""
+    def paths(self, *remotepaths: str, share_id: Optional[str] = None) -> List[Optional[PcsFile]]:
+        """Get the pcs files' info by the given absolute `remotepaths`
 
-        return [self.path(rp, share_id=share_id) for rp in remotepaths]
+        Important:
+            The `path` property of the returned `PcsFile` is the argument `remotepath`.
+        """
 
-    def list_path_iter(
+        return [self.path(remote_path, share_id=share_id) for remote_path in remotepaths]
+
+    def walk(
         self,
-        remotepath: str,
-        file_id: str = None,
-        share_id: str = None,
-        desc: bool = False,
-        name: bool = False,
-        time: bool = False,
-        size: bool = False,
+        file_id: str,
+        share_id: str = "",
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
-        recursive: bool = False,
-        include_dir: bool = True,
-    ) -> Iterator[PcsFile]:
-        """Iterate the `remotepath`"""
-
-        if not file_id:
-            pf = self.path(remotepath, share_id=share_id)
-            if not pf:
-                return
-            file_id = pf.file_id
+    ) -> Iterable[PcsFile]:
+        """Recursively Walk through the directory tree which has `file_id`
 
-        dirname = posix_path_dirname(remotepath)
+        Args:
+            file_id (str): The directory's file id.
+            share_id (str): The share id if the file_id is in shared link.
+            all (bool): Unknown, just for the request.
+            limit (int): The number of one request queries.
+            url_expire_sec (int): The download url's expire time.
+            include_dir (bool): Include directory in the result.
+
+        Returns:
+            Iterable[PcsFile]: The iterator of `PcsFile`.
+
+        Important:
+            These PcsFile instances' path property is the path from the first sub-directory of the `file_id` to the file.
+            e.g.
+                If the directory (owned `file_id`) has path `level0/`, a sub-directory which of path is
+                `level0/level1/level2` then its corresponding PcsFile.path is `level1/level2`.
 
-        for p in self.list_iter(
-            file_id,
-            share_id=share_id,
-            desc=desc,
-            name=name,
-            time=time,
-            size=size,
-            all=all,
-            limit=limit,
-            url_expire_sec=url_expire_sec,
-            recursive=recursive,
-            include_dir=include_dir,
-        ):
-            p.path = join_path(dirname, p.path)
-            yield p
+        """
 
-    def list_path(
-        self,
-        remotepath: str,
-        file_id: str = None,
-        share_id: str = None,
-        desc: bool = False,
-        name: bool = False,
-        time: bool = False,
-        size: bool = False,
-        all: bool = False,
-        limit: int = 200,
-        url_expire_sec: int = 14400,
-    ) -> List[PcsFile]:
-        return list(
-            self.list_path_iter(
-                remotepath,
-                file_id=file_id,
+        file_id_to_path = {file_id: ""}
+        next_marker = ""
+        while True:
+            info = self._alipcs.walk(
+                file_id,
                 share_id=share_id,
-                desc=desc,
-                name=name,
-                time=time,
-                size=size,
                 all=all,
                 limit=limit,
                 url_expire_sec=url_expire_sec,
+                next_marker=next_marker,
             )
-        )
+            for v in info["items"]:
+                pcs_file = PcsFile.from_(v)
+                pcs_file.path = join_path(file_id_to_path[pcs_file.parent_file_id], pcs_file.name)
+                file_id_to_path[pcs_file.file_id] = pcs_file.path
+                yield pcs_file
+
+            next_marker = info["next_marker"]
+            if not next_marker:
+                return
 
     def create_file(
         self,
         filename: str,
         dir_id: str,
         size: int,
         pre_hash: str = "",
@@ -396,21 +544,21 @@
         proof_code: str,
         check_name_mode: CheckNameMode = "auto_rename",
     ) -> PcsPreparedFile:
         return self.create_file(
             filename, dir_id, size, content_hash=content_hash, proof_code=proof_code, check_name_mode=check_name_mode
         )
 
-    def upload_slice(self, io: IO, url: str, callback: Callable[[MultipartEncoderMonitor], None] = None) -> None:
+    def upload_slice(self, io: IO, url: str, callback_for_monitor: Optional[Callable[[int], Any]] = None) -> None:
         """Upload an io as a slice
 
-        callable: the callback for monitoring uploading progress
+        callable: the callback for monitor
         """
 
-        self._alipcs.upload_slice(io, url, callback=callback)
+        self._alipcs.upload_slice(io, url, callback_for_monitor=callback_for_monitor)
 
     def upload_complete(self, file_id: str, upload_id: str) -> PcsFile:
         """Tell server that all slices have been uploaded
 
         After uploading all slices using `AliPCSApi.upload_slice`, we need to
         tell server that all slice have been uploaded. Then, the server will
         return the final file info back.
@@ -467,20 +615,35 @@
 
             if not next_marker:
                 break
 
         return pcs_files
 
     def makedir(self, dir_id: str, name: str) -> PcsFile:
+        """Make a directory in the `dir_id` directory
+
+        Important:
+            The `path` property of the returned `PcsFile` is only the name of the directory.
+        """
+
         info = self._alipcs.makedir(dir_id, name)
         return PcsFile.from_(info)
 
-    def makedir_path(self, remotedir: str) -> PcsFile:
+    def makedir_path(self, remotedir: str) -> List[PcsFile]:
+        """Make a directory by the absolute `remotedir` path
+
+        Return the list of all `PcsFile`s from the directory to the top level directory.
+
+        Important:
+            The `path` property of the returned `PcsFile` has absolute path.
+        """
+
         # Use lock to ignore make a directory twice
         with _ALI_PCS_API_LOCK:
+            paths = []
             parts = split_posix_path(remotedir)
             parent = PcsFile.root()
             for i, part in enumerate(parts):
                 if part == "/":  # ignore root
                     continue
 
                 # Find the sub directory which has the name of `part`
@@ -493,54 +656,67 @@
                 if pf.name == part:
                     assert pf.is_dir, f"{now_dir} is a file"
                 else:
                     pf = self.makedir(parent.file_id, part)
 
                 pf.path = now_dir
                 parent = pf
-            return parent
+                paths.append(pf)
+
+            paths.reverse()
+            return paths
 
     def move(self, *file_ids: str) -> List[bool]:
         """Move `file_ids[:-1]` to `file_ids[-1]`"""
 
         info = self._alipcs.move(*file_ids)
 
         # Remove nodes from self._path_tree
         for file_id in file_ids[:-1]:
             self._path_tree.pop_by_file_id(file_id)
 
         return ["code" not in v["body"] for v in info["responses"]]
 
     def rename(self, file_id: str, name: str) -> PcsFile:
+        """Rename the file with `file_id` to `name`
+
+        Important:
+            The `path` property of the returned `PcsFile` is only the name of the file.
+        """
+
         info = self._alipcs.rename(file_id, name)
 
         # Remove node from self._path_tree
         self._path_tree.pop_by_file_id(file_id)
 
         return PcsFile.from_(info)
 
     def copy(self, *file_ids: str) -> List[PcsFile]:
-        """Copy `remotepaths[:-1]` to `remotepaths[-1]`"""
+        """Copy `file_ids[:-1]` to `file_ids[-1]`
+
+        Important:
+            The `path` property of the returned `PcsFile` is only the name of the file.
+        """
 
         info = self._alipcs.copy(*file_ids)
         return [PcsFile.from_(v["body"]) for v in info["responses"]]
 
     def remove(self, *file_ids: str) -> List[bool]:
-        """Remove all `remotepaths`"""
+        """Remove all `file_ids`"""
 
         info = self._alipcs.remove(*file_ids)
 
         # Remove nodes from self._path_tree
-        for file_id in file_ids[:-1]:
+        for file_id in file_ids:
             self._path_tree.pop_by_file_id(file_id)
 
         return ["code" not in v for v in info["responses"]]
 
     def share(self, *file_ids: str, password: str = "", period: int = 0, description: str = "") -> PcsSharedLink:
-        """Share `remotepaths` to public with a optional password
+        """Share `file_ids` to public with a optional password
 
         Args:
             period (int): The days for expiring. `0` means no expiring
         """
 
         info = self._alipcs.share(*file_ids, password=password, period=period, description=description)
         return PcsSharedLink.from_(info)
@@ -648,30 +824,30 @@
                 pcs_file.download_url = pcs_url.url
         return pcs_file
 
     def file_stream(
         self,
         file_id: str,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         """File stream as a normal io"""
 
         return self._alipcs.file_stream(
             file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
         )
 
     def shared_file_stream(
         self,
         shared_file_id: str,
         share_id: str,
         expire_duration: int = 10 * 60,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         """Shared file stream as a normal io"""
 
         return self._alipcs.shared_file_stream(
             shared_file_id,
             share_id,
@@ -679,15 +855,15 @@
             max_chunk_size=max_chunk_size,
             callback=callback,
             encrypt_password=encrypt_password,
         )
 
 
 class AliOpenPCSApi:
-    """Aliyundrive Open PCS Api
+    """Alipan drive PCS Open Api
 
     This is the wrapper of `AliPCS`. It parses the content of response of raw
     AliPCS requests to some inner data structions.
     """
 
     def __init__(
         self,
@@ -700,14 +876,19 @@
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
         token_type: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
+        error_max_retries: int = 2,
+        max_keepalive_connections: int = 50,
+        max_connections: int = 50,
+        keepalive_expiry: float = 10 * 60,
+        connection_max_retries: int = 2,
     ):
         self._aliopenpcs = AliOpenPCS(
             refresh_token,
             access_token=access_token,
             expire_time=expire_time,
             client_id=client_id,
             client_secret=client_secret,
@@ -715,14 +896,19 @@
             user_id=user_id,
             user_name=user_name,
             nick_name=nick_name,
             token_type=token_type,
             default_drive_id=default_drive_id,
             role=role,
             status=status,
+            error_max_retries=error_max_retries,
+            max_keepalive_connections=max_keepalive_connections,
+            max_connections=max_connections,
+            keepalive_expiry=keepalive_expiry,
+            connection_max_retries=connection_max_retries,
         )
 
         # The path tree is for user's own files
         self._path_tree = PathTree(self)
 
         # Map `share_id` to a `PathTree` for that shared link
         self._shared_path_tree: DefaultDict[str, PathTree] = defaultdict(partial(PathTree, self))
@@ -775,30 +961,21 @@
     def role(self) -> str:
         return self._aliopenpcs.role
 
     @property
     def status(self) -> str:
         return self._aliopenpcs.status
 
-    def meta(self, *file_ids: str, share_id: str = None) -> List[PcsFile]:
-        """Meta data of `remotepaths`"""
-
-        pcs_files = [PcsFile.root() if fid == "root" else None for fid in file_ids]
-        fids = [fid for fid in file_ids if fid != "root"]
-
-        if fids:
-            info = self._aliopenpcs.meta(*fids, share_id=share_id)
-            pfs = [PcsFile.from_(v.get("body")) for v in info["responses"]]
-            j = 0
-            for i in range(len(pcs_files)):
-                if pcs_files[i] is None:
-                    pcs_files[i] = pfs[j]
-                    j += 1
+    def meta(self, file_id: str, share_id: Optional[str] = None) -> Optional[PcsFile]:
+        """Get meta info of the file"""
 
-        return [pf for pf in pcs_files if pf is not None]
+        info = self._aliopenpcs.meta(file_id, share_id=share_id)
+        if info.get("code") == "NotFound.File":
+            return None
+        return PcsFile.from_(info)
 
     def exists(self, file_id: str) -> bool:
         """Check whether `remotepath` exists"""
 
         return self._aliopenpcs.exists(file_id)
 
     def is_file(self, file_id: str) -> bool:
@@ -810,15 +987,15 @@
         """Check whether `remotepath` is a directory"""
 
         return self._aliopenpcs.is_dir(file_id)
 
     def list(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
@@ -845,32 +1022,34 @@
         )
         next_marker = info["next_marker"]
         return [PcsFile.from_(v) for v in info.get("items", [])], next_marker
 
     def list_iter(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
         recursive: bool = False,
         include_dir: bool = True,
-    ) -> Iterator[PcsFile]:
+    ) -> Iterable[PcsFile]:
         """Iterate the directory by its `file_id`
 
         Iterate all files and directories at the directory (which has the `file_id`).
         """
 
         next_marker = ""
-        pcs_file = self.meta(file_id, share_id=share_id)[0]
+        pcs_file = self.meta(file_id, share_id=share_id)
+        if pcs_file is None:
+            return
         dirname = pcs_file.name
         while True:
             pcs_files, next_marker = self.list(
                 file_id,
                 share_id=share_id,
                 desc=desc,
                 name=name,
@@ -905,42 +1084,42 @@
                             yield sub_pf
                 else:
                     yield pf
 
             if not next_marker:
                 return
 
-    def path(self, remotepath: str, share_id: str = None) -> Optional[PcsFile]:
+    def path(self, remotepath: str, share_id: Optional[str] = None) -> Optional[PcsFile]:
         """Get the pcs file's info by the given absolute `remotepath`"""
 
         if share_id:
             return self._shared_path_tree[share_id].search(remotepath=remotepath, share_id=share_id)
         else:
             return self._path_tree.search(remotepath=remotepath)
 
-    def paths(self, *remotepaths: str, share_id: str = None) -> List[Optional[PcsFile]]:
+    def paths(self, *remotepaths: str, share_id: Optional[str] = None) -> List[Optional[PcsFile]]:
         """Get the pcs files' info by the given absolute `remotepaths`"""
 
-        return [self.path(rp, share_id=share_id) for rp in remotepaths]
+        return [self.path(remote_path, share_id=share_id) for remote_path in remotepaths]
 
     def list_path_iter(
         self,
         remotepath: str,
-        file_id: str = None,
-        share_id: str = None,
+        file_id: Optional[str] = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
         recursive: bool = False,
         include_dir: bool = True,
-    ) -> Iterator[PcsFile]:
+    ) -> Iterable[PcsFile]:
         """Iterate the `remotepath`"""
 
         if not file_id:
             pf = self.path(remotepath, share_id=share_id)
             if not pf:
                 return
             file_id = pf.file_id
@@ -962,16 +1141,16 @@
         ):
             p.path = join_path(dirname, p.path)
             yield p
 
     def list_path(
         self,
         remotepath: str,
-        file_id: str = None,
-        share_id: str = None,
+        file_id: Optional[str] = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
@@ -1012,25 +1191,62 @@
                 pcs_file.download_url = pcs_url.url
         return pcs_file
 
     def file_stream(
         self,
         file_id: str,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         """File stream as a normal io"""
 
         return self._aliopenpcs.file_stream(
             file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
         )
 
 
 class AliPCSApiMix(AliPCSApi):
+    """The class mixed with `AliPCSApi` and `AliOpenPCSApi`
+
+    Only following methods are used from AliOpenPCSApi:
+        - download_link
+        - update_download_url
+        - file_stream
+    Other methods are used from AliPCSApi.
+
+    Args:
+        web_refresh_token (str): The refresh token from browser.
+        web_access_token (str, optional): The access token from browser.
+        web_token_type (str): The token type. Default is "Bearer".
+        web_expire_time (int, optional): The expire time of the token.
+
+        openapi_refresh_token (str): The refresh token from alipan openapi.
+        openapi_access_token (str, optional): The access token from alipan openai.
+        openapi_token_type (str): The token type. Default is "Bearer".
+        openapi_expire_time (int, optional): The expire time of the token.
+        client_id (str, optional): The client id of the app for openapi.
+        client_secret (str, optional): The client secret of the app for openapi.
+        client_server (str, optional): The client server of the app for openapi to access token.
+            If `client_id` and `client_secret` are provided, the `client_server` is not needed, vice versa.
+
+        user_id (str, optional): The user id of the user.
+        user_name (str, optional): The user name of the user.
+        nick_name (str, optional): The nick name of the user.
+        device_id (str, optional): The device id of the user.
+        default_drive_id (str, optional): The default drive id of the user.
+        role (str, optional): The role of the user.
+        status (str, optional): The status of the user.
+        error_max_retries (int): The max retries when a client request error occurs. Default is 2.
+        max_keepalive_connections (int): The max keepalive connections. Default is 50.
+        max_connections (int): The max number of connections in the pool. Default is 50.
+        keepalive_expiry (float): The keepalive expiry. Default is 10 * 60 seconds.
+        connection_max_retries (int): The max retries when a connection error occurs. Default is 2.
+    """
+
     def __init__(
         self,
         web_refresh_token: str,
         web_access_token: str = "",
         web_token_type: str = "",
         web_expire_time: int = 0,
         openapi_refresh_token: str = "",
@@ -1043,27 +1259,37 @@
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
         device_id: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
+        error_max_retries: int = 2,
+        max_keepalive_connections: int = 50,
+        max_connections: int = 50,
+        keepalive_expiry: float = 10 * 60,
+        connection_max_retries: int = 2,
     ):
         super().__init__(
             refresh_token=web_refresh_token,
             access_token=web_access_token,
             token_type=web_token_type,
             expire_time=web_expire_time,
             user_id=user_id,
             user_name=user_name,
             nick_name=nick_name,
             device_id=device_id,
             default_drive_id=default_drive_id,
             role=role,
             status=status,
+            error_max_retries=error_max_retries,
+            max_keepalive_connections=max_keepalive_connections,
+            max_connections=max_connections,
+            keepalive_expiry=keepalive_expiry,
+            connection_max_retries=connection_max_retries,
         )
 
         self._aliopenpcsapi: Optional[AliOpenPCSApi] = None
         if openapi_refresh_token and ((client_id and client_secret) or client_server):
             self._aliopenpcsapi = AliOpenPCSApi(
                 refresh_token=openapi_refresh_token,
                 access_token=openapi_access_token,
@@ -1074,14 +1300,19 @@
                 client_server=client_server,
                 user_id=user_id,
                 user_name=user_name,
                 nick_name=nick_name,
                 default_drive_id=default_drive_id,
                 role=role,
                 status=status,
+                error_max_retries=error_max_retries,
+                max_keepalive_connections=max_keepalive_connections,
+                max_connections=max_connections,
+                keepalive_expiry=keepalive_expiry,
+                connection_max_retries=connection_max_retries,
             )
 
     def download_link(self, file_id: str) -> Optional[PcsDownloadUrl]:
         """Get the download link of the `file_id`"""
 
         if self._aliopenpcsapi is not None:
             return self._aliopenpcsapi.download_link(file_id)
@@ -1101,15 +1332,15 @@
         else:
             return super().update_download_url(pcs_file)
 
     def file_stream(
         self,
         file_id: str,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         """File stream as a normal io"""
 
         if self._aliopenpcsapi is not None:
             return self._aliopenpcsapi.file_stream(
                 file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
@@ -1190,35 +1421,36 @@
         """Add a node to self._file_id_to_node"""
 
         self._file_id_to_node[node.file_id] = node
 
     def _pop(self, file_id: str) -> Optional[_Node]:
         """Pop a node from self._file_id_to_node"""
 
-        try:
-            return self._file_id_to_node.pop(file_id)
-        except KeyError:
-            return None
+        return self._file_id_to_node.pop(file_id, None)
 
-    def search(self, remotepath: str = "", topdown: Iterable[str] = [], share_id: str = None) -> Optional[PcsFile]:
+    def search(
+        self, remotepath: str = "", topdown: Iterable[str] = [], share_id: Optional[str] = None
+    ) -> Optional[PcsFile]:
         """Search the PcsFile which has remote path as `remotepath`
         or has the tree path `topdown`
         """
 
         if not topdown:
             assert remotepath.startswith("/")
             topdown = split_posix_path(remotepath)
 
         node = self._dfs(list(topdown), self.root, share_id=share_id)
         if node:
             return deepcopy(node.pcs_file)
         else:
             return None
 
-    def _dfs(self, topdown: List[str], root: _Node, pull: bool = True, share_id: str = None) -> Optional[_Node]:
+    def _dfs(
+        self, topdown: List[str], root: _Node, pull: bool = True, share_id: Optional[str] = None
+    ) -> Optional[_Node]:
         """Search a node with the path `topdown` using depth first search"""
 
         if not topdown:
             return root
 
         next_key = topdown[0]
         if next_key == "/":
@@ -1249,15 +1481,15 @@
         if not topdown:
             assert remotepath.startswith("/")
             topdown = split_posix_path(remotepath)
 
         parts = list(topdown)
         dest = parts[-1]
         parent = parts[:-1]
-        assert len(parent) > 0, "NO pop root"
+        assert len(parent) > 0, "Can not pop root"
 
         node = self._dfs(list(parent), self.root, pull=False)
         if node:
             if dest in node.sub_nodes:
                 sub_node = node.pop(dest)
                 if sub_node:
                     self._pop(sub_node.file_id)
```

### Comparing `alipcs_py-0.7.0/alipcs_py/alipcs/inner.py` & `alipcs_py-0.8.0/alipcs_py/alipcs/inner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-from typing import Optional, List, Dict, Any, TYPE_CHECKING
+from typing import Optional, List, Dict, Any, TYPE_CHECKING, Tuple, TypeVar
 from dataclasses import dataclass
-from collections import namedtuple
 import time
 import re
 import urllib.parse
 import warnings
 
+
 from alipcs_py.common.date import iso_8601_to_timestamp, now_timestamp
 
 if TYPE_CHECKING:
     from alipcs_py.alipcs.api import AliPCSApi
 
 
+# FromTo type is used to represent the direction of the file transfer
+# When the direction is from local to remote, the type is FromTo[PathType, str]
+# When the direction is from remote to local, the type is FromTo[str, PathType]
+F = TypeVar("F")
+T = TypeVar("T")
+FromTo = Tuple[F, T]
+
+
 @dataclass
 class PcsRapidUploadInfo:
     """Rapid Upload Info"""
 
     content_hash: str
     content_length: int
     content_hash_name: str = "sha1"
@@ -47,42 +55,57 @@
     @staticmethod
     def default_hash_link_protocol() -> str:
         return "ali"
 
 
 @dataclass
 class PcsFile:
-    """
-    A Ali PCS file
+    """The remote file/directory information
 
-    path: str  # remote absolute path
-    is_dir: Optional[bool] = None
-    is_file: Optional[bool] = None
-    fs_id: Optional[int] = None  # file id
-    size: Optional[int] = None
-    md5: Optional[str] = None
-    block_list: Optional[List[str]] = None  # block md5 list
-    category: Optional[int] = None
-    user_id: Optional[int] = None
-    created_at: Optional[int] = None  # server created time
-    updated_at: Optional[int] = None  # server updated time
-    shared: Optional[bool] = None  # this file is shared if True
+    Args:
+        file_id (str): The unique identifier of the file.
+        name (str): The name of the file.
+        parent_file_id (str): The unique identifier of the parent file. If the parent directory  is '/', its id is 'root'.
+        type (str): The type of the file, such as "file" or "folder".
+        is_dir (bool): Indicates whether the file is a directory.
+        is_file (bool): Indicates whether the file is a regular file.
+        size (int): The size of the file in bytes.
+        path (str): The remote path of the file. Default is the name of the file.
+        created_at (Optional[int]): The timestamp of when the file was created on the server.
+        updated_at (Optional[int]): The timestamp of when the file was last updated on the server.
+        file_extension (Optional[str]): The file extension of the file.
+        content_type (Optional[str]): The content type of the file.
+        mime_type (Optional[str]): The MIME type of the file.
+        mime_extension (Optional[str]): The MIME type extension of the file.
+        labels (Optional[List[str]]): A list of labels associated with the file.
+        status (Optional[str]): The status of the file.
+        hidden (Optional[bool]): Indicates whether the file is hidden.
+        starred (Optional[bool]): Indicates whether the file is starred.
+        category (Optional[str]): The category of the file.
+        punish_flag (Optional[int]): A flag indicating whether the file has been punished.
+        encrypt_mode (Optional[str]): The encryption mode of the file.
+        drive_id (Optional[str]): The unique identifier of the drive the file is stored in.
+        domain_id (Optional[str]): The unique identifier of the domain the file is associated with.
+        upload_id (Optional[str]): The unique identifier of the file upload.
+        async_task_id (Optional[str]): The unique identifier of the asynchronous task associated with the file.
+        rapid_upload_info (Optional[PcsRapidUploadInfo]): Information about the rapid upload of the file.
+        download_url (Optional[str]): The URL for downloading the file.
     """
 
     file_id: str
     name: str
     parent_file_id: str
     type: str
     is_dir: bool
     is_file: bool
     size: int = 0
-    path: str = ""  # remote absolute path
+    path: str = ""
 
     created_at: Optional[int] = None  # server created time
-    updated_at: Optional[int] = None  # server updated time (updated time)
+    updated_at: Optional[int] = None  # server updated time
 
     file_extension: Optional[str] = None
     content_type: Optional[str] = None
     mime_type: Optional[str] = None
     mime_extension: Optional[str] = None
     labels: Optional[List[str]] = None
 
@@ -116,22 +139,24 @@
                 content_hash=info.get("content_hash"),
                 content_length=info.get("size"),
                 content_hash_name=info.get("content_hash_name"),
                 crc64_hash=info.get("crc64_hash"),
                 name=info.get("name"),
             )
 
+        filename = info.get("name") or info.get("file_name", "")
         return PcsFile(
             file_id=info.get("file_id", ""),
-            name=info.get("name", ""),
+            name=filename,
             parent_file_id=info.get("parent_file_id", ""),
             type=info.get("type", ""),
             is_dir=info.get("type") == "folder",
             is_file=info.get("type") == "file",
             size=info.get("size"),
+            path=filename,  # Default path is the name of the file
             created_at=created_at,
             updated_at=updated_at,
             file_extension=info.get("file_extension"),
             content_type=info.get("content_type"),
             mime_type=info.get("mime_type"),
             mime_extension=info.get("mime_extension"),
             labels=info.get("labels"),
@@ -172,33 +197,14 @@
             mod = re.search(r"oss-expires=(\d+)", self.download_url)
             if mod:
                 expire_time = float(mod.group(1))
                 if time.time() < expire_time - 5:
                     return False
         return True
 
-    def update_download_url(self, api: "AliPCSApi"):
-        """Update the download url if it expires"""
-
-        warnings.warn(
-            "This method is deprecated and will be removed in a future version, use `update_download_url` in `AliPCSApi` instead",
-            DeprecationWarning,
-        )
-
-        if self.is_file:
-            if self.download_url_expires():
-                pcs_url = api.download_link(self.file_id)
-                if pcs_url:
-                    self.download_url = pcs_url.url
-            else:
-                if getattr(api, "_aliopenpcsapi", None):
-                    pcs_url = api.download_link(self.file_id)
-                    if pcs_url:
-                        self.download_url = pcs_url.url
-
 
 @dataclass
 class PcsUploadUrl:
     upload_url: Optional[str] = None
     internal_upload_url: Optional[str] = None
     content_type: Optional[str] = None
     part_number: Optional[int] = None
@@ -415,17 +421,14 @@
             info=info,
         )
 
     def is_expired(self) -> bool:
         return time.time() >= self.expire_time
 
 
-FromTo = namedtuple("FromTo", ["from_", "to_"])
-
-
 @dataclass
 class PcsSpace:
     used_size: int
     total_size: int
 
     @staticmethod
     def from_(info) -> "PcsSpace":
@@ -589,14 +592,26 @@
     cdn_url: Optional[str] = None
     size: Optional[int] = None
 
     method: Optional[str] = None
     expiration: Optional[int] = None
     ratelimit: Optional[PcsRateLimit] = None
 
+    def expires(self) -> bool:
+        """Check whether the `self.download_url` expires"""
+
+        url = self.download_url or self.url
+        if url:
+            mod = re.search(r"oss-expires=(\d+)", url)
+            if mod:
+                expire_time = float(mod.group(1))
+                if time.time() < expire_time - 5:
+                    return False
+        return True
+
     @staticmethod
     def from_(info) -> "PcsDownloadUrl":
         expiration = None
         if info.get("expiration"):
             expiration = iso_8601_to_timestamp(info["expiration"])
 
         return PcsDownloadUrl(
```

### Comparing `alipcs_py-0.7.0/alipcs_py/alipcs/pcs.py` & `alipcs_py-0.8.0/alipcs_py/alipcs/pcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 from alipcs_py.common.date import now_timestamp, iso_8601_to_timestamp, timestamp_to_iso_8601
 from alipcs_py.common import constant
 from alipcs_py.common.io import RangeRequestIO, DEFAULT_MAX_CHUNK_SIZE, ChunkIO, total_len
 from alipcs_py.common.cache import timeout_cache
 from alipcs_py.common.crypto import generate_secp256k1_keys
-from alipcs_py.alipcs.errors import AliPCSError, parse_error, handle_error
-from alipcs_py.alipcs.errors import assert_ok
+from alipcs_py.alipcs.errors import AliPCSError, make_alipcs_error, handle_error
 from alipcs_py.alipcs.inner import SharedAuth
+from alipcs_py.common.net import make_http_session
 
 
 UPLOAD_CHUNK_SIZE = 10 * constant.OneM
 
 APP_ID = "5dde4e1bdf9e4966b387ba58f4b3fdc3"
 
 ALIYUNDRIVE_COM = "https://www.aliyundrive.com"
 ALIYUNDRIVE_COM_API = "https://api.aliyundrive.com"
 ALIYUNDRIVE_OPENAPI_DOMAIN = "https://openapi.aliyundrive.com"
 
-# TODO: Update UA
-PCS_UA = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
+PCS_UA = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
 PCS_HEADERS = {"Origin": ALIYUNDRIVE_COM, "Referer": ALIYUNDRIVE_COM + "/", "User-Agent": PCS_UA}
 
 CheckNameMode = Literal[
     "overwrite",  # 直接覆盖，以后多版本有用
     "auto_rename",  # 自动换一个随机名称
     "refuse",  # 不会创建，告诉你已经存在
     "ignore",  # 会创建重名的
@@ -47,14 +46,17 @@
     f"""Aliyundrive PCS Nodes which use {ALIYUNDRIVE_COM_API}"""
 
     Token = "v2/account/token"
     Refresh = "token/refresh"
     CreateSession = "users/v1/users/device/create_session"
 
     FileList = "adrive/v3/file/list"
+    Walk = "v2/file/walk"
+    GetPath = "adrive/v1/file/get_path"
+    MetaByPath = "v2/file/get_by_path"
     Meta = "v2/file/get"
     Search = "adrive/v3/file/search"
     DownloadUrl = "v2/file/get_download_url"
 
     CreateFile = "v2/file/create"
     UploadUrl = "v2/file/get_upload_url"
     UploadComplete = "v2/file/complete"
@@ -82,15 +84,39 @@
 
 
 # The Lock is used to refresh token
 _LOCK = threading.Lock()
 
 
 class AliPCS:
-    """`AliPCS` provides pcs's apis which return raw json"""
+    """Alipan Drive Personal Cloud Service Raw API
+
+    The core class is used to interact with Alipan Drive Personal Cloud Service.
+    It provides the basic operations of the service and handles the raw requests and responses.
+
+    An `AliPCSError` error will be raised if the code of the response occurs.
+
+    Args:
+        refresh_token (str): The refresh token of the user.
+        access_token (str, optional): The access token of the user.
+        token_type (str): The token type. Default is "Bearer".
+        expire_time (int, optional): The expire time of the token.
+        user_id (str, optional): The user id of the user.
+        user_name (str, optional): The user name of the user.
+        nick_name (str, optional): The nick name of the user.
+        device_id (str, optional): The device id of the user.
+        default_drive_id (str, optional): The default drive id of the user.
+        role (str, optional): The role of the user.
+        status (str, optional): The status of the user.
+        error_max_retries (int): The max retries when a client request error occurs. Default is 2.
+        max_keepalive_connections (int): The max keepalive connections. Default is 50.
+        max_connections (int): The max number of connections in the pool. Default is 50.
+        keepalive_expiry (float): The keepalive expiry. Default is 10 * 60 seconds.
+        connection_max_retries (int): The max retries when a connection error occurs. Default is 2.
+    """
 
     SHARE_AUTHS: Dict[str, SharedAuth] = {}
 
     def __init__(
         self,
         refresh_token: str,
         access_token: str = "",
@@ -99,16 +125,29 @@
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
         device_id: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
+        error_max_retries: int = 2,
+        max_keepalive_connections: int = 50,
+        max_connections: int = 50,
+        keepalive_expiry: float = 10 * 60,
+        connection_max_retries: int = 2,
     ):
-        self._session = requests.Session()
+        self._session = make_http_session(
+            max_keepalive_connections=max_keepalive_connections,
+            max_connections=max_connections,
+            keepalive_expiry=keepalive_expiry,
+            max_retries=connection_max_retries,
+        )
+
+        self._error_max_retries = error_max_retries
+
         self._refresh_token = refresh_token
         self._access_token = access_token
         self._token_type = token_type
         self._expire_time = expire_time
 
         self._user_id = user_id
         self._user_name = user_name
@@ -240,26 +279,26 @@
 
         try:
             resp = self._session.request(
                 method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
             )
             return resp
         except Exception as err:
-            raise AliPCSError("AliPCS._request", cause=err)
+            raise AliPCSError("AliPCS._request") from err
 
     def refresh(self):
         """Refresh token"""
 
         url = PcsNode.Refresh.url()
         data = dict(refresh_token=self._refresh_token)
         resp = self._request(Method.Post, url, json=data, refresh=True)
         info = resp.json()
 
         if "code" in info:
-            err = parse_error(info["code"], info=info)
+            err = make_alipcs_error(info["code"], info=info)
             raise err
 
         self._user_id = info["user_id"]
         self._user_name = info["user_name"]
         self._nick_name = info["nick_name"]
 
         self._refresh_token = info["refresh_token"]
@@ -303,91 +342,180 @@
 
         info = do(self)
         if info["result"] and info["success"]:
             self._signature = sign
 
         return info
 
-    def meta(self, *file_ids: str, share_id: str = None):
-        assert "root" not in file_ids, '"root" has NOT meta info'
+    @handle_error
+    def path_traceback(self, file_id: str, share_id: Optional[str] = None):
+        """Traceback the path of the file by its file_id
+
+        Return the list of all parent directories' info from the file to the top level directory.
+        """
+
+        url = PcsNode.GetPath.url()
 
         headers = dict(PCS_HEADERS)
         headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
 
         if share_id:
             share_token = self.share_token(share_id)
             assert share_token, "Need share_token"
 
             headers["x-share-token"] = share_token
 
-        responses = []
-        for file_id in file_ids:
-            data = dict(
-                file_id=file_id,
-                fields="*",
-                image_thumbnail_process="image/resize,w_400/format,jpeg",
-                image_url_process="image/resize,w_375/format,jpeg",
-                video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_375",
-            )
+        data = dict(file_id=file_id, fields="*")
 
-            if share_id:
-                data["share_id"] = share_id
-            else:
-                data["drive_id"] = self.default_drive_id
+        if share_id:
+            data["share_id"] = share_id
+        else:
+            data["drive_id"] = self.default_drive_id
 
-            url = PcsNode.Meta.url()
-            resp = self._request(Method.Post, url, headers=headers, json=data)
-            info = resp.json()
-            responses.append(dict(body=info))
+        resp = self._request(Method.Post, url, headers=headers, json=data)
+        info = resp.json()
+        return info
+
+    @handle_error
+    def meta_by_path(self, remotepath: str):
+        """Get meta info of the file by its path
+
+        Can not get the shared files' meta info.
+        """
+
+        assert remotepath.startswith("/"), "Path should start with '/'"
+
+        url = PcsNode.MetaByPath.url()
+        headers = dict(PCS_HEADERS)
+        headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
+
+        data = dict(
+            file_path=remotepath,
+            fields="*",
+            drive_id=self.default_drive_id,
+            image_thumbnail_process="image/resize,w_400/format,jpeg",
+            image_url_process="image/resize,w_375/format,jpeg",
+            video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_375",
+        )
+
+        resp = self._request(Method.Post, url, headers=headers, json=data)
+        info = resp.json()
+        return info
+
+    @handle_error
+    def meta(self, file_id: str, share_id: Optional[str] = None):
+        """Get meta info of the file by its file_id"""
 
-        return dict(responses=responses)
+        url = PcsNode.Meta.url()
+        headers = dict(PCS_HEADERS)
+        headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
+
+        if share_id:
+            share_token = self.share_token(share_id)
+            assert share_token, "Need share_token"
+
+            headers["x-share-token"] = share_token
+
+        data = dict(
+            file_id=file_id,
+            fields="*",
+            image_thumbnail_process="image/resize,w_400/format,jpeg",
+            image_url_process="image/resize,w_375/format,jpeg",
+            video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_375",
+        )
+
+        if share_id:
+            data["share_id"] = share_id
+        else:
+            data["drive_id"] = self.default_drive_id
+
+        resp = self._request(Method.Post, url, headers=headers, json=data)
+        info = resp.json()
+        return info
 
     def exists(self, file_id: str) -> bool:
+        """Check whether the file exists
+
+        Return True if the file exists and does not in the trash else False.
+        """
+
         if file_id == "root":
             return True
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
+        if info.get("parent_file_id") == "recyclebin":
+            # The file is not exists or in the trash
             return False
         else:
             return True
 
+    def exists_in_trash(self, file_id: str) -> bool:
+        """Check whether the file exists in the trash
+
+        Return True if the file exists in the trash else False.
+        """
+
+        if file_id == "recyclebin":
+            return True
+
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
+        if info.get("parent_file_id") == "recyclebin":
+            return True
+        else:
+            return False
+
     def is_file(self, file_id: str) -> bool:
         if file_id == "root":
             return False
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
-            return False
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
         if info["type"] == "file":
             return True
         else:
             return False
 
     def is_dir(self, file_id: str) -> bool:
         if file_id == "root":
             return True
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
-            return False
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
         if info["type"] == "folder":
             return True
         else:
             return False
 
-    @assert_ok
     @handle_error
     def list(
         self,
         file_id: str,
-        share_id: str = "",
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14400,
@@ -437,14 +565,57 @@
             data["share_id"] = share_id
             data.pop("drive_id")
             headers["x-share-token"] = share_token
 
         resp = self._request(Method.Post, url, headers=headers, json=data)
         return resp.json()
 
+    @handle_error
+    def walk(
+        self,
+        file_id: str,
+        share_id: Optional[str] = None,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
+        next_marker: str = "",
+    ):
+        """Walk through the directory tree which has `file_id`"""
+
+        url = PcsNode.Walk.url()
+
+        headers = dict(PCS_HEADERS)
+        headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
+
+        data = dict(
+            all=all,
+            drive_id=self.default_drive_id,
+            fields="*",
+            limit=limit,
+            parent_file_id=file_id,
+            url_expire_sec=url_expire_sec,
+            image_thumbnail_process="image/resize,w_256/format,jpeg",
+            image_url_process="image/resize,w_1920/format,jpeg/interlace,1",
+            video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_256",
+        )
+        if next_marker:
+            data["marker"] = next_marker
+
+        if share_id:
+            share_token = self.share_token(share_id)
+            assert share_token, "Need share_token"
+
+            data["share_id"] = share_id
+            data.pop("drive_id")
+            headers["x-share-token"] = share_token
+
+        resp = self._request(Method.Post, url, headers=headers, json=data)
+        info = resp.json()
+        return info
+
     @staticmethod
     def part_info_list(part_number: int) -> List[Dict[str, int]]:
         return [dict(part_number=i) for i in range(1, part_number + 1)]
 
     @handle_error
     def create_file(
         self,
@@ -498,14 +669,15 @@
 
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     def prepare_file(self, filename: str, dir_id: str, size: int, pre_hash: str = "", part_number: int = 1):
         return self.create_file(filename, dir_id, size, pre_hash=pre_hash, part_number=part_number)
 
+    @handle_error
     def get_upload_url(self, upload_id: str, file_id: str, part_number: int):
         """Get upload slices' urls
 
         It is useful to get new upload slice url when these urls gotten from
         `AliPCS.prepare_file` or `AliPCS.create_file` are expired.
         """
 
@@ -516,49 +688,46 @@
             drive_id=self.default_drive_id,
             part_info_list=self.part_info_list(part_number),
         )
 
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
-    @handle_error
     def rapid_upload_file(self, filename: str, dir_id: str, size: int, content_hash: str, proof_code: str):
         """Rapid Upload File
 
         size (int): the length of total content.
         content_hash (str): the sha1 of total content.
         """
 
         return self.create_file(filename, dir_id, size, content_hash=content_hash, proof_code=proof_code)
 
-    def upload_slice(self, io: IO, url: str, callback: Callable[[MultipartEncoderMonitor], None] = None) -> None:
+    def upload_slice(self, io: IO, url: str, callback_for_monitor: Optional[Callable[[int], Any]] = None) -> None:
         """Upload the content of io to remote url"""
 
-        cio = ChunkIO(io, total_len(io))
-        monitor = MultipartEncoderMonitor(cio, callback=callback)
+        data = ChunkIO(io, total_len(io))
+        if callback_for_monitor is not None:
+            data = MultipartEncoderMonitor(data, callback=lambda monitor: callback_for_monitor(monitor.bytes_read))
 
         session = requests.Session()
         session.request(
             "PUT",
             url,
             headers=dict(PCS_HEADERS),
-            data=monitor,
+            data=data,
             timeout=(3, 9),  # (connect timeout, read timeout)
         )
 
-    @assert_ok
     @handle_error
     def upload_complete(self, file_id: str, upload_id: str):
         url = PcsNode.UploadComplete.url()
         data = dict(drive_id=self.default_drive_id, file_id=file_id, upload_id=upload_id)
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
     @handle_error
     def search(
         self,
         keyword: str,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
@@ -588,29 +757,27 @@
             image_thumbnail_process="image/resize,w_160/format,jpeg",
             image_url_process="image/resize,w_1920/format,jpeg",
             video_thumbnail_process="video/snapshot,t_0,f_jpg,ar_auto,w_300",
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
     @handle_error
     def makedir(self, dir_id: str, name: str):
         url = PcsNode.CreateWithFolders.url()
         data = dict(
             check_name_mode="refuse",  # or "auto_rename"
             drive_id=self.default_drive_id,
             name=name,
             parent_file_id=dir_id,
             type="folder",
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
     @handle_error
     def batch_operate(
         self, requests_: List[Dict[str, Any]], resource: str = "file", headers: Optional[Dict[str, str]] = None
     ):
         url = PcsNode.Batch.url()
         data = dict(resource=resource, requests=requests_)
         resp = self._request(Method.Post, url, headers=headers, json=data)
@@ -644,15 +811,14 @@
                     to_parent_file_id=dest_id,
                 ),
             )
             requests_.append(req)
 
         return self.batch_operate(requests_, resource="file")
 
-    @assert_ok
     @handle_error
     def rename(self, file_id: str, name: str):
         """Rename the file to `name`"""
 
         url = PcsNode.Update.url()
         data = dict(
             check_name_mode="refuse",
@@ -694,28 +860,26 @@
                 id=file_id,
                 headers={"Content-Type": "application/json"},
                 body=dict(drive_id=self.default_drive_id, file_id=file_id),
             )
             requests_.append(req)
         return self.batch_operate(requests_, resource="file")
 
-    @assert_ok
     @handle_error
     def check_available(self, file_ids: str):
         """Check whether file_ids are available"""
 
         url = PcsNode.Available.url()
         data = dict(
             drive_id=self.default_drive_id,
             file_id_list=list(file_ids),
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
     @handle_error
     def share(self, *file_ids: str, password: str = "", period: int = 0, description: str = ""):
         """Share `remotepaths` to public
 
         period (int): The days for expiring. `0` means no expiring
         """
 
@@ -730,15 +894,14 @@
             file_id_list=list(file_ids),
             share_pwd=password,
             description=description,
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    @assert_ok
     @handle_error
     def list_shared(self, next_marker: str = ""):
         """List shared links"""
 
         url = PcsNode.SharedList.url()
         data = dict(
             creator=self.user_id,
@@ -760,15 +923,14 @@
                 headers={"Content-Type": "application/json"},
                 body=dict(share_id=share_id),
             )
             requests_.append(req)
 
         return self.batch_operate(requests_, resource="file")
 
-    @assert_ok
     @handle_error
     def get_share_token(self, share_id: str, share_password: str = ""):
         """Get share token"""
 
         shared_auth = self.__class__.SHARE_AUTHS.get(share_id)
         if shared_auth is not None:
             share_password = share_password or shared_auth.share_password
@@ -788,15 +950,14 @@
 
     def share_token(self, share_id: str) -> str:
         self.get_share_token(share_id)
 
         shared_auth = self.__class__.SHARE_AUTHS[share_id]
         return shared_auth.share_token
 
-    @assert_ok
     @handle_error
     def shared_info(self, share_id: str):
         """Get shared items info"""
 
         url = PcsNode.SharedInfo.url()
         params = dict(share_id=share_id)
         data = dict(share_id=share_id)
@@ -834,15 +995,14 @@
         assert share_token, "Need share_token"
 
         headers = dict(PCS_HEADERS)
         headers["x-share-token"] = share_token
 
         return self.batch_operate(requests_, resource="file", headers=headers)
 
-    @assert_ok
     @handle_error
     def _get_shared_file_download_url(self, shared_file_id: str, share_id: str, expire_duration: int = 10 * 60):
         url = PcsNode.SharedFileDownloadUrl.url()
         data = dict(expire_sec=expire_duration, file_id=shared_file_id, share_id=share_id)
 
         share_token = self.share_token(share_id)
         assert share_token, "Need share_token"
@@ -858,15 +1018,14 @@
         url = info["url"]
 
         headers = dict(PCS_HEADERS)
         headers["Referer"] = "https://www.aliyundrive.com/"
         resp = requests.get(url, headers=headers, allow_redirects=False)
         return resp.headers["Location"]
 
-    @assert_ok
     @handle_error
     def user_info(self):
         url = PcsNode.User.url()
         resp = self._request(Method.Post, url, json={})
         info1 = resp.json()
 
         headers = dict(PCS_HEADERS)
@@ -878,33 +1037,38 @@
         url = PcsNode.UserVip.url()
         resp = self._request(Method.Post, url, headers=headers, json={})
         info3 = resp.json()
 
         return {**info1, **info2, "user_vip_info": info3}
 
     @timeout_cache(1 * 60 * 60)  # 1 hour timeout
-    @assert_ok
     @handle_error
     def download_link(self, file_id: str):
-        info = self.meta(file_id)["responses"][0]["body"]
+        """Get download link of the file by its file_id
+
+        First try to get the download link from the meta info of the file.
+        If the download link is not in the meta info, then request the getting download url api.
+        """
+
+        info = self.meta(file_id)
         if info.get("url") or info.get("download_url"):
             return info
 
         url = PcsNode.DownloadUrl.url()
         data = dict(drive_id=self.default_drive_id, file_id=file_id)
         headers = dict(PCS_HEADERS)
         headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
         resp = self._request(Method.Post, url, headers=headers, json=data)
         return resp.json()
 
     def file_stream(
         self,
         file_id: str,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         info = self.download_link(file_id)
         url = info.get("url") or info.get("download_url")
 
         headers = {
             "User-Agent": PCS_UA,
@@ -924,15 +1088,15 @@
 
     def shared_file_stream(
         self,
         shared_file_id: str,
         share_id: str,
         expire_duration: int = 10 * 60,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         url = self.shared_file_download_url(shared_file_id, share_id, expire_duration=expire_duration)
 
         headers = {
             "User-Agent": PCS_UA,
             "Connection": "Keep-Alive",
@@ -991,15 +1155,39 @@
     UserVip = "adrive/v1.0/user/getVipInfo"
 
     def url(self) -> str:
         return f"{ALIYUNDRIVE_OPENAPI_DOMAIN}/{self.value}"
 
 
 class AliOpenPCS:
-    """`Aliyundrive Open PCS` provides pcs's apis which return raw json"""
+    """Alipan Drive Personal Cloud Service Raw Open API
+
+    The core class is used to interact with Alipan Drive Personal Cloud Service with open apis.
+    It provides the basic operations of the service and handles the raw requests and responses.
+
+    An `AliPCSError` error will be raised if the code of the response occurs.
+
+    Args:
+        refresh_token (str): The refresh token of the user.
+        access_token (str, optional): The access token of the user.
+        token_type (str): The token type. Default is "Bearer".
+        expire_time (int, optional): The expire time of the token.
+        user_id (str, optional): The user id of the user.
+        user_name (str, optional): The user name of the user.
+        nick_name (str, optional): The nick name of the user.
+        device_id (str, optional): The device id of the user.
+        default_drive_id (str, optional): The default drive id of the user.
+        role (str, optional): The role of the user.
+        status (str, optional): The status of the user.
+        error_max_retries (int): The max retries when a client request error occurs. Default is 2.
+        max_keepalive_connections (int): The max keepalive connections. Default is 50.
+        max_connections (int): The max number of connections in the pool. Default is 50.
+        keepalive_expiry (float): The keepalive expiry. Default is 10 * 60 seconds.
+        connection_max_retries (int): The max retries when a connection error occurs. Default is 2.
+    """
 
     SHARE_AUTHS: Dict[str, SharedAuth] = {}
 
     def __init__(
         self,
         refresh_token: str,
         access_token: str = "",
@@ -1010,20 +1198,32 @@
         client_server: str = "",
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
+        error_max_retries: int = 2,
+        max_keepalive_connections: int = 50,
+        max_connections: int = 50,
+        keepalive_expiry: float = 10 * 60,
+        connection_max_retries: int = 2,
     ):
         assert (
             client_id and client_secret
         ) or client_server, "(client_id and client_secret) or client_server must be set"
 
-        self._session = requests.Session()
+        self._session = make_http_session(
+            max_keepalive_connections=max_keepalive_connections,
+            max_connections=max_connections,
+            keepalive_expiry=keepalive_expiry,
+            max_retries=connection_max_retries,
+        )
+
+        self._error_max_retries = error_max_retries
 
         self._refresh_token = refresh_token
         self._access_token = access_token
         self._token_type = token_type
         self._expire_time = expire_time
 
         self._client_id = client_id
@@ -1154,15 +1354,15 @@
 
         try:
             resp = self._session.request(
                 method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
             )
             return resp
         except Exception as err:
-            raise AliPCSError("AliPCS._request", cause=err)
+            raise AliPCSError("AliPCS._request") from err
 
     def _update_refresh_token(self):
         """Update refresh token"""
 
         data = dict(refresh_token=self._refresh_token, grant_type="refresh_token")
         if self._client_id and self._client_secret:
             url = OpenPcsNode.UpdateRefreshToken.url()
@@ -1171,15 +1371,15 @@
         else:
             url = urljoin(self._client_server, OpenPcsNode.UpdateRefreshToken.value)
 
         resp = self._request(Method.Post, url, json=data, refresh=True)
         info = resp.json()
 
         if "code" in info:
-            err = parse_error(info["code"], info=info)
+            err = make_alipcs_error(info["code"], info=info)
             raise err
 
         self._refresh_token = info["refresh_token"]
         self._access_token = info["access_token"]
         self._token_type = info["token_type"]
         self._expire_time = now_timestamp() + info["expires_in"]
 
@@ -1191,83 +1391,85 @@
         url = OpenPcsNode.DriveInfo.url()
         data = dict()
 
         resp = self._request(Method.Post, url, json=data)
         info = resp.json()
 
         if "code" in info:
-            err = parse_error(info["code"], info=info)
+            err = make_alipcs_error(info["code"], info=info)
             raise err
 
         self._user_id = info["user_id"]
         self._user_name = info["user_name"]
         self._nick_name = info["nick_name"]
         self._default_drive_id = info["default_drive_id"]
         self._domain_id = info.get("domain_id")
         self._role = info.get("role")
         self._status = info.get("status")
 
         return info
 
-    def meta(self, *file_ids: str, share_id: str = None):
-        assert "root" not in file_ids, '"root" has NOT meta info'
-
-        responses = []
-        for file_id in file_ids:
-            data = dict(file_id=file_id, fields="*", drive_id=self.default_drive_id)
-            url = OpenPcsNode.Meta.url()
-            resp = self._request(Method.Post, url, json=data)
-            info = resp.json()
-            responses.append(dict(body=info))
-
-        return dict(responses=responses)
+    @handle_error
+    def meta(self, file_id: str, share_id: Optional[str] = None):
+        data = dict(file_id=file_id, fields="*", drive_id=self.default_drive_id)
+        url = OpenPcsNode.Meta.url()
+        resp = self._request(Method.Post, url, json=data)
+        info = resp.json()
+        return info
 
     def exists(self, file_id: str) -> bool:
         if file_id == "root":
             return True
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
-            return False
-        else:
-            return True
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
+        return True
 
     def is_file(self, file_id: str) -> bool:
         if file_id == "root":
             return False
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
-            return False
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
         if info["type"] == "file":
             return True
         else:
             return False
 
     def is_dir(self, file_id: str) -> bool:
         if file_id == "root":
             return True
 
-        r = self.meta(file_id)
-        info = r["responses"][0]["body"]
-        if info.get("code") == "NotFound.File":
-            return False
+        try:
+            info = self.meta(file_id)
+        except AliPCSError as err:
+            if err.error_code and err.error_code.startswith("NotFound."):
+                return False
+            raise err
+
         if info["type"] == "folder":
             return True
         else:
             return False
 
-    @assert_ok
     @handle_error
     def list(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: Optional[str] = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
         limit: int = 200,
         url_expire_sec: int = 14200,
@@ -1308,27 +1510,26 @@
         return resp.json()
 
     @staticmethod
     def part_info_list(part_number: int) -> List[Dict[str, int]]:
         return [dict(part_number=i) for i in range(1, part_number + 1)]
 
     @timeout_cache(4 * 60 * 60)  # 4 hour timeout
-    @assert_ok
     @handle_error
     def download_link(self, file_id: str):
         url = OpenPcsNode.DownloadUrl.url()
         data = dict(drive_id=self.default_drive_id, file_id=file_id, expire_sec=14400)
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     def file_stream(
         self,
         file_id: str,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[..., None]] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         info = self.download_link(file_id)
         url = info["url"]
 
         headers = {
             "User-Agent": PCS_UA,
@@ -1375,15 +1576,15 @@
 
         try:
             resp = self._session.request(
                 method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
             )
             return resp
         except Exception as err:
-            raise AliPCSError("AliOpenAuth._request", cause=err)
+            raise AliPCSError("AliOpenAuth._request") from err
 
     @staticmethod
     def qrcode_url(sid: str) -> str:
         return OpenPcsNode.QrcodeUrl.url().format(sid)
 
     @handle_error
     def get_qrcode_info(self):
```

### Comparing `alipcs_py-0.7.0/alipcs_py/alipcs/phone.py` & `alipcs_py-0.8.0/alipcs_py/alipcs/phone.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/alipcs/tree.py` & `alipcs_py-0.8.0/alipcs_py/alipcs/tree.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/app/account.py` & `alipcs_py-0.8.0/alipcs_py/app/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         """Serialize to local path"""
 
         data_path = data_path or self._data_path
         assert data_path, "No data path"
 
         data_path = Path(data_path).expanduser()
         if not data_path.parent.exists():
-            data_path.parent.mkdir(parents=True)
+            data_path.parent.mkdir(parents=True, exist_ok=True)
 
         apis = self._apis
         self._apis = {}  # Ignore to save apis
 
         pickle.dump(self, open(data_path, "wb"))
 
         self._apis = apis
```

### Comparing `alipcs_py-0.7.0/alipcs_py/app/app.py` & `alipcs_py-0.8.0/alipcs_py/app/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,21 +43,20 @@
 from alipcs_py.commands.list_files import list_files
 from alipcs_py.commands.cat import cat as _cat
 from alipcs_py.commands import file_operators
 from alipcs_py.commands.search import search as _search
 from alipcs_py.commands.download import (
     download as _download,
     Downloader,
-    DownloadParams,
     DEFAULT_DOWNLOADER,
     DEFAULT_CONCURRENCY,
     DEFAULT_CHUNK_SIZE,
 )
 from alipcs_py.commands.play import play as _play, Player, DEFAULT_PLAYER
-from alipcs_py.commands.upload import upload as _upload, from_tos, CPU_NUM, UploadType
+from alipcs_py.commands.upload import upload as _upload, from_tos, CPU_NUM
 from alipcs_py.commands.sync import sync as _sync
 from alipcs_py.commands import share as _share
 from alipcs_py.commands.server import start_server
 from alipcs_py.commands.log import get_logger
 from alipcs_py.storage.store import AliPCSApiMixWithSharedStore, SharedStore
 from alipcs_py.config import AppConfig
 from alipcs_py.app.config import init_config
@@ -324,15 +323,15 @@
         if cmd_name not in ALIAS:
             ctx.fail(f"No command: {cmd_name}")
 
         normal_cmd_name = ALIAS[cmd_name]
         return click.Group.get_command(self, ctx, normal_cmd_name)
 
     def list_commands(self, ctx):
-        return self.commands
+        return list(self.commands)
 
 
 _APP_DOC = f"""AliPCS App v{__version__}
 
     \b
     如果第一次使用，你需要运行 `AliPCS-Py useradd` 添加 `refresh_token`。
     如何获取 `refresh_token` 见 https://github.com/PeterDing/AliPCS-Py#%E6%B7%BB%E5%8A%A0%E7%94%A8%E6%88%B7
@@ -1043,15 +1042,17 @@
             share_id=share_id,
             share_url=share_url,
             password=password,
             sifters=sifters,
             recursive=recursive,
             from_index=from_index,
             downloader=getattr(Downloader, downloader),
-            downloadparams=DownloadParams(concurrency=concurrency, chunk_size=chunk_size, quiet=quiet),
+            concurrency=concurrency,
+            chunk_size=chunk_size,
+            show_progress=not quiet,
             out_cmd=out_cmd,
             encrypt_password=encrypt_password,
         )
     else:
         pwd = _pwd(ctx)
         remotepaths = [join_path(pwd, r) for r in remotepaths]
         _download(
@@ -1059,15 +1060,17 @@
             remotepaths,
             file_id,
             outdir,
             sifters=sifters,
             recursive=recursive,
             from_index=from_index,
             downloader=getattr(Downloader, downloader),
-            downloadparams=DownloadParams(concurrency=concurrency, chunk_size=chunk_size, quiet=quiet),
+            concurrency=concurrency,
+            chunk_size=chunk_size,
+            show_progress=not quiet,
             out_cmd=out_cmd,
             encrypt_password=encrypt_password,
         )
 
 
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
@@ -1138,14 +1141,15 @@
         sifters.append(IncludeSifter(include_regex, regex=True))
     if exclude:
         sifters.append(ExcludeSifter(exclude, regex=False))
     if exclude_regex:
         sifters.append(ExcludeSifter(exclude_regex, regex=True))
 
     local_server = ""
+    ps = None
     if use_local_server:
         if share_id or file_id:
             assert ValueError("Recently local server can't play others shared items and using `file_id`")
 
         encrypt_password = encrypt_password or _encrypt_password(ctx)
 
         host = "localhost"
@@ -1206,32 +1210,21 @@
             quiet=quiet,
             shuffle=shuffle,
             ignore_ext=ignore_ext,
             out_cmd=out_cmd,
             local_server=local_server,
         )
 
-    if use_local_server:
+    if use_local_server and ps is not None:
         ps.terminate()
 
 
 @app.command()
 @click.argument("localpaths", nargs=-1, type=str)
 @click.argument("remotedir", nargs=1, type=str)
-@click.option(
-    "--upload-type",
-    "-t",
-    type=click.Choice([t.name for t in UploadType]),
-    default=UploadType.Many.name,
-    help=(
-        "上传方式，Many: 同时上传多个文件，"
-        "One: 一次只上传一个文件，但同时上传文件的多个分片 "
-        "(阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效)"
-    ),
-)
 @click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.option(
     "--encrypt-type",
     "-e",
     type=click.Choice([t.name for t in EncryptType]),
     default=EncryptType.No.name,
     help="文件加密方法，默认为 No 不加密",
@@ -1243,26 +1236,22 @@
 @handle_error
 @save_modified_user_data
 @multi_user_do
 def upload(
     ctx,
     localpaths,
     remotedir,
-    upload_type,
     encrypt_password,
     encrypt_type,
     max_workers,
     no_ignore_existing,
     no_show_progress,
 ):
     """上传文件"""
 
-    if upload_type == UploadType.One.name:
-        raise ValueError("阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效")
-
     # Keyboard listener start
     keyboard_listener_start()
 
     api = _recent_api(ctx)
     if not api:
         return
 
@@ -1279,15 +1268,14 @@
         init_progress_bar()
 
     check_name_mode = "refuse" if not no_ignore_existing else "auto_rename"
 
     _upload(
         api,
         from_to_list,
-        upload_type=getattr(UploadType, upload_type),
         check_name_mode=check_name_mode,
         encrypt_password=encrypt_password,
         encrypt_type=getattr(EncryptType, encrypt_type),
         max_workers=max_workers,
         show_progress=not no_show_progress,
     )
 
@@ -1633,16 +1621,16 @@
     """
 
     app_config = _app_config(ctx)
     if not app_config.share.store:
         print("App configuration `[share] store is false`. So the command does not work")
         return
 
-    api: AliPCSApiMixWithSharedStore = _recent_api(ctx)
-    if not api:
+    api = _recent_api(ctx)
+    if not isinstance(api, AliPCSApiMixWithSharedStore):
         return
 
     store = api.sharedstore
     if not store:
         return
 
     shared_links = store.list_shared_links()
```

### Comparing `alipcs_py-0.7.0/alipcs_py/app/config.py` & `alipcs_py-0.8.0/alipcs_py/app/config.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/cat.py` & `alipcs_py-0.8.0/alipcs_py/commands/cat.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 def cat(
     api: AliPCSApi,
     remotepath: str,
     encoding: Optional[str] = None,
     encrypt_password: bytes = b"",
 ):
-    pcs_file = api.path(remotepath)
-
+    pcs_file = api.get_file(remotepath=remotepath)
     if not pcs_file:
         return
 
     fs = api.file_stream(pcs_file.file_id, encrypt_password=encrypt_password)
     if not fs:
         display_blocked_remotepath(remotepath)
         return
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/crypto.py` & `alipcs_py-0.8.0/alipcs_py/commands/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     assert exists(from_encrypted)
 
     dio = to_decryptio(open(from_encrypted, "rb"), encrypt_password=encrypt_password)
 
     dpath = Path(to_decrypted)
     dir_ = dpath.parent
     if not dir_.exists():
-        dir_.mkdir(parents=True)
+        dir_.mkdir(parents=True, exist_ok=True)
 
     with dpath.open("wb") as dfd:
         while True:
             data = dio.read(READ_SIZE)
             if not data:
                 break
             dfd.write(data)
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/display.py` & `alipcs_py-0.8.0/alipcs_py/commands/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         return
 
     table = Table(box=SIMPLE, padding=0, show_edge=False)
     table.add_column("From", justify="left", overflow="fold")
     table.add_column("To", justify="left", overflow="fold")
 
     for from_to in from_to_list:
-        table.add_row(from_to.from_, from_to.to_)
+        table.add_row(*from_to)
 
     console = Console()
     console.print(table)
 
 
 _SHARED_LINK_INFO_FORMAT = (
     "share id: {share_id}\n"
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/index.html` & `alipcs_py-0.8.0/alipcs_py/commands/index.html`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/list_files.py` & `alipcs_py-0.8.0/alipcs_py/commands/list_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,36 +37,34 @@
     show_file_id: bool = False,
     show_hash: bool = False,
     show_absolute_path: bool = False,
     show_dl_link: bool = False,
     csv: bool = False,
     only_dl_link: bool = False,
 ):
-    pcs_file: Optional[PcsFile]
-    if file_id:
-        pcs_file = api.meta(file_id, share_id=share_id)[0]
-    else:
-        pcs_file = api.path(remotepath, share_id=share_id)
-    if not pcs_file:
+    pcs_file = api.get_file(remotepath=remotepath, file_id=file_id, share_id=share_id)
+    if pcs_file is None:
         return
 
     is_dir = pcs_file.is_dir
     if is_dir:
-        pcs_files = api.list_path(
-            remotepath,
-            file_id=pcs_file.file_id,
+        pcs_files = []
+        for sub_pf in api.list_iter(
+            pcs_file.file_id,
             share_id=share_id,
             desc=desc,
             name=name,
             time=time,
             size=size,
             all=all,
             limit=limit,
             url_expire_sec=url_expire_sec,
-        )
+        ):
+            sub_pf.path = join_path(remotepath, sub_pf.path)
+            pcs_files.append(sub_pf)
     else:
         pcs_files = [pcs_file]
 
     pcs_files = sift(pcs_files, sifters, recursive=recursive)
     if not pcs_files:
         return
 
@@ -91,15 +89,15 @@
         )
 
     if is_dir and recursive:
         for pcs_file in pcs_files:
             if pcs_file.is_dir:
                 list_file(
                     api,
-                    join_path(remotepath, pcs_file.name),
+                    pcs_file.path,
                     file_id=pcs_file.file_id,
                     share_id=share_id,
                     desc=desc,
                     name=name,
                     time=time,
                     size=size,
                     all=all,
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/login.py` & `alipcs_py-0.8.0/alipcs_py/commands/login.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/play.py` & `alipcs_py-0.8.0/alipcs_py/commands/play.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from typing import Optional, List, Dict
+from typing import Optional, List
 from enum import Enum
-from pathlib import Path
 import os
 import shutil
 import subprocess
 import random
 import time
-from urllib.parse import quote
 
 from alipcs_py.alipcs import AliPCSApi, PcsFile
 from alipcs_py.alipcs.errors import AliPCSError
 from alipcs_py.commands.sifter import Sifter, sift
 from alipcs_py.commands.download import USER_AGENT
 from alipcs_py.commands.errors import CommandError
 from alipcs_py.common.file_type import MEDIA_EXTS
-from alipcs_py.common.path import join_path
 
 from rich import print
 
 
 _print = __builtins__["print"]  # type: ignore
 
 
@@ -122,15 +119,15 @@
     use_local_server = bool(local_server)
 
     if share_id:
         shared_pcs_file_id = pcs_file.file_id
         shared_pcs_filename = pcs_file.name
         use_local_server = False
         remote_temp_dir = "/__alipcs_py_temp__"
-        pcs_temp_dir = api.path(remote_temp_dir) or api.makedir_path(remote_temp_dir)
+        pcs_temp_dir = api.path(remote_temp_dir) or api.makedir_path(remote_temp_dir)[0]
         pf = api.transfer_shared_files([shared_pcs_file_id], pcs_temp_dir.file_id, share_id)[0]
         target_file_id = pf.file_id
         while True:
             pfs = api.search_all(shared_pcs_filename)
             for pf_ in pfs:
                 if pf_.file_id == target_file_id:
                     pcs_file = pf_
@@ -185,42 +182,39 @@
     player_params: List[str] = [],
     quiet: bool = False,
     shuffle: bool = False,
     ignore_ext: bool = False,
     out_cmd: bool = False,
     local_server: str = "",
 ):
-    if pcs_file.path.startswith("/"):
-        remotefiles = list(api.list_path(pcs_file.path, share_id=share_id))
-    else:
-        remotefiles = list(api.list_iter(pcs_file.file_id, share_id=share_id))
-    remotefiles = sift(remotefiles, sifters, recursive=recursive)
+    sub_pcs_files = list(api.list_iter(pcs_file.file_id, share_id=share_id))
+    sub_pcs_files = sift(sub_pcs_files, sifters, recursive=recursive)
 
     if shuffle:
         rg = random.Random(time.time())
-        rg.shuffle(remotefiles)
+        rg.shuffle(sub_pcs_files)
 
-    for rp in remotefiles[from_index:]:
-        if rp.is_file:
+    for pf in sub_pcs_files[from_index:]:
+        if pf.is_file:
             play_file(
                 api,
-                rp,
+                pf,
                 share_id=share_id,
                 player=player,
                 player_params=player_params,
                 quiet=quiet,
                 ignore_ext=ignore_ext,
                 out_cmd=out_cmd,
                 local_server=local_server,
             )
         else:  # is_dir
             if recursive:
                 play_dir(
                     api,
-                    rp,
+                    pf,
                     share_id=share_id,
                     sifters=sifters,
                     recursive=recursive,
                     from_index=from_index,
                     player=player,
                     player_params=player_params,
                     quiet=quiet,
@@ -289,16 +283,16 @@
                 shuffle=shuffle,
                 ignore_ext=ignore_ext,
                 out_cmd=out_cmd,
                 local_server=local_server,
             )
 
     for file_id in file_ids:
-        rpf = api.meta(file_id, share_id=share_id)[0]
-        if not rpf:
+        rpf = api.get_file(file_id=file_id, share_id=share_id)
+        if rpf is None:
             print(f"[yellow]WARNING[/yellow]: file_id `{file_id}` does not exist.")
             continue
 
         if rpf.is_file:
             play_file(
                 api,
                 rpf,
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/search.py` & `alipcs_py-0.8.0/alipcs_py/commands/search.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/server.py` & `alipcs_py-0.8.0/alipcs_py/commands/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
-if sys.version_info > (3, 8):
-    from typing import Annotated
-else:
+if sys.version_info < (3, 9):
     from typing_extensions import Annotated
+else:
+    from typing import Annotated
 
 from typing import Optional, Dict, Any
 
 from pathlib import Path
 import os
 import mimetypes
 import secrets
@@ -124,26 +124,26 @@
     if not rpf:
         raise HTTPException(status_code=404, detail="Item not found")
 
     is_dir = rpf.is_dir
     if is_dir:
         chunks = ["/"] + (remotepath.split("/") if remotepath != "" else [])
         navigation = [(i - 1, "../" * (len(chunks) - i), name) for i, name in enumerate(chunks, 1)]
-        pcs_files = _api.list_path_iter(_rp, desc=desc, name=name, time=time, size=size)
         entries = []
-        for f in pcs_files:
-            p = Path(f.path)
+        pcs_files = _api.list_iter(rpf.file_id, desc=desc, name=name, time=time, size=size)
+        for pf in pcs_files:
+            p = rpf.path / Path(pf.path)
             entries.append(
                 (
-                    f.file_id,
-                    f.is_dir,
+                    pf.file_id,
+                    pf.is_dir,
                     p.name,
                     quote(p.name),
-                    f.size,
-                    format_date(f.updated_at or 0),
+                    pf.size,
+                    format_date(pf.updated_at or 0),
                 )
             )
         cn = _html_tempt.render(root_dir=remotepath, navigation=navigation, entries=entries)
         return HTMLResponse(cn)
     else:
         return get_file(rpf.file_id, remotepath, _range)
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/share.py` & `alipcs_py-0.8.0/alipcs_py/commands/share.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import List, Dict, Set
+from typing import List, Dict, Set, Union
 from pathlib import PurePosixPath
 from collections import deque
 import re
 
 from alipcs_py.alipcs import AliPCSApi, PcsFile
 from alipcs_py.commands.list_files import list_files
 from alipcs_py.commands.sifter import Sifter
 from alipcs_py.commands.display import (
     display_invalid_shared_link_infos,
     display_shared_files,
     display_shared_link_infos,
     display_shared_links,
 )
 from alipcs_py.commands.download import (
+    DEFAULT_CHUNK_SIZE,
+    DEFAULT_CONCURRENCY,
     download,
     Downloader,
     DEFAULT_DOWNLOADER,
-    DownloadParams,
-    DEFAULT_DOWNLOADPARAMS,
 )
 from alipcs_py.commands.play import play, Player, DEFAULT_PLAYER
 
 import requests  # type: ignore
 
 from rich import print
 
@@ -79,73 +79,77 @@
 def save_shared_by_file_ids(
     api: AliPCSApi,
     remotedir: str,
     share_id: str,
     file_ids: List[str],
     password: str = "",
 ):
+    """Save shared files to the remote directory `remotedir`. Ignore existed files."""
+
     assert share_id
 
     api.get_share_token(share_id, share_password=password)
 
     file_ids = file_ids or ["root"]
 
-    sfs = api.meta(*file_ids, share_id=share_id)
-    for sf in sfs:
-        if not sf.path:
-            sf.path = sf.name
-    shared_files = deque(sfs)
-
-    # Record the remotedir of each shared_file
-    _remotedirs: Dict[str, str] = {}
-    for sp in shared_files:
-        _remotedirs[sp.file_id] = remotedir
-
-    # Map the remotedir to its pcs_file
-    dest_pcs_files: Dict[str, PcsFile] = {}
-
-    while shared_files:
-        shared_file = shared_files.popleft()
-        rd = _remotedirs[shared_file.file_id]
-
-        # Make sure remote dir exists
-        if rd not in dest_pcs_files:
-            dest_pcs_files[rd] = api.makedir_path(rd)
-        dest_pcs_file = dest_pcs_files[rd]
+    shared_pcs_files = deque()
+    for file_id in file_ids:
+        pf = api.get_file(file_id=file_id, share_id=share_id)
+        if pf is not None:
+            shared_pcs_files.append(pf)
+
+    # Record the remote directory of each shared_file
+    shared_file_id_to_remotedir: Dict[str, str] = {}
+    for sp in shared_pcs_files:
+        shared_file_id_to_remotedir[sp.file_id] = remotedir
+
+    # Map the remote directory to its pcs_file
+    remotedir_to_its_pcs_file: Dict[str, PcsFile] = {}
+
+    while shared_pcs_files:
+        shared_file = shared_pcs_files.popleft()
+        remote_dir = shared_file_id_to_remotedir[shared_file.file_id]
+
+        # Make sure remote directory exists
+        if remote_dir not in remotedir_to_its_pcs_file:
+            remotedir_to_its_pcs_file[remote_dir] = api.makedir_path(remote_dir)[0]
+        dest_pcs_file = remotedir_to_its_pcs_file[remote_dir]
 
-        if not shared_file.is_root() and not remotepath_exists(api, shared_file.name, rd):
+        if not shared_file.is_root() and not remotepath_exists(api, shared_file.name, dest_pcs_file.file_id):
             api.transfer_shared_files(
                 [shared_file.file_id],
                 dest_pcs_file.file_id,
                 share_id,
                 auto_rename=False,
             )
-            print(f"save: `{shared_file.path}` to `{rd}`")
+            print(f"save: `{shared_file.path}` to `{remote_dir}`")
         else:
             # Ignore existed file
             if shared_file.is_file:
-                print(f"[yellow]WARNING[/]: `{shared_file.path}` has be in `{rd}`")
+                print(f"[yellow]WARNING[/]: `{shared_file.path}` has be in `{remote_dir}`")
                 continue
             else:  # shared_file.is_dir
-                sub_files = list(api.list_path_iter(shared_file.path, file_id=shared_file.file_id, share_id=share_id))
+                sub_files = list(api.list_iter(shared_file.file_id, share_id=share_id))
 
-                rd = (PurePosixPath(rd) / shared_file.name).as_posix()
+                remote_dir = (PurePosixPath(remote_dir) / shared_file.name).as_posix()
                 for sp in sub_files:
-                    _remotedirs[sp.file_id] = rd
-                shared_files.extendleft(sub_files[::-1])
+                    shared_file_id_to_remotedir[sp.file_id] = remote_dir
+                shared_pcs_files.extendleft(sub_files[::-1])
 
 
 def save_shared(
     api: AliPCSApi,
     remotedir: str,
     share_id: str = "",
     share_url: str = "",
     file_ids: List[str] = [],
     password: str = "",
 ):
+    """Save shared files of the shared url to the remote directory `remotedir`."""
+
     assert remotedir.startswith("/"), "`remotedir` must be an absolute path"
 
     assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     if share_url:
         save_shared_by_url(api, remotedir, share_url, password=password)
     else:
@@ -171,14 +175,16 @@
     show_size: bool = False,
     show_date: bool = False,
     show_file_id: bool = False,
     show_hash: bool = False,
     show_absolute_path: bool = False,
     csv: bool = False,
 ):
+    """List shared files in the shared url or shared id."""
+
     assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
@@ -211,38 +217,45 @@
         show_file_id=show_file_id,
         show_hash=show_hash,
         show_absolute_path=show_absolute_path,
         csv=csv,
     )
 
 
-def remotepath_exists(api: AliPCSApi, name: str, rd: str, _cache: Dict[str, Set[str]] = {}) -> bool:
-    names = _cache.get(rd)
+def remotepath_exists(api: AliPCSApi, name: str, remote_file_id: str, _cache: Dict[str, Set[str]] = {}) -> bool:
+    """Check if the `name` exists in the remote directory `remote_file_id`."""
+
+    names = _cache.get(remote_file_id)
     if not names:
-        names = set([sp.name for sp in api.list_path_iter(rd)])
-        _cache[rd] = names
+        names = set(sp.name for sp in api.list_iter(remote_file_id))
+        _cache[remote_file_id] = names
     return name in names
 
 
 def download_shared(
     api: AliPCSApi,
-    remotepaths: List[str],
+    remotepaths: List[Union[str, PcsFile]],
     file_ids: List[str],
     localdir: str,
     share_id: str = "",
     share_url: str = "",
     password: str = "",
     sifters: List[Sifter] = [],
     recursive: bool = False,
     from_index: int = 0,
     downloader: Downloader = DEFAULT_DOWNLOADER,
-    downloadparams: DownloadParams = DEFAULT_DOWNLOADPARAMS,
+    concurrency: int = DEFAULT_CONCURRENCY,
+    chunk_size: Union[str, int] = DEFAULT_CHUNK_SIZE,
+    show_progress: bool = False,
+    max_retries: int = 2,
     out_cmd: bool = False,
     encrypt_password: bytes = b"",
 ):
+    """Download shared files in the shared url or shared id."""
+
     assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
@@ -262,15 +275,18 @@
         file_ids=file_ids,
         localdir=localdir,
         share_id=share_id,
         sifters=sifters,
         recursive=recursive,
         from_index=from_index,
         downloader=downloader,
-        downloadparams=downloadparams,
+        concurrency=concurrency,
+        chunk_size=chunk_size,
+        show_progress=show_progress,
+        max_retries=max_retries,
         out_cmd=out_cmd,
         encrypt_password=encrypt_password,
     )
 
 
 def play_shared(
     api: AliPCSApi,
@@ -286,14 +302,16 @@
     player_params: List[str] = [],
     quiet: bool = False,
     shuffle: bool = False,
     ignore_ext: bool = False,
     out_cmd: bool = False,
     local_server: str = "",
 ):
+    """Play shared files in the shared url or shared id."""
+
     assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
@@ -322,14 +340,16 @@
         ignore_ext=ignore_ext,
         out_cmd=out_cmd,
         local_server=local_server,
     )
 
 
 def get_share_token(api: AliPCSApi, share_id: str, share_url: str = "", password: str = "") -> str:
+    """Initiate a shared link (or id) and get the share token."""
+
     assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
```

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/sifter.py` & `alipcs_py-0.8.0/alipcs_py/commands/sifter.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/commands/sync.py` & `alipcs_py-0.8.0/alipcs_py/commands/sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Optional, List, Tuple
+from typing import List, Tuple
 from pathlib import Path
+import os
 
 from alipcs_py.alipcs import AliPCSApi, PcsFile, FromTo
-from alipcs_py.common.path import walk, join_path
+from alipcs_py.common.path import PathType, join_path
 from alipcs_py.common.crypto import calc_sha1
 from alipcs_py.common.constant import CPU_NUM
 from alipcs_py.common.io import EncryptType
-from alipcs_py.commands.upload import UploadType, upload as _upload, DEFAULT_SLICE_SIZE
+from alipcs_py.commands.upload import upload, DEFAULT_SLICE_SIZE
 from alipcs_py.commands.log import get_logger
 
 from rich import print
 
 logger = get_logger(__name__)
 
 
@@ -19,75 +20,67 @@
     localdir: str,
     remotedir: str,
     encrypt_password: bytes = b"",
     encrypt_type: EncryptType = EncryptType.No,
     max_workers: int = CPU_NUM,
     slice_size: int = DEFAULT_SLICE_SIZE,
     show_progress: bool = True,
-    rapiduploadinfo_file: Optional[str] = None,
-    user_id: Optional[str] = None,
-    user_name: Optional[str] = None,
 ):
+    """Sync local directory to remote directory."""
+
     localdir = Path(localdir).as_posix()
     remotedir = Path(remotedir).as_posix()
 
-    rpf = api.makedir_path(remotedir)
-    assert rpf and rpf.is_dir, "remotedir must be a directory"
+    remote_pcs_file = api.makedir_path(remotedir)[0]
+    assert remote_pcs_file and remote_pcs_file.is_dir, "remotedir must be a directory"
 
-    if remotedir == "/":
-        remotedir_len = 0
-    else:
-        remotedir_len = len(remotedir)
-
-    all_pcs_files = {
-        pcs_file.path[remotedir_len + 1 :]: pcs_file
-        for pcs_file in api.list_path_iter(remotedir, recursive=True, include_dir=False)
+    sub_path_to_its_pcs_file = {
+        pcs_file.path: pcs_file
+        for pcs_file in api.list_iter(remote_pcs_file.file_id, recursive=True, include_dir=False)
     }
 
-    fts: List[FromTo] = []
-    check_list: List[Tuple[str, PcsFile]] = []
+    needed_uploads: List[FromTo[PathType, str]] = []
+    needed_checks: List[Tuple[Path, PcsFile]] = []
     all_localpaths = set()
-    for localpath in walk(localdir):
-        path = localpath[len(localdir) + 1 :]
-        all_localpaths.add(path)
-
-        if path not in all_pcs_files:
-            fts.append(FromTo(localpath, join_path(remotedir, path)))
-        else:
-            check_list.append((localpath, all_pcs_files[path]))
+    for root, _, filenames in os.walk(localdir):
+        for filename in filenames:
+            localpath = Path(root[len(localdir) + 1 :]) / filename
+            localpath_posix = localpath.as_posix()
+            all_localpaths.add(localpath_posix)
+
+            if localpath_posix not in sub_path_to_its_pcs_file:
+                needed_uploads.append((root / localpath, join_path(remotedir, localpath)))
+            else:
+                needed_checks.append((root / localpath, sub_path_to_its_pcs_file[localpath_posix]))
 
-    for lp, pf in check_list:
-        sha1 = calc_sha1(Path(lp).open("rb"))
+    for lp, pf in needed_checks:
+        sha1 = calc_sha1(lp.open("rb"))
 
         if pf.rapid_upload_info and sha1.lower() != pf.rapid_upload_info.content_hash.lower():
-            fts.append(FromTo(lp, pf.path))
+            needed_uploads.append((lp, pf.path))
 
     need_deleted_file_ids = []
-    for rp in all_pcs_files.keys():
+    for rp in sub_path_to_its_pcs_file.keys():
         if rp not in all_localpaths:
-            need_deleted_file_ids.append(all_pcs_files[rp].file_id)
+            need_deleted_file_ids.append(sub_path_to_its_pcs_file[rp].file_id)
 
     logger.debug(
         "`sync`: all localpaths: %s, localpaths needed to upload: %s, remotepaths needed to delete: %s",
         len(all_localpaths),
-        len(fts),
+        len(needed_uploads),
         len(need_deleted_file_ids),
     )
 
-    _upload(
+    upload(
         api,
-        fts,
-        upload_type=UploadType.Many,
+        needed_uploads,
         check_name_mode="overwrite",
         encrypt_password=encrypt_password,
         encrypt_type=encrypt_type,
         max_workers=max_workers,
         slice_size=slice_size,
         show_progress=show_progress,
-        rapiduploadinfo_file=rapiduploadinfo_file,
-        user_id=user_id,
-        user_name=user_name,
     )
 
     if need_deleted_file_ids:
         api.remove(*need_deleted_file_ids)
         print(f"Delete: [i]{len(need_deleted_file_ids)}[/i] remote paths")
```

### Comparing `alipcs_py-0.7.0/alipcs_py/common/cache.py` & `alipcs_py-0.8.0/alipcs_py/common/cache.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/crypto.py` & `alipcs_py-0.8.0/alipcs_py/common/crypto.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/date.py` & `alipcs_py-0.8.0/alipcs_py/common/date.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/downloader.py` & `alipcs_py-0.8.0/alipcs_py/common/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from typing import Optional, Any, Callable
-from os import PathLike
 from pathlib import Path
 
 from alipcs_py.common.io import RangeRequestIO
 from alipcs_py.common.concurrent import retry
+from alipcs_py.common.path import PathType
 
 
 DEFAULT_MAX_WORKERS = 5
 
 
 class MeDownloader:
+    """Download the content from `range_request_io` to `localpath`"""
+
     def __init__(
         self,
         range_request_io: RangeRequestIO,
-        localpath: PathLike,
+        localpath: PathType,
         continue_: bool = False,
-        retries: int = 2,
+        max_retries: int = 2,
         done_callback: Optional[Callable[..., Any]] = None,
         except_callback: Optional[Callable[[Exception], Any]] = None,
     ) -> None:
         self.range_request_io = range_request_io
         self.localpath = localpath
         self.continue_ = continue_
-        self.retries = retries
+        self.max_retries = max_retries
         self.done_callback = done_callback
         self.except_callback = except_callback
 
     def _init_fd(self):
         if self.continue_:
             path = Path(self.localpath)
             if self.range_request_io.seekable():
@@ -40,24 +42,23 @@
             offset = 0
             fd = open(self.localpath, "wb")
 
         self.offset = offset
         self.fd = fd
 
     def download(self):
-        """
-        Download the url content to `localpath`
+        """Download the url content to `localpath`
 
         Args:
             continue_ (bool): If set to True, only downloading the remain content depended on
             the size of `localpath`
         """
 
         @retry(
-            self.retries,
+            self.max_retries,
             except_callback=lambda err, fails: (
                 self.range_request_io.reset(),
                 self.except_callback(err) if self.except_callback else None,
             ),
         )
         def _download():
             self._init_fd()
```

### Comparing `alipcs_py-0.7.0/alipcs_py/common/event.py` & `alipcs_py-0.8.0/alipcs_py/common/event.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/file_type.py` & `alipcs_py-0.8.0/alipcs_py/common/file_type.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/io.py` & `alipcs_py-0.8.0/alipcs_py/common/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,21 +1007,34 @@
         left = list(range(start, end, self._max_chunk_size))
         left.append(end)
         right = [i - 1 for i in left]
         return [(s, e) for s, e in zip(left[:-1], right[1:])]
 
 
 class RangeRequestIO(IO):
+    """Request IO with range header
+
+    Args:
+        method (str): HTTP method
+        url (str): URL
+        headers (Optional[Dict[str, str]]): HTTP headers
+        max_chunk_size (int): The max chunk size
+        callback (Optional[Callable[[int], None]]): Callback function for progress monitor,
+            the argument is the current offset.
+        encrypt_password (bytes): Encrypt password
+        **kwargs: Other kwargs for request
+    """
+
     def __init__(
         self,
         method: str,
         url: str,
         headers: Optional[Dict[str, str]] = None,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
-        callback: Callable[..., None] = None,
+        callback: Optional[Callable[[int], Any]] = None,
         encrypt_password: bytes = b"",
         **kwargs,
     ):
         kwargs["stream"] = True
 
         self._method = method
         self._url = url
@@ -1052,22 +1065,22 @@
             return b""
 
         if size == -1:
             size = len(self) - self._offset
 
         start, end = self._offset, self._offset + size
 
-        buf = b""
-        for b in self._auto_decrypt_request.read((start, end)):
-            buf += b
-            self._offset += len(b)
+        buffer = b""
+        for buf in self._auto_decrypt_request.read((start, end)):
+            buffer += buf
+            self._offset += len(buf)
             # Call callback
             if self._callback:
                 self._callback(self._offset)
-        return buf
+        return buffer
 
     def read_iter(self, size: int = -1) -> Iterable[bytes]:
         if size == 0:
             return b""
 
         if size == -1:
             size = len(self) - self._offset
@@ -1092,14 +1105,17 @@
         self._offset = max(0, self._offset)
         self._offset = min(len(self), self._offset)
         return self._offset
 
     def tell(self) -> int:
         return self._offset
 
+    def readable(self) -> bool:
+        return True
+
     def seekable(self) -> bool:
         return self._auto_decrypt_request.rangeable()
 
     def writable(self) -> bool:
         return False
 
     def close(self):
```

### Comparing `alipcs_py-0.7.0/alipcs_py/common/keyboard.py` & `alipcs_py-0.8.0/alipcs_py/common/keyboard.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/log.py` & `alipcs_py-0.8.0/alipcs_py/common/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,14 @@
     stream_handler.setFormatter(logging.Formatter(fmt))
     logger.addHandler(stream_handler)
 
     if filename:
         filename = Path(filename)
         _dir = filename.parent
         if not _dir.exists():
-            _dir.mkdir()
+            _dir.mkdir(parents=True, exist_ok=True)
 
         file_handler = logging.FileHandler(filename)
         file_handler.setFormatter(logging.Formatter(fmt))
         logger.addHandler(file_handler)
 
     return logger
```

### Comparing `alipcs_py-0.7.0/alipcs_py/common/progress_bar.py` & `alipcs_py-0.8.0/alipcs_py/common/progress_bar.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/common/simple_cipher.pyx` & `alipcs_py-0.8.0/alipcs_py/common/simple_cipher.pyx`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/config/__init__.py` & `alipcs_py-0.8.0/alipcs_py/config/__init__.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/storage/store.py` & `alipcs_py-0.8.0/alipcs_py/storage/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,26 +142,25 @@
             shared_link_info = self._sharedstore.get_shared_link_info(share_id)
             if not shared_link_info:
                 shared_link_info = self.shared_info(share_id)
                 self._sharedstore.add_shared_link_info(shared_link_info)
 
         return token
 
-    def meta(self, *args, **kwargs):
-        share_id = kwargs.get("share_id")
-
-        pcs_files = super().meta(*args, **kwargs)
+    def meta(self, file_id: str, share_id: Optional[str] = None) -> Optional[PcsFile]:
+        pcs_file = super().meta(file_id, share_id=share_id)
+        if pcs_file is None:
+            return None
         if not self._sharedstore:
-            return pcs_files
+            return pcs_file
 
         if share_id:
-            for pcs_file in pcs_files:
-                self._sharedstore.add_shared_file(share_id, pcs_file)
+            self._sharedstore.add_shared_file(share_id, pcs_file)
 
-        return pcs_files
+        return pcs_file
 
     def list(self, *args, **kwargs):
         share_id = kwargs.get("share_id")
 
         pcs_files, next_marker = super().list(*args, **kwargs)
         if not self._sharedstore:
             return pcs_files, next_marker
```

### Comparing `alipcs_py-0.7.0/alipcs_py/storage/tables.py` & `alipcs_py-0.8.0/alipcs_py/storage/tables.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/alipcs_py/utils.py` & `alipcs_py-0.8.0/alipcs_py/utils.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/build.py` & `alipcs_py-0.8.0/build.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.7.0/pyproject.toml` & `alipcs_py-0.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "AliPCS-Py"
 homepage = "https://github.com/PeterDing/AliPCS-Py"
-version = "0.7.0"
+version = "0.8.0"
 description = "Ali Pcs Api and App"
 authors = ["PeterDing <dfhayst@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -47,14 +47,16 @@
 cryptography = ">=41.0"
 ecdsa = ">=0.18"
 cython = ">=3.0"
 passlib = ">=1.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4"
+pytest-cov = ">=5.0"
+Faker = ">=24"
 ruff = ">=0.3"
 setuptools = ">=69.0"
 cython = ">=3.0"
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = true
```

### Comparing `alipcs_py-0.7.0/setup.py` & `alipcs_py-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
  'uvicorn>=0.24']
 
 entry_points = \
 {'console_scripts': ['AliPCS-Py = alipcs_py.app:main']}
 
 setup_kwargs = {
     'name': 'AliPCS-Py',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'Ali Pcs Api and App',
-    'long_description': '# AliPCS-Py\n\n**2023-04-24 支持 阿里云盘开放平台 api。**\n\n**2023-02-15 使用临时 API 接口，让下载可用。**\n\n**2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**\n\n[![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)\n![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)\n\nAn AliPCS API and An App\n\nAliPCS-Py 是阿里云盘的非官方 api 和一个命令行运用程序。\n\n变更日志在 [CHANGELOG.md](./CHANGELOG.md)。\n\n---\n\n## 百度云盘 api 和 命令行客户端在 https://github.com/PeterDing/BaiduPCS-Py\n\n---\n\n- [安装](#安装)\n- [更新](#更新)\n- [API](#API)\n- [用法](#用法)\n- [命令别名](#命令别名)\n- [对多个帐号进行相同操作](#对多个帐号进行相同操作)\n\n#### 用户相关命令\n\n- [添加用户](#添加用户)\n- [显示当前用户的信息](#显示当前用户的信息)\n- [更新用户信息](#更新用户信息)\n- [显示所有用户](#显示所有用户)\n- [切换当前用户](#切换当前用户)\n- [删除一个用户](#删除一个用户)\n- [显示当前工作目录](#显示当前工作目录)\n- [切换当前工作目录](#切换当前工作目录)\n\n#### 无感加密解密文件\n\n- [设置文件加密密码](#设置文件加密密码)\n\n#### 文件操作相关命令\n\n- [文件操作](#文件操作)\n- [列出网盘路径下的文件](#列出网盘路径下的文件)\n- [搜索文件](#搜索文件)\n- [显示文件内容](#显示文件内容)\n- [创建目录](#创建目录)\n- [移动文件](#移动文件)\n- [文件重命名](#文件重命名)\n- [拷贝文件](#拷贝文件)\n- [删除文件](#删除文件)\n- [下载文件或目录](#下载文件或目录)\n- [播放媒体文件](#播放媒体文件)\n- [上传文件](#上传文件)\n- [同步本地目录到远端](#同步本地目录到远端)\n\n#### 秒传\n\n- [关于秒传连接](#关于秒传连接)\n\n#### 分享相关命令\n\n- [分享文件](#分享文件)\n- [列出分享链接](#列出分享链接)\n- [取消分享链接](#取消分享链接)\n- [列出其他用户分享链接中的文件](#列出其他用户分享链接中的文件)\n- [下载他人分享的文件](#下载他人分享的文件)\n- [播放他人分享的文件](#播放他人分享的文件)\n- [保存其他用户分享的链接](#保存其他用户分享的链接)\n\n#### 本地保存分享连接\n\n- [保存分享连接至本地](#保存分享连接至本地)\n- [显示本地保存的分享连接](#显示本地保存的分享连接)\n- [显示本地保存的分享文件](#显示本地保存的分享文件)\n- [查找本地保存的分享连接](#查找本地保存的分享连接)\n- [查找本地保存的分享文件](#查找本地保存的分享文件)\n- [查找本地保存的分享连接和文件](#查找本地保存的分享连接和文件)\n- [删除本地保存的分享连接或文件](#删除本地保存的分享连接或文件)\n- [清理本地保存的无效分享连接](#清理本地保存的无效分享连接)\n\n#### HTTP 服务\n\n- [开启 HTTP 服务](#开启-HTTP-服务)\n\n## 安装\n\n需要 Python 版本大于或等于 3.8\n\n```\npip3 install Cython\npip3 install AliPCS-Py\n```\n\n### Windows 依赖\n\n在 Windows 上，AliPCS-Py 依赖 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。\n\n在安装 AliPCS-Py 前，请先安装 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)，再在其中勾选 `C++ 生成工具` 并安装。完成后即可安装 AliPCS-Py。\n\n## 更新\n\n```\npip3 install AliPCS-Py --upgrade\n```\n\n## API\n\nAliPCS-Py 的阿里云盘 API 只依赖 requests，方便用户开发自己的运用。\n\n```python\nfrom alipcs_py.alipcs import AliPCSApi\n\napi = AliPCSApi(refresh_token)\n```\n\n## 用法\n\n```\nAliPCS-Py --help\n```\n\n## 命令别名\n\n可以用下面的命令别名代替原来的命令名。\n\n| 别名 | 原名         |\n| ---- | ------------ |\n| w    | who          |\n| uu   | updateuser   |\n| su   | su           |\n| ul   | userlist     |\n| ua   | useradd      |\n| ep   | encryptpwd   |\n| ud   | userdel      |\n| l    | ls           |\n| f    | search       |\n| md   | mkdir        |\n| mv   | move         |\n| rn   | rename       |\n| cp   | copy         |\n| rm   | remove       |\n| d    | download     |\n| p    | play         |\n| u    | upload       |\n| sn   | sync         |\n| S    | share        |\n| sl   | shared       |\n| cs   | cancelshared |\n| s    | save         |\n| sv   | server       |\n\n## 对多个帐号进行相同操作\n\nAliPCS-Py 支持对多个帐号进行相同操作。比如，用相同关键字搜索多个帐号，上传相同的文件/目录到多个帐号，等等。\n\n使用者只需用 `--users` 选项来指定要操作的帐号名即可。\n\n`--users` 接受一个参数，这个参数是用“,”连接的要进行操作帐号名的部分字符。假设我们现在有 3 个帐号，帐号名分别是 `Tom`，`Peter`，`Joy`。\n现在我要同时对`Tom`和`Joy`进行关键字搜索。我们可以用下面的命令进行：\n\n```\nAliPCS-Py --users \'Tom,Joy\' search \'keyword\' / -R\n```\n\n或者给出帐号名的部分片段：\n\n```\nAliPCS-Py --users \'om,oy\' search \'keyword\' / -R\n```\n\n更简单可以用：\n\n```\n# Tom, Joy 都包含字符 "o"\nAliPCS-Py --users \'o\' search \'keyword\' / -R\n```\n\n如果要对所有帐号进行操作用 `--users \'\'`。\n\n如果不使用 `--users` 选项，默认只对当前帐号进行操作。\n\n以下命令支持对多个帐号进行操作：\n\n- pwd\n- ls\n- search\n- cat\n- mkdir\n- move\n- rename\n- copy\n- remove\n- download\n- play\n- upload\n- sync\n- share\n- shared\n- cancelshared\n- save\n- server\n\n**注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。\n\n## 添加用户\n\n**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**\n\nAliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。\n\n### 使用 web `refresh_token` 和 第三方认证地址 登录\n\n第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-server "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录\n\n如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 登录\n\n使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。\n\n使用者可以用下面的方式获取用户的 `refresh_token` 值。\n\n1. 登录 https://www.aliyundrive.com/drive/\n2. 打开浏览器的开发者工具(如 Chrome DevTools)。\n3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。\n\n![refresh_token](./imgs/refresh_token.png)\n\n现在找到了 `refresh_token` 值，我们可以用下面的命令添加一个用户。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..."\n```\n\nAliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。\n\n**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**\n\n## 显示当前用户的信息\n\n```\nAliPCS-Py who\n```\n\n或者：\n\n```\nAliPCS-Py who user_id\n```\n\n指明显示用户 id 为 `user_id` 的用户信息。\n\n### 选项\n\n| Option                       | Description                |\n| ---------------------------- | -------------------------- |\n| -K, --show-encrypt-password  | 显示加密密码               |\n| --account-name TEXT          | 账号名 [默认为 user id]    |\n| --web-refresh-token TEXT     | 用户 web_refresh_token     |\n| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |\n| --client-id TEXT             | openapi client id          |\n| --client-secret TEXT         | openapi client secret      |\n| --client-server TEXT         | openapi client server      |\n\n## 更新用户信息\n\n默认更新当前用户信息。\n\n```\nAliPCS-Py updateuser\n```\n\n也可指定多个 `user_id`\n\n```\nAliPCS-Py updateuser user_id\n```\n\n## 显示所有用户\n\n```\nAliPCS-Py userlist\n```\n\n## 切换当前用户\n\n```\nAliPCS-Py su\n```\n\n或者指定用户列表中用户所在的位置：\n\n```\nAliPCS-Py su 2\n```\n\n## 删除一个用户\n\n```\nAliPCS-Py userdel\n```\n\n## 设置文件加密密码\n\nAliPCS-Py 支持“无感的”文件加密。\n\nAliPCS-Py 可以加密上传文件，在下载的时候自动解密，让使用者感觉不到加密解密的过程。\n\n如果使用者需要将保密文件上传至阿里云盘保存，可以使用这个方法。即使帐号被盗，攻击者也无法还原文件内容。\n\nAliPCS-Py 支持以下加密方法：\n\n- **Simple** 一种简单的加密算法。根据密钥生成一个字节对照表来加密解密文件。\n  速度快，但**不安全**，不建议加密重要文件。\n  因为这种算法加解密不需要知道上下文信息，所以，下载时支持分段下载，如果是媒体文件则支持拖动播放。\n  推荐用于加密不重要的媒体文件。\n- **ChaCha20** 工业级加密算法，速度快，推荐用于加密重要文件。不支持分段下载。\n- **AES256CBC** 工业级加密算法，推荐用于加密重要文件。不支持分段下载。\n\n**注意**：用命令 `encryptpwd` 设置的密码**只是为当前用户**的。\n\n为当前用户设置加密密码:\n\n交互添加：\n\n```\nAliPCS-Py encryptpwd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py encryptpwd --encrypt-password \'my-encrypt-password\'\n```\n\n上传并加密文件：\n\n上传和同步文件时只需要指定加密算法就可。如果不指定就不加密。\n\n```\n# 默认使用上面设置的 `encrypt-password`\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type AES256CBC\n```\n\n下载并用上面设置的 `encrypt-password` 自动解密文件：\n\n```\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/\n```\n\n也可以使用临时的 `encrypt-password`：\n\n```\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type Simple --encrypt-password \'onlyyou\'\n```\n\n但在使用临时的 `encrypt-password` 后，`cat`、下载和播放这些文件时需要指定 `encrypt-password`，但不需要指定加密算法，程序会自动检查加密算法：\n\n```\n# 下载\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/  --encrypt-password \'onlyyou\'\n\n# 开启本地服务并播放\nAliPCS-Py play /to/here/some-file.mp4 --encrypt-password \'onlyyou\' --use-local-server\n```\n\n显示当前用户的密钥：\n\n```\nAliPCS-Py who --show-encrypt-password\n```\n\nAliPCS-Py 下载时默认会解密文件，如果想要下载但不解密文件，需要加 `--no-decrypt`\n\n```\nAliPCS-Py download some-file --no-decrypt\n```\n\n## 文件操作\n\nAliPCS-Py 操作网盘中的文件可以使用文件的绝对路径或相对路径（相对与当前目录 pwd）。\n\n每一个用户都有自己的当前工作目录（pwd），默认为 `/` 根目录。\n\n使用者可以用 `cd` 命令来切换当前的工作目录（pwd）。\n\n下面所有涉及网盘路径的命令，其中如果网盘路径用的是相对路径，那么是相对于当前工作目录（pwd）的。\n如果是网盘路径用的是绝对路径，那么就是这个绝对路径。\n\n## 显示当前工作目录\n\n```\nAliPCS-Py pwd\n```\n\n## 切换当前工作目录\n\n切换到绝对路径：\n\n```\nAliPCS-Py cd /to/some/path\n```\n\n切换到相对路径：\n\n```\n# 切换到 (pwd)/../path\nAliPCS-Py cd ../path\n```\n\n## 列出网盘路径下的文件\n\n使用文件路径：\n\n```\nAliPCS-Py ls [OPTIONS] [REMOTEPATHS]...\n\nAliPCS-Py ls /absolute/path\n\n# or\nAliPCS-Py ls relative/path\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py ls -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                     | Description                                           |\n| -------------------------- | ----------------------------------------------------- |\n| -i, --file-id TEXT         | 文件 ID                                               |\n| --share-id, --si TEXT      | 列出这个分享 ID 下的文件                              |\n| --share-url, --su TEXT     | 列出这个分享 url 下的文件                             |\n| -p, --password TEXT        | 分享链接密码，如果没有不用设置                        |\n| -r, --desc                 | 逆序排列文件                                          |\n| -n, --name                 | 依名字排序                                            |\n| -t, --time                 | 依时间排序                                            |\n| -s, --size                 | 依文件大小排序                                        |\n| -R, --recursive            | 递归列出文件                                          |\n| -I, --include TEXT         | 筛选包含这个字符串的文件                              |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件                          |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件                      |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件                  |\n| -f, --is-file              | 筛选 **非** 目录文件                                  |\n| -d, --is-dir               | 筛选目录文件                                          |\n| --no-highlight, --NH       | 取消匹配高亮                                          |\n| -S, --show-size            | 显示文件大小                                          |\n| -D, --show-date            | 显示文件创建时间                                      |\n| --show-file-id, --ID       | 显示文件 ID                                           |\n| -M, --show-hash            | 显示文件 sha1                                         |\n| -A, --show-absolute-path   | 显示文件绝对路径                                      |\n| --show-dl-link, --DL       | 显示文件下载连接                                      |\n| --csv                      | 用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用 |\n| --only-dl-link, --ODL      | 只显示文件下载连接                                    |\n\n## 搜索文件\n\n搜索包含 `keyword` 的文件\n\n```\nAliPCS-Py search [OPTIONS] KEYWORD [REMOTEDIR]\n\n# 在当前工作目录中搜索\nAliPCS-Py search keyword\n\n# or\nAliPCS-Py search keyword /absolute/path\n\n# or\nAliPCS-Py search keyword relative/path\n```\n\n### 选项\n\n| Option                     | Description                          |\n| -------------------------- | ------------------------------------ |\n| -R, --recursive            | 递归搜索文件                         |\n| -I, --include TEXT         | 筛选包含这个字符串的文件             |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件         |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件     |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件 |\n| -f, --is-file              | 筛选 **非** 目录文件                 |\n| -d, --is-dir               | 筛选目录文件                         |\n| --no-highlight, --NH       | 取消匹配高亮                         |\n| -S, --show-size            | 显示文件大小                         |\n| -D, --show-date            | 显示文件创建时间                     |\n| -M, --show-hash            | 显示文件 sha1                        |\n| --csv                      | 用 csv 格式显示                      |\n\n## 显示文件内容\n\n```\nAliPCS-Py cat [OPTIONS] REMOTEPATH\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| -e, --encoding TEXT           | 文件编码，默认自动解码       |\n| --no-decrypt, --ND            | 不解密                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n\n## 创建目录\n\n```\nAliPCS-Py mkdir [OPTIONS] [REMOTEDIRS]...\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示目录    |\n\n## 移动文件\n\n移动一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 文件重命名\n\n```\nAliPCS-Py rename [OPTIONS] REMOTEPATH NEW_NAME\n```\n\ne.g.\n\n重命名 `/path/to/far` to `/path/to/foo`\n\n```\nAliPCS-Py rename /path/to/far foo\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 拷贝文件\n\n拷贝一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 删除文件\n\n```\nAliPCS-Py remove [OPTIONS] [REMOTEPATHS]...\n\n# 指定 路径\nAliPCS-Py remove /some/path\n# 指定 file-id\nAliPCS-Py remove --file-id ...\n```\n\n### 选项\n\n| Option        | Description  |\n| ------------- | ------------ |\n| -i, --file-id | TEXT 文件 ID |\n\n## 下载文件或目录\n\n> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。\n> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py download [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py download -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                    |\n| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| -i, --file-id TEXT                                     | 文件 ID                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| --share-id, --si TEXT                                  | 下载这个分享 ID 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --share-url, --su TEXT                                 | 下载这个分享 url 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                      |\n| -p, --password TEXT                                    | 分享链接密码，如果没有不用设置                                                                                                                                                                                                                                                                                                                                                                                                                                 |\n| -o, --outdir TEXT                                      | 指定下载本地目录，默认为当前目录                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -R, --recursive                                        | 递归下载                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| -f, --from-index INTEGER                               | 从所有目录中的第几个文件开始下载，默认为 0（第一个）                                                                                                                                                                                                                                                                                                                                                                                                           |\n| -I, --include TEXT                                     | 筛选包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --include-regex, --IR TEXT                             | 筛选包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| -E, --exclude TEXT                                     | 筛选 不 包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| --exclude-regex, --ER TEXT                             | 筛选 不 包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -s, --concurrency INTEGER                              | 下载同步链接数，默认为 5。建议小于 10。                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| -k, --chunk-size TEXT                                  | 同步链接分块大小，默认为 50MB                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| -d, --downloader [ me \\| aget_py \\| aget_rs \\| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |\n| --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n\n## 播放媒体文件\n\n> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。\n> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py play [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n**注意：目前，使用 `--share-id` 或 `--file-id` 时，无法使用 `--use-local-server`**\n\n```\nAliPCS-Py play -i file_id1 -i file_id2 -i ...\n```\n\n`play` 命令默认播放带有媒体后缀的文件，如 `abc.mp4`, `abc.mp3`。如果需要播放的媒体文件没有用常规的媒体文件后缀，则需要加选项 `--ignore-ext`。\n\n### 选项\n\n| Option                        | Description                                          |\n| ----------------------------- | ---------------------------------------------------- |\n| -i, --file-id TEXT            | 文件 ID                                              |\n| --share-id, --si TEXT         | 播放这个分享 ID 下的文件                             |\n| --share-url, --su TEXT        | 播放这个分享 url 下的文件                            |\n| -p, --password TEXT           | 链接密码，如果没有不用设置                           |\n| -R, --recursive               | 递归播放                                             |\n| -f, --from-index INTEGER      | 从所有目录中的第几个文件开始播放，默认为 0（第一个） |\n| -I, --include TEXT            | 筛选包含这个字符串的文件                             |\n| --include-regex, --IR TEXT    | 筛选包含这个正则表达式的文件                         |\n| -E, --exclude TEXT            | 筛选 不 包含这个字符串的文件                         |\n| --exclude-regex, --ER TEXT    | 筛选 不 包含这个正则表达式的文件                     |\n| --player-params, --PP TEXT    | 第三方播放器参数                                     |\n| -q, --quiet                   | 取消第三方播放器输出                                 |\n| --shuffle, --sf               | 随机播放                                             |\n| --ignore-ext, --IE            | 不用文件名后缀名来判断媒体文件                       |\n| --out-cmd, --OC               | 输出第三方播放器命令                                 |\n| --pl, --player [mpv]          | 指定第三方播放器<br><br>默认为 mpv (https://mpv.io)  |\n| -s, --use-local-server        | 使用本地服务器播放。                                 |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的                         |\n\n## 上传文件\n\n上传一些本地文件或目录到网盘目录。\n\nAliPCS-Py 首先会尝试秒传。如果秒传失败，会使用分片上传上传文件。\n\n上传过程中，按 “p” 可以暂停或继续上传。\n\n```\nAliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定上传方式：\n\n`--upload-type Many`: 同时上传多个文件。\n\n适合大多数文件长度小于 100M 以下的情况。\n\n```\nAliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>\n\n<del>适合大多数文件长度大于 1G 以上的情况。</del>\n\n**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**\n\n```\nAliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定同时上传连接数量:\n\n`--max-workers` 默认为 CPU 核数。\n\n```\nAliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n如果上传本地目录 `localdir` 到远端目录 `remotedir`，AliPCS-Py 是将 `localdir` 这个目录上传到远端目录 `remotedir` 下。\n\n比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。\n\n如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`\n\n### 选项\n\n| Option                                                     | Description                             |\n| ---------------------------------------------------------- | --------------------------------------- |\n| -t, --upload-type [One \\| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密          |\n| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |\n| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |\n| --no-show-progress, --NP                                   | 不显示上传进度                          |\n\n## 同步本地目录到远端\n\n同步本地目录到远端。\n\n如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。\n\n```\nAliPCS-Py sync [OPTIONS] LOCALDIR REMOTEDIR\n```\n\n### 选项\n\n| Option                                                     | Description                    |\n| ---------------------------------------------------------- | ------------------------------ |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的   |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密 |\n| -w, --max-workers INTEGER                                  | 同时上传文件数                 |\n| --no-show-progress, --NP                                   | 不显示上传进度                 |\n\n## 关于秒传连接\n\n**阿里云盘已经不能实现用秒传连接上传。**\n\n## 分享文件\n\n```\nAliPCS-Py share [OPTIONS] [REMOTEPATHS]...\n```\n\n### 选项\n\n| Option                      | Description                      |\n| --------------------------- | -------------------------------- |\n| -p, --password TEXT         | 设置秘密，4 个字符。默认没有秘密 |\n| --period-time, --pt INTEGER | 设置分享有效期，单位为天         |\n\n## 列出分享链接\n\n```\nAliPCS-Py shared\n```\n\n### 选项\n\n| Option         | Description                                  |\n| -------------- | -------------------------------------------- |\n| -A, --show-all | 显示所有分享的链接，默认只显示有效的分享链接 |\n\n## 取消分享链接\n\n```\nAliPCS-Py cancelshared [OPTIONS] [SHARE_IDS]...\n```\n\n## 列出其他用户分享链接中的文件\n\n给 `ls` 命令加参数，我们可以列出其他用户分享链接中的文件。\n\n**注意: 这里 `remotepaths` 只能是绝对路径。**\n\n如果有分享密码，加上 `--password PASSWORD`。\n\n- 使用分享连接\n\n  ```\n  AliPCS-Py ls --share-url SHARE_URL\n\n  # e.g.\n\n  # 列出这个分享url的根目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归列出这个分享url的文件\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 列出这个分享url的指定目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  分享 ID 是 https://www.aliyundrive.com/s/DaNNsdvi9bi 中的 `DaNNsdvi9bi`\n\n  ```\n  AliPCS-Py ls /path --share-id SHARE_ID\n\n  # e.g.\n\n  # 列出这个分享ID的根目录\n  AliPCS-Py ls / --share-id DaNNsdvi9bi\n\n  # 列出这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py ls --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `ls` 命令。\n\n## 下载他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`download` 命令可以直接下载他人分享的文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py download /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py download /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py download --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 下载这个分享url的指定目录\n  AliPCS-Py download --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi -R\n\n  # 下载这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py download --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `download` 命令。\n\n## 播放他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`play` 命令可以直接播放他人分享的媒体文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py play /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py play /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py play --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 播放这个分享url的指定目录\n  AliPCS-Py play --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi -R\n\n  # 播放这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py play --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `play` 命令。\n\n## 保存其他用户分享的链接\n\n保存其他用户分享的链接到远端目录。\n\n```\nAliPCS-Py save [OPTIONS] SHARE_URL_OR_ID REMOTEDIR\n```\n\n指定 `--file-id` 可以保存指定的文件。\n\n### 选项\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -i, --file-id TEXT  | 文件 ID                        |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 本地保存分享连接\n\n可以将他人分享了连接保存至本地，而不需要保存在网盘。这只作为一个记录。在需要是提供查看搜索功能。\n\n使用这个功能，需要使用者在本地配置文件(`~/.alipcs-py/config.toml`)中配置:\n\n```toml\n[share]\nstore = true\n```\n\n这个功能开启后，所有与他人分享连接的操作，都会将连接和其中访问过的文件信息保存在本地文件 `~/.alipcs-py/shared-store.sqlite3` 中。\n\n使用者可以用下面的命令来查看或搜索保存的分享连接。\n\n## 保存分享连接至本地\n\n```\nAliPCS-Py storesharedlinks [OPTIONS] [SHARE_URLS_OR_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 显示本地保存的分享连接\n\n```\nAliPCS-Py listsharedlinks\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 显示本地保存的分享文件\n\n```\nAliPCS-Py listsharedfiles [OPTIONS]\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description                |\n| --------------------- | -------------------------- |\n| --share-id, --si TEXT | 指定显示 share id 下的文件 |\n\n## 查找本地保存的分享连接\n\n```\nAliPCS-Py findsharedlinks [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 查找本地保存的分享文件\n\n```\nAliPCS-Py findsharedfiles [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description       |\n| --------------------- | ----------------- |\n| --share-id, --si TEXT | 要搜索的 share id |\n| -v, --verbose         | 显示细节          |\n\n## 查找本地保存的分享连接和文件\n\n```\nAliPCS-Py findshared [OPTIONS] [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option        | Description |\n| ------------- | ----------- |\n| -v, --verbose | 显示细节    |\n\n## 删除本地保存的分享连接或文件\n\n```\nAliPCS-Py deletestoredshared [OPTIONS] [SHARE_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option             | Description                                                |\n| ------------------ | ---------------------------------------------------------- |\n| -k, --keyword TEXT | 要删除文件名的关键字，如果为空则删除 share_id 下的所有文件 |\n\n## 清理本地保存的无效分享连接\n\n```\nAliPCS-Py cleanstore\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 开启 HTTP 服务\n\n在远端 `ROOT_DIR` 目录下开启 HTTP 服务。\n\n`ROOT_DIR` 默认为 `/`\n\n```\nAliPCS-Py AliPCS-Py server [OPTIONS] [ROOT_DIR]\n```\n\n如果需要设置认证，使用下面的选项设置用户名和密钥：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --username \'foo\' --password \'bar\'\n```\n\n也可以指定服务路径：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --path \'/my/pan\'\n\n# 访问 http://localhost:8000/my/pan/\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| --path TEXT                   | 服务路径，默认为 “/”         |\n| -h, --host TEXT               | 监听 host                    |\n| -p, --port INTEGER            | 监听 port                    |\n| -w, --workers INTEGER         | 进程数                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n| --username TEXT               | HTTP Basic Auth 用户名       |\n| --password TEXT               | HTTP Basic Auth 密钥         |\n',
+    'long_description': '# AliPCS-Py\n\n**2023-04-24 支持 阿里云盘开放平台 api。**\n\n**2023-02-15 使用临时 API 接口，让下载可用。**\n\n**2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**\n\n[![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)\n![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)\n\nAn AliPCS API and An App\n\nAliPCS-Py 是阿里云盘的非官方 api 和一个命令行运用程序。\n\n变更日志在 [CHANGELOG.md](./CHANGELOG.md)。\n\n---\n\n## 百度云盘 api 和 命令行客户端在 https://github.com/PeterDing/BaiduPCS-Py\n\n---\n\n- [安装](#安装)\n- [更新](#更新)\n- [API](#API)\n- [用法](#用法)\n- [命令别名](#命令别名)\n- [对多个帐号进行相同操作](#对多个帐号进行相同操作)\n\n#### 用户相关命令\n\n- [添加用户](#添加用户)\n- [显示当前用户的信息](#显示当前用户的信息)\n- [更新用户信息](#更新用户信息)\n- [显示所有用户](#显示所有用户)\n- [切换当前用户](#切换当前用户)\n- [删除一个用户](#删除一个用户)\n- [显示当前工作目录](#显示当前工作目录)\n- [切换当前工作目录](#切换当前工作目录)\n\n#### 无感加密解密文件\n\n- [设置文件加密密码](#设置文件加密密码)\n\n#### 文件操作相关命令\n\n- [文件操作](#文件操作)\n- [列出网盘路径下的文件](#列出网盘路径下的文件)\n- [搜索文件](#搜索文件)\n- [显示文件内容](#显示文件内容)\n- [创建目录](#创建目录)\n- [移动文件](#移动文件)\n- [文件重命名](#文件重命名)\n- [拷贝文件](#拷贝文件)\n- [删除文件](#删除文件)\n- [下载文件或目录](#下载文件或目录)\n- [播放媒体文件](#播放媒体文件)\n- [上传文件](#上传文件)\n- [同步本地目录到远端](#同步本地目录到远端)\n\n#### 秒传\n\n- [关于秒传连接](#关于秒传连接)\n\n#### 分享相关命令\n\n- [分享文件](#分享文件)\n- [列出分享链接](#列出分享链接)\n- [取消分享链接](#取消分享链接)\n- [列出其他用户分享链接中的文件](#列出其他用户分享链接中的文件)\n- [下载他人分享的文件](#下载他人分享的文件)\n- [播放他人分享的文件](#播放他人分享的文件)\n- [保存其他用户分享的链接](#保存其他用户分享的链接)\n\n#### 本地保存分享连接\n\n- [保存分享连接至本地](#保存分享连接至本地)\n- [显示本地保存的分享连接](#显示本地保存的分享连接)\n- [显示本地保存的分享文件](#显示本地保存的分享文件)\n- [查找本地保存的分享连接](#查找本地保存的分享连接)\n- [查找本地保存的分享文件](#查找本地保存的分享文件)\n- [查找本地保存的分享连接和文件](#查找本地保存的分享连接和文件)\n- [删除本地保存的分享连接或文件](#删除本地保存的分享连接或文件)\n- [清理本地保存的无效分享连接](#清理本地保存的无效分享连接)\n\n#### HTTP 服务\n\n- [开启 HTTP 服务](#开启-HTTP-服务)\n\n## 安装\n\n需要 Python 版本大于或等于 3.8\n\n```\npip3 install Cython\npip3 install AliPCS-Py\n```\n\n### Windows 依赖\n\n在 Windows 上，AliPCS-Py 依赖 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。\n\n在安装 AliPCS-Py 前，请先安装 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)，再在其中勾选 `C++ 生成工具` 并安装。完成后即可安装 AliPCS-Py。\n\n## 更新\n\n```\npip3 install AliPCS-Py --upgrade\n```\n\n## API\n\nAliPCS-Py 的阿里云盘 API 只依赖 requests，方便用户开发自己的运用。\n\n```python\nfrom alipcs_py.alipcs import AliPCSApi\n\napi = AliPCSApi(refresh_token)\n```\n\n## 用法\n\n```\nAliPCS-Py --help\n```\n\n## 命令别名\n\n可以用下面的命令别名代替原来的命令名。\n\n| 别名 | 原名         |\n| ---- | ------------ |\n| w    | who          |\n| uu   | updateuser   |\n| su   | su           |\n| ul   | userlist     |\n| ua   | useradd      |\n| ep   | encryptpwd   |\n| ud   | userdel      |\n| l    | ls           |\n| f    | search       |\n| md   | mkdir        |\n| mv   | move         |\n| rn   | rename       |\n| cp   | copy         |\n| rm   | remove       |\n| d    | download     |\n| p    | play         |\n| u    | upload       |\n| sn   | sync         |\n| S    | share        |\n| sl   | shared       |\n| cs   | cancelshared |\n| s    | save         |\n| sv   | server       |\n\n## 对多个帐号进行相同操作\n\nAliPCS-Py 支持对多个帐号进行相同操作。比如，用相同关键字搜索多个帐号，上传相同的文件/目录到多个帐号，等等。\n\n使用者只需用 `--users` 选项来指定要操作的帐号名即可。\n\n`--users` 接受一个参数，这个参数是用“,”连接的要进行操作帐号名的部分字符。假设我们现在有 3 个帐号，帐号名分别是 `Tom`，`Peter`，`Joy`。\n现在我要同时对`Tom`和`Joy`进行关键字搜索。我们可以用下面的命令进行：\n\n```\nAliPCS-Py --users \'Tom,Joy\' search \'keyword\' / -R\n```\n\n或者给出帐号名的部分片段：\n\n```\nAliPCS-Py --users \'om,oy\' search \'keyword\' / -R\n```\n\n更简单可以用：\n\n```\n# Tom, Joy 都包含字符 "o"\nAliPCS-Py --users \'o\' search \'keyword\' / -R\n```\n\n如果要对所有帐号进行操作用 `--users \'\'`。\n\n如果不使用 `--users` 选项，默认只对当前帐号进行操作。\n\n以下命令支持对多个帐号进行操作：\n\n- pwd\n- ls\n- search\n- cat\n- mkdir\n- move\n- rename\n- copy\n- remove\n- download\n- play\n- upload\n- sync\n- share\n- shared\n- cancelshared\n- save\n- server\n\n**注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。\n\n## 添加用户\n\n**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**\n\nAliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。\n\n### 使用 web `refresh_token` 和 第三方认证地址 登录\n\n第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-server "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录\n\n如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 登录\n\n使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。\n\n使用者可以用下面的方式获取用户的 `refresh_token` 值。\n\n1. 登录 https://www.aliyundrive.com/drive/\n2. 打开浏览器的开发者工具(如 Chrome DevTools)。\n3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。\n\n![refresh_token](./imgs/refresh_token.png)\n\n现在找到了 `refresh_token` 值，我们可以用下面的命令添加一个用户。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..."\n```\n\nAliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。\n\n**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**\n\n## 显示当前用户的信息\n\n```\nAliPCS-Py who\n```\n\n或者：\n\n```\nAliPCS-Py who user_id\n```\n\n指明显示用户 id 为 `user_id` 的用户信息。\n\n### 选项\n\n| Option                       | Description                |\n| ---------------------------- | -------------------------- |\n| -K, --show-encrypt-password  | 显示加密密码               |\n| --account-name TEXT          | 账号名 [默认为 user id]    |\n| --web-refresh-token TEXT     | 用户 web_refresh_token     |\n| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |\n| --client-id TEXT             | openapi client id          |\n| --client-secret TEXT         | openapi client secret      |\n| --client-server TEXT         | openapi client server      |\n\n## 更新用户信息\n\n默认更新当前用户信息。\n\n```\nAliPCS-Py updateuser\n```\n\n也可指定多个 `user_id`\n\n```\nAliPCS-Py updateuser user_id\n```\n\n## 显示所有用户\n\n```\nAliPCS-Py userlist\n```\n\n## 切换当前用户\n\n```\nAliPCS-Py su\n```\n\n或者指定用户列表中用户所在的位置：\n\n```\nAliPCS-Py su 2\n```\n\n## 删除一个用户\n\n```\nAliPCS-Py userdel\n```\n\n## 设置文件加密密码\n\nAliPCS-Py 支持“无感的”文件加密。\n\nAliPCS-Py 可以加密上传文件，在下载的时候自动解密，让使用者感觉不到加密解密的过程。\n\n如果使用者需要将保密文件上传至阿里云盘保存，可以使用这个方法。即使帐号被盗，攻击者也无法还原文件内容。\n\nAliPCS-Py 支持以下加密方法：\n\n- **Simple** 一种简单的加密算法。根据密钥生成一个字节对照表来加密解密文件。\n  速度快，但**不安全**，不建议加密重要文件。\n  因为这种算法加解密不需要知道上下文信息，所以，下载时支持分段下载，如果是媒体文件则支持拖动播放。\n  推荐用于加密不重要的媒体文件。\n- **ChaCha20** 工业级加密算法，速度快，推荐用于加密重要文件。不支持分段下载。\n- **AES256CBC** 工业级加密算法，推荐用于加密重要文件。不支持分段下载。\n\n**注意**：用命令 `encryptpwd` 设置的密码**只是为当前用户**的。\n\n为当前用户设置加密密码:\n\n交互添加：\n\n```\nAliPCS-Py encryptpwd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py encryptpwd --encrypt-password \'my-encrypt-password\'\n```\n\n上传并加密文件：\n\n上传和同步文件时只需要指定加密算法就可。如果不指定就不加密。\n\n```\n# 默认使用上面设置的 `encrypt-password`\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type AES256CBC\n```\n\n下载并用上面设置的 `encrypt-password` 自动解密文件：\n\n```\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/\n```\n\n也可以使用临时的 `encrypt-password`：\n\n```\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type Simple --encrypt-password \'onlyyou\'\n```\n\n但在使用临时的 `encrypt-password` 后，`cat`、下载和播放这些文件时需要指定 `encrypt-password`，但不需要指定加密算法，程序会自动检查加密算法：\n\n```\n# 下载\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/  --encrypt-password \'onlyyou\'\n\n# 开启本地服务并播放\nAliPCS-Py play /to/here/some-file.mp4 --encrypt-password \'onlyyou\' --use-local-server\n```\n\n显示当前用户的密钥：\n\n```\nAliPCS-Py who --show-encrypt-password\n```\n\nAliPCS-Py 下载时默认会解密文件，如果想要下载但不解密文件，需要加 `--no-decrypt`\n\n```\nAliPCS-Py download some-file --no-decrypt\n```\n\n## 文件操作\n\nAliPCS-Py 操作网盘中的文件可以使用文件的绝对路径或相对路径（相对与当前目录 pwd）。\n\n每一个用户都有自己的当前工作目录（pwd），默认为 `/` 根目录。\n\n使用者可以用 `cd` 命令来切换当前的工作目录（pwd）。\n\n下面所有涉及网盘路径的命令，其中如果网盘路径用的是相对路径，那么是相对于当前工作目录（pwd）的。\n如果是网盘路径用的是绝对路径，那么就是这个绝对路径。\n\n## 显示当前工作目录\n\n```\nAliPCS-Py pwd\n```\n\n## 切换当前工作目录\n\n切换到绝对路径：\n\n```\nAliPCS-Py cd /to/some/path\n```\n\n切换到相对路径：\n\n```\n# 切换到 (pwd)/../path\nAliPCS-Py cd ../path\n```\n\n## 列出网盘路径下的文件\n\n使用文件路径：\n\n```\nAliPCS-Py ls [OPTIONS] [REMOTEPATHS]...\n\nAliPCS-Py ls /absolute/path\n\n# or\nAliPCS-Py ls relative/path\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py ls -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                     | Description                                           |\n| -------------------------- | ----------------------------------------------------- |\n| -i, --file-id TEXT         | 文件 ID                                               |\n| --share-id, --si TEXT      | 列出这个分享 ID 下的文件                              |\n| --share-url, --su TEXT     | 列出这个分享 url 下的文件                             |\n| -p, --password TEXT        | 分享链接密码，如果没有不用设置                        |\n| -r, --desc                 | 逆序排列文件                                          |\n| -n, --name                 | 依名字排序                                            |\n| -t, --time                 | 依时间排序                                            |\n| -s, --size                 | 依文件大小排序                                        |\n| -R, --recursive            | 递归列出文件                                          |\n| -I, --include TEXT         | 筛选包含这个字符串的文件                              |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件                          |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件                      |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件                  |\n| -f, --is-file              | 筛选 **非** 目录文件                                  |\n| -d, --is-dir               | 筛选目录文件                                          |\n| --no-highlight, --NH       | 取消匹配高亮                                          |\n| -S, --show-size            | 显示文件大小                                          |\n| -D, --show-date            | 显示文件创建时间                                      |\n| --show-file-id, --ID       | 显示文件 ID                                           |\n| -M, --show-hash            | 显示文件 sha1                                         |\n| -A, --show-absolute-path   | 显示文件绝对路径                                      |\n| --show-dl-link, --DL       | 显示文件下载连接                                      |\n| --csv                      | 用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用 |\n| --only-dl-link, --ODL      | 只显示文件下载连接                                    |\n\n## 搜索文件\n\n搜索包含 `keyword` 的文件\n\n```\nAliPCS-Py search [OPTIONS] KEYWORD [REMOTEDIR]\n\n# 在当前工作目录中搜索\nAliPCS-Py search keyword\n\n# or\nAliPCS-Py search keyword /absolute/path\n\n# or\nAliPCS-Py search keyword relative/path\n```\n\n### 选项\n\n| Option                     | Description                          |\n| -------------------------- | ------------------------------------ |\n| -R, --recursive            | 递归搜索文件                         |\n| -I, --include TEXT         | 筛选包含这个字符串的文件             |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件         |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件     |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件 |\n| -f, --is-file              | 筛选 **非** 目录文件                 |\n| -d, --is-dir               | 筛选目录文件                         |\n| --no-highlight, --NH       | 取消匹配高亮                         |\n| -S, --show-size            | 显示文件大小                         |\n| -D, --show-date            | 显示文件创建时间                     |\n| -M, --show-hash            | 显示文件 sha1                        |\n| --csv                      | 用 csv 格式显示                      |\n\n## 显示文件内容\n\n```\nAliPCS-Py cat [OPTIONS] REMOTEPATH\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| -e, --encoding TEXT           | 文件编码，默认自动解码       |\n| --no-decrypt, --ND            | 不解密                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n\n## 创建目录\n\n```\nAliPCS-Py mkdir [OPTIONS] [REMOTEDIRS]...\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示目录    |\n\n## 移动文件\n\n移动一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 文件重命名\n\n```\nAliPCS-Py rename [OPTIONS] REMOTEPATH NEW_NAME\n```\n\ne.g.\n\n重命名 `/path/to/far` to `/path/to/foo`\n\n```\nAliPCS-Py rename /path/to/far foo\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 拷贝文件\n\n拷贝一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 删除文件\n\n```\nAliPCS-Py remove [OPTIONS] [REMOTEPATHS]...\n\n# 指定 路径\nAliPCS-Py remove /some/path\n# 指定 file-id\nAliPCS-Py remove --file-id ...\n```\n\n### 选项\n\n| Option        | Description  |\n| ------------- | ------------ |\n| -i, --file-id | TEXT 文件 ID |\n\n## 下载文件或目录\n\n> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。\n> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py download [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py download -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                    |\n| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| -i, --file-id TEXT                                     | 文件 ID                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| --share-id, --si TEXT                                  | 下载这个分享 ID 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --share-url, --su TEXT                                 | 下载这个分享 url 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                      |\n| -p, --password TEXT                                    | 分享链接密码，如果没有不用设置                                                                                                                                                                                                                                                                                                                                                                                                                                 |\n| -o, --outdir TEXT                                      | 指定下载本地目录，默认为当前目录                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -R, --recursive                                        | 递归下载                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| -f, --from-index INTEGER                               | 从所有目录中的第几个文件开始下载，默认为 0（第一个）                                                                                                                                                                                                                                                                                                                                                                                                           |\n| -I, --include TEXT                                     | 筛选包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --include-regex, --IR TEXT                             | 筛选包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| -E, --exclude TEXT                                     | 筛选 不 包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| --exclude-regex, --ER TEXT                             | 筛选 不 包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -s, --concurrency INTEGER                              | 下载同步链接数，默认为 5。建议小于 10。                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| -k, --chunk-size TEXT                                  | 同步链接分块大小，默认为 50MB                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| -d, --downloader [ me \\| aget_py \\| aget_rs \\| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |\n| --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n\n## 播放媒体文件\n\n> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。\n> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py play [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n**注意：目前，使用 `--share-id` 或 `--file-id` 时，无法使用 `--use-local-server`**\n\n```\nAliPCS-Py play -i file_id1 -i file_id2 -i ...\n```\n\n`play` 命令默认播放带有媒体后缀的文件，如 `abc.mp4`, `abc.mp3`。如果需要播放的媒体文件没有用常规的媒体文件后缀，则需要加选项 `--ignore-ext`。\n\n### 选项\n\n| Option                        | Description                                          |\n| ----------------------------- | ---------------------------------------------------- |\n| -i, --file-id TEXT            | 文件 ID                                              |\n| --share-id, --si TEXT         | 播放这个分享 ID 下的文件                             |\n| --share-url, --su TEXT        | 播放这个分享 url 下的文件                            |\n| -p, --password TEXT           | 链接密码，如果没有不用设置                           |\n| -R, --recursive               | 递归播放                                             |\n| -f, --from-index INTEGER      | 从所有目录中的第几个文件开始播放，默认为 0（第一个） |\n| -I, --include TEXT            | 筛选包含这个字符串的文件                             |\n| --include-regex, --IR TEXT    | 筛选包含这个正则表达式的文件                         |\n| -E, --exclude TEXT            | 筛选 不 包含这个字符串的文件                         |\n| --exclude-regex, --ER TEXT    | 筛选 不 包含这个正则表达式的文件                     |\n| --player-params, --PP TEXT    | 第三方播放器参数                                     |\n| -q, --quiet                   | 取消第三方播放器输出                                 |\n| --shuffle, --sf               | 随机播放                                             |\n| --ignore-ext, --IE            | 不用文件名后缀名来判断媒体文件                       |\n| --out-cmd, --OC               | 输出第三方播放器命令                                 |\n| --pl, --player [mpv]          | 指定第三方播放器<br><br>默认为 mpv (https://mpv.io)  |\n| -s, --use-local-server        | 使用本地服务器播放。                                 |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的                         |\n\n## 上传文件\n\n上传一些本地文件或目录到网盘目录。\n\nAliPCS-Py 首先会尝试秒传。如果秒传失败，会使用分片上传上传文件。\n\n上传过程中，按 “p” 可以暂停或继续上传。\n\n```\nAliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定同时上传连接数量:\n\n`--max-workers` 默认为 CPU 核数。\n\n```\nAliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n如果上传本地目录 `localdir` 到远端目录 `remotedir`，AliPCS-Py 是将 `localdir` 这个目录上传到远端目录 `remotedir` 下。\n\n比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。\n\n如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`\n\n### 选项\n\n| Option                                                     | Description                           |\n| ---------------------------------------------------------- | ------------------------------------- |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的          |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密        |\n| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数 |\n| --no-ignore-existing, --NI                                 | 上传已经存在的文件                    |\n| --no-show-progress, --NP                                   | 不显示上传进度                        |\n\n## 同步本地目录到远端\n\n同步本地目录到远端。\n\n如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。\n\n```\nAliPCS-Py sync [OPTIONS] LOCALDIR REMOTEDIR\n```\n\n### 选项\n\n| Option                                                     | Description                    |\n| ---------------------------------------------------------- | ------------------------------ |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的   |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密 |\n| -w, --max-workers INTEGER                                  | 同时上传文件数                 |\n| --no-show-progress, --NP                                   | 不显示上传进度                 |\n\n## 关于秒传连接\n\n**阿里云盘已经不能实现用秒传连接上传。**\n\n## 分享文件\n\n```\nAliPCS-Py share [OPTIONS] [REMOTEPATHS]...\n```\n\n### 选项\n\n| Option                      | Description                      |\n| --------------------------- | -------------------------------- |\n| -p, --password TEXT         | 设置秘密，4 个字符。默认没有秘密 |\n| --period-time, --pt INTEGER | 设置分享有效期，单位为天         |\n\n## 列出分享链接\n\n```\nAliPCS-Py shared\n```\n\n### 选项\n\n| Option         | Description                                  |\n| -------------- | -------------------------------------------- |\n| -A, --show-all | 显示所有分享的链接，默认只显示有效的分享链接 |\n\n## 取消分享链接\n\n```\nAliPCS-Py cancelshared [OPTIONS] [SHARE_IDS]...\n```\n\n## 列出其他用户分享链接中的文件\n\n给 `ls` 命令加参数，我们可以列出其他用户分享链接中的文件。\n\n**注意: 这里 `remotepaths` 只能是绝对路径。**\n\n如果有分享密码，加上 `--password PASSWORD`。\n\n- 使用分享连接\n\n  ```\n  AliPCS-Py ls --share-url SHARE_URL\n\n  # e.g.\n\n  # 列出这个分享url的根目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归列出这个分享url的文件\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 列出这个分享url的指定目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  分享 ID 是 https://www.aliyundrive.com/s/DaNNsdvi9bi 中的 `DaNNsdvi9bi`\n\n  ```\n  AliPCS-Py ls /path --share-id SHARE_ID\n\n  # e.g.\n\n  # 列出这个分享ID的根目录\n  AliPCS-Py ls / --share-id DaNNsdvi9bi\n\n  # 列出这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py ls --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `ls` 命令。\n\n## 下载他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`download` 命令可以直接下载他人分享的文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py download /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py download /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py download --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 下载这个分享url的指定目录\n  AliPCS-Py download --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi -R\n\n  # 下载这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py download --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `download` 命令。\n\n## 播放他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`play` 命令可以直接播放他人分享的媒体文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py play /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py play /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py play --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 播放这个分享url的指定目录\n  AliPCS-Py play --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi -R\n\n  # 播放这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py play --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `play` 命令。\n\n## 保存其他用户分享的链接\n\n保存其他用户分享的链接到远端目录。\n\n```\nAliPCS-Py save [OPTIONS] SHARE_URL_OR_ID REMOTEDIR\n```\n\n指定 `--file-id` 可以保存指定的文件。\n\n### 选项\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -i, --file-id TEXT  | 文件 ID                        |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 本地保存分享连接\n\n可以将他人分享了连接保存至本地，而不需要保存在网盘。这只作为一个记录。在需要是提供查看搜索功能。\n\n使用这个功能，需要使用者在本地配置文件(`~/.alipcs-py/config.toml`)中配置:\n\n```toml\n[share]\nstore = true\n```\n\n这个功能开启后，所有与他人分享连接的操作，都会将连接和其中访问过的文件信息保存在本地文件 `~/.alipcs-py/shared-store.sqlite3` 中。\n\n使用者可以用下面的命令来查看或搜索保存的分享连接。\n\n## 保存分享连接至本地\n\n```\nAliPCS-Py storesharedlinks [OPTIONS] [SHARE_URLS_OR_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 显示本地保存的分享连接\n\n```\nAliPCS-Py listsharedlinks\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 显示本地保存的分享文件\n\n```\nAliPCS-Py listsharedfiles [OPTIONS]\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description                |\n| --------------------- | -------------------------- |\n| --share-id, --si TEXT | 指定显示 share id 下的文件 |\n\n## 查找本地保存的分享连接\n\n```\nAliPCS-Py findsharedlinks [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 查找本地保存的分享文件\n\n```\nAliPCS-Py findsharedfiles [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description       |\n| --------------------- | ----------------- |\n| --share-id, --si TEXT | 要搜索的 share id |\n| -v, --verbose         | 显示细节          |\n\n## 查找本地保存的分享连接和文件\n\n```\nAliPCS-Py findshared [OPTIONS] [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option        | Description |\n| ------------- | ----------- |\n| -v, --verbose | 显示细节    |\n\n## 删除本地保存的分享连接或文件\n\n```\nAliPCS-Py deletestoredshared [OPTIONS] [SHARE_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option             | Description                                                |\n| ------------------ | ---------------------------------------------------------- |\n| -k, --keyword TEXT | 要删除文件名的关键字，如果为空则删除 share_id 下的所有文件 |\n\n## 清理本地保存的无效分享连接\n\n```\nAliPCS-Py cleanstore\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 开启 HTTP 服务\n\n在远端 `ROOT_DIR` 目录下开启 HTTP 服务。\n\n`ROOT_DIR` 默认为 `/`\n\n```\nAliPCS-Py AliPCS-Py server [OPTIONS] [ROOT_DIR]\n```\n\n如果需要设置认证，使用下面的选项设置用户名和密钥：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --username \'foo\' --password \'bar\'\n```\n\n也可以指定服务路径：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --path \'/my/pan\'\n\n# 访问 http://localhost:8000/my/pan/\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| --path TEXT                   | 服务路径，默认为 “/”         |\n| -h, --host TEXT               | 监听 host                    |\n| -p, --port INTEGER            | 监听 port                    |\n| -w, --workers INTEGER         | 进程数                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n| --username TEXT               | HTTP Basic Auth 用户名       |\n| --password TEXT               | HTTP Basic Auth 密钥         |\n',
     'author': 'PeterDing',
     'author_email': 'dfhayst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PeterDing/AliPCS-Py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `alipcs_py-0.7.0/PKG-INFO` & `alipcs_py-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AliPCS-Py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Ali Pcs Api and App
 Home-page: https://github.com/PeterDing/AliPCS-Py
 License: MIT
 Author: PeterDing
 Author-email: dfhayst@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -760,34 +760,14 @@
 
 上传过程中，按 “p” 可以暂停或继续上传。
 
 ```
 AliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR
 ```
 
-指定上传方式：
-
-`--upload-type Many`: 同时上传多个文件。
-
-适合大多数文件长度小于 100M 以下的情况。
-
-```
-AliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR
-```
-
-<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>
-
-<del>适合大多数文件长度大于 1G 以上的情况。</del>
-
-**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**
-
-```
-AliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR
-```
-
 指定同时上传连接数量:
 
 `--max-workers` 默认为 CPU 核数。
 
 ```
 AliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR
 ```
@@ -796,22 +776,21 @@
 
 比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。
 
 如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`
 
 ### 选项
 
-| Option                                                     | Description                             |
-| ---------------------------------------------------------- | --------------------------------------- |
-| -t, --upload-type [One \| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |
-| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |
-| -e, --encrypt-type [No \| Simple \| ChaCha20 \| AES256CBC] | 文件加密方法，默认为 No 不加密          |
-| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |
-| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |
-| --no-show-progress, --NP                                   | 不显示上传进度                          |
+| Option                                                     | Description                           |
+| ---------------------------------------------------------- | ------------------------------------- |
+| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的          |
+| -e, --encrypt-type [No \| Simple \| ChaCha20 \| AES256CBC] | 文件加密方法，默认为 No 不加密        |
+| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数 |
+| --no-ignore-existing, --NI                                 | 上传已经存在的文件                    |
+| --no-show-progress, --NP                                   | 不显示上传进度                        |
 
 ## 同步本地目录到远端
 
 同步本地目录到远端。
 
 如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。
```

