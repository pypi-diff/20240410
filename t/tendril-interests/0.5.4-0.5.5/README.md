# Comparing `tmp/tendril-interests-0.5.4.tar.gz` & `tmp/tendril-interests-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-interests-0.5.4.tar", last modified: Mon Apr  1 10:19:21 2024, max compression
+gzip compressed data, was "tendril-interests-0.5.5.tar", last modified: Wed Apr 10 18:38:49 2024, max compression
```

## Comparing `tendril-interests-0.5.4.tar` & `tendril-interests-0.5.5.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.631064 tendril-interests-0.5.4/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.5.4/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3549 2023-09-02 16:30:49.000000 tendril-interests-0.5.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.631064 tendril-interests-0.5.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.5.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.5.4/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.5.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21600 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.5.4/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.5.4/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.5.4/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.5.4/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.5.4/src/tendril/authz/roles/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril-interests-0.5.4/src/tendril/authz/roles/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.5.4/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.5.4/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.5.4/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.635064 tendril-interests-0.5.4/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.5.4/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.5.4/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.5.4/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.5.4/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril-interests-0.5.4/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.5.4/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.5.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril-interests-0.5.4/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 21:22:37.000000 tendril-interests-0.5.4/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      361 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/core/topology/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.5.4/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.5.4/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril-interests-0.5.4/src/tendril/db/controllers/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril-interests-0.5.4/src/tendril/db/controllers/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.5.4/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.5.4/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.5.4/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril-interests-0.5.4/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.5.4/src/tendril/db/models/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril-interests-0.5.4/src/tendril/db/models/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.5.4/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril-interests-0.5.4/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8294 2024-03-27 02:50:01.000000 tendril-interests-0.5.4/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-03-24 22:21:57.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/export.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-03-26 04:23:43.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/localizers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20183 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril-interests-0.5.4/src/tendril/interests/mixins/policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.5.4/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.5.4/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5996 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.639064 tendril-interests-0.5.4/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.5.4/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.5.4/src/tendril/libraries/mixins/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril-interests-0.5.4/src/tendril/libraries/mixins/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril-interests-0.5.4/src/tendril/libraries/mixins/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.5.4/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril-interests-0.5.4/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/src/tendril/policies/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril-interests-0.5.4/src/tendril/policies/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril-interests-0.5.4/src/tendril/policies/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril-interests-0.5.4/src/tendril/policies/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2024-04-01 10:19:21.000000 tendril-interests-0.5.4/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3228 2024-04-01 10:19:21.000000 tendril-interests-0.5.4/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-01 10:19:21.000000 tendril-interests-0.5.4/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      703 2024-04-01 10:19:21.000000 tendril-interests-0.5.4/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-01 10:19:21.000000 tendril-interests-0.5.4/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-01 10:19:21.643064 tendril-interests-0.5.4/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.5.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.967794 tendril-interests-0.5.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2024-04-10 18:38:49.967794 tendril-interests-0.5.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.5.5/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-10 18:38:49.967794 tendril-interests-0.5.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3582 2024-04-09 19:31:13.000000 tendril-interests-0.5.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.939795 tendril-interests-0.5.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.943795 tendril-interests-0.5.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.5.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.947795 tendril-interests-0.5.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.5.5/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.947795 tendril-interests-0.5.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.5.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.947795 tendril-interests-0.5.5/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21600 2024-04-05 09:10:59.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1552 2024-04-09 22:17:28.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.947795 tendril-interests-0.5.5/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.5.5/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.951795 tendril-interests-0.5.5/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.5.5/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.5.5/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.951795 tendril-interests-0.5.5/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.5.5/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.5.5/src/tendril/authz/roles/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril-interests-0.5.5/src/tendril/authz/roles/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.951795 tendril-interests-0.5.5/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.5.5/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.5.5/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.951795 tendril-interests-0.5.5/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.5.5/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.951795 tendril-interests-0.5.5/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.5.5/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.5.5/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.5.5/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.5.5/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril-interests-0.5.5/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.5.5/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.5.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril-interests-0.5.5/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril-interests-0.5.5/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      361 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/core/topology/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.5.5/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.5.5/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril-interests-0.5.5/src/tendril/db/controllers/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril-interests-0.5.5/src/tendril/db/controllers/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.955795 tendril-interests-0.5.5/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.5.5/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.5.5/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.959794 tendril-interests-0.5.5/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.5.5/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril-interests-0.5.5/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.5.5/src/tendril/db/models/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril-interests-0.5.5/src/tendril/db/models/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.959794 tendril-interests-0.5.5/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.5.5/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril-interests-0.5.5/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8294 2024-03-27 02:50:01.000000 tendril-interests-0.5.5/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.959794 tendril-interests-0.5.5/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-04-05 09:10:45.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/export.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-10 17:57:57.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-04-05 09:09:51.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/localizers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20183 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril-interests-0.5.5/src/tendril/interests/mixins/policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.959794 tendril-interests-0.5.5/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.5.5/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.963794 tendril-interests-0.5.5/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.5.5/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5996 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.963794 tendril-interests-0.5.5/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.5.5/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.5.5/src/tendril/libraries/mixins/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2024-04-09 21:11:30.000000 tendril-interests-0.5.5/src/tendril/libraries/mixins/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril-interests-0.5.5/src/tendril/libraries/mixins/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril-interests-0.5.5/src/tendril/libraries/mixins/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.963794 tendril-interests-0.5.5/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.5.5/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril-interests-0.5.5/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.963794 tendril-interests-0.5.5/src/tendril/policies/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril-interests-0.5.5/src/tendril/policies/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril-interests-0.5.5/src/tendril/policies/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril-interests-0.5.5/src/tendril/policies/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.967794 tendril-interests-0.5.5/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2024-04-10 18:38:49.000000 tendril-interests-0.5.5/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3368 2024-04-10 18:38:49.000000 tendril-interests-0.5.5/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-10 18:38:49.000000 tendril-interests-0.5.5/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      729 2024-04-10 18:38:49.000000 tendril-interests-0.5.5/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-10 18:38:49.000000 tendril-interests-0.5.5/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:38:49.967794 tendril-interests-0.5.5/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.5.5/tox.ini
```

### Comparing `tendril-interests-0.5.4/.gitignore` & `tendril-interests-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/.readthedocs.yml` & `tendril-interests-0.5.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/.travis.yml` & `tendril-interests-0.5.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/LICENSE` & `tendril-interests-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/PKG-INFO` & `tendril-interests-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.5.4
+Version: 0.5.5
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.5.4/README.rst` & `tendril-interests-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/Makefile` & `tendril-interests-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/_static/custom.css` & `tendril-interests-0.5.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/_static/favicon.ico` & `tendril-interests-0.5.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/_static/logo.png` & `tendril-interests-0.5.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/_static/logo_packed.png` & `tendril-interests-0.5.5/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/_templates/about.html` & `tendril-interests-0.5.5/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/conf.py` & `tendril-interests-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/index.rst` & `tendril-interests-0.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/docs/installation.rst` & `tendril-interests-0.5.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/setup.py` & `tendril-interests-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     'makefun',
     'asgiref',
     'inflection',
     'deepdiff[optimize]',
     'tendril-utils-types',
     'tendril-connector-rabbitmq',
     'tendril-connector-influxdb',
+    'tendril-connector-grafana',
     'tendril-apiserver-core',  # Need this because of HTTPCodedException import which are otherwise unused. Cleanup instead.
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
```

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.5.5/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/templates/base.py` & `tendril-interests-0.5.5/src/tendril/apiserver/templates/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.5.5/src/tendril/apiserver/templates/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_approvals.py` & `tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_monitors.py` & `tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_monitors.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/apiserver/templates/interests_policies.py` & `tendril-interests-0.5.5/src/tendril/apiserver/templates/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/authz/approvals/interests.py` & `tendril-interests-0.5.5/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/authz/approvals/manager.py` & `tendril-interests-0.5.5/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/authz/roles/interests.py` & `tendril-interests-0.5.5/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/authz/roles/interests_approvals.py` & `tendril-interests-0.5.5/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/common/interests/approvals.py` & `tendril-interests-0.5.5/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.5.5/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/common/interests/memberships.py` & `tendril-interests-0.5.5/src/tendril/common/interests/memberships.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/config/__init__.py` & `tendril-interests-0.5.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/config/interests.py` & `tendril-interests-0.5.5/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/controllers/interests.py` & `tendril-interests-0.5.5/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/controllers/interests_approvals.py` & `tendril-interests-0.5.5/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/controllers/interests_policies.py` & `tendril-interests-0.5.5/src/tendril/db/controllers/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/models/interests.py` & `tendril-interests-0.5.5/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/models/interests_approvals.py` & `tendril-interests-0.5.5/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/db/models/interests_policies.py` & `tendril-interests-0.5.5/src/tendril/db/models/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/base.py` & `tendril-interests-0.5.5/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/manager.py` & `tendril-interests-0.5.5/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/mixins/approvals.py` & `tendril-interests-0.5.5/src/tendril/interests/mixins/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/mixins/export.py` & `tendril-interests-0.5.5/src/tendril/interests/mixins/export.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/mixins/localizers.py` & `tendril-interests-0.5.5/src/tendril/interests/mixins/localizers.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/mixins/monitors.py` & `tendril-interests-0.5.5/src/tendril/interests/mixins/monitors.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/interests/mixins/policies.py` & `tendril-interests-0.5.5/src/tendril/interests/mixins/policies.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/libraries/interests/base.py` & `tendril-interests-0.5.5/src/tendril/libraries/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.5.5/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/monitors/spec.py` & `tendril-interests-0.5.5/src/tendril/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/policies/base.py` & `tendril-interests-0.5.5/src/tendril/policies/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril/policies/manager.py` & `tendril-interests-0.5.5/src/tendril/policies/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.5.5/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.5.4
+Version: 0.5.5
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.5.4/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.5.5/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/interests.py
 src/tendril/apiserver/templates/__init__.py
 src/tendril/apiserver/templates/base.py
 src/tendril/apiserver/templates/interests.py
 src/tendril/apiserver/templates/interests_approvals.py
+src/tendril/apiserver/templates/interests_graphs.py
 src/tendril/apiserver/templates/interests_monitors.py
 src/tendril/apiserver/templates/interests_policies.py
 src/tendril/authz/__init__.py
 src/tendril/authz/approvals/__init__.py
 src/tendril/authz/approvals/interests.py
 src/tendril/authz/approvals/manager.py
 src/tendril/authz/roles/__init__.py
@@ -66,23 +67,25 @@
 src/tendril/interests/__init__.py
 src/tendril/interests/base.py
 src/tendril/interests/manager.py
 src/tendril/interests/mixins/__init__.py
 src/tendril/interests/mixins/approvals.py
 src/tendril/interests/mixins/base.py
 src/tendril/interests/mixins/export.py
+src/tendril/interests/mixins/graphs.py
 src/tendril/interests/mixins/localizers.py
 src/tendril/interests/mixins/monitors.py
 src/tendril/interests/mixins/policies.py
 src/tendril/libraries/__init__.py
 src/tendril/libraries/interests/__init__.py
 src/tendril/libraries/interests/base.py
 src/tendril/libraries/interests/manager.py
 src/tendril/libraries/mixins/__init__.py
 src/tendril/libraries/mixins/interests_approvals.py
+src/tendril/libraries/mixins/interests_graphs.py
 src/tendril/libraries/mixins/interests_monitors.py
 src/tendril/libraries/mixins/interests_policies.py
 src/tendril/monitors/__init__.py
 src/tendril/monitors/spec.py
 src/tendril/policies/__init__.py
 src/tendril/policies/base.py
 src/tendril/policies/manager.py
```

### Comparing `tendril-interests-0.5.4/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.5.5/src/tendril_interests.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 makefun
 asgiref
 inflection
 deepdiff[optimize]
 tendril-utils-types
 tendril-connector-rabbitmq
 tendril-connector-influxdb
+tendril-connector-grafana
 tendril-apiserver-core
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
```

### Comparing `tendril-interests-0.5.4/tests/coveralls.py` & `tendril-interests-0.5.5/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.5.4/tox.ini` & `tendril-interests-0.5.5/tox.ini`

 * *Files identical despite different names*
