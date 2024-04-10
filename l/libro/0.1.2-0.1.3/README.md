# Comparing `tmp/libro-0.1.2.tar.gz` & `tmp/libro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libro-0.1.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `libro-0.1.2.tar` & `libro-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,534 @@
--rw-r--r--   0        0        0      556 2024-01-24 11:00:49.902070 libro-0.1.2/README.md
--rw-r--r--   0        0        0        6 2024-04-03 06:18:16.905512 libro-0.1.2/libro_server/.gitignore
--rw-r--r--   0        0        0      348 2024-04-03 06:20:34.869920 libro-0.1.2/libro_server/__init__.py
--rw-r--r--   0        0        0       46 2024-04-03 06:20:44.616869 libro-0.1.2/libro_server/_version.py
--rw-r--r--   0        0        0     2927 2024-04-03 06:18:16.906606 libro-0.1.2/libro_server/app.py
--rw-r--r--   0        0        0     1933 2024-04-03 06:18:16.910291 libro-0.1.2/libro_server/handler.py
--rw-r--r--   0        0        0        0 2024-04-03 06:18:16.910853 libro-0.1.2/libro_server/static/.gitkeep
--rw-r--r--   0        0        0     4817 2024-04-03 06:25:37.869451 libro-0.1.2/libro_server/static/1330.async.js
--rw-r--r--   0        0        0     6234 2024-04-03 06:25:37.870047 libro-0.1.2/libro_server/static/1438.async.js
--rw-r--r--   0        0        0     4800 2024-04-03 06:25:37.870780 libro-0.1.2/libro_server/static/161.async.js
--rw-r--r--   0        0        0     6175 2024-04-03 06:25:37.871284 libro-0.1.2/libro_server/static/1639.async.js
--rw-r--r--   0        0        0     5813 2024-04-03 06:25:37.871633 libro-0.1.2/libro_server/static/1772.async.js
--rw-r--r--   0        0        0     5091 2024-04-03 06:25:37.872295 libro-0.1.2/libro_server/static/1838.async.js
--rw-r--r--   0        0        0     6197 2024-04-03 06:25:37.872471 libro-0.1.2/libro_server/static/2048.async.js
--rw-r--r--   0        0        0     5473 2024-04-03 06:25:37.872754 libro-0.1.2/libro_server/static/2118.async.js
--rw-r--r--   0        0        0     6218 2024-04-03 06:25:37.872983 libro-0.1.2/libro_server/static/2130.async.js
--rw-r--r--   0        0        0     6224 2024-04-03 06:25:37.873126 libro-0.1.2/libro_server/static/2999.async.js
--rw-r--r--   0        0        0     4818 2024-04-03 06:25:37.873245 libro-0.1.2/libro_server/static/3572.async.js
--rw-r--r--   0        0        0     6232 2024-04-03 06:25:37.873363 libro-0.1.2/libro_server/static/405.async.js
--rw-r--r--   0        0        0      213 2024-04-03 06:25:37.873510 libro-0.1.2/libro_server/static/4113.async.js
--rw-r--r--   0        0        0     6242 2024-04-03 06:25:37.873714 libro-0.1.2/libro_server/static/4116.async.js
--rw-r--r--   0        0        0     6177 2024-04-03 06:25:37.873844 libro-0.1.2/libro_server/static/4123.async.js
--rw-r--r--   0        0        0     6231 2024-04-03 06:25:37.873967 libro-0.1.2/libro_server/static/417.async.js
--rw-r--r--   0        0        0     5190 2024-04-03 06:25:37.874179 libro-0.1.2/libro_server/static/4266.async.js
--rw-r--r--   0        0        0     6230 2024-04-03 06:25:37.874440 libro-0.1.2/libro_server/static/4343.async.js
--rw-r--r--   0        0        0     5114 2024-04-03 06:25:37.874578 libro-0.1.2/libro_server/static/4541.async.js
--rw-r--r--   0        0        0     5419 2024-04-03 06:25:37.874718 libro-0.1.2/libro_server/static/4621.async.js
--rw-r--r--   0        0        0     5741 2024-04-03 06:25:37.874985 libro-0.1.2/libro_server/static/4658.async.js
--rw-r--r--   0        0        0     6090 2024-04-03 06:25:37.875123 libro-0.1.2/libro_server/static/4849.async.js
--rw-r--r--   0        0        0     6238 2024-04-03 06:25:37.875300 libro-0.1.2/libro_server/static/4887.async.js
--rw-r--r--   0        0        0     5066 2024-04-03 06:25:37.875421 libro-0.1.2/libro_server/static/5250.async.js
--rw-r--r--   0        0        0  9350375 2024-04-03 06:25:37.884122 libro-0.1.2/libro_server/static/5332.async.js
--rw-r--r--   0        0        0     6174 2024-04-03 06:25:37.888836 libro-0.1.2/libro_server/static/610.async.js
--rw-r--r--   0        0        0     5310 2024-04-03 06:25:37.888955 libro-0.1.2/libro_server/static/628.async.js
--rw-r--r--   0        0        0     5113 2024-04-03 06:25:37.889086 libro-0.1.2/libro_server/static/6357.async.js
--rw-r--r--   0        0        0     5001 2024-04-03 06:25:37.889206 libro-0.1.2/libro_server/static/6404.async.js
--rw-r--r--   0        0        0     6235 2024-04-03 06:25:37.889341 libro-0.1.2/libro_server/static/6486.async.js
--rw-r--r--   0        0        0     7189 2024-04-03 06:25:37.889472 libro-0.1.2/libro_server/static/6730.async.js
--rw-r--r--   0        0        0     5089 2024-04-03 06:25:37.889604 libro-0.1.2/libro_server/static/6962.async.js
--rw-r--r--   0        0        0     5811 2024-04-03 06:25:37.889729 libro-0.1.2/libro_server/static/6999.async.js
--rw-r--r--   0        0        0     3130 2024-04-03 06:25:37.889836 libro-0.1.2/libro_server/static/7162.async.js
--rw-r--r--   0        0        0     5118 2024-04-03 06:25:37.889950 libro-0.1.2/libro_server/static/7715.async.js
--rw-r--r--   0        0        0     6232 2024-04-03 06:25:37.890063 libro-0.1.2/libro_server/static/7851.async.js
--rw-r--r--   0        0        0     5162 2024-04-03 06:25:37.890173 libro-0.1.2/libro_server/static/79.async.js
--rw-r--r--   0        0        0     6237 2024-04-03 06:25:37.890287 libro-0.1.2/libro_server/static/8227.async.js
--rw-r--r--   0        0        0     6233 2024-04-03 06:25:37.890401 libro-0.1.2/libro_server/static/8305.async.js
--rw-r--r--   0        0        0     5172 2024-04-03 06:25:37.890520 libro-0.1.2/libro_server/static/8370.async.js
--rw-r--r--   0        0        0     6175 2024-04-03 06:25:37.890661 libro-0.1.2/libro_server/static/8525.async.js
--rw-r--r--   0        0        0    74158 2024-04-03 06:25:37.890816 libro-0.1.2/libro_server/static/8945.chunk.css
--rw-r--r--   0        0        0     5082 2024-04-03 06:25:37.890962 libro-0.1.2/libro_server/static/9095.async.js
--rw-r--r--   0        0        0     6238 2024-04-03 06:25:37.891102 libro-0.1.2/libro_server/static/9150.async.js
--rw-r--r--   0        0        0     5392 2024-04-03 06:25:37.891232 libro-0.1.2/libro_server/static/9402.async.js
--rw-r--r--   0        0        0     6222 2024-04-03 06:25:37.891354 libro-0.1.2/libro_server/static/9669.async.js
--rw-r--r--   0        0        0     4995 2024-04-03 06:25:37.891471 libro-0.1.2/libro_server/static/9674.async.js
--rw-r--r--   0        0        0 28118062 2024-04-03 06:25:37.918458 libro-0.1.2/libro_server/static/9709.async.js
--rw-r--r--   0        0        0   255768 2024-04-03 06:25:37.919473 libro-0.1.2/libro_server/static/9709.chunk.css
--rw-r--r--   0        0        0     6233 2024-04-03 06:25:37.919621 libro-0.1.2/libro_server/static/9749.async.js
--rw-r--r--   0        0        0     5189 2024-04-03 06:25:37.919737 libro-0.1.2/libro_server/static/9905.async.js
--rw-r--r--   0        0        0     1427 2024-04-03 06:25:37.919857 libro-0.1.2/libro_server/static/index.html
--rw-r--r--   0        0        0     8432 2024-04-03 06:25:37.920009 libro-0.1.2/libro_server/static/p__libro__index.async.js
--rw-r--r--   0        0        0      105 2024-04-03 06:25:37.921425 libro-0.1.2/libro_server/static/p__libro__index.chunk.css
--rw-r--r--   0        0        0    73464 2024-04-03 06:25:38.000456 libro-0.1.2/libro_server/static/static/codicon.589e0820.ttf
--rw-r--r--   0        0        0    49764 2024-04-03 06:25:38.001172 libro-0.1.2/libro_server/static/static/devopicons.3c46801a.woff2
--rw-r--r--   0        0        0    90680 2024-04-03 06:25:38.001953 libro-0.1.2/libro_server/static/static/file-icons.2cbb51ef.woff2
--rw-r--r--   0        0        0   165742 2024-04-03 06:25:38.002323 libro-0.1.2/libro_server/static/static/fontawesome-webfont.2b13baa7.eot
--rw-r--r--   0        0        0   165548 2024-04-03 06:25:38.002933 libro-0.1.2/libro_server/static/static/fontawesome-webfont.8a7cb27d.ttf
--rw-r--r--   0        0        0    98024 2024-04-03 06:25:38.003194 libro-0.1.2/libro_server/static/static/fontawesome-webfont.cf011583.woff
--rw-r--r--   0        0        0    77160 2024-04-03 06:25:38.003418 libro-0.1.2/libro_server/static/static/fontawesome-webfont.e9955780.woff2
--rw-r--r--   0        0        0   387787 2024-04-03 06:25:38.003996 libro-0.1.2/libro_server/static/static/fontawesome-webfont.f05dad85.svg
--rw-r--r--   0        0        0    77160 2024-04-03 06:25:38.004227 libro-0.1.2/libro_server/static/static/fontawesome.e9955780.woff2
--rw-r--r--   0        0        0    24412 2024-04-03 06:25:38.004378 libro-0.1.2/libro_server/static/static/mfixx.8e0807ce.woff2
--rw-r--r--   0        0        0    20248 2024-04-03 06:25:38.004542 libro-0.1.2/libro_server/static/static/octicons.c982f59d.woff2
--rw-r--r--   0        0        0   466610 2024-04-03 06:25:38.005022 libro-0.1.2/libro_server/static/static/onig.25dd2e6f.wasm
--rw-r--r--   0        0        0      741 2024-04-03 06:25:38.005176 libro-0.1.2/libro_server/static/static/plotly.eb7b9072.svg
--rw-r--r--   0        0        0   847831 2024-04-03 06:25:37.922235 libro-0.1.2/libro_server/static/umi.js
--rw-r--r--   0        0        0      457 2024-04-03 06:18:16.910976 libro-0.1.2/libro_server/templates/error.html
--rw-r--r--   0        0        0     1050 2024-04-03 06:18:16.911049 libro-0.1.2/libro_server/templates/libro.html
--rw-r--r--   0        0        0      591 2024-04-03 06:18:16.911305 libro-0.1.2/libro_server/templates/page.html
--rw-r--r--   0        0        0     1115 2024-04-03 06:23:02.581456 libro-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       33 2024-01-11 03:02:15.930969 libro-0.1.2/setup.py
--rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 libro-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 libro-0.1.3/.npmrc
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro-0.1.3/.python-version
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 libro-0.1.3/package.json
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.package-lock.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.bin/installServerIntoExtension -> ../vscode-languageserver/bin/installServerIntoExtension
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/.bin/libro-analyzer -> ../@difizen/libro-analyzer/index.js
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/LICENSE.txt
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/README.md
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/index.js
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@difizen/libro-analyzer/package.json
+-rwxr-xr-x   0        0        0    10640 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/CHANGELOG.md
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/LICENSE
+-rwxr-xr-x   0        0        0    18226 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/README.md
+-rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/index.d.ts
+-rwxr-xr-x   0        0        0     2710 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/package.json
+-rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-async.js
+-rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-pretty-error.js
+-rwxr-xr-x   0        0        0     1625 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-stream.js
+-rwxr-xr-x   0        0        0      415 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse-string.js
+-rwxr-xr-x   0        0        0      227 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/parse.js
+-rwxr-xr-x   0        0        0     8292 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/stringify.js
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/toml.js
+-rwxr-xr-x   0        0        0      485 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-date.js
+-rwxr-xr-x   0        0        0      663 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-datetime-float.js
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-datetime.js
+-rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/create-time.js
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/format-num.js
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/parser-debug.js
+-rwxr-xr-x   0        0        0     2975 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/parser.js
+-rwxr-xr-x   0        0        0    45566 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@iarna/toml/lib/toml-parser.js
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/LICENSE
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/README.md
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/index.d.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@types/emscripten/package.json
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.d.ts
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/AliasFS.js
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.d.ts
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/CwdFS.js
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.d.ts
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/FakeFS.js
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.d.ts
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/JailFS.js
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.d.ts
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/LazyFS.js
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.d.ts
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NoFS.js
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.d.ts
+-rw-r--r--   0        0        0    17379 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodeFS.js
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.d.ts
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/NodePathFS.js
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/PosixFS.d.ts
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/PosixFS.js
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.d.ts
+-rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ProxiedFS.js
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.d.ts
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/VirtualFS.js
+-rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.d.ts
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipFS.js
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.d.ts
+-rw-r--r--   0        0        0    36407 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/ZipOpenFS.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/constants.d.ts
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/constants.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.d.ts
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/errors.js
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.d.ts
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/index.js
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.d.ts
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/path.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.d.ts
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/statUtils.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.d.ts
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/xfs.js
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.d.ts
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/copyPromise.js
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.d.ts
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/opendir.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.d.ts
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile.js
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.d.ts
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/algorithms/watchFile/CustomStatWatcher.js
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.d.ts
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/FileHandle.js
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.d.ts
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/fslib/lib/patchFs/patchFs.js
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/package.json
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.d.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/async.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/emscripten.d.ts
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipAsync.d.ts
+-rw-r--r--   0        0        0   372811 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipAsync.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipSync.d.ts
+-rw-r--r--   0        0        0   364127 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/libzipSync.js
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.d.ts
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/makeInterface.js
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.d.ts
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/@yarnpkg/libzip/lib/sync.js
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/index.d.ts
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/license
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/ansi-styles/readme.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/LICENSE
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/index.d.ts
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/index.js
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/LICENSE
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/README.hbs
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/README.md
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/index.mjs
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/array-back/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/binary-extensions.json.d.ts
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/index.d.ts
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/index.js
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/license
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/binary-extensions/readme.md
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/LICENSE
+-rw-r--r--   0        0        0    21130 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/README.md
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/index.js
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/compile.js
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/constants.js
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/expand.js
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/parse.js
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/stringify.js
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/braces/lib/utils.js
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/LICENSE
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/index.js
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/buffer-from/readme.md
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/index.d.ts
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/license
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/package.json
+-rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/readme.md
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/index.js
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/templates.js
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chalk/source/util.js
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/LICENSE
+-rw-r--r--   0        0        0    14392 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/README.md
+-rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/index.js
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/constants.js
+-rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/fsevents-handler.js
+-rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/lib/nodefs-handler.js
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/chokidar/types/index.d.ts
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/CHANGELOG.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/LICENSE
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/README.md
+-rw-r--r--   0        0        0    17040 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/conversions.js
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/index.js
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-convert/route.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/README.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/index.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/color-name/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/LICENSE
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/README.md
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/index.mjs
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/package.json
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/argv-parser.mjs
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/argv-tools.mjs
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-definition.mjs
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-definitions.mjs
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option-flag.mjs
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/option.mjs
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/output-grouped.mjs
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/command-line-args/lib/output.mjs
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/LICENSE
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/README.md
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/index.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/LICENSE
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/README.hbs
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/README.md
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/index.mjs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/find-replace/package.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/LICENSE
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/README.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.d.ts
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.js
+-rwxr-xr-x   0        0        0   163626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/fsevents.node
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/fsevents/package.json
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/CHANGELOG.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/LICENSE
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/index.js
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/index.d.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/license
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/has-flag/readme.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/index.d.ts
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/index.js
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/license
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-binary-path/readme.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/LICENSE
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/index.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/LICENSE
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/README.md
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/index.js
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/LICENSE
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/README.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/index.js
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/LICENSE.md
+-rw-r--r--   0        0        0    14129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/README.md
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/SECURITY.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/package.json
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.d.ts
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/main.js
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/edit.js
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/format.js
+-rw-r--r--   0        0        0    24708 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/parser.js
+-rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/scanner.js
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/esm/impl/string-intern.js
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/main.js
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/edit.js
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/format.js
+-rw-r--r--   0        0        0    28290 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/parser.js
+-rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/scanner.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/jsonc-parser/lib/umd/impl/string-intern.js
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/index.d.ts
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/license
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/leven/readme.md
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/LICENSE
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/README.md
+-rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/index.js
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/lodash.camelcase/package.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/LICENSE
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/README.md
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/index.js
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/CHANGELOG.md
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/LICENSE
+-rw-r--r--   0        0        0    27445 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/README.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/index.js
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/constants.js
+-rw-r--r--   0        0        0    27763 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/parse.js
+-rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/picomatch.js
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/scan.js
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/picomatch/lib/utils.js
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/LICENSE
+-rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/README.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/index.d.ts
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/index.js
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/CHANGELOG.md
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/LICENSE
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/README.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/source-map.d.ts
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/source-map.js
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/array-set.js
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/base64-vlq.js
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/base64.js
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/binary-search.js
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/mapping-list.js
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/quick-sort.js
+-rw-r--r--   0        0        0    40562 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-map-consumer.js
+-rw-r--r--   0        0        0    14356 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-map-generator.js
+-rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/source-node.js
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map/lib/util.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/LICENSE.md
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/README.md
+-rw-r--r--   0        0        0    53583 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/browser-source-map-support.js
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/register-hook-require.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/register.js
+-rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/source-map-support/source-map-support.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/browser.js
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/index.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/license
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/supports-color/readme.md
+-rw-r--r--   0        0        0    16509 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/LICENSE
+-rw-r--r--   0        0        0    12531 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/README.md
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/package.json
+-rw-r--r--   0        0        0    22676 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tmp/lib/tmp.js
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/LICENSE
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/README.md
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/index.js
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/CopyrightNotice.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/LICENSE.txt
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/README.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/package.json
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.d.ts
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.es6.html
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.es6.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.html
+-rw-r--r--   0        0        0    13204 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/tslib.js
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/modules/index.js
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/LICENSE
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/README.hbs
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/README.md
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/index.mjs
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/typical/package.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/License.txt
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/browser.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/node.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/thirdpartynotices.txt
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/main.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/ril.d.ts
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/browser/ril.js
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.d.ts
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/api.js
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.d.ts
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/cancellation.js
+-rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.d.ts
+-rw-r--r--   0        0        0    51184 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/connection.js
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/disposable.d.ts
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/disposable.js
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.d.ts
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/encoding.js
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.d.ts
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/events.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/is.d.ts
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/is.js
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.d.ts
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/linkedMap.js
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.d.ts
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageBuffer.js
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.d.ts
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageReader.js
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.d.ts
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messageWriter.js
+-rw-r--r--   0        0        0    12626 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.d.ts
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/messages.js
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.d.ts
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/ral.js
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/semaphore.d.ts
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/semaphore.js
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.d.ts
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/common/sharedArrayCancellation.js
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.d.ts
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/main.js
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/ril.d.ts
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/lib/node/ril.js
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-jsonrpc/typings/thenable.d.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/License.txt
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/browser.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/node.js
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/package.json
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/thirdpartynotices.txt
+-rwxr-xr-x   0        0        0     2754 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/bin/installServerIntoExtension
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/browser/main.js
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.d.ts
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/api.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.d.ts
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/callHierarchy.js
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/configuration.d.ts
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/configuration.js
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.d.ts
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/diagnostic.js
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.d.ts
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/fileOperations.js
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.d.ts
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlayHint.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.d.ts
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/inlineValue.js
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.d.ts
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/linkedEditingRange.js
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/moniker.d.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/moniker.js
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.d.ts
+-rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/notebook.js
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.d.ts
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/progress.js
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.d.ts
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/semanticTokens.js
+-rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.d.ts
+-rw-r--r--   0        0        0    34971 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/server.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/showDocument.d.ts
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/showDocument.js
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.d.ts
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/textDocuments.js
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.d.ts
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/typeHierarchy.js
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/workspaceFolder.d.ts
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/workspaceFolder.js
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.d.ts
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/is.js
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.d.ts
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/common/utils/uuid.js
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.d.ts
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/files.js
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.d.ts
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/main.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/resolve.d.ts
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/lib/node/resolve.js
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver/typings/thenable.d.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/License.txt
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/README.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/browser.d.ts
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/browser.js
+-rw-r--r--   0        0        0    21796 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/metaModel.schema.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.cmd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.d.ts
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/node.js
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/package.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/thirdpartynotices.txt
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/browser/main.d.ts
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/browser/main.js
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.d.ts
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/api.js
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.d.ts
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/connection.js
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.d.ts
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/messages.js
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.d.ts
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.$.js
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.d.ts
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.callHierarchy.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.d.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.colorProvider.js
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.d.ts
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.configuration.js
+-rw-r--r--   0        0        0   112267 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.d.ts
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.d.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.declaration.js
+-rw-r--r--   0        0        0    10782 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.d.ts
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.diagnostic.js
+-rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.d.ts
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.fileOperations.js
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.d.ts
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.foldingRange.js
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.d.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.implementation.js
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.d.ts
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlayHint.js
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.d.ts
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.inlineValue.js
+-rw-r--r--   0        0        0    55332 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.js
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.d.ts
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.linkedEditingRange.js
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.d.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.moniker.js
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.d.ts
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.notebook.js
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.d.ts
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.progress.js
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.d.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.selectionRange.js
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.d.ts
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.semanticTokens.js
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.d.ts
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.showDocument.js
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.d.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeDefinition.js
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.d.ts
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.typeHierarchy.js
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.d.ts
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/protocol.workspaceFolder.js
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.d.ts
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/common/utils/is.js
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.d.ts
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-protocol/lib/node/main.js
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/License.txt
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/thirdpartynotices.txt
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.d.ts
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/esm/main.js
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-textdocument/lib/umd/main.js
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/License.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/README.md
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/package.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/thirdpartynotices.txt
+-rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.d.ts
+-rw-r--r--   0        0        0    78825 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/esm/main.js
+-rw-r--r--   0        0        0    97126 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.d.ts
+-rw-r--r--   0        0        0    92006 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-languageserver-types/lib/umd/main.js
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/LICENSE.md
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/README.md
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/SECURITY.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/package.json
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs
+-rw-r--r--   0        0        0    62941 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/esm/index.mjs.map
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/charCode.d.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/charCode.js
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.d.ts
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js
+-rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/index.js.map
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/platform.d.ts
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/platform.js
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.d.ts
+-rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/uri.js
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.d.ts
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 libro-0.1.3/node_modules/vscode-uri/lib/umd/utils.js
+-rw-r--r--   0        0        0    68855 2020-02-02 00:00:00.000000 libro-0.1.3/src/dev-config/jupyter_server_config.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/_version.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/app.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/handler.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/error.html
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/libro.html
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 libro-0.1.3/src/libro_server/templates/page.html
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 libro-0.1.3/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 libro-0.1.3/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 libro-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 libro-0.1.3/PKG-INFO
```

### Comparing `libro-0.1.2/libro_server/app.py` & `libro-0.1.3/src/libro_server/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from glob import glob
 from jupyter_server.extension.application import ExtensionApp, ExtensionAppJinjaMixin
 from traitlets import Unicode
-from jupyterlab_server import LabConfig, add_handlers
+from jupyterlab_server import LabConfig, LabServerApp, add_handlers
 from jupyter_server.utils import url_path_join as ujoin
 from os.path import relpath
 
 from libro_server.handler import LibroLabHandler, LibroWorkspaceHandler
 
 DEFAULT_STATIC_FILES_PATH = os.path.join(os.path.dirname(__file__), "static")
 DEFAULT_TEMPLATE_FILES_PATH = os.path.join(os.path.dirname(__file__), "templates")
 
-class LibroApp(ExtensionAppJinjaMixin, LabConfig, ExtensionApp):
+
+class LibroApp(LabServerApp):
 
     # -------------- Required traits --------------
     name = "libro"
     default_url = Unicode("/libro", help="The default URL to redirect to from `/`")
     extension_url = "/libro"
     load_other_extensions = True
     file_url_prefix = "/libro-render"
@@ -46,27 +47,29 @@
                 ujoin(self.labextensions_url, relpath(path, extension_path))
                 for path in glob(f"{extension_path}/**/static", recursive=True)
             ]
 
             immutable_cache.update(extensions_url)
 
         self.settings.update({"static_immutable_cache": list(immutable_cache)})
+
     def initialize_templates(self) -> None:
         """Initialize templates."""
         # self.static_paths = [self.static_dir]
         # self.template_paths = [os.path.join(os.path.dirname(__file__), "templates")]
 
     def initialize_handlers(self) -> None:
         """Initialize handlers."""
         # LIBRO_URL_PATTERN = (r"/(?P<libro>/libro/.*)?")
         # url_pattern = LIBRO_URL_PATTERN.format(self.app_url.replace("/", ""))
         self.handlers.append((rf"/{self.name}/?", LibroLabHandler))
         self.handlers.append((rf"/{self.name}/api/workspace", LibroWorkspaceHandler))
         add_handlers(self.handlers, self)
 
+
 # -----------------------------------------------------------------------------
 # Main entry point
 # -----------------------------------------------------------------------------
 
 main = launch_new_instance = LibroApp.launch_instance
 
 if __name__ == "__main__":
```

### Comparing `libro-0.1.2/libro_server/handler.py` & `libro-0.1.3/src/libro_server/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 from jupyter_server.base.handlers import JupyterHandler, APIHandler
 from jupyter_server.extension.handler import (
     ExtensionHandlerMixin,
-    ExtensionHandlerJinjaMixin
+    ExtensionHandlerJinjaMixin,
 )
 from jupyterlab_server import LabHandler
 from tornado import template, web
 
-class BaseTemplateHandler(ExtensionHandlerJinjaMixin, ExtensionHandlerMixin, JupyterHandler):
+
+class BaseTemplateHandler(ExtensionHandlerJinjaMixin, ExtensionHandlerMixin, JupyterHandler):  # type: ignore
     """The base template handler."""
 
     pass
 
+
 class TemplateHandler(BaseTemplateHandler):
     """A template handler."""
 
     def get(self):
         """Optionally, you can print(self.get_template('simple1.html'))"""
         self.write(self.render_template("libro.html"))
 
@@ -26,37 +28,39 @@
     def get(self, path):
         """Write_error renders template from error.html file."""
         self.write_error(400)
 
 
 class LibroLabHandler(LabHandler):
     """Render the JupyterLab View."""
+
     @web.authenticated
     @web.removeslash
-    def get(
-        self, mode=None, workspace=None, tree=None
-    ) -> None:
+    def get(self, mode=None, workspace=None, tree=None) -> None:
         """Get the JupyterLab html page."""
-        workspace = "default" if workspace is None else workspace.replace("/workspaces/", "")
+        workspace = (
+            "default" if workspace is None else workspace.replace("/workspaces/", "")
+        )
         tree_path = "" if tree is None else tree.replace("/tree/", "")
 
         page_config = self.get_page_config()
 
         # Add parameters parsed from the URL
         if mode == "doc":
             page_config["mode"] = "single-document"
         else:
             page_config["mode"] = "multiple-document"
-        
+
         page_config["workspace"] = workspace
         page_config["treePath"] = tree_path
 
         # Write the template with the config.
-        tpl = self.render_template("libro.html", page_config=page_config)  # type:ignore[no-untyped-call]
+        tpl = self.render_template(
+            "libro.html", page_config=page_config
+        )  # type:ignore[no-untyped-call]
         self.write(tpl)
 
+
 class LibroWorkspaceHandler(APIHandler):
-    async def get(
-        self
-    ) -> None:
-        page_config = self.settings.get('page_config_data')
-        self.write(json.dumps(page_config))
+    async def get(self) -> None:
+        page_config = self.settings.get("page_config_data")
+        self.write(json.dumps(page_config))
```

### Comparing `libro-0.1.2/libro_server/templates/libro.html` & `libro-0.1.3/src/libro_server/templates/libro.html`

 * *Files identical despite different names*

### Comparing `libro-0.1.2/libro_server/templates/page.html` & `libro-0.1.3/src/libro_server/templates/page.html`

 * *Files identical despite different names*

