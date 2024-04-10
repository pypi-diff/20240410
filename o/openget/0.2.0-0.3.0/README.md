# Comparing `tmp/openget-0.2.0.tar.gz` & `tmp/openget-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openget-0.2.0.tar", last modified: Fri Apr 28 03:33:33 2023, max compression
+gzip compressed data, was "openget-0.3.0.tar", last modified: Tue Apr  9 15:28:30 2024, max compression
```

## Comparing `openget-0.2.0.tar` & `openget-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251543 openget-0.2.0/
--rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.2.0/LICENSE
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-28 03:33:33.251421 openget-0.2.0/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      505 2023-01-14 16:55:04.000000 openget-0.2.0/README.md
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.247490 openget-0.2.0/openget/
--rw-r--r--   0 dytttf     (501) staff       (20)       40 2023-04-28 03:29:34.000000 openget-0.2.0/openget/__init__.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.249649 openget-0.2.0/openget/db/
--rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db.py
--rw-r--r--   0 dytttf     (501) staff       (20)    20309 2023-04-28 03:29:34.000000 openget-0.2.0/openget/db/db_mysql.py
--rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_oracle.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38448 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_oss.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_redis.py
--rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_sqlite.py
--rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/util.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1096 2023-04-28 03:29:34.000000 openget-0.2.0/openget/env.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.250282 openget-0.2.0/openget/network/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    17631 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/downloader.py
--rw-r--r--   0 dytttf     (501) staff       (20)    25752 2023-04-28 03:29:34.000000 openget-0.2.0/openget/network/proxy.py
--rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/request.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/response.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-04-28 02:48:09.000000 openget-0.2.0/openget/setting.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.250636 openget-0.2.0/openget/spiders/
--rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.2.0/openget/spiders/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    15789 2023-04-28 03:29:34.000000 openget-0.2.0/openget/spiders/base.py
--rw-r--r--   0 dytttf     (501) staff       (20)    54681 2023-01-14 16:55:04.000000 openget-0.2.0/openget/spiders/batch_spider.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38777 2023-01-14 16:55:04.000000 openget-0.2.0/openget/util.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251034 openget-0.2.0/openget/utils/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2605 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/log.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251243 openget-0.2.0/openget/utils/message/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/message/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/message/dingtalk.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.248459 openget-0.2.0/openget.egg-info/
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      776 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/SOURCES.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        1 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/dependency_links.txt
--rw-r--r--   0 dytttf     (501) staff       (20)      103 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/requires.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        8 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/top_level.txt
--rw-r--r--   0 dytttf     (501) staff       (20)      810 2023-04-28 03:29:34.000000 openget-0.2.0/pyproject.toml
--rw-r--r--   0 dytttf     (501) staff       (20)       38 2023-04-28 03:33:33.251574 openget-0.2.0/setup.cfg
--rw-r--r--   0 dytttf     (501) staff       (20)     1042 2023-04-28 03:29:34.000000 openget-0.2.0/setup.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.462805 openget-0.3.0/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.3.0/LICENSE
+-rw-r--r--   0 dytttf     (501) staff       (20)     1425 2024-04-09 15:28:30.462685 openget-0.3.0/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      918 2024-04-09 15:25:54.000000 openget-0.3.0/README.md
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.459869 openget-0.3.0/openget/
+-rw-r--r--   0 dytttf     (501) staff       (20)       40 2024-04-09 15:25:54.000000 openget-0.3.0/openget/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      892 2024-04-09 15:25:54.000000 openget-0.3.0/openget/__main__.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.461273 openget-0.3.0/openget/db/
+-rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/db.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    25283 2024-04-09 15:25:54.000000 openget-0.3.0/openget/db/db_mysql.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/db_oracle.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    38449 2024-04-09 15:25:54.000000 openget-0.3.0/openget/db/db_oss.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    20304 2024-04-09 15:25:54.000000 openget-0.3.0/openget/db/db_postgresql.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/db_redis.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/db_sqlite.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.3.0/openget/db/util.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1099 2024-04-09 15:25:54.000000 openget-0.3.0/openget/env.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.461762 openget-0.3.0/openget/network/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.3.0/openget/network/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    17748 2024-04-09 15:25:54.000000 openget-0.3.0/openget/network/downloader.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    25752 2023-04-28 03:29:34.000000 openget-0.3.0/openget/network/proxy.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.3.0/openget/network/request.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.3.0/openget/network/response.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-04-28 02:48:09.000000 openget-0.3.0/openget/setting.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.462047 openget-0.3.0/openget/spiders/
+-rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.3.0/openget/spiders/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    15876 2024-04-09 15:25:54.000000 openget-0.3.0/openget/spiders/base.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    54692 2024-04-09 15:25:54.000000 openget-0.3.0/openget/spiders/batch_spider.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    25363 2024-04-09 15:25:54.000000 openget-0.3.0/openget/util.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.462336 openget-0.3.0/openget/utils/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.3.0/openget/utils/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2618 2024-04-09 15:25:54.000000 openget-0.3.0/openget/utils/log.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.462529 openget-0.3.0/openget/utils/message/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.3.0/openget/utils/message/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.3.0/openget/utils/message/dingtalk.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    13577 2024-04-09 15:25:54.000000 openget-0.3.0/openget/utils/s3.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2024-04-09 15:28:30.460358 openget-0.3.0/openget.egg-info/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1425 2024-04-09 15:28:30.000000 openget-0.3.0/openget.egg-info/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      844 2024-04-09 15:28:30.000000 openget-0.3.0/openget.egg-info/SOURCES.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        1 2024-04-09 15:28:30.000000 openget-0.3.0/openget.egg-info/dependency_links.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)      103 2024-04-09 15:28:30.000000 openget-0.3.0/openget.egg-info/requires.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        8 2024-04-09 15:28:30.000000 openget-0.3.0/openget.egg-info/top_level.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)      809 2024-04-09 15:25:54.000000 openget-0.3.0/pyproject.toml
+-rw-r--r--   0 dytttf     (501) staff       (20)       38 2024-04-09 15:28:30.462836 openget-0.3.0/setup.cfg
+-rw-r--r--   0 dytttf     (501) staff       (20)     1042 2023-04-28 03:29:34.000000 openget-0.3.0/setup.py
```

### Comparing `openget-0.2.0/LICENSE` & `openget-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/PKG-INFO` & `openget-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
@@ -18,25 +18,36 @@
 # openget
 A Spider FrameWork.
 
 ## Installation
 You can install openget by simply doing:
 
     pip install openget
+    pip install git+https://github.com/dytttf/openget.git@main
+    pip install git+https://github.com/dytttf/openget.git@dev
+
     
 ## Usage
 **Very Important Thing**
 This line must be the first line in code
 ```
 from openget.spiders import *
 ```
+### 命令行支持
+1. 生成配置文件样例
+```shell
+# 环境变量类型的配置文件
+python -m openget --gen_env_example
+```
 
 
 ## About Environment Variable
-> ~/.openget/.env < $(pwd)/.env
+### 优先级
+1. $(pwd)/.env
+2. ~/.openget/.env
 
 
 ## docker build
 ```shell
 cd docekr
 bash build.sh
 ```
@@ -44,7 +55,11 @@
 ## TODO
 - ftp download
 - auto add task
 - statis crawl speed
 - browser support: zhipin.com tmall.com
 - sqlite.db rename
 - use cmd to create spider template
+- 金融许可证 卡死问题处理
+- 环境变量定义优化
+- 新项目创建优化
+- 极简模式、完整模式 减少包的依赖
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openget-0.2.0/openget/db/db.py` & `openget-0.3.0/openget/db/db.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/db/db_mysql.py` & `openget-0.3.0/openget/db/db_postgresql.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,715 +1,684 @@
-# coding:utf8
-"""
-MySQL utils
+# -*- coding: utf-8 -*-
 
-Known Issue:
-    Sometimes, in gevent environment, pymysql will raise an error:
-        RuntimeError: reentrant call inside <_io.BufferedReader name=8>
 """
+"""
+import json
 import copy
 import datetime
-import json
-import logging
+import threading
 import time
 from collections import OrderedDict, defaultdict
-from typing import List, Tuple, Dict
-
-import pymysql
-
-escape_str = pymysql.converters.escape_str
-
-try:
-    import_mysqldb_error = None
-    import MySQLdb
-except ImportError as e:
-    MySQLdb = None
-    import_mysqldb_error = e
+import psycopg2
 
 from openget.utils import log
 
+mutex = threading.RLock()
 
-MysqlError = (pymysql.OperationalError, pymysql.ProgrammingError)
 
-if MySQLdb:
-    MysqlError = (
-        pymysql.OperationalError,
-        MySQLdb.OperationalError,
-        pymysql.ProgrammingError,
-        MySQLdb.ProgrammingError,
-    )
-
-
-def get_connection(options: Dict, **kwargs):
-    """
-    Args:
-        options:
-        **kwargs:
-
-    Returns:
-
-    """
-    username = options["username"]
-    password = options["password"]
-    host = options["host"]
-    port = options["port"]
-    if port is None:
-        port = 3306
-    db_default = options["db"]
-    params = options["params"]
-    charset = params.get("charset", ["utf8mb4"])[0]
-
-    if "pymysql" in options["type"]:
-        connection = pymysql.connect(
-            host=host,
-            port=port,
-            user=username,
-            passwd=password,
-            db=db_default,
-            charset=charset,
-            **kwargs,
-        )
-        connection.set_charset(charset)
-    elif "mysqldb" in options["type"]:
-        if not MySQLdb:
-            # 抛出异常
-            raise import_mysqldb_error
-        connection = MySQLdb.connect(
-            host=host,
-            port=port,
-            user=username,
-            passwd=password,
-            db=db_default,
-            charset=charset,
-            **kwargs,
-        )
-        connection.set_character_set(charset)
-    else:
-        raise ValueError("unknown mysql type: {}".format(options["type"]))
-    connection.autocommit(True)
-    return connection
+def escape_string(s: str):
+    return s.replace("'", "''")
 
 
 class Cursor(object):
-    """
-    Cursor class, catch timeout errors and reconnect
-    """
-
-    def __init__(
-        self,
-        connection: pymysql.Connection,
-        options: Dict,
-        logger: logging.Logger = None,
-        **kwargs,
-    ):
+    """重新封装cursor使得可以自动捕获mysql连接超时错误并重新连接"""
 
-        self.connection = connection
-        self.cursor = self.connection.cursor()
+    def __init__(self, connection, options, logger=None, cursor_class=None, **kwargs):
+        self.conn = connection
+        self.cursor = None
+        self.cursor_class = cursor_class
+        self.reconnect(connection)
 
         self.kwargs = kwargs
         self.options = options
 
         self.logger = self.kwargs.pop("logger", logger) or log.get_logger(__file__)
 
-        self._init()
-
     def __getattr__(self, name):
+        """不存在的属性调用原cursor"""
         return getattr(self.cursor, name)
 
-    def _init(self):
-        """
-            1、at the session level, set range_optimizer_max_mem_size=83886080 to optimize update performance, the default is 8388608(8M).
-
-        Returns:
-
-        """
-        try:
-            sql = "show variables like '%range_optimizer_max_mem_size%';"
-            self.cursor.execute(sql)
-            _r = self.cursor.fetchall()
-            if _r:
-                # PolorDB doesn't have this variable
-                old_size = int(_r[0][1])
-                if old_size < 83_886_080:
-                    self.cursor.execute(
-                        "set session range_optimizer_max_mem_size=83886080;"
-                    )
-        except Exception:
-            self.logger.exception("set range_optimizer_max_mem_size failed")
-        return
+    def reconnect(self, conn=None):
+        conn = conn or PostgreSQLOpt.get_conn(self.options, **self.kwargs)
+        self.cursor = conn.cursor()
+        self.conn = conn
+        return self.conn, self.cursor
 
     def execute(self, sql, args=None, retry=0):
         try:
-            result = self.cursor.execute(sql, args=args)
-        except MysqlError as e:
-            # catch: timeout error, closed error, ...
-            if retry < 20 and e.args[0] in (
-                2006,
-                2013,
-                "cursor closed",
-                "Cursor closed",
+            mutex.acquire()
+            try:
+                self.conn.ping(reconnect=True)
+            except:
+                pass
+            self.cursor.execute(sql, args)
+            result = 1
+        except (psycopg2.OperationalError, psycopg2.ProgrammingError) as e:
+            # 捕获超时异常 关闭异常
+            if retry < 20 and str(e.args[0]).lower() in (
+                "server closed the connection unexpectedly",
+                "connection has been closed unexpectedly",
+                "server closed the connection without sending any data",
             ):
-                self.logger.debug("mysql connect error:{}  try reconnect...".format(e))
+                self.logger.debug(f"pg连接错误:{e}  重连(retry={retry})中...")
                 time.sleep(retry * 5)
                 # 重连
-                self.connectioin = get_connection(self.options, **self.kwargs)
-                self.cursor = self.connectioin.cursor()
+                self.reconnect()
                 return self.execute(sql, args=args, retry=retry + 1)
             raise e
+        finally:
+            mutex.release()
         return result
 
 
-class MySQLOpt(object):
+class PostgreSQLOpt(object):
+    """和mysql方法保持一致，按说应该提取出基类，有点懒先这么写吧"""
+
+    # 连接池 共用
     connection_list = {}
 
-    def __init__(self, options: Dict, **kwargs):
+    def __init__(
+        self, options, is_pool: bool = True, cursor_class: str = None, **kwargs
+    ):
         """
         Args:
-            options:
+            options: postgresql连接参数字典
+            is_pool: 是否使用连接池模式
+            cursor_class:
+                cursor, dict_cursor, ss_cursor, ss_dict_cursor
             **kwargs:
-                reuse_connection:
+                autocommit:
         """
-        self.reuse_connection = kwargs.pop("reuse_connection", True)
+        self.is_pool = is_pool
+        self.cursor_class = cursor_class
+        self.autocommit = kwargs.setdefault("autocommit", True)
+        if self.is_pool:
+            print("警告: 在多线程中用同一个postgresql连接同时进行插入和查询操作时，插入操作会影响到查询结果...")
 
+        # 额外参数
         self.kwargs = kwargs
+
         self.options = options
         self.key = repr(options)
 
-        self.logger: logging.Logger = self.kwargs.pop("logger", None) or log.get_logger(
-            __file__
-        )
+        self.logger = self.kwargs.pop("logger", None) or log.get_logger(__file__)
 
         self.table_name = ""
 
-        #
-        self._connection = None
+        # 私有变量
+        self._conn = None
         self._cursor = None
 
     def __del__(self):
         try:
             self.close()
-        except Exception:
+        except Exception as e:
             pass
 
     @property
-    def connection(self):
-        self._connection = self.cursor.connection
-        return self._connection
+    def conn(self):
+        """
+        获取mysql连接
+        Returns:
+
+        """
+        self._conn = self.cursor.conn
+        return self._conn
 
     @property
     def cursor(self):
+        """
+        获取游标
+        Returns:
+
+        """
         if not self._cursor:
-            if (
-                not self.reuse_connection
-                or self.key not in MySQLOpt.connection_list.keys()
-            ):
+            if not self.is_pool or self.key not in self.connection_list.keys():
                 self._cursor = self.get_cursor()
-                if self.reuse_connection:
-                    MySQLOpt.connection_list[self.key] = self._cursor
+                if self.is_pool:
+                    self.connection_list[self.key] = self._cursor
             else:
-                self._cursor = MySQLOpt.connection_list[self.key]
+                self._cursor = self.connection_list[self.key]
         return self._cursor
 
-    def get_cursor(self, connection: pymysql.Connection = None):
+    @staticmethod
+    def get_conn(options, **kwargs):
         """
+            建立pg连接
         Args:
-            connection:
+            options:
+            **kwargs:
 
         Returns:
 
         """
-        connection = connection or get_connection(self.options, **self.kwargs)
-        cursor = Cursor(connection, self.options, logger=self.logger, **self.kwargs)
-        return cursor
 
-    @staticmethod
-    def escape_str(*args, **kwargs):
-        return escape_str(*args, **kwargs)
+        autocommit = kwargs.pop("autocommit", True)
 
-    @staticmethod
-    def escape_values(
-        data: Dict, sort_keys: List = None, strip: bool = True
-    ) -> OrderedDict:
-        """
-            Convert data to mysql support types.
-
-            string/int/float/datetime -> string
-            None -> null
-            others -> json.dumps()
+        db_user = options["username"]
+        db_passwd = options["password"]
+        db_host = options["host"]
+        db_port = options["port"]
+        if db_port is None:
+            db_port = 5432
+        db_default = options["db"]
+
+        conn = psycopg2.connect(
+            host=db_host,
+            port=db_port,
+            user=db_user,
+            password=db_passwd,
+            database=db_default,
+            **kwargs,
+        )
+
+        conn.autocommit = autocommit
+        return conn
 
+    def get_cursor(self, connection=None):
+        """
+        mysql获取cursor  重新封装过的
+        """
+        connection = connection or PostgreSQLOpt.get_conn(self.options, **self.kwargs)
+        cursor = Cursor(
+            connection,
+            self.options,
+            logger=self.logger,
+            cursor_class=self.cursor_class,
+            **self.kwargs,
+        )
+        return cursor
+
+    @staticmethod
+    def handle_values(data, keys=None, strip=True) -> OrderedDict:
+        """
+        处理字典中的值 转换为pg接受的格式
         Args:
             data:
-            sort_keys:
-            strip: if set True, the string value will be striped
+            keys: 使用给定的key顺序
+            strip: 是否对字符串类型的值进行strip操作
 
         Returns:
-            OrderedDict
-        """
-        if not sort_keys:
-            sort_keys = list(data.keys())
 
-        order_data = OrderedDict()
-        for k in sort_keys:
+        """
+        if not keys:
+            keys = list(data.keys())
+        handle_k_list = []
+        handle_v_list = []
+        for k in keys:
             v = data[k]
-            k = f"`{k}`"
+            handle_k_list.append('"{}"'.format(k))
             if isinstance(v, str):
                 if strip:
                     v = v.strip()
-                v = escape_str(v)
+                handle_v_list.append("'{}'".format(escape_string(v)))
             elif isinstance(v, (int, float)):
-                v = str(v)
+                # np.nan is float
+                handle_v_list.append("{}".format(v))
             elif isinstance(v, (datetime.date, datetime.time)):
-                v = "'{}'".format(v)
+                handle_v_list.append("'{}'".format(v))
             elif v is None:
-                v = "null"
+                handle_v_list.append("null")
             else:
                 v = json.dumps(v, ensure_ascii=False)
-                v = escape_str(v)
-            order_data[k] = v
-        return order_data
+                handle_v_list.append("'{}'".format(escape_string(v)))
+        data = OrderedDict(zip(handle_k_list, handle_v_list))
+        return data
 
     @staticmethod
-    def group_data_by_keys(data: List[Dict]) -> List[List]:
-        """
-
-        Args:
-            data:
-
-        Returns:
-
-        """
+    def group_data_by_keys(data: list):
+        """"""
         data = copy.deepcopy(data)
         group_data_dict = defaultdict(list)
         for item in data:
             keys = list(item.keys())
             keys.sort()
             keys_flag = " ".join(keys)
             group_data_dict[keys_flag].append(item)
         return list(group_data_dict.values())
 
     def add(
         self,
-        data: Dict,
+        data: dict,
         *,
         table_name: str = "",
         ignore_duplicate: bool = True,
-    ) -> int:
+        **kwargs,
+    ):
         """
-            save data to database
+            save one data to database
         Args:
             data:
             table_name:
             ignore_duplicate: ignore duplicate errors
+            **kwargs: 0写入成功  1重复
 
         Returns:
             0: success
             1: duplicate
+
         """
         data = copy.deepcopy(data)
         table_name = table_name or self.table_name
         if not table_name:
-            raise ValueError("table name must be not empty")
+            raise ValueError("table name {}".format(table_name))
         if not data:
-            raise ValueError("data must be not empty")
+            raise ValueError("data is {}".format(data))
         sql = "insert into {table_name} ({keys}) values({values});"
         # 拼接sql
-        order_data = self.escape_values(data)
+        order_data = self.handle_values(data)
         sql = sql.format(
             **{
                 "keys": ",".join(order_data.keys()),
                 "values": ",".join(order_data.values()),
                 "table_name": table_name,
             }
         )
         try:
             self.cursor.execute(sql)
+            if self.autocommit:
+                self.cursor.conn.commit()
             resp = 0
         except Exception as e:
             if ignore_duplicate and "Duplicate entry" in str(e):
                 self.logger.error(e)
                 resp = 1
             else:
                 raise e
         return resp
 
     def add_many(
         self,
-        data: List,
+        data: list,
         *,
         table_name: str = "",
-        batch_size: int = 100,
+        batch=100,
         group_by_keys: bool = False,
-        ignore_duplicate: bool = True,
-        show_log=True,
-    ) -> int:
+        ignore_duplicate: bool = False,
+        autocommit: bool = False,
+        **kwargs,
+    ):
         """
-            save data list to database
-            !!! not atomicity
+        批量保存数据
         Args:
-            data:
-            table_name:
-            batch_size:
-            group_by_keys:
-                if set True, the data will be grouped by keys when is has different keys
-                else, raise an error
+            data: 数据
+            table_name: 表名
+            batch: 分批入库数量
+            group_by_keys: 是否按照keys分组处理 默认False 则如果遇到数据中存在key不一致的情况 会抛出异常
+            ignore_duplicate:
+            autocommit:
+            **kwargs:
+
+        Returns:
+
+        """
+        for sql in self.get_add_many_sql(
+            data,
+            table_name=table_name,
+            batch=batch,
+            group_by_keys=group_by_keys,
+            ignore_duplicate=ignore_duplicate,
+        ):
+            self.cursor.execute(sql)
+            if autocommit:
+                self.cursor.conn.commit()
+
+    def get_add_many_sql(
+        self,
+        data: list,
+        *,
+        table_name: str = "",
+        batch=100,
+        group_by_keys: bool = False,
+        ignore_duplicate: bool = False,
+        **kwargs,
+    ):
+        """
+        批量保存数据
+        Args:
+            data: 数据
+            table_name: 表名
+            batch: 分批入库数量
+            group_by_keys: 是否按照keys分组处理 默认False 则如果遇到数据中存在key不一致的情况 会抛出异常
             ignore_duplicate:
-            show_log:
+            **kwargs:
 
         Returns:
-            Number of affected rows
 
         """
         data = copy.deepcopy(data)
-        table_name = table_name or self.table_name
         if not table_name:
-            raise ValueError("table name must be not empty")
+            raise ValueError("table name {}".format(table_name))
         if not data:
-            raise ValueError("data must be not empty")
+            return []
         if not isinstance(data, (list, tuple)):
             data = [data]
 
+        # 数据分组 按照keys是否相同
+        # 防止由于key个数不一致导致的出错
         data_group_list = self.group_data_by_keys(data)
-        if not group_by_keys and len(data_group_list) != 1:
-            raise ValueError("data has different keys")
+        if not group_by_keys:
+            assert len(data_group_list) == 1, "待入库数据结构不一致"
+
+        sql_list = []
 
-        effect_count = 0
         for data in data_group_list:
-            # keys must has same order, otherwise, save data to database may be  in the confusion;
+            # 固定keys 取第一个数据
+            # 如果不固定 则当给定数据的key顺序不固定时会出现入库错乱
             first_data_keys = list(data[0].keys())
             while data:
-                _data = data[:batch_size]
-                data = data[batch_size:]
-                #
+                _data = data[:batch]
+                data = data[batch:]
+                # 每次100
                 if ignore_duplicate:
-                    sql = "insert ignore into {table_name} ({keys}) values{values};"
+                    sql = "insert into {table_name} ({keys}) values{values} on conflict do nothing;"
                 else:
                     sql = "insert into {table_name} ({keys}) values{values};"
-                # concat sql
+                # 拼接sql
                 values_list = []
                 for item in _data:
-                    order_data = self.escape_values(item, sort_keys=first_data_keys)
+                    order_data = self.handle_values(item, keys=first_data_keys)
                     keys = ",".join(order_data.keys())
                     values = ",".join(order_data.values())
                     values_list.append("({})".format(values))
 
                 sql = sql.format(
                     **{
                         "keys": keys,
                         "values": ",".join(values_list),
                         "table_name": table_name,
                     }
                 )
-                try:
-                    rows = self.cursor.execute(sql)
-                    effect_count += rows
-                    if show_log:
-                        self.logger.debug("insert rows {}".format(rows))
-                except Exception as e:
-                    if "Unknown column" in str(e) and show_log:
-                        self.logger.debug("error data: {}".format(_data[0]))
-                    raise e
-        return effect_count
+                sql_list.append(sql)
+        return sql_list
 
     def update(
         self,
         data,
         *,
-        condition: Dict = None,
+        condition: dict = None,
         table_name: str = "",
         where_sql: str = "",
+        **kwargs,
     ):
         """
-            update
         Args:
-            data:
-            condition:
-                same as sql syntax: where
-                but use dict and only support `and` with dict keys
-            table_name:
-            where_sql:
-                same as sql syntax: where
-                if set this field, the 'condition' field will be ignored.
+            data: 待更新字段 dict
+            condition: 条件字段 dict 默认无序直接and
+            table_name: 表名
+            where_sql: 若存在此字段则忽略 condition 适用于需要排序或者有除了and之外的where字句
+            **kwargs:
 
         Returns:
-            Number of affected rows
+
         """
         data = copy.deepcopy(data)
         table_name = table_name or self.table_name
         if not table_name:
-            raise ValueError("table name must be not empty")
+            raise ValueError("table name {}".format(table_name))
         if not condition:
             condition = {}
         sql = "update {table_name} set {update_data} where {where_sql};"
-        order_data = self.escape_values(data)
-        # set update data
+        order_data = self.handle_values(data)
+        # 组合待更新数据
         update_data = ["{}={}".format(k, v) for k, v in order_data.items()]
         update_data = ",".join(update_data)
 
-        # set where condition
-        order_condition = self.escape_values(condition, strip=False)
+        # 组合条件语句 默认使用and连接
+        order_condition = self.handle_values(condition, strip=False)
         order_condition = [f"{k}={v}" for k, v in order_condition.items()]
         order_condition = " and ".join(order_condition)
 
-        # first use where_sql
+        # where_sql 优先
         where_sql = where_sql or order_condition
 
         sql = sql.format(
             **{
                 "table_name": table_name,
                 "update_data": update_data,
                 "where_sql": where_sql,
             }
         )
-        return self.cursor.execute(sql)
+        ret = self.cursor.execute(sql)
+        if self.autocommit:
+            self.cursor.conn.commit()
+        return ret
 
-    def upsert(
+    def delete(
+        self,
+        *,
+        condition: dict = None,
+        table_name: str = "",
+        where_sql: str = "",
+        **kwargs,
+    ):
+        """
+        根据条件删除内容
+        Args:
+            condition: 条件字段 dict 默认无序直接and
+            table_name:
+            where_sql: 若存在此字段则忽略 condition 适用于需要排序或者有除了and之外的where字句
+            **kwargs:
+
+        Returns:
+            受影响行数
+        """
+
+        table_name = table_name or self.table_name
+        if not table_name:
+            raise ValueError("table name {}".format(table_name))
+        if not condition:
+            condition = {}
+        sql = "delete from  {table_name}  where {where_sql};"
+
+        # 组合条件语句 默认使用and连接
+        order_condition = self.handle_values(condition)
+        order_condition = ["{}={}".format(k, v) for k, v in order_condition.items()]
+        order_condition = " and ".join(order_condition)
+
+        # where_sql 优先
+        where_sql = where_sql or order_condition
+
+        sql = sql.format(**{"table_name": table_name, "where_sql": where_sql})
+        ret = self.cursor.execute(sql)
+        if self.autocommit:
+            self.cursor.conn.commit()
+        return ret
+
+    def get_upsert_sql(
         self,
         data: list,
         *,
         table_name: str = "",
+        conflict_target: str = "",
+        constraint_name: str = "",
+        conflict_columns: list = None,
         **kwargs,
     ):
         """
-            使用upsert语法入库
+        拼接upsert语法的sql
+            https://www.postgresql.org/docs/devel/sql-insert.html
         Args:
             data: 数据
+            conflict_target: 约束条件
+                例如:
+                    id
+                    "id"
+            constraint_name: 约束名称
+                例如:
+                    test_table_unique_index
+            conflict_columns: 唯一索引中包含的全部列名
+                例如:
+                    ["name", "id"]
             table_name: 表名
             **kwargs:
 
         Returns:
 
         """
         data = copy.deepcopy(data)
         if not table_name:
             raise ValueError("table name {}".format(table_name))
+        if not any([conflict_target, conflict_columns, constraint_name]):
+            raise ValueError("must be set one of conflict_columns or constraint_name")
         if not data:
             return []
         if not isinstance(data, (list, tuple)):
             data = [data]
 
-        r = 0
+        conflict_columns = conflict_columns or []
+
+        sql_list = []
+
+        if conflict_target:
+            conflict_expr = f"conflict({conflict_target})"
+        elif conflict_columns:
+            conflict_expr = 'conflict("{}")'.format('","'.join(conflict_columns))
+        elif constraint_name:
+            conflict_expr = f'conflict on constraint "{constraint_name}"'
+        else:
+            raise ValueError("must be set one of conflict_columns or constraint_name")
+
         for item in data:
+            # 固定keys 取第一个数据
             # 如果不固定 则当给定数据的key顺序不固定时会出现入库错乱
-            sql = "insert into {table_name} ({keys}) values({values}) on duplicate key update {update_data};"
+            sql = "insert into {table_name} ({keys}) values({values}) on {conflict_expr} do update set {update_data};"
             # 拼接sql
-            order_data = self.escape_values(item)
+            order_data = self.handle_values(item)
             keys = ",".join(order_data.keys())
             values = ",".join(order_data.values())
 
             sql = sql.format(
                 **{
                     "keys": keys,
                     "values": values,
                     "table_name": table_name,
                     "update_data": ",".join(
                         [f"{k} = {v}" for k, v in order_data.items()]
                     ),
+                    "conflict_expr": conflict_expr,
                 }
             )
-            r += self.cursor.execute(sql)
-        return r
+            sql_list.append(sql)
+        return sql_list
 
-    def delete(
-        self,
-        *,
-        condition: Dict = None,
-        table_name: str = "",
-        where_sql: str = "",
-    ):
+    def upsert(self, data: list, *, table_name: str = "", **kwargs):
         """
-            delete
+        upsert
         Args:
-            condition:
-                same as sql syntax: where
-                but use dict and only support `and` with dict keys
-            table_name:
-            where_sql:
-                same as sql syntax: where
-                if set this field, the 'condition' field will be ignored.
-            **kwargs:
+            data: 数据
+            table_name: 表名
+            **kwargs: 参考 get_upsert_sql 字段
 
         Returns:
-            Number of affected rows
-        """
-
-        table_name = table_name or self.table_name
-        if not table_name:
-            raise ValueError("table name {}".format(table_name))
-        if not condition:
-            condition = {}
-        sql = "delete from {table_name} where {where_sql};"
 
-        # set where condition
-        order_condition = self.escape_values(condition)
-        order_condition = ["{}={}".format(k, v) for k, v in order_condition.items()]
-        order_condition = " and ".join(order_condition)
+        """
+        r = 0
+        for sql in self.get_upsert_sql(data, table_name=table_name, **kwargs):
+            r += self.cursor.execute(sql)
+            if self.autocommit:
+                self.cursor.conn.commit()
+        return r
 
-        # first use where_sql
-        where_sql = where_sql or order_condition
+    def get_table_field_list(self, table_name):
+        """
+        获取表字段
 
-        sql = sql.format(**{"table_name": table_name, "where_sql": where_sql})
-        return self.cursor.execute(sql)
+        :param table_name: 表名
+        :return: 字段列表
+        """
+        _sql = f"SELECT * FROM {table_name} LIMIT 0"
+        _cursor = self.get_cursor(connection=self.conn)
+        _cursor.execute(_sql)
+        # 获取表头字段
+        column_names = [column[0] for column in _cursor.description]
+        _cursor.close()
+        # 打印表头字段
+        return column_names
 
-    def query_all(self, sql, *, args=None) -> List[Tuple]:
+    def query_one(self, sql, *, args=None):
         """
-            cursor.execute + fetchall
+            cursor.execute + fetchone
         Args:
             sql:
             args:
 
         Returns:
 
         """
-        # create new cursor object to prevent multi query in same time
-        _cursor = self.get_cursor(connection=self.connection)
+        # 重新获取cursor是为了防止同一个cursor在多个线程下使用导致数据混乱
+        _cursor = self.get_cursor(connection=self.conn)
         _cursor.execute(sql, args=args)
-        result = _cursor.fetchall()
+        result = _cursor.fetchone()
         _cursor.close()
         return result
 
-    def query_single_field(self, sql, *, args=None) -> List:
+    def query_all(self, sql, *, args=None, autocommit=False):
         """
-            Collect first field in each row.
-
+            cursor.execute + fetchall
         Args:
             sql:
             args:
+            autocommit:
 
         Returns:
 
         """
+
+        self.cursor.execute(sql, args=args)
+        result = self.cursor.fetchall()
+        if autocommit:
+            # 如果不commit的话，由于事务的隔离等级问题，会导致读到的数据是经过缓存无变化的
+            self.cursor.conn.commit()
+        return result
+
+    def query_single_attr(self, sql, *, args=None):
+        """
+        查询单个字段使用
+        Args:
+            sql: 查询sql
+            args: list [1,2,3,4,5]
+
+        Returns:
+
+        """
+        # 假如用了 dict_cursor 会挂掉的
         return [item[0] for item in self.query_all(sql, args=args)]
 
     def close(self):
+        """
+        关闭数据库连接
+        Returns:
+
+        """
         try:
             if self._cursor:
                 self._cursor.close()
         except:
             pass
         try:
-            if self._connection:
-                self._connection.close()
-            self.logger.debug("Successfully closed mysql connection")
+            if self._conn:
+                self._conn.close()
+            self.logger.debug("pg连接关闭成功")
         except:
             pass
         # 删除链接池中的链接
         self._cursor = None
-        self._connection = None
-        MySQLOpt.connection_list.pop(self.key, None)
+        self._conn = None
+        PostgreSQLOpt.connection_list.pop(self.key, "")
 
     def copy(self, *, protocol="", **kwargs):
         """
-            Copy self and modify some properties
+        复制一个新连接 可以修改有限的一些参数
+
         Args:
-            protocol:
+            protocol: mysql连接协议  mysql+pymysql   mysql+mysqldb
             **kwargs:
 
         Returns:
 
         """
         _kwargs = copy.deepcopy(self.kwargs)
         _kwargs.update(kwargs)
-        _kwargs.update({"reuse_connection": False})
-        #
-        options = self.options.copy()
-        if protocol:
-            assert protocol in ["mysql+pymysql", "mysql+mysqldb"]
-            options["type"] = protocol
-        #
-        db_opt = MySQLOpt(options, **_kwargs)
+        _kwargs.update({"is_pool": False})
+        db_opt = PostgreSQLOpt(self.options, **_kwargs)
         return db_opt
-
-    def create(
-        self,
-        fields: Dict[str, str] = None,
-        unique: List[str] = None,
-        table_name: str = "",
-        type="",
-        exists_ok=True,
-        sql="",
-        **kwargs,
-    ):
-        """
-            create table
-        Args:
-            table_name:
-            sql: DDL
-            **kwargs:
-
-        Returns:
-
-        """
-
-        assert type in ["", "task", "batch_record", "batch_value"]
-
-        # default fields
-        default_fields = [
-            "id",
-            "created_time",
-            "state",
-            "batch_date",
-        ]
-
-        # use translate
-        sql_list = [
-            "begin",
-        ]
-
-        if sql:
-            sql_list.append(sql)
-        else:
-            if not fields:
-                self.logger.warning("no fields")
-                return 0
-            fields_keys = [x.lower() for x in fields]
-
-            if "id" not in fields_keys:
-                fields["id"] = "bigint NOT NULL AUTO_INCREMENT"
-            if "created_time" not in fields_keys:
-                fields[
-                    "created_time"
-                ] = "datetime(0) NOT NULL  DEFAULT CURRENT_TIMESTAMP(0)"
-
-            if type == "task":
-                if "state" not in fields_keys:
-                    fields["state"] = "int DEFAULT 0"
-            elif type == "batch_value":
-                if "batch_date" not in fields_keys:
-                    fields["batch_date"] = "datetime(0) NULL"
-
-            # fields sorted
-            fields = fields.items()
-            fields = (
-                [x for x in fields if x[0].lower() == "id"]
-                + [x for x in fields if x[0].lower() not in default_fields]
-                + [
-                    x
-                    for x in fields
-                    if x[0].lower() in default_fields and x[0].lower() != "id"
-                ]
-            )
-
-            sql = """
-CREATE TABLE {}(
-    {},
-    PRIMARY KEY (`id`)
-) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
-            """.format(
-                "IF NOT EXISTS {}".format(table_name) if exists_ok else table_name,
-                ",\n    ".join("{} {}".format(k, v) for k, v in fields),
-            )
-            sql_list.append(sql)
-
-            if unique:
-                unique = [x.strip("`") for x in unique]
-                sql = "ALTER TABLE {} ADD UNIQUE INDEX `{}_unique`(`{}`);".format(
-                    table_name, table_name, "`,`".join(unique)
-                )
-                sql_list.append(sql)
-
-        #
-        cursor = self.get_cursor()
-        for sql in sql_list:
-            self.logger.info(sql)
-            cursor.execute(sql)
-        cursor.connection.commit()
-        return 0
```

### Comparing `openget-0.2.0/openget/db/db_oracle.py` & `openget-0.3.0/openget/db/db_oracle.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/db/db_oss.py` & `openget-0.3.0/openget/db/db_oss.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import datetime
 import tempfile
 from typing import Dict
 
 import redis
 
 from openget import util
-from openget.utils import log
+from openget.utils import log, s3
 
 #
 redis_pool_cache = {}
 
 
 class RedisCacheList(object):
     def __init__(
@@ -234,15 +234,15 @@
         """
         获取唯一id 增加时间戳方便查看
         :return:
         """
         return "{}_{}".format(str(time.time()), str(uuid.uuid1()))
 
     def split(self, key):
-        """"切分"""
+        """ "切分"""
         data_length_limit = int(self._cache_limit * 1.2)
         # 获取一条数据
         _data = self.redis_client.lindex(key, 0)
         if _data is not None:
             _data_size = sys.getsizeof(_data)
             _data_length_limit = int(self._cache_size_limit // _data_size)
             # 根据数据大小算出来一个长度上限  使用最小的
@@ -476,22 +476,22 @@
         self.service_line = (
             self.setting_dict["params"].get("service_line", [""])[0].strip()
         )
         self.module = self.setting_dict["params"].get("module", [""])[0].strip()
         if not self.service_line or not self.module:
             raise ValueError("no service_line or module")
 
-        self.file_handler = util.OSSHandler(
+        self.file_handler = s3.OSSHandler(
             AccessKeyId=self.AccessKeyId,
             AccessKeySecret=self.AccessKeySecret,
             endpoint=self.endpoint,
             bucket_name=self.bucket_name,
         )
         if html_cache_bucket:
-            self.html_file_handler = util.OSSHandler(
+            self.html_file_handler = s3.OSSHandler(
                 AccessKeyId=self.AccessKeyId,
                 AccessKeySecret=self.AccessKeySecret,
                 endpoint=self.endpoint,
                 bucket_name=html_cache_bucket,
             )
         else:
             self.html_file_handler = None
```

### Comparing `openget-0.2.0/openget/db/db_redis.py` & `openget-0.3.0/openget/db/db_redis.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/db/db_sqlite.py` & `openget-0.3.0/openget/db/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/db/util.py` & `openget-0.3.0/openget/db/util.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/env.py` & `openget-0.3.0/openget/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "OPENGET_REDIS_URI": "redis://localhost:6379/0",
     # default proxy service url
     "OPENGET_PROXY_SERVICE_URL": None,
     # docker mode
     "OPENGET_IN_DOCKER": "false",
     # logging
     # forbidden better_exceptions
-    "OPENGET_FORBIDDED_BETTER_EXCEPTIONS": None,
+    "OPENGET_FORBIDDED_BETTER_EXCEPTIONS": "false",
 }
 
 
 # from ~/.openget/.env
 GLOBAL_ENV_FILE = path.join(path.expanduser("~"), ".openget/.env")
 if GLOBAL_ENV_FILE:
     load_dotenv(GLOBAL_ENV_FILE)
```

### Comparing `openget-0.2.0/openget/network/downloader.py` & `openget-0.3.0/openget/network/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,17 +490,19 @@
 
         Returns:
 
         """
         # compatible allow_redirects
         if "allow_redirects" in kwargs:
             kwargs["follow_redirects"] = kwargs.pop("allow_redirects")
+        # 默认True 为了跟 requests 的行为一致
+        kwargs.setdefault("follow_redirects", True)
         #
         stream = kwargs.pop("stream")
-        proxies: Dict = kwargs.pop("proxies", None)
+        proxies: Union[Dict, None] = kwargs.pop("proxies", None)
         verify = kwargs.pop("verify")
         cert = kwargs.pop("cert", None)
         cookies = kwargs.pop("cookies", None)
         if proxies or verify is not None or cert is not None or cookies is not None:
             if proxies is not None:
                 proxies = {
                     k if "://" in k else f"{k}://": v for k, v in proxies.items()
@@ -530,15 +532,15 @@
                         "timeout",
                     ]
                 },
             )
             response = session.send(
                 request=request,
                 auth=kwargs.get("auth"),
-                follow_redirects=kwargs.get("follow_redirects"),
+                follow_redirects=kwargs["follow_redirects"],
                 stream=True,
             )
         return response
 
     @util.retry_decorator(Exception)
     def _download(self, request, **kwargs) -> httpx.Response:
         """
```

### Comparing `openget-0.2.0/openget/network/proxy.py` & `openget-0.3.0/openget/network/proxy.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/network/request.py` & `openget-0.3.0/openget/network/request.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/network/response.py` & `openget-0.3.0/openget/network/response.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/setting.py` & `openget-0.3.0/openget/setting.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/spiders/__init__.py` & `openget-0.3.0/openget/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget/spiders/base.py` & `openget-0.3.0/openget/spiders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,15 @@
                         spider_break = 1
                         self.suicide()
                         break
             else:
                 logger.debug("break spider")
         except Exception as e:
             raise_exception = e
+        # TODO 支持设置等待线程结束的最大时间 超时则KILL不再等待
         while 1:
             qsize = self.request_queue.qsize()
             if qsize <= 0:
                 # when all thread is stopped, stop self
                 if sum(self._thread_status.values()) == 0:
                     self.event_exit.set()
                     break
```

### Comparing `openget-0.2.0/openget/spiders/batch_spider.py` & `openget-0.3.0/openget/spiders/batch_spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 
             #
             task_mysql_limit -= self.task_mysql_limit_step
 
             _cache_group_task_list = []
             task_list = []
             for _, *field in sql_result:
-                # 强转datetime
+                # TODO 为啥强转datetime
                 _task = {
                     _k: "'{}'".format(_v) if isinstance(_v, datetime.date) else _v
                     for _k, _v in zip(self.task_field_list, field)
                 }
                 if self.task_group_limit > 1:
                     _cache_group_task_list.append(_task)
                     if len(_cache_group_task_list) >= self.task_group_limit:
```

### Comparing `openget-0.2.0/openget/utils/log.py` & `openget-0.3.0/openget/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     #
     def _format_exception(exc_info):
         exc_str = format_exception(*exc_info)
         return "\n".join(exc_str) if not isinstance(exc_str, str) else exc_str
 
     #
     formatter = logging.Formatter(log_format)
-    if os.getenv("OPENGET_FORBIDDED_BETTER_EXCEPTIONS", None) is None:
+    if os.getenv("OPENGET_FORBIDDED_BETTER_EXCEPTIONS", "false").lower() != "true":
         formatter.formatException = _format_exception
 
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(formatter)
     # check duplicate
     handle_exists = 0
     for _handler in _logger.handlers:
```

### Comparing `openget-0.2.0/openget/utils/message/dingtalk.py` & `openget-0.3.0/openget/utils/message/dingtalk.py`

 * *Files identical despite different names*

### Comparing `openget-0.2.0/openget.egg-info/PKG-INFO` & `openget-0.3.0/openget.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
@@ -18,25 +18,36 @@
 # openget
 A Spider FrameWork.
 
 ## Installation
 You can install openget by simply doing:
 
     pip install openget
+    pip install git+https://github.com/dytttf/openget.git@main
+    pip install git+https://github.com/dytttf/openget.git@dev
+
     
 ## Usage
 **Very Important Thing**
 This line must be the first line in code
 ```
 from openget.spiders import *
 ```
+### 命令行支持
+1. 生成配置文件样例
+```shell
+# 环境变量类型的配置文件
+python -m openget --gen_env_example
+```
 
 
 ## About Environment Variable
-> ~/.openget/.env < $(pwd)/.env
+### 优先级
+1. $(pwd)/.env
+2. ~/.openget/.env
 
 
 ## docker build
 ```shell
 cd docekr
 bash build.sh
 ```
@@ -44,7 +55,11 @@
 ## TODO
 - ftp download
 - auto add task
 - statis crawl speed
 - browser support: zhipin.com tmall.com
 - sqlite.db rename
 - use cmd to create spider template
+- 金融许可证 卡死问题处理
+- 环境变量定义优化
+- 新项目创建优化
+- 极简模式、完整模式 减少包的依赖
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openget-0.2.0/openget.egg-info/SOURCES.txt` & `openget-0.3.0/openget.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 openget/__init__.py
+openget/__main__.py
 openget/env.py
 openget/setting.py
 openget/util.py
 openget.egg-info/PKG-INFO
 openget.egg-info/SOURCES.txt
 openget.egg-info/dependency_links.txt
 openget.egg-info/requires.txt
 openget.egg-info/top_level.txt
 openget/db/__init__.py
 openget/db/db.py
 openget/db/db_mysql.py
 openget/db/db_oracle.py
 openget/db/db_oss.py
+openget/db/db_postgresql.py
 openget/db/db_redis.py
 openget/db/db_sqlite.py
 openget/db/util.py
 openget/network/__init__.py
 openget/network/downloader.py
 openget/network/proxy.py
 openget/network/request.py
 openget/network/response.py
 openget/spiders/__init__.py
 openget/spiders/base.py
 openget/spiders/batch_spider.py
 openget/utils/__init__.py
 openget/utils/log.py
+openget/utils/s3.py
 openget/utils/message/__init__.py
 openget/utils/message/dingtalk.py
```

### Comparing `openget-0.2.0/pyproject.toml` & `openget-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "openget"
-version = "0.1.0"
+version = "0.2.1"
 description = "A Spider FrameWork"
 authors = ["dytttf <dytttf@foxmail.com>"]
 license = "BSD"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-urllib3 = "^1.26.7"
-gevent = "^21.8.0"
-pymysql = "^1.0.2"
-redis = "^3.5.3"
+urllib3 = "^2.1.0"
+gevent = "^23.9.1"
+pymysql = "^1.1.0"
+redis = "^5.0.0"
 better-exceptions = "^0.3.3"
 tqdm = "^4.62.3"
 #mysqlclient = "^2.0.3"
-httpx = {extras = ["http2"], version = "^0.20.0"}
+httpx = {extras = ["http2"], version = "^0.25.2"}
 user-agent2 = "^2021.11.1"
 crontab = "^0.23.0"
 oss2 = "^2.15.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.0"
 cx-oracle = "^8.3.0"
```

### Comparing `openget-0.2.0/setup.py` & `openget-0.3.0/setup.py`

 * *Files identical despite different names*

