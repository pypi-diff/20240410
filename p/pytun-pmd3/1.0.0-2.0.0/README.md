# Comparing `tmp/pytun-pmd3-1.0.0.tar.gz` & `tmp/pytun-pmd3-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytun-pmd3-1.0.0.tar", last modified: Thu Sep  7 11:01:52 2023, max compression
+gzip compressed data, was "pytun-pmd3-2.0.0.tar", last modified: Wed Apr 10 18:19:18 2024, max compression
```

## Comparing `pytun-pmd3-1.0.0.tar` & `pytun-pmd3-2.0.0.tar`

### file list

```diff
@@ -1,90 +1,144 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.323682 pytun-pmd3-1.0.0/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.297835 pytun-pmd3-1.0.0/.git/
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/FETCH_HEAD
--rw-r--r--   0 runner     (501) staff       (20)       41 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/HEAD
--rw-r--r--   0 runner     (501) staff       (20)      403 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/config
--rw-r--r--   0 runner     (501) staff       (20)       73 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/description
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.304968 pytun-pmd3-1.0.0/.git/hooks/
--rwxr-xr-x   0 runner     (501) staff       (20)      478 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner     (501) staff       (20)      896 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     4726 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner     (501) staff       (20)      189 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner     (501) staff       (20)      424 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     1643 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner     (501) staff       (20)      416 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     1374 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     4898 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner     (501) staff       (20)      544 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     1492 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     2783 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     2308 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner     (501) staff       (20)     3650 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/hooks/update.sample
--rw-r--r--   0 runner     (501) staff       (20)     1209 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/index
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.305452 pytun-pmd3-1.0.0/.git/info/
--rw-r--r--   0 runner     (501) staff       (20)      240 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/info/exclude
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.305942 pytun-pmd3-1.0.0/.git/logs/
--rw-r--r--   0 runner     (501) staff       (20)      188 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/logs/HEAD
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.288509 pytun-pmd3-1.0.0/.git/objects/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.306589 pytun-pmd3-1.0.0/.git/objects/02/
--r--r--r--   0 runner     (501) staff       (20)       51 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/02/00fddf811408de6bdc77aef9891dc2bab56bf8
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.307151 pytun-pmd3-1.0.0/.git/objects/05/
--r--r--r--   0 runner     (501) staff       (20)      644 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.307749 pytun-pmd3-1.0.0/.git/objects/08/
--r--r--r--   0 runner     (501) staff       (20)      538 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/08/af5a317ee4183a167ef85805d1377f4c9b769c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.308286 pytun-pmd3-1.0.0/.git/objects/0b/
--r--r--r--   0 runner     (501) staff       (20)      207 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.308948 pytun-pmd3-1.0.0/.git/objects/11/
--r--r--r--   0 runner     (501) staff       (20)     1054 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/11/c56969531862430cb7b1f7229e3af67b4cd4a2
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.309556 pytun-pmd3-1.0.0/.git/objects/30/
--r--r--r--   0 runner     (501) staff       (20)      107 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/30/b9ae6f25de9828b7a1473270fe3154cbbb67f8
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.310200 pytun-pmd3-1.0.0/.git/objects/33/
--r--r--r--   0 runner     (501) staff       (20)     5344 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/33/b28167e71d9d18e42b1971392821ec70e38951
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.310860 pytun-pmd3-1.0.0/.git/objects/60/
--r--r--r--   0 runner     (501) staff       (20)      581 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/60/2030c63bbc02e1a780aeec03f96cd9f1d8bc6f
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.311432 pytun-pmd3-1.0.0/.git/objects/7f/
--r--r--r--   0 runner     (501) staff       (20)      343 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/7f/ee09114efb25e74bcd7f31a42808b3316dc4ac
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.312011 pytun-pmd3-1.0.0/.git/objects/a2/
--r--r--r--   0 runner     (501) staff       (20)      171 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/a2/ce3543af4fd431390be37e3cb758d57d2eecfc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.312574 pytun-pmd3-1.0.0/.git/objects/af/
--r--r--r--   0 runner     (501) staff       (20)       51 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.313255 pytun-pmd3-1.0.0/.git/objects/b5/
--r--r--r--   0 runner     (501) staff       (20)      128 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.313838 pytun-pmd3-1.0.0/.git/objects/cb/
--r--r--r--   0 runner     (501) staff       (20)     1019 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/cb/ee9104a0e8a07d0057461d2df7146a3bd0caa5
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.314928 pytun-pmd3-1.0.0/.git/objects/d6/
--r--r--r--   0 runner     (501) staff       (20)       92 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/d6/1acd60de2ec118aec5492b69c819b478578270
--r--r--r--   0 runner     (501) staff       (20)      235 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/d6/5be742be8e767a356248138ad23c056c76f275
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.315480 pytun-pmd3-1.0.0/.git/objects/da/
--r--r--r--   0 runner     (501) staff       (20)       83 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/da/28e16ce09d713ce3c49ab1d3d04d3523741c2d
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.316125 pytun-pmd3-1.0.0/.git/objects/dd/
--r--r--r--   0 runner     (501) staff       (20)      383 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/dd/494ae1faa46494e15a7c1a16febb5f8343d063
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.316709 pytun-pmd3-1.0.0/.git/objects/ee/
--r--r--r--   0 runner     (501) staff       (20)     4086 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/objects/ee/54e24d12d7011cc1db7211d542f2c2a14bad07
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.288951 pytun-pmd3-1.0.0/.git/refs/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.317226 pytun-pmd3-1.0.0/.git/refs/tags/
--rw-r--r--   0 runner     (501) staff       (20)       41 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/refs/tags/v1.0.0
--rw-r--r--   0 runner     (501) staff       (20)       41 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.git/shallow
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.289481 pytun-pmd3-1.0.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.318272 pytun-pmd3-1.0.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)      630 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner     (501) staff       (20)     1038 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner     (501) staff       (20)      105 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1055 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       42 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2326 2023-09-07 11:01:52.323132 pytun-pmd3-1.0.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)      312 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/common.h
--rw-r--r--   0 runner     (501) staff       (20)    14702 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/darwin_pytun.c
--rw-r--r--   0 runner     (501) staff       (20)    22929 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/linux_pytun.c
--rw-r--r--   0 runner     (501) staff       (20)     1175 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.321260 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2326 2023-09-07 11:01:52.000000 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1940 2023-09-07 11:01:52.000000 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-09-07 11:01:52.000000 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       15 2023-09-07 11:01:52.000000 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       21 2023-09-07 11:01:52.000000 pytun-pmd3-1.0.0/pytun_pmd3.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-09-07 11:01:52.323791 pytun-pmd3-1.0.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      351 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-09-07 11:01:52.322203 pytun-pmd3-1.0.0/test/
--rw-r--r--   0 runner     (501) staff       (20)     3069 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/test/test_tap.py
--rw-r--r--   0 runner     (501) staff       (20)     3254 2023-09-07 11:01:29.000000 pytun-pmd3-1.0.0/test/test_tun.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/
+-rw-rw-rw-   0        0        0      127 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/FETCH_HEAD
+-rw-rw-rw-   0        0        0       41 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/HEAD
+-rw-rw-rw-   0        0        0      378 2024-04-10 18:18:18.000000 pytun-pmd3-2.0.0/.git/config
+-rw-rw-rw-   0        0        0       73 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/description
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/hooks/
+-rw-rw-rw-   0        0        0      478 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/applypatch-msg.sample
+-rw-rw-rw-   0        0        0      896 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/commit-msg.sample
+-rw-rw-rw-   0        0        0     4726 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/fsmonitor-watchman.sample
+-rw-rw-rw-   0        0        0      189 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/post-update.sample
+-rw-rw-rw-   0        0        0      424 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-applypatch.sample
+-rw-rw-rw-   0        0        0     1649 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-commit.sample
+-rw-rw-rw-   0        0        0      416 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-merge-commit.sample
+-rw-rw-rw-   0        0        0     1374 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-push.sample
+-rw-rw-rw-   0        0        0     4898 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-rebase.sample
+-rw-rw-rw-   0        0        0      544 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/pre-receive.sample
+-rw-rw-rw-   0        0        0     1492 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/prepare-commit-msg.sample
+-rw-rw-rw-   0        0        0     2783 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/push-to-checkout.sample
+-rw-rw-rw-   0        0        0     2308 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/sendemail-validate.sample
+-rw-rw-rw-   0        0        0     3650 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/hooks/update.sample
+-rw-rw-rw-   0        0        0     2460 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/index
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/info/
+-rw-rw-rw-   0        0        0      240 2024-04-10 18:18:15.000000 pytun-pmd3-2.0.0/.git/info/exclude
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/logs/
+-rw-rw-rw-   0        0        0      191 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/logs/HEAD
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.118552 pytun-pmd3-2.0.0/.git/objects/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/00/
+-r--r--r--   0        0        0   185785 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
+-r--r--r--   0        0        0       58 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/00/3f66a2318ebfb30afd90d8293b260cdd3d6999
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/05/
+-r--r--r--   0        0        0      644 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/0b/
+-r--r--r--   0        0        0      207 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/14/
+-r--r--r--   0        0        0      151 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/14/ec9680550691c925edbd3a65f14a25062bb71f
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/16/
+-r--r--r--   0        0        0     4796 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/2a/
+-r--r--r--   0        0        0   279805 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/30/
+-r--r--r--   0        0        0      107 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/30/b9ae6f25de9828b7a1473270fe3154cbbb67f8
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.134182 pytun-pmd3-2.0.0/.git/objects/33/
+-r--r--r--   0        0        0     5344 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/33/b28167e71d9d18e42b1971392821ec70e38951
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/34/
+-r--r--r--   0        0        0       51 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/48/
+-r--r--r--   0        0        0      113 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/4d/
+-r--r--r--   0        0        0       55 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/51/
+-r--r--r--   0        0        0      597 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/52/
+-r--r--r--   0        0        0       55 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/55/
+-r--r--r--   0        0        0     3227 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/56/
+-r--r--r--   0        0        0       53 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/5f/
+-r--r--r--   0        0        0      688 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/71/
+-r--r--r--   0        0        0       55 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/7f/
+-r--r--r--   0        0        0      126 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/81/
+-r--r--r--   0        0        0       55 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/8c/
+-r--r--r--   0        0        0      168 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/8c/2ddee41aa1c6951653ee252434a2e862bb63e0
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/8d/
+-r--r--r--   0        0        0     1024 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/8d/e62c37cc8fcf845ecd68838240936924cf9906
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/a9/
+-r--r--r--   0        0        0     1058 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/a9/de0cc5100692d182a38a2e85ee739bdd771c7a
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/ae/
+-r--r--r--   0        0        0   209806 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/af/
+-r--r--r--   0        0        0       51 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/b4/
+-r--r--r--   0        0        0       83 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/b4/9ac67e351cffd016971fe56eb32564da10b8da
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/b5/
+-r--r--r--   0        0        0      128 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/bc/
+-r--r--r--   0        0        0     2554 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/c0/
+-r--r--r--   0        0        0      287 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/c0/ba173809fe5ff5902ff791514796bd6f528b26
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/c5/
+-r--r--r--   0        0        0      150 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/c8/
+-r--r--r--   0        0        0      626 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/c8/3faddaf014ad1dc356006dd9dc2b527680d57a
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/c9/
+-r--r--r--   0        0        0      416 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/c9/13b6a346e1e791c8d0906140900f694f417c60
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/d4/
+-r--r--r--   0        0        0     3292 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/d4/cb4438b5bf15e244a6c5873db243ab511cac0b
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/dc/
+-r--r--r--   0        0        0   107745 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/ee/
+-r--r--r--   0        0        0     4086 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/ee/54e24d12d7011cc1db7211d542f2c2a14bad07
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/objects/f4/
+-r--r--r--   0        0        0       53 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.118552 pytun-pmd3-2.0.0/.git/refs/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.git/refs/tags/
+-rw-rw-rw-   0        0        0       41 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/refs/tags/v2.0.0
+-rw-rw-rw-   0        0        0       41 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.git/shallow
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.118552 pytun-pmd3-2.0.0/.github/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1438 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.github/workflows/python-publish-macos-and-linux.yml
+-rw-rw-rw-   0        0        0     1130 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.github/workflows/python-publish-windows.yml
+-rw-rw-rw-   0        0        0      118 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/.gitignore
+-rw-rw-rw-   0        0        0     1074 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2444 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      130 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/README.md
+-rw-rw-rw-   0        0        0      331 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/common.h
+-rw-rw-rw-   0        0        0    15299 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/darwin_pytun.c
+-rw-rw-rw-   0        0        0    23997 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/linux_pytun.c
+-rw-rw-rw-   0        0        0     1355 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.149809 pytun-pmd3-2.0.0/pytun_pmd3/
+-rw-rw-rw-   0        0        0       44 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/__init__.py
+-rw-rw-rw-   0        0        0       47 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/
+-rw-rw-rw-   0        0        0     5431 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/LICENSE.txt
+-rw-rw-rw-   0        0        0    13916 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.118552 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/amd64/
+-rw-rw-rw-   0        0        0   427552 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/amd64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/arm/
+-rw-rw-rw-   0        0        0   364552 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/arm/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/arm64/
+-rw-rw-rw-   0        0        0   222488 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/arm64/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/x86/
+-rw-rw-rw-   0        0        0   550928 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/bin/x86/wintun.dll
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3/wintun/include/
+-rw-rw-rw-   0        0        0    10362 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun/include/wintun.h
+-rw-rw-rw-   0        0        0    10682 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/pytun_pmd3/wintun.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/
+-rw-rw-rw-   0        0        0     2444 2024-04-10 18:19:18.000000 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3277 2024-04-10 18:19:18.000000 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 18:19:18.000000 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 18:19:18.000000 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-10 18:19:18.000000 pytun-pmd3-2.0.0/pytun_pmd3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:19:18.165429 pytun-pmd3-2.0.0/test/
+-rw-rw-rw-   0        0        0     3160 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/test/test_tap.py
+-rw-rw-rw-   0        0        0     3348 2024-04-10 18:18:19.000000 pytun-pmd3-2.0.0/test/test_tun.py
```

### Comparing `pytun-pmd3-1.0.0/.git/hooks/commit-msg.sample` & `pytun-pmd3-2.0.0/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/fsmonitor-watchman.sample` & `pytun-pmd3-2.0.0/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/pre-commit.sample` & `pytun-pmd3-2.0.0/.git/hooks/pre-commit.sample`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Cross platform projects tend to avoid non-ASCII filenames; prevent
 # them from being added to the repository. We exploit the fact that the
 # printable range starts at the space character and ends with tilde.
 if [ "$allownonascii" != "true" ] &&
 	# Note that the use of brackets around a tr range is ok here, (it's
 	# even required, for portability to Solaris 10's /usr/bin/tr), since
 	# the square bracket bytes happen to fall in the designated range.
-	test $(git diff --cached --name-only --diff-filter=A -z $against |
+	test $(git diff-index --cached --name-only --diff-filter=A -z $against |
 	  LC_ALL=C tr -d '[ -~]\0' | wc -c) != 0
 then
 	cat <<\EOF
 Error: Attempt to add a non-ASCII file name.
 
 This can cause problems if you want to work with people on other platforms.
```

### Comparing `pytun-pmd3-1.0.0/.git/hooks/pre-push.sample` & `pytun-pmd3-2.0.0/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/pre-rebase.sample` & `pytun-pmd3-2.0.0/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/pre-receive.sample` & `pytun-pmd3-2.0.0/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/prepare-commit-msg.sample` & `pytun-pmd3-2.0.0/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/push-to-checkout.sample` & `pytun-pmd3-2.0.0/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/sendemail-validate.sample` & `pytun-pmd3-2.0.0/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/hooks/update.sample` & `pytun-pmd3-2.0.0/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82` & `pytun-pmd3-2.0.0/.git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/objects/33/b28167e71d9d18e42b1971392821ec70e38951` & `pytun-pmd3-2.0.0/.git/objects/33/b28167e71d9d18e42b1971392821ec70e38951`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.git/objects/ee/54e24d12d7011cc1db7211d542f2c2a14bad07` & `pytun-pmd3-2.0.0/.git/objects/ee/54e24d12d7011cc1db7211d542f2c2a14bad07`

 * *Files identical despite different names*

### Comparing `pytun-pmd3-1.0.0/.github/workflows/python-publish.yml` & `pytun-pmd3-2.0.0/.github/workflows/python-publish-windows.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-# This workflows will upload a Python Package using Twine when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
-name: Upload Python Package
-
-
-on:
-  release:
-    types: [created]
-
-
-jobs:
-  deploy:
-
-    runs-on: ${{ matrix.os }}
-
-    strategy:
-      matrix:
-        python-version: [ 3.8, 3.9, "3.10", "3.11" ]
-        os: [ ubuntu-latest, macos-latest ]
-
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -U build setuptools wheel twine
-    - name: Build and publish
-      env:
-        TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        python -m build
-        twine upload dist/*
+# This workflows will upload a Python Package using Twine when a release is created
+# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
+
+name: Upload python package for windows
+
+on:
+  release:
+    types: [ created ]
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
+jobs:
+  build:
+    if: '! github.event.pull_request.draft'
+    runs-on: windows-latest
+
+    steps:
+      - uses: actions/checkout@v4
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.x'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -U build setuptools wheel twine
+      - name: Build and publish
+        env:
+          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
+          CIBW_ARCHS: ${{ matrix.arch }}
+        run: |
+          python3 -m build
+          twine upload dist/* --skip-existing
```

### Comparing `pytun-pmd3-1.0.0/LICENSE` & `pytun-pmd3-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2011, montag451.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+Copyright (c) 2011, montag451.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `pytun-pmd3-1.0.0/PKG-INFO` & `pytun-pmd3-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-Metadata-Version: 2.1
-Name: pytun-pmd3
-Version: 1.0.0
-Summary: python-pytun fork with Darwin support (IPv6-ONLY)
-Author-email: doronz88 <doron88@gmail.com>
-Maintainer-email: doronz88 <doron88@gmail.com>
-License: Copyright (c) 2011, montag451.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/doronz88/pytun-pmd3
-Project-URL: Bug Reports, https://github.com/doronz88/pytun-pmd3/issues
-Keywords: tun,tuntap,darwin,pymobiledevice3,macos
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-
-# Linux & Darwin TUN/TAP wrapper for Python
-
-This is a fork of https://github.com/montag451/pytun with partial Darwin support.
+Metadata-Version: 2.1
+Name: pytun-pmd3
+Version: 2.0.0
+Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
+Author-email: doronz88 <doron88@gmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>
+License: Copyright (c) 2011, montag451.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/doronz88/pytun-pmd3
+Project-URL: Bug Reports, https://github.com/doronz88/pytun-pmd3/issues
+Keywords: tun,tuntap,darwin,pymobiledevice3,macos,windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
+# Linux & Darwin TUN/TAP wrapper for Python
+
+This is a fork of https://github.com/montag451/pytun with partial Darwin support.
```

### Comparing `pytun-pmd3-1.0.0/darwin_pytun.c` & `pytun-pmd3-2.0.0/darwin_pytun.c`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,597 +1,597 @@
-#define PY_SSIZE_T_CLEAN
-
-#include <Python.h>
-#include <string.h>
-#include <unistd.h>
-#include <sys/socket.h>
-#include <sys/ioctl.h>
-#include <net/if.h>
-#include <stdio.h>
-#include <sys/kern_event.h>
-#include <sys/kern_control.h>
-
-#include "common.h"
-
-#define KERN_SUCCESS (0)
-#define UTUN_CONTROL_NAME "com.apple.net.utun_control"
-#define UTUN_OPT_IFNAME (2)
-
-#ifndef PyVarObject_HEAD_INIT
-#define PyVarObject_HEAD_INIT(type, size) \
-    PyObject_HEAD_INIT(type) size,
-#endif
-
-static PyObject *pytun_error = NULL;
-
-PyDoc_STRVAR(pytun_error_doc,
-             "This exception is raised when an error occurs. The accompanying value is\n\
-either a string telling what went wrong or a pair (errno, string)\n\
-representing an error returned by a system call, similar to the value\n\
-accompanying os.error. See the module errno, which contains names for the\n\
-error codes defined by the underlying operating system.");
-
-static void raise_error(const char *errmsg) {
-    PyErr_SetString(pytun_error, errmsg);
-}
-
-static void raise_error_from_errno(void) {
-    PyErr_SetFromErrno(pytun_error);
-}
-
-static int create_utun_interface(u_int32_t num, size_t ifname_len, char *ifname) {
-    struct sockaddr_ctl addr;
-    struct ctl_info info;
-
-    int fd = socket(PF_SYSTEM, SOCK_DGRAM, SYSPROTO_CONTROL);
-
-    bzero(&info, sizeof(info));
-    strncpy(info.ctl_name, UTUN_CONTROL_NAME, MAX_KCTL_NAME);
-    if (ioctl(fd, CTLIOCGINFO, &info) != KERN_SUCCESS) {
-        close(fd);
-        return -1;
-    }
-
-    addr.sc_id = info.ctl_id;
-    addr.sc_len = sizeof(addr);
-    addr.sc_family = AF_SYSTEM;
-    addr.ss_sysaddr = AF_SYS_CONTROL;
-    addr.sc_unit = num + 1; // utunX where X is sc.sc_unit -1
-    if (connect(fd, (struct sockaddr *) &addr, sizeof(addr)) != KERN_SUCCESS) {
-        close(fd);
-        return -1;
-    }
-
-    if (getsockopt(fd, SYSPROTO_CONTROL, UTUN_OPT_IFNAME, ifname, (socklen_t *) &ifname_len) != KERN_SUCCESS) {
-        close(fd);
-        return -1;
-    }
-
-    return fd;
-}
-
-static PyObject *pytun_tuntap_new(PyTypeObject *type, PyObject *args, PyObject *kwds) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) type->tp_alloc(type, 0);
-    int i = 0;
-    int fd;
-
-    char name[sizeof(tuntap->name)];
-    while (-1 == (fd = create_utun_interface(i, sizeof(name), name))) {
-        ++i;
-    }
-    if (-1 == fd) {
-        raise_error("Failed to create tun device");
-    }
-    tuntap->fd = fd;
-    strcpy(tuntap->name, name);
-    return (PyObject *) tuntap;
-}
-
-static void pytun_tuntap_dealloc(PyObject *self) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-
-    if (tuntap->fd >= 0) {
-        Py_BEGIN_ALLOW_THREADS
-            close(tuntap->fd);
-        Py_END_ALLOW_THREADS
-    }
-    self->ob_type->tp_free(self);
-}
-
-static PyObject *pytun_tuntap_get_name(PyObject *self, void *d) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-
-#if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromString(tuntap->name);
-#else
-    return PyString_FromString(tuntap->name);
-#endif
-}
-
-static int pytun_tuntap_set_addr(PyObject *self, PyObject *value, void *d) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    int ret = 0;
-    char cmd[1024];
-
-#if PY_MAJOR_VERSION >= 3
-    PyObject *tmp_addr;
-#endif
-    const char *addr;
-
-#if PY_MAJOR_VERSION >= 3
-    tmp_addr = PyUnicode_AsASCIIString(value);
-    addr = tmp_addr != NULL ? PyBytes_AS_STRING(tmp_addr) : NULL;
-#else
-    addr = PyString_AsString(value);
-#endif
-    if (addr == NULL) {
-        ret = -1;
-        goto out;
-    }
-
-    sprintf(cmd, "ifconfig %s inet6 %s prefixlen 64", tuntap->name, addr);
-    if (system(cmd) != 0) {
-        ret = -1;
-        goto out;
-    }
-
-    out:
-#if PY_MAJOR_VERSION >= 3
-    Py_XDECREF(tmp_addr);
-#endif
-
-    return ret;
-}
-
-static PyObject *pytun_tuntap_get_mtu(PyObject *self, void *d) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    struct ifreq req;
-    int ret;
-
-    memset(&req, 0, sizeof(req));
-    strcpy(req.ifr_name, tuntap->name);
-
-    Py_BEGIN_ALLOW_THREADS;
-        ret = ioctl(tuntap->fd, SIOCGIFMTU, &req);
-    Py_END_ALLOW_THREADS;
-    if (ret < 0) {
-        raise_error_from_errno();
-        return NULL;
-    }
-
-#if PY_MAJOR_VERSION >= 3
-    return PyLong_FromLong(req.ifr_mtu);
-#else
-    return PyInt_FromLong(req.ifr_mtu);
-#endif
-}
-
-static int pytun_tuntap_set_mtu(PyObject *self, PyObject *value, void *d) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    struct ifreq req;
-    int mtu;
-    int err;
-
-    mtu = (int) PyLong_AsLong(value);
-    if (mtu <= 0) {
-        if (!PyErr_Occurred()) {
-            raise_error("Bad MTU, should be > 0");
-        }
-        return -1;
-    }
-    memset(&req, 0, sizeof(req));
-    strcpy(req.ifr_name, tuntap->name);
-    req.ifr_mtu = mtu;
-
-    Py_BEGIN_ALLOW_THREADS;
-        err = ioctl(tuntap->fd, SIOCSIFMTU, &req);
-    Py_END_ALLOW_THREADS;
-    if (err < 0) {
-        raise_error_from_errno();
-        return -1;
-    }
-
-    return 0;
-}
-
-static PyGetSetDef pytun_tuntap_prop[] =
-{
-    {
-     "name",
-     pytun_tuntap_get_name,
-     NULL,
-     NULL,
-     NULL
-    },
-    {
-     "addr",
-     NULL,
-     pytun_tuntap_set_addr,
-     NULL,
-     NULL
-    },
-    {
-     "dstaddr",
-     NULL,
-     NULL,
-     NULL, 
-     NULL
-    },
-    {
-     "hwaddr",
-     NULL,
-     NULL,
-     NULL,
-     NULL
-    },
-    {
-     "netmask",
-     NULL,
-     NULL,
-     NULL,
-     NULL
-    },
-    {
-     "mtu",
-     pytun_tuntap_get_mtu,
-     pytun_tuntap_set_mtu,
-     NULL,
-     NULL
-    },
-    {NULL, NULL, NULL, NULL, NULL}
-};
-
-static PyObject *pytun_tuntap_close(PyObject *self) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-
-    if (tuntap->fd >= 0) {
-        Py_BEGIN_ALLOW_THREADS
-            close(tuntap->fd), tuntap->fd = -1;
-        Py_END_ALLOW_THREADS
-    }
-
-    Py_RETURN_NONE;
-}
-
-PyDoc_STRVAR(pytun_tuntap_close_doc,
-             "close() -> None.\n\
-Close the device.");
-
-static PyObject *pytun_tuntap_up(PyObject *self) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    struct ifreq req;
-
-    memset(&req, 0, sizeof(req));
-    strcpy(req.ifr_name, tuntap->name);
-    if (ioctl(tuntap->fd, SIOCGIFFLAGS, &req) < 0) {
-        return NULL;
-    }
-    if (!(req.ifr_flags & IFF_UP)) {
-        req.ifr_flags |= IFF_UP;
-        if (ioctl(tuntap->fd, SIOCSIFFLAGS, &req) < 0) {
-            return NULL;
-        }
-    }
-
-    Py_RETURN_NONE;
-}
-
-PyDoc_STRVAR(pytun_tuntap_up_doc,
-             "up() -> None.\n\
-Bring up the device.");
-
-static PyObject *pytun_tuntap_down(PyObject *self) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    struct ifreq req;
-
-    memset(&req, 0, sizeof(req));
-    strcpy(req.ifr_name, tuntap->name);
-    if (ioctl(tuntap->fd, SIOCGIFFLAGS, &req) < 0) {
-        return NULL;
-    }
-    if (req.ifr_flags & IFF_UP) {
-        req.ifr_flags &= ~IFF_UP;
-        if (ioctl(tuntap->fd, SIOCSIFFLAGS, &req) < 0) {
-            return NULL;
-        }
-    }
-
-    Py_RETURN_NONE;
-}
-
-PyDoc_STRVAR(pytun_tuntap_down_doc,
-             "down() -> None.\n\
-Bring down the device.");
-
-static PyObject *pytun_tuntap_read(PyObject *self, PyObject *args) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    unsigned int rdlen;
-    ssize_t outlen;
-    PyObject *buf;
-
-
-    if (!PyArg_ParseTuple(args, "I:read", &rdlen)) {
-        return NULL;
-    }
-
-    /* Allocate a new string */
-#if PY_MAJOR_VERSION >= 3
-    buf = PyBytes_FromStringAndSize(NULL, rdlen);
-#else
-    buf = PyString_FromStringAndSize(NULL, rdlen);
-#endif
-    if (buf == NULL) {
-        return NULL;
-    }
-    /* Read data */
-    Py_BEGIN_ALLOW_THREADS;
-#if PY_MAJOR_VERSION >= 3
-        outlen = read(tuntap->fd, PyBytes_AS_STRING(buf), rdlen);
-#else
-        outlen = read(tuntap->fd, PyString_AS_STRING(buf), rdlen);
-#endif
-    Py_END_ALLOW_THREADS;
-
-    if (outlen < 0) {
-        /* An error occurred, release the string and return an error */
-        raise_error_from_errno();
-        return NULL;
-    }
-    if (outlen < rdlen) {
-        /* We did not read as many bytes as we anticipated, resize the
-           string if possible and be successful. */
-#if PY_MAJOR_VERSION >= 3
-        if (_PyBytes_Resize(&buf, outlen) < 0)
-#else
-            if (_PyString_Resize(&buf, outlen) < 0)
-#endif
-        {
-            return NULL;
-        }
-    }
-
-    return buf;
-}
-
-PyDoc_STRVAR(pytun_tuntap_read_doc,
-             "read(size) -> read at most size bytes, returned as a string.");
-
-static PyObject *pytun_tuntap_write(PyObject *self, PyObject *args) {
-    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
-    char *buf;
-    Py_ssize_t len;
-    ssize_t written;
-
-    if (!PyArg_ParseTuple(args, "s#:write", &buf, &len)) {
-        return NULL;
-    }
-
-    Py_BEGIN_ALLOW_THREADS
-        written = write(tuntap->fd, buf, len);
-    Py_END_ALLOW_THREADS
-    if (written < 0) {
-        raise_error_from_errno();
-        return NULL;
-    }
-
-#if PY_MAJOR_VERSION >= 3
-    return PyLong_FromSsize_t(written);
-#else
-    return PyInt_FromSsize_t(written);
-#endif
-}
-
-PyDoc_STRVAR(pytun_tuntap_write_doc,
-             "write(str) -> number of bytes written.\n\
-Write str to device.");
-
-static PyObject *pytun_tuntap_fileno(PyObject *self) {
-#if PY_MAJOR_VERSION >= 3
-    return PyLong_FromLong(((pytun_tuntap_t *) self)->fd);
-#else
-    return PyInt_FromLong(((pytun_tuntap_t*)self)->fd);
-#endif
-}
-
-PyDoc_STRVAR(pytun_tuntap_fileno_doc,
-             "fileno() -> integer \"file descriptor\".");
-
-static PyObject *pytun_tuntap_persist(PyObject *self, PyObject *args) {
-    Py_RETURN_NONE;
-}
-
-PyDoc_STRVAR(pytun_tuntap_persist_doc,
-             "persist(flag) -> None.\n\
-Make the TUN/TAP persistent if flags is True else\n\
-make it non-persistent.");
-
-#ifdef IFF_MULTI_QUEUE
-static PyObject* pytun_tuntap_mq_attach(PyObject* self, PyObject* args)
-{
-    pytun_tuntap_t* tuntap = (pytun_tuntap_t*)self;
-    PyObject* tmp = NULL;
-    struct ifreq req;
-    int ret;
-
-    if (!PyArg_ParseTuple(args, "|O!:attach", &PyBool_Type, &tmp))
-    {
-        return NULL;
-    }
-
-    memset(&req, 0, sizeof(req));
-    if (tmp == NULL || tmp == Py_True)
-    {
-        req.ifr_flags = IFF_ATTACH_QUEUE;
-    }
-    else
-    {
-        req.ifr_flags = IFF_DETACH_QUEUE;
-    }
-
-    Py_BEGIN_ALLOW_THREADS
-    ret = ioctl(tuntap->fd, TUNSETQUEUE, &req);
-    Py_END_ALLOW_THREADS
-    if (ret < 0)
-    {
-        raise_error_from_errno();
-        return NULL;
-    }
-
-    Py_RETURN_NONE;
-}
-
-PyDoc_STRVAR(pytun_tuntap_mq_attach_doc,
-"mq_attach(flag) -> None.\n\
-Enable the queue if flags is True else\n\
-disable the queue.");
-#endif
-
-static PyMethodDef pytun_tuntap_meth[] =
-        {
-                {
-                        "close",
-                        (PyCFunction) pytun_tuntap_close,
-                        METH_NOARGS,
-                        pytun_tuntap_close_doc
-                },
-                {
-                        "up",
-                        (PyCFunction) pytun_tuntap_up,
-                        METH_NOARGS,
-                        pytun_tuntap_up_doc
-                },
-                {
-                        "down",
-                        (PyCFunction) pytun_tuntap_down,
-                        METH_NOARGS,
-                        pytun_tuntap_down_doc
-                },
-                {
-                        "read",
-                        (PyCFunction) pytun_tuntap_read,
-                        METH_VARARGS,
-                        pytun_tuntap_read_doc
-                },
-                {
-                        "write",
-                        (PyCFunction) pytun_tuntap_write,
-                        METH_VARARGS,
-                        pytun_tuntap_write_doc
-                },
-                {
-                        "fileno",
-                        (PyCFunction) pytun_tuntap_fileno,
-                        METH_NOARGS,
-                        pytun_tuntap_fileno_doc
-                },
-                {
-                        "persist",
-                        (PyCFunction) pytun_tuntap_persist,
-                        METH_VARARGS,
-                        pytun_tuntap_persist_doc
-                },
-#ifdef IFF_MULTI_QUEUE
-                {
-                 "mq_attach",
-                 (PyCFunction)pytun_tuntap_mq_attach,
-                 METH_VARARGS,
-                 pytun_tuntap_mq_attach_doc
-                },
-#endif
-                {NULL, NULL, 0, NULL}
-        };
-
-PyDoc_STRVAR(pytun_tuntap_doc,
-             "TunTapDevice(name='', flags=IFF_TUN, dev='/dev/net/tun') -> TUN/TAP device object.");
-
-static PyTypeObject pytun_tuntap_type =
-        {
-                PyVarObject_HEAD_INIT(&PyType_Type, 0)
-                .tp_name = "pytun.TunTapDevice",
-                .tp_basicsize = sizeof(pytun_tuntap_t),
-                .tp_dealloc = pytun_tuntap_dealloc,
-                .tp_flags = Py_TPFLAGS_DEFAULT,
-                .tp_doc = pytun_tuntap_doc,
-                .tp_methods = pytun_tuntap_meth,
-                .tp_getset = pytun_tuntap_prop,
-                .tp_new = pytun_tuntap_new
-        };
-
-#if PY_MAJOR_VERSION >= 3
-static struct PyModuleDef pytun_module =
-        {
-                .m_base = PyModuleDef_HEAD_INIT,
-                .m_name = "pytun",
-                .m_doc = NULL,
-                .m_size = -1,
-                .m_methods = NULL,
-#if PY_MINOR_VERSION <= 4
-                .m_reload = NULL,
-#else
-                .m_slots = NULL,
-#endif
-                .m_traverse = NULL,
-                .m_clear = NULL,
-                .m_free = NULL
-        };
-#endif
-
-#if PY_MAJOR_VERSION >= 3
-PyMODINIT_FUNC PyInit_pytun_pmd3(void)
-#else
-PyMODINIT_FUNC initpytun(void)
-#endif
-{
-    PyObject *m;
-    PyObject *pytun_error_dict = NULL;
-
-#if PY_MAJOR_VERSION >= 3
-    m = PyModule_Create(&pytun_module);
-#else
-    m = Py_InitModule(MODULE_NAME, NULL);
-#endif
-    if (m == NULL) {
-        goto error;
-    }
-
-    if (PyType_Ready(&pytun_tuntap_type) != 0) {
-        goto error;
-    }
-    Py_INCREF((PyObject *) &pytun_tuntap_type);
-    if (PyModule_AddObject(m, "TunTapDevice", (PyObject *) &pytun_tuntap_type) != 0) {
-        Py_DECREF((PyObject *) &pytun_tuntap_type);
-        goto error;
-    }
-
-    pytun_error_dict = Py_BuildValue("{ss}", "__doc__", pytun_error_doc);
-    if (pytun_error_dict == NULL) {
-        goto error;
-    }
-    pytun_error = PyErr_NewException("pytun.Error", PyExc_IOError, pytun_error_dict);
-    Py_DECREF(pytun_error_dict);
-    if (pytun_error == NULL) {
-        goto error;
-    }
-    Py_INCREF(pytun_error);
-    if (PyModule_AddObject(m, "Error", pytun_error) != 0) {
-        Py_DECREF(pytun_error);
-        goto error;
-    }
-
-    goto out;
-
-    error:
-#if PY_MAJOR_VERSION >= 3
-    Py_XDECREF(pytun_error);
-    Py_XDECREF(m);
-    pytun_error = NULL;
-    m = NULL;
-#endif
-
-    out:
-#if PY_MAJOR_VERSION >= 3
-    return m;
-#else
-    return;
-#endif
-}
-
+#define PY_SSIZE_T_CLEAN
+
+#include <Python.h>
+#include <string.h>
+#include <unistd.h>
+#include <sys/socket.h>
+#include <sys/ioctl.h>
+#include <net/if.h>
+#include <stdio.h>
+#include <sys/kern_event.h>
+#include <sys/kern_control.h>
+
+#include "common.h"
+
+#define KERN_SUCCESS (0)
+#define UTUN_CONTROL_NAME "com.apple.net.utun_control"
+#define UTUN_OPT_IFNAME (2)
+
+#ifndef PyVarObject_HEAD_INIT
+#define PyVarObject_HEAD_INIT(type, size) \
+    PyObject_HEAD_INIT(type) size,
+#endif
+
+static PyObject *pytun_error = NULL;
+
+PyDoc_STRVAR(pytun_error_doc,
+             "This exception is raised when an error occurs. The accompanying value is\n\
+either a string telling what went wrong or a pair (errno, string)\n\
+representing an error returned by a system call, similar to the value\n\
+accompanying os.error. See the module errno, which contains names for the\n\
+error codes defined by the underlying operating system.");
+
+static void raise_error(const char *errmsg) {
+    PyErr_SetString(pytun_error, errmsg);
+}
+
+static void raise_error_from_errno(void) {
+    PyErr_SetFromErrno(pytun_error);
+}
+
+static int create_utun_interface(u_int32_t num, size_t ifname_len, char *ifname) {
+    struct sockaddr_ctl addr;
+    struct ctl_info info;
+
+    int fd = socket(PF_SYSTEM, SOCK_DGRAM, SYSPROTO_CONTROL);
+
+    bzero(&info, sizeof(info));
+    strncpy(info.ctl_name, UTUN_CONTROL_NAME, MAX_KCTL_NAME);
+    if (ioctl(fd, CTLIOCGINFO, &info) != KERN_SUCCESS) {
+        close(fd);
+        return -1;
+    }
+
+    addr.sc_id = info.ctl_id;
+    addr.sc_len = sizeof(addr);
+    addr.sc_family = AF_SYSTEM;
+    addr.ss_sysaddr = AF_SYS_CONTROL;
+    addr.sc_unit = num + 1; // utunX where X is sc.sc_unit -1
+    if (connect(fd, (struct sockaddr *) &addr, sizeof(addr)) != KERN_SUCCESS) {
+        close(fd);
+        return -1;
+    }
+
+    if (getsockopt(fd, SYSPROTO_CONTROL, UTUN_OPT_IFNAME, ifname, (socklen_t *) &ifname_len) != KERN_SUCCESS) {
+        close(fd);
+        return -1;
+    }
+
+    return fd;
+}
+
+static PyObject *pytun_tuntap_new(PyTypeObject *type, PyObject *args, PyObject *kwds) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) type->tp_alloc(type, 0);
+    int i = 0;
+    int fd;
+
+    char name[sizeof(tuntap->name)];
+    while (-1 == (fd = create_utun_interface(i, sizeof(name), name))) {
+        ++i;
+    }
+    if (-1 == fd) {
+        raise_error("Failed to create tun device");
+    }
+    tuntap->fd = fd;
+    strcpy(tuntap->name, name);
+    return (PyObject *) tuntap;
+}
+
+static void pytun_tuntap_dealloc(PyObject *self) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+
+    if (tuntap->fd >= 0) {
+        Py_BEGIN_ALLOW_THREADS
+            close(tuntap->fd);
+        Py_END_ALLOW_THREADS
+    }
+    self->ob_type->tp_free(self);
+}
+
+static PyObject *pytun_tuntap_get_name(PyObject *self, void *d) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromString(tuntap->name);
+#else
+    return PyString_FromString(tuntap->name);
+#endif
+}
+
+static int pytun_tuntap_set_addr(PyObject *self, PyObject *value, void *d) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    int ret = 0;
+    char cmd[1024];
+
+#if PY_MAJOR_VERSION >= 3
+    PyObject *tmp_addr;
+#endif
+    const char *addr;
+
+#if PY_MAJOR_VERSION >= 3
+    tmp_addr = PyUnicode_AsASCIIString(value);
+    addr = tmp_addr != NULL ? PyBytes_AS_STRING(tmp_addr) : NULL;
+#else
+    addr = PyString_AsString(value);
+#endif
+    if (addr == NULL) {
+        ret = -1;
+        goto out;
+    }
+
+    sprintf(cmd, "ifconfig %s inet6 %s prefixlen 64", tuntap->name, addr);
+    if (system(cmd) != 0) {
+        ret = -1;
+        goto out;
+    }
+
+    out:
+#if PY_MAJOR_VERSION >= 3
+    Py_XDECREF(tmp_addr);
+#endif
+
+    return ret;
+}
+
+static PyObject *pytun_tuntap_get_mtu(PyObject *self, void *d) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    struct ifreq req;
+    int ret;
+
+    memset(&req, 0, sizeof(req));
+    strcpy(req.ifr_name, tuntap->name);
+
+    Py_BEGIN_ALLOW_THREADS;
+        ret = ioctl(tuntap->fd, SIOCGIFMTU, &req);
+    Py_END_ALLOW_THREADS;
+    if (ret < 0) {
+        raise_error_from_errno();
+        return NULL;
+    }
+
+#if PY_MAJOR_VERSION >= 3
+    return PyLong_FromLong(req.ifr_mtu);
+#else
+    return PyInt_FromLong(req.ifr_mtu);
+#endif
+}
+
+static int pytun_tuntap_set_mtu(PyObject *self, PyObject *value, void *d) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    struct ifreq req;
+    int mtu;
+    int err;
+
+    mtu = (int) PyLong_AsLong(value);
+    if (mtu <= 0) {
+        if (!PyErr_Occurred()) {
+            raise_error("Bad MTU, should be > 0");
+        }
+        return -1;
+    }
+    memset(&req, 0, sizeof(req));
+    strcpy(req.ifr_name, tuntap->name);
+    req.ifr_mtu = mtu;
+
+    Py_BEGIN_ALLOW_THREADS;
+        err = ioctl(tuntap->fd, SIOCSIFMTU, &req);
+    Py_END_ALLOW_THREADS;
+    if (err < 0) {
+        raise_error_from_errno();
+        return -1;
+    }
+
+    return 0;
+}
+
+static PyGetSetDef pytun_tuntap_prop[] =
+{
+    {
+     "name",
+     pytun_tuntap_get_name,
+     NULL,
+     NULL,
+     NULL
+    },
+    {
+     "addr",
+     NULL,
+     pytun_tuntap_set_addr,
+     NULL,
+     NULL
+    },
+    {
+     "dstaddr",
+     NULL,
+     NULL,
+     NULL, 
+     NULL
+    },
+    {
+     "hwaddr",
+     NULL,
+     NULL,
+     NULL,
+     NULL
+    },
+    {
+     "netmask",
+     NULL,
+     NULL,
+     NULL,
+     NULL
+    },
+    {
+     "mtu",
+     pytun_tuntap_get_mtu,
+     pytun_tuntap_set_mtu,
+     NULL,
+     NULL
+    },
+    {NULL, NULL, NULL, NULL, NULL}
+};
+
+static PyObject *pytun_tuntap_close(PyObject *self) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+
+    if (tuntap->fd >= 0) {
+        Py_BEGIN_ALLOW_THREADS
+            close(tuntap->fd), tuntap->fd = -1;
+        Py_END_ALLOW_THREADS
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(pytun_tuntap_close_doc,
+             "close() -> None.\n\
+Close the device.");
+
+static PyObject *pytun_tuntap_up(PyObject *self) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    struct ifreq req;
+
+    memset(&req, 0, sizeof(req));
+    strcpy(req.ifr_name, tuntap->name);
+    if (ioctl(tuntap->fd, SIOCGIFFLAGS, &req) < 0) {
+        return NULL;
+    }
+    if (!(req.ifr_flags & IFF_UP)) {
+        req.ifr_flags |= IFF_UP;
+        if (ioctl(tuntap->fd, SIOCSIFFLAGS, &req) < 0) {
+            return NULL;
+        }
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(pytun_tuntap_up_doc,
+             "up() -> None.\n\
+Bring up the device.");
+
+static PyObject *pytun_tuntap_down(PyObject *self) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    struct ifreq req;
+
+    memset(&req, 0, sizeof(req));
+    strcpy(req.ifr_name, tuntap->name);
+    if (ioctl(tuntap->fd, SIOCGIFFLAGS, &req) < 0) {
+        return NULL;
+    }
+    if (req.ifr_flags & IFF_UP) {
+        req.ifr_flags &= ~IFF_UP;
+        if (ioctl(tuntap->fd, SIOCSIFFLAGS, &req) < 0) {
+            return NULL;
+        }
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(pytun_tuntap_down_doc,
+             "down() -> None.\n\
+Bring down the device.");
+
+static PyObject *pytun_tuntap_read(PyObject *self, PyObject *args) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    unsigned int rdlen;
+    ssize_t outlen;
+    PyObject *buf;
+
+
+    if (!PyArg_ParseTuple(args, "I:read", &rdlen)) {
+        return NULL;
+    }
+
+    /* Allocate a new string */
+#if PY_MAJOR_VERSION >= 3
+    buf = PyBytes_FromStringAndSize(NULL, rdlen);
+#else
+    buf = PyString_FromStringAndSize(NULL, rdlen);
+#endif
+    if (buf == NULL) {
+        return NULL;
+    }
+    /* Read data */
+    Py_BEGIN_ALLOW_THREADS;
+#if PY_MAJOR_VERSION >= 3
+        outlen = read(tuntap->fd, PyBytes_AS_STRING(buf), rdlen);
+#else
+        outlen = read(tuntap->fd, PyString_AS_STRING(buf), rdlen);
+#endif
+    Py_END_ALLOW_THREADS;
+
+    if (outlen < 0) {
+        /* An error occurred, release the string and return an error */
+        raise_error_from_errno();
+        return NULL;
+    }
+    if (outlen < rdlen) {
+        /* We did not read as many bytes as we anticipated, resize the
+           string if possible and be successful. */
+#if PY_MAJOR_VERSION >= 3
+        if (_PyBytes_Resize(&buf, outlen) < 0)
+#else
+            if (_PyString_Resize(&buf, outlen) < 0)
+#endif
+        {
+            return NULL;
+        }
+    }
+
+    return buf;
+}
+
+PyDoc_STRVAR(pytun_tuntap_read_doc,
+             "read(size) -> read at most size bytes, returned as a string.");
+
+static PyObject *pytun_tuntap_write(PyObject *self, PyObject *args) {
+    pytun_tuntap_t *tuntap = (pytun_tuntap_t *) self;
+    char *buf;
+    Py_ssize_t len;
+    ssize_t written;
+
+    if (!PyArg_ParseTuple(args, "s#:write", &buf, &len)) {
+        return NULL;
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+        written = write(tuntap->fd, buf, len);
+    Py_END_ALLOW_THREADS
+    if (written < 0) {
+        raise_error_from_errno();
+        return NULL;
+    }
+
+#if PY_MAJOR_VERSION >= 3
+    return PyLong_FromSsize_t(written);
+#else
+    return PyInt_FromSsize_t(written);
+#endif
+}
+
+PyDoc_STRVAR(pytun_tuntap_write_doc,
+             "write(str) -> number of bytes written.\n\
+Write str to device.");
+
+static PyObject *pytun_tuntap_fileno(PyObject *self) {
+#if PY_MAJOR_VERSION >= 3
+    return PyLong_FromLong(((pytun_tuntap_t *) self)->fd);
+#else
+    return PyInt_FromLong(((pytun_tuntap_t*)self)->fd);
+#endif
+}
+
+PyDoc_STRVAR(pytun_tuntap_fileno_doc,
+             "fileno() -> integer \"file descriptor\".");
+
+static PyObject *pytun_tuntap_persist(PyObject *self, PyObject *args) {
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(pytun_tuntap_persist_doc,
+             "persist(flag) -> None.\n\
+Make the TUN/TAP persistent if flags is True else\n\
+make it non-persistent.");
+
+#ifdef IFF_MULTI_QUEUE
+static PyObject* pytun_tuntap_mq_attach(PyObject* self, PyObject* args)
+{
+    pytun_tuntap_t* tuntap = (pytun_tuntap_t*)self;
+    PyObject* tmp = NULL;
+    struct ifreq req;
+    int ret;
+
+    if (!PyArg_ParseTuple(args, "|O!:attach", &PyBool_Type, &tmp))
+    {
+        return NULL;
+    }
+
+    memset(&req, 0, sizeof(req));
+    if (tmp == NULL || tmp == Py_True)
+    {
+        req.ifr_flags = IFF_ATTACH_QUEUE;
+    }
+    else
+    {
+        req.ifr_flags = IFF_DETACH_QUEUE;
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    ret = ioctl(tuntap->fd, TUNSETQUEUE, &req);
+    Py_END_ALLOW_THREADS
+    if (ret < 0)
+    {
+        raise_error_from_errno();
+        return NULL;
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(pytun_tuntap_mq_attach_doc,
+"mq_attach(flag) -> None.\n\
+Enable the queue if flags is True else\n\
+disable the queue.");
+#endif
+
+static PyMethodDef pytun_tuntap_meth[] =
+        {
+                {
+                        "close",
+                        (PyCFunction) pytun_tuntap_close,
+                        METH_NOARGS,
+                        pytun_tuntap_close_doc
+                },
+                {
+                        "up",
+                        (PyCFunction) pytun_tuntap_up,
+                        METH_NOARGS,
+                        pytun_tuntap_up_doc
+                },
+                {
+                        "down",
+                        (PyCFunction) pytun_tuntap_down,
+                        METH_NOARGS,
+                        pytun_tuntap_down_doc
+                },
+                {
+                        "read",
+                        (PyCFunction) pytun_tuntap_read,
+                        METH_VARARGS,
+                        pytun_tuntap_read_doc
+                },
+                {
+                        "write",
+                        (PyCFunction) pytun_tuntap_write,
+                        METH_VARARGS,
+                        pytun_tuntap_write_doc
+                },
+                {
+                        "fileno",
+                        (PyCFunction) pytun_tuntap_fileno,
+                        METH_NOARGS,
+                        pytun_tuntap_fileno_doc
+                },
+                {
+                        "persist",
+                        (PyCFunction) pytun_tuntap_persist,
+                        METH_VARARGS,
+                        pytun_tuntap_persist_doc
+                },
+#ifdef IFF_MULTI_QUEUE
+                {
+                 "mq_attach",
+                 (PyCFunction)pytun_tuntap_mq_attach,
+                 METH_VARARGS,
+                 pytun_tuntap_mq_attach_doc
+                },
+#endif
+                {NULL, NULL, 0, NULL}
+        };
+
+PyDoc_STRVAR(pytun_tuntap_doc,
+             "TunTapDevice(name='', flags=IFF_TUN, dev='/dev/net/tun') -> TUN/TAP device object.");
+
+static PyTypeObject pytun_tuntap_type =
+        {
+                PyVarObject_HEAD_INIT(&PyType_Type, 0)
+                .tp_name = "pytun.TunTapDevice",
+                .tp_basicsize = sizeof(pytun_tuntap_t),
+                .tp_dealloc = pytun_tuntap_dealloc,
+                .tp_flags = Py_TPFLAGS_DEFAULT,
+                .tp_doc = pytun_tuntap_doc,
+                .tp_methods = pytun_tuntap_meth,
+                .tp_getset = pytun_tuntap_prop,
+                .tp_new = pytun_tuntap_new
+        };
+
+#if PY_MAJOR_VERSION >= 3
+static struct PyModuleDef pytun_module =
+        {
+                .m_base = PyModuleDef_HEAD_INIT,
+                .m_name = "pytun",
+                .m_doc = NULL,
+                .m_size = -1,
+                .m_methods = NULL,
+#if PY_MINOR_VERSION <= 4
+                .m_reload = NULL,
+#else
+                .m_slots = NULL,
+#endif
+                .m_traverse = NULL,
+                .m_clear = NULL,
+                .m_free = NULL
+        };
+#endif
+
+#if PY_MAJOR_VERSION >= 3
+PyMODINIT_FUNC PyInit_pytun_pmd3(void)
+#else
+PyMODINIT_FUNC initpytun(void)
+#endif
+{
+    PyObject *m;
+    PyObject *pytun_error_dict = NULL;
+
+#if PY_MAJOR_VERSION >= 3
+    m = PyModule_Create(&pytun_module);
+#else
+    m = Py_InitModule(MODULE_NAME, NULL);
+#endif
+    if (m == NULL) {
+        goto error;
+    }
+
+    if (PyType_Ready(&pytun_tuntap_type) != 0) {
+        goto error;
+    }
+    Py_INCREF((PyObject *) &pytun_tuntap_type);
+    if (PyModule_AddObject(m, "TunTapDevice", (PyObject *) &pytun_tuntap_type) != 0) {
+        Py_DECREF((PyObject *) &pytun_tuntap_type);
+        goto error;
+    }
+
+    pytun_error_dict = Py_BuildValue("{ss}", "__doc__", pytun_error_doc);
+    if (pytun_error_dict == NULL) {
+        goto error;
+    }
+    pytun_error = PyErr_NewException("pytun.Error", PyExc_IOError, pytun_error_dict);
+    Py_DECREF(pytun_error_dict);
+    if (pytun_error == NULL) {
+        goto error;
+    }
+    Py_INCREF(pytun_error);
+    if (PyModule_AddObject(m, "Error", pytun_error) != 0) {
+        Py_DECREF(pytun_error);
+        goto error;
+    }
+
+    goto out;
+
+    error:
+#if PY_MAJOR_VERSION >= 3
+    Py_XDECREF(pytun_error);
+    Py_XDECREF(m);
+    pytun_error = NULL;
+    m = NULL;
+#endif
+
+    out:
+#if PY_MAJOR_VERSION >= 3
+    return m;
+#else
+    return;
+#endif
+}
+
```

### Comparing `pytun-pmd3-1.0.0/pyproject.toml` & `pytun-pmd3-2.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-[project]
-name = "pytun-pmd3"
-version = "1.0.0"
-description = "python-pytun fork with Darwin support (IPv6-ONLY)"
-readme = "README.md"
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
-keywords = ["tun", "tuntap", "darwin", "pymobiledevice3", "macos"]
-authors = [
-    { name = "doronz88", email = "doron88@gmail.com" }
-]
-maintainers = [
-    { name = "doronz88", email = "doron88@gmail.com" }
-]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-]
-
-[project.optional-dependencies]
-test = ["pytest"]
-
-[project.urls]
-"Homepage" = "https://github.com/doronz88/pytun-pmd3"
-"Bug Reports" = "https://github.com/doronz88/pytun-pmd3/issues"
-
-[tool.setuptools.packages.find]
-exclude = ["docs*", "tests*"]
-
-[build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+[project]
+name = "pytun-pmd3"
+version = "2.0.0"
+description = "python-pytun fork with darwin and windows support (IPv6-ONLY)"
+readme = "README.md"
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+keywords = ["tun", "tuntap", "darwin", "pymobiledevice3", "macos", "windows"]
+authors = [
+    { name = "doronz88", email = "doron88@gmail.com" }
+]
+maintainers = [
+    { name = "doronz88", email = "doron88@gmail.com" }
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3 :: Only",
+]
+
+[project.optional-dependencies]
+test = ["pytest"]
+
+[project.urls]
+"Homepage" = "https://github.com/doronz88/pytun-pmd3"
+"Bug Reports" = "https://github.com/doronz88/pytun-pmd3/issues"
+
+[tool.setuptools]
+package-data = { "pytun_pmd3" = ["wintun/**/*"] }
+
+[tool.setuptools.packages.find]
+exclude = ["docs*", "tests*"]
+
+[build-system]
+requires = ["setuptools>=43.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
```

### Comparing `pytun-pmd3-1.0.0/pytun_pmd3.egg-info/PKG-INFO` & `pytun-pmd3-2.0.0/pytun_pmd3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-Metadata-Version: 2.1
-Name: pytun-pmd3
-Version: 1.0.0
-Summary: python-pytun fork with Darwin support (IPv6-ONLY)
-Author-email: doronz88 <doron88@gmail.com>
-Maintainer-email: doronz88 <doron88@gmail.com>
-License: Copyright (c) 2011, montag451.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/doronz88/pytun-pmd3
-Project-URL: Bug Reports, https://github.com/doronz88/pytun-pmd3/issues
-Keywords: tun,tuntap,darwin,pymobiledevice3,macos
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-
-# Linux & Darwin TUN/TAP wrapper for Python
-
-This is a fork of https://github.com/montag451/pytun with partial Darwin support.
+Metadata-Version: 2.1
+Name: pytun-pmd3
+Version: 2.0.0
+Summary: python-pytun fork with darwin and windows support (IPv6-ONLY)
+Author-email: doronz88 <doron88@gmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>
+License: Copyright (c) 2011, montag451.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/doronz88/pytun-pmd3
+Project-URL: Bug Reports, https://github.com/doronz88/pytun-pmd3/issues
+Keywords: tun,tuntap,darwin,pymobiledevice3,macos,windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
+# Linux & Darwin TUN/TAP wrapper for Python
+
+This is a fork of https://github.com/montag451/pytun with partial Darwin support.
```

### Comparing `pytun-pmd3-1.0.0/pytun_pmd3.egg-info/SOURCES.txt` & `pytun-pmd3-2.0.0/pytun_pmd3.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -25,35 +25,63 @@
 .git/hooks/pre-receive.sample
 .git/hooks/prepare-commit-msg.sample
 .git/hooks/push-to-checkout.sample
 .git/hooks/sendemail-validate.sample
 .git/hooks/update.sample
 .git/info/exclude
 .git/logs/HEAD
-.git/objects/02/00fddf811408de6bdc77aef9891dc2bab56bf8
+.git/objects/00/17794f4638f1a1b4e469619a9824accac6ccea
+.git/objects/00/3f66a2318ebfb30afd90d8293b260cdd3d6999
 .git/objects/05/52d33a5e80692f9646b6dac657a43fa4011e82
-.git/objects/08/af5a317ee4183a167ef85805d1377f4c9b769c
 .git/objects/0b/87183182ca91979436d9e9965719d62cda4b12
-.git/objects/11/c56969531862430cb7b1f7229e3af67b4cd4a2
+.git/objects/14/ec9680550691c925edbd3a65f14a25062bb71f
+.git/objects/16/e6a680fefc2fc02952634fce616297c1725157
+.git/objects/2a/b97dba062208bcb6ffc32bef8347d586751038
 .git/objects/30/b9ae6f25de9828b7a1473270fe3154cbbb67f8
 .git/objects/33/b28167e71d9d18e42b1971392821ec70e38951
-.git/objects/60/2030c63bbc02e1a780aeec03f96cd9f1d8bc6f
-.git/objects/7f/ee09114efb25e74bcd7f31a42808b3316dc4ac
-.git/objects/a2/ce3543af4fd431390be37e3cb758d57d2eecfc
+.git/objects/34/0815e53a01e17a3d4682f7d020696fb3a587da
+.git/objects/48/2f0e082621cd6d9d699c4cdfa55ba322166de4
+.git/objects/4d/76d949a3568d0ff1d0f73fe6858f1dfe6af0a6
+.git/objects/51/caff11e470f0cfa91e2d07b67ccf52a285824e
+.git/objects/52/06f67ae5433525c632716e1e595eb02e6856ef
+.git/objects/55/d441f4a8017b2ea30eae55137c52f2829dba5f
+.git/objects/56/d9c426af16617a614e2e17ba6e01afe9b2c9c0
+.git/objects/5f/b524da018127adcf64a2ffa97bf9be86e9ecb2
+.git/objects/71/beb6065e5d841f0bb2b7a1d0be99436fe906d4
+.git/objects/7f/f8524670c0aed9f1a4439279b78a5e7c137f6f
+.git/objects/81/7d73b0ac42a4dfc956fd81fd9e130a4ab61aaa
+.git/objects/8c/2ddee41aa1c6951653ee252434a2e862bb63e0
+.git/objects/8d/e62c37cc8fcf845ecd68838240936924cf9906
+.git/objects/a9/de0cc5100692d182a38a2e85ee739bdd771c7a
+.git/objects/ae/e04e77bfbd6601adbcd5a46435f059e31cf6e4
 .git/objects/af/348689d62b32e0021ab0d82c0f8fc156db4728
+.git/objects/b4/9ac67e351cffd016971fe56eb32564da10b8da
 .git/objects/b5/77e4de768ad66f0d36c258491c30b8f89d64a0
-.git/objects/cb/ee9104a0e8a07d0057461d2df7146a3bd0caa5
-.git/objects/d6/1acd60de2ec118aec5492b69c819b478578270
-.git/objects/d6/5be742be8e767a356248138ad23c056c76f275
-.git/objects/da/28e16ce09d713ce3c49ab1d3d04d3523741c2d
-.git/objects/dd/494ae1faa46494e15a7c1a16febb5f8343d063
+.git/objects/bc/8d3f0e60565567a8b8598972614dce7d4ffccd
+.git/objects/c0/ba173809fe5ff5902ff791514796bd6f528b26
+.git/objects/c5/8a3c8a6e3b698ea353d97545c477154a0d3e0b
+.git/objects/c8/3faddaf014ad1dc356006dd9dc2b527680d57a
+.git/objects/c9/13b6a346e1e791c8d0906140900f694f417c60
+.git/objects/d4/cb4438b5bf15e244a6c5873db243ab511cac0b
+.git/objects/dc/4e4aeeb1400f75fa40bfd4d2503a029c03c52c
 .git/objects/ee/54e24d12d7011cc1db7211d542f2c2a14bad07
-.git/refs/tags/v1.0.0
-.github/workflows/build.yml
-.github/workflows/python-publish.yml
+.git/objects/f4/2f5d6747f39938e3b2cf67d0dce66b54b1dc73
+.git/refs/tags/v2.0.0
+.github/workflows/python-publish-macos-and-linux.yml
+.github/workflows/python-publish-windows.yml
+pytun_pmd3/__init__.py
+pytun_pmd3/exceptions.py
+pytun_pmd3/wintun.py
 pytun_pmd3.egg-info/PKG-INFO
 pytun_pmd3.egg-info/SOURCES.txt
 pytun_pmd3.egg-info/dependency_links.txt
 pytun_pmd3.egg-info/requires.txt
 pytun_pmd3.egg-info/top_level.txt
+pytun_pmd3/wintun/LICENSE.txt
+pytun_pmd3/wintun/README.md
+pytun_pmd3/wintun/bin/amd64/wintun.dll
+pytun_pmd3/wintun/bin/arm/wintun.dll
+pytun_pmd3/wintun/bin/arm64/wintun.dll
+pytun_pmd3/wintun/bin/x86/wintun.dll
+pytun_pmd3/wintun/include/wintun.h
 test/test_tap.py
 test/test_tun.py
```

### Comparing `pytun-pmd3-1.0.0/test/test_tap.py` & `pytun-pmd3-2.0.0/test/test_tap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,89 @@
-import sys
-import optparse
-import socket
-import select
-import errno
-import pytun
-
-class TunnelServer(object):
-
-    def __init__(self, taddr, tmask, tmtu, laddr, lport, raddr, rport):
-        self._tap = pytun.TunTapDevice(flags=pytun.IFF_TAP|pytun.IFF_NO_PI)
-        self._tap.addr = taddr
-        self._tap.netmask = tmask
-        self._tap.mtu = tmtu
-        self._tap.up()
-        self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self._sock.bind((laddr, lport))
-        self._raddr = raddr
-        self._rport = rport
-
-    def run(self):
-        mtu = self._tap.mtu
-        r = [self._tap, self._sock]; w = []; x = []
-        to_tap = ''
-        to_sock = ''
-        while True:
-            try:
-                r, w, x = select.select(r, w, x)
-                if self._tap in r:
-                    to_sock = self._tap.read(mtu)
-                if self._sock in r:
-                    to_tap, addr = self._sock.recvfrom(65535)
-                    if addr[0] != self._raddr or addr[1] != self._rport:
-                        to_tap = '' # drop packet
-                if self._tap in w:
-                    self._tap.write(to_tap)
-                    to_tap = ''
-                if self._sock in w:
-                    self._sock.sendto(to_sock, (self._raddr, self._rport))
-                    to_sock = ''
-                r = []; w = []
-                if to_tap:
-                    w.append(self._tap)
-                else:
-                    r.append(self._sock)
-                if to_sock:
-                    w.append(self._sock)
-                else:
-                    r.append(self._tap)
-            except (select.error, socket.error, pytun.Error), e:
-                if e[0] == errno.EINTR:
-                    continue
-                print >> sys.stderr, str(e)
-                break
-
-def main():
-    parser = optparse.OptionParser()
-    parser.add_option('--tap-addr', dest='taddr',
-            help='set tunnel local address')
-    parser.add_option('--tap-netmask', default='255.255.255.0',dest='tmask',
-            help='set tunnel netmask')
-    parser.add_option('--tap-mtu', type='int', default=1500,dest='tmtu',
-            help='set tunnel MTU')
-    parser.add_option('--local-addr', default='0.0.0.0', dest='laddr',
-            help='set local address [%default]')
-    parser.add_option('--local-port', type='int', default=12000, dest='lport',
-            help='set local port [%default]')
-    parser.add_option('--remote-addr', dest='raddr',
-            help='set remote address')
-    parser.add_option('--remote-port', type='int', dest='rport',
-            help='set remote port')
-    opt, args = parser.parse_args()
-    if not (opt.taddr and opt.raddr and opt.rport):
-        parser.print_help()
-        return 1
-    try:
-        server = TunnelServer(opt.taddr, opt.tmask, opt.tmtu, opt.laddr,
-                opt.lport, opt.raddr, opt.rport)
-    except (pytun.Error, socket.error), e:
-        print >> sys.stderr, str(e)
-        return 1
-    server.run()
-    return 0
-
-if __name__ == '__main__':
-    sys.exit(main())
-
+import errno
+import optparse
+import select
+import socket
+import sys
+
+import pytun
+
+
+class TunnelServer(object):
+
+    def __init__(self, taddr, tmask, tmtu, laddr, lport, raddr, rport):
+        self._tap = pytun.TunTapDevice(flags=pytun.IFF_TAP|pytun.IFF_NO_PI)
+        self._tap.addr = taddr
+        self._tap.netmask = tmask
+        self._tap.mtu = tmtu
+        self._tap.up()
+        self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self._sock.bind((laddr, lport))
+        self._raddr = raddr
+        self._rport = rport
+
+    def run(self):
+        mtu = self._tap.mtu
+        r = [self._tap, self._sock]; w = []; x = []
+        to_tap = ''
+        to_sock = ''
+        while True:
+            try:
+                r, w, x = select.select(r, w, x)
+                if self._tap in r:
+                    to_sock = self._tap.read(mtu)
+                if self._sock in r:
+                    to_tap, addr = self._sock.recvfrom(65535)
+                    if addr[0] != self._raddr or addr[1] != self._rport:
+                        to_tap = '' # drop packet
+                if self._tap in w:
+                    self._tap.write(to_tap)
+                    to_tap = ''
+                if self._sock in w:
+                    self._sock.sendto(to_sock, (self._raddr, self._rport))
+                    to_sock = ''
+                r = []; w = []
+                if to_tap:
+                    w.append(self._tap)
+                else:
+                    r.append(self._sock)
+                if to_sock:
+                    w.append(self._sock)
+                else:
+                    r.append(self._tap)
+            except (select.error, socket.error, pytun.Error), e:
+                if e[0] == errno.EINTR:
+                    continue
+                print >> sys.stderr, str(e)
+                break
+
+def main():
+    parser = optparse.OptionParser()
+    parser.add_option('--tap-addr', dest='taddr',
+            help='set tunnel local address')
+    parser.add_option('--tap-netmask', default='255.255.255.0',dest='tmask',
+            help='set tunnel netmask')
+    parser.add_option('--tap-mtu', type='int', default=1500,dest='tmtu',
+            help='set tunnel MTU')
+    parser.add_option('--local-addr', default='0.0.0.0', dest='laddr',
+            help='set local address [%default]')
+    parser.add_option('--local-port', type='int', default=12000, dest='lport',
+            help='set local port [%default]')
+    parser.add_option('--remote-addr', dest='raddr',
+            help='set remote address')
+    parser.add_option('--remote-port', type='int', dest='rport',
+            help='set remote port')
+    opt, args = parser.parse_args()
+    if not (opt.taddr and opt.raddr and opt.rport):
+        parser.print_help()
+        return 1
+    try:
+        server = TunnelServer(opt.taddr, opt.tmask, opt.tmtu, opt.laddr,
+                opt.lport, opt.raddr, opt.rport)
+    except (pytun.Error, socket.error), e:
+        print >> sys.stderr, str(e)
+        return 1
+    server.run()
+    return 0
+
+if __name__ == '__main__':
+    sys.exit(main())
+
```

### Comparing `pytun-pmd3-1.0.0/test/test_tun.py` & `pytun-pmd3-2.0.0/test/test_tun.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,92 @@
-import sys
-import optparse
-import socket
-import select
-import errno
-import pytun
-
-class TunnelServer(object):
-
-    def __init__(self, taddr, tdstaddr, tmask, tmtu, laddr, lport, raddr, rport):
-        self._tun = pytun.TunTapDevice(flags=pytun.IFF_TUN|pytun.IFF_NO_PI)
-        self._tun.addr = taddr
-        self._tun.dstaddr = tdstaddr
-        self._tun.netmask = tmask
-        self._tun.mtu = tmtu
-        self._tun.up()
-        self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self._sock.bind((laddr, lport))
-        self._raddr = raddr
-        self._rport = rport
-
-    def run(self):
-        mtu = self._tun.mtu
-        r = [self._tun, self._sock]; w = []; x = []
-        to_tun = ''
-        to_sock = ''
-        while True:
-            try:
-                r, w, x = select.select(r, w, x)
-                if self._tun in r:
-                    to_sock = self._tun.read(mtu)
-                if self._sock in r:
-                    to_tun, addr = self._sock.recvfrom(65535)
-                    if addr[0] != self._raddr or addr[1] != self._rport:
-                        to_tun = '' # drop packet
-                if self._tun in w:
-                    self._tun.write(to_tun)
-                    to_tun = ''
-                if self._sock in w:
-                    self._sock.sendto(to_sock, (self._raddr, self._rport))
-                    to_sock = ''
-                r = []; w = []
-                if to_tun:
-                    w.append(self._tun)
-                else:
-                    r.append(self._sock)
-                if to_sock:
-                    w.append(self._sock)
-                else:
-                    r.append(self._tun)
-            except (select.error, socket.error, pytun.Error), e:
-                if e[0] == errno.EINTR:
-                    continue
-                print >> sys.stderr, str(e)
-                break
-
-def main():
-    parser = optparse.OptionParser()
-    parser.add_option('--tun-addr', dest='taddr',
-            help='set tunnel local address')
-    parser.add_option('--tun-dstaddr', dest='tdstaddr',
-            help='set tunnel destination address')
-    parser.add_option('--tun-netmask', default='255.255.255.0',dest='tmask',
-            help='set tunnel netmask')
-    parser.add_option('--tun-mtu', type='int', default=1500,dest='tmtu',
-            help='set tunnel MTU')
-    parser.add_option('--local-addr', default='0.0.0.0', dest='laddr',
-            help='set local address [%default]')
-    parser.add_option('--local-port', type='int', default=12000, dest='lport',
-            help='set local port [%default]')
-    parser.add_option('--remote-addr', dest='raddr',
-            help='set remote address')
-    parser.add_option('--remote-port', type='int', dest='rport',
-            help='set remote port')
-    opt, args = parser.parse_args()
-    if not (opt.taddr and opt.tdstaddr and opt.raddr and opt.rport):
-        parser.print_help()
-        return 1
-    try:
-        server = TunnelServer(opt.taddr, opt.tdstaddr, opt.tmask, opt.tmtu,
-                opt.laddr, opt.lport, opt.raddr, opt.rport)
-    except (pytun.Error, socket.error), e:
-        print >> sys.stderr, str(e)
-        return 1
-    server.run()
-    return 0
-
-if __name__ == '__main__':
-    sys.exit(main())
-
+import errno
+import optparse
+import select
+import socket
+import sys
+
+import pytun
+
+
+class TunnelServer(object):
+
+    def __init__(self, taddr, tdstaddr, tmask, tmtu, laddr, lport, raddr, rport):
+        self._tun = pytun.TunTapDevice(flags=pytun.IFF_TUN|pytun.IFF_NO_PI)
+        self._tun.addr = taddr
+        self._tun.dstaddr = tdstaddr
+        self._tun.netmask = tmask
+        self._tun.mtu = tmtu
+        self._tun.up()
+        self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self._sock.bind((laddr, lport))
+        self._raddr = raddr
+        self._rport = rport
+
+    def run(self):
+        mtu = self._tun.mtu
+        r = [self._tun, self._sock]; w = []; x = []
+        to_tun = ''
+        to_sock = ''
+        while True:
+            try:
+                r, w, x = select.select(r, w, x)
+                if self._tun in r:
+                    to_sock = self._tun.read(mtu)
+                if self._sock in r:
+                    to_tun, addr = self._sock.recvfrom(65535)
+                    if addr[0] != self._raddr or addr[1] != self._rport:
+                        to_tun = '' # drop packet
+                if self._tun in w:
+                    self._tun.write(to_tun)
+                    to_tun = ''
+                if self._sock in w:
+                    self._sock.sendto(to_sock, (self._raddr, self._rport))
+                    to_sock = ''
+                r = []; w = []
+                if to_tun:
+                    w.append(self._tun)
+                else:
+                    r.append(self._sock)
+                if to_sock:
+                    w.append(self._sock)
+                else:
+                    r.append(self._tun)
+            except (select.error, socket.error, pytun.Error), e:
+                if e[0] == errno.EINTR:
+                    continue
+                print >> sys.stderr, str(e)
+                break
+
+def main():
+    parser = optparse.OptionParser()
+    parser.add_option('--tun-addr', dest='taddr',
+            help='set tunnel local address')
+    parser.add_option('--tun-dstaddr', dest='tdstaddr',
+            help='set tunnel destination address')
+    parser.add_option('--tun-netmask', default='255.255.255.0',dest='tmask',
+            help='set tunnel netmask')
+    parser.add_option('--tun-mtu', type='int', default=1500,dest='tmtu',
+            help='set tunnel MTU')
+    parser.add_option('--local-addr', default='0.0.0.0', dest='laddr',
+            help='set local address [%default]')
+    parser.add_option('--local-port', type='int', default=12000, dest='lport',
+            help='set local port [%default]')
+    parser.add_option('--remote-addr', dest='raddr',
+            help='set remote address')
+    parser.add_option('--remote-port', type='int', dest='rport',
+            help='set remote port')
+    opt, args = parser.parse_args()
+    if not (opt.taddr and opt.tdstaddr and opt.raddr and opt.rport):
+        parser.print_help()
+        return 1
+    try:
+        server = TunnelServer(opt.taddr, opt.tdstaddr, opt.tmask, opt.tmtu,
+                opt.laddr, opt.lport, opt.raddr, opt.rport)
+    except (pytun.Error, socket.error), e:
+        print >> sys.stderr, str(e)
+        return 1
+    server.run()
+    return 0
+
+if __name__ == '__main__':
+    sys.exit(main())
+
```

