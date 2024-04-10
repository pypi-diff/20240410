# Comparing `tmp/weni_rp_apps-2.8.0a6.tar.gz` & `tmp/weni_rp_apps-2.8.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.8.0a6.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.8.0a7.tar", max compression
```

## Comparing `weni_rp_apps-2.8.0a6.tar` & `weni_rp_apps-2.8.0a7.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0      646 2024-04-08 15:32:17.119150 weni_rp_apps-2.8.0a6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a6/weni/activities/__init__.py
--rw-r--r--   0        0        0      245 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a6/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a6/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     2525 2024-04-08 15:28:34.683585 weni_rp_apps-2.8.0a6/weni/activities/signals.py
--rw-r--r--   0        0        0      325 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      371 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.0a6/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     9067 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.0a6/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/auth/apps.py
--rw-r--r--   0        0        0     1327 2024-03-13 14:14:33.907599 weni_rp_apps-2.8.0a6/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2024-02-02 22:05:28.147811 weni_rp_apps-2.8.0a6/weni/auth/decorators.py
--rw-r--r--   0        0        0      810 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      347 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2063 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11364 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a6/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4070 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4081 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7987 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1356 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1174 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6493 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1588 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a6/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      680 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2764 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2836 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     4020 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9821 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3132 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3916 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10076 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a6/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/backends.py
--rw-r--r--   0        0        0     5484 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16305 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a6/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      394 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     8711 2023-11-09 13:18:30.163158 weni_rp_apps-2.8.0a6/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1527 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8626 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      318 2023-09-25 18:26:36.872113 weni_rp_apps-2.8.0a6/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     2803 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      113 2024-03-08 15:16:47.101420 weni_rp_apps-2.8.0a6/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2024-01-16 13:08:31.627802 weni_rp_apps-2.8.0a6/weni/internal/clients/base.py
--rw-r--r--   0        0        0     1108 2024-03-08 15:16:51.401431 weni_rp_apps-2.8.0a6/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     2476 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      546 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     4243 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1460 2024-04-08 15:29:20.755225 weni_rp_apps-2.8.0a6/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4436 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a6/weni/internal/flows/urls.py
--rw-r--r--   0        0        0     1838 2024-04-08 15:29:30.565258 weni_rp_apps-2.8.0a6/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1484 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/globals/views.py
--rw-r--r--   0        0        0     1247 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      916 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/models.py
--rw-r--r--   0        0        0     4281 2023-11-22 18:45:11.406539 weni_rp_apps-2.8.0a6/weni/internal/msgs/## Índice.md
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/msgs/__init__.py
--rw-r--r--   0        0        0     4814 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/msgs/tasks.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/msgs/tests/tests.py
--rw-r--r--   0        0        0      259 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/msgs/urls.py
--rw-r--r--   0        0        0     2995 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a6/weni/internal/msgs/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     4275 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a6/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    16862 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a6/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a6/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     5863 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a6/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/internal/permissions.py
--rw-r--r--   0        0        0     2164 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a6/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0     1007 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/statistic/views.py
--rw-r--r--   0        0        0       67 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/tasks.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1150 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a6/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3360 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      521 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.0a6/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     2385 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.0a6/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1417 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    12563 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5849 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a6/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-04-13 12:17:16.348555 weni_rp_apps-2.8.0a6/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/s3/apps.py
--rw-r--r--   0        0        0      219 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/s3/views.py
--rw-r--r--   0        0        0       93 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2791 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/business.py
--rw-r--r--   0        0        0      619 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     3354 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2770 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/template_message/apps.py
--rw-r--r--   0        0        0     2040 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5292 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/templates/__init__.py
--rw-r--r--   0        0        0      545 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a6/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a6/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a6/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.8.0a6/PKG-INFO
+-rw-r--r--   0        0        0      646 2024-04-09 20:04:11.701334 weni_rp_apps-2.8.0a7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a7/weni/activities/__init__.py
+-rw-r--r--   0        0        0      245 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a7/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.0a7/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     3010 2024-04-09 19:59:48.835629 weni_rp_apps-2.8.0a7/weni/activities/signals.py
+-rw-r--r--   0        0        0      325 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      371 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.0a7/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     9067 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.0a7/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/auth/apps.py
+-rw-r--r--   0        0        0     1327 2024-03-13 14:14:33.907599 weni_rp_apps-2.8.0a7/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2024-02-02 22:05:28.147811 weni_rp_apps-2.8.0a7/weni/auth/decorators.py
+-rw-r--r--   0        0        0      810 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      347 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2063 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11364 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.0a7/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4070 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4081 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7987 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1356 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1174 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6493 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.0a7/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      680 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2764 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2836 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     4020 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9821 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3132 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3916 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10076 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.0a7/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/backends.py
+-rw-r--r--   0        0        0     5484 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16305 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.0a7/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      394 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     8711 2023-11-09 13:18:30.163158 weni_rp_apps-2.8.0a7/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1527 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8626 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      318 2023-09-25 18:26:36.872113 weni_rp_apps-2.8.0a7/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     2803 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      113 2024-03-08 15:16:47.101420 weni_rp_apps-2.8.0a7/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2024-01-16 13:08:31.627802 weni_rp_apps-2.8.0a7/weni/internal/clients/base.py
+-rw-r--r--   0        0        0     1108 2024-03-08 15:16:51.401431 weni_rp_apps-2.8.0a7/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     2476 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      546 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     4243 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1460 2024-04-09 19:52:24.783528 weni_rp_apps-2.8.0a7/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4436 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a7/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0     1838 2024-04-09 19:52:24.783528 weni_rp_apps-2.8.0a7/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1484 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/globals/views.py
+-rw-r--r--   0        0        0     1247 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/models.py
+-rw-r--r--   0        0        0     4281 2023-11-22 18:45:11.406539 weni_rp_apps-2.8.0a7/weni/internal/msgs/## Índice.md
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/msgs/__init__.py
+-rw-r--r--   0        0        0     4814 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/msgs/tasks.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/msgs/tests/tests.py
+-rw-r--r--   0        0        0      259 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/msgs/urls.py
+-rw-r--r--   0        0        0     2995 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.0a7/weni/internal/msgs/views.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     4275 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a7/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    16862 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a7/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a7/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     5863 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.0a7/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/internal/permissions.py
+-rw-r--r--   0        0        0     2164 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a7/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0     1007 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0       67 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/tasks.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.0a7/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3360 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      521 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.0a7/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     2385 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.0a7/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1417 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    12563 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5849 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.0a7/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-04-13 12:17:16.348555 weni_rp_apps-2.8.0a7/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/s3/apps.py
+-rw-r--r--   0        0        0      219 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/s3/views.py
+-rw-r--r--   0        0        0       93 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2791 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      619 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2770 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2040 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5292 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/templates/__init__.py
+-rw-r--r--   0        0        0      545 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.0a7/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.0a7/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.0a7/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.8.0a7/PKG-INFO
```

### Comparing `weni_rp_apps-2.8.0a6/pyproject.toml` & `weni_rp_apps-2.8.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.8.0a6"
+version = "2.8.0a7"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.8.0a6/weni/activities/signals.py` & `weni_rp_apps-2.8.0a7/weni/activities/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,36 +6,45 @@
 from temba.flows.models import Flow
 from temba.triggers.models import Trigger
 from temba.campaigns.models import Campaign
 from temba.event_driven.publisher.rabbitmq_publisher import RabbitmqPublisher
 
 
 def create_recent_activity(instance: models.Model, created: bool, delete=None):
-    routing_key = ""
     if instance.is_active:
+        rabbitmq_publisher = RabbitmqPublisher()
         if delete:
             action = "DELETE"
-            routing_key = "flow-delete"
-        else:
-            action = "CREATE" if created else "UPDATE"
-        rabbitmq_publisher = RabbitmqPublisher()
-        rabbitmq_publisher.send_message(
+            rabbitmq_publisher.send_message(
             body=dict(
                 action=action,
                 entity=instance.__class__.__name__.upper(),
                 entity_name=getattr(instance, "name", None),
                 entity_uuid=str(instance.uuid),
                 project_uuid=str(instance.org.project.project_uuid),
                 user=instance.modified_by.email,
                 flow_organization=str(instance.org.uuid),
             ),
             exchange="recent-activities.topic",
-            routing_key=routing_key,
+            routing_key="flow-delete",
         )
-
+        else:
+            action = "CREATE" if created else "UPDATE"
+            rabbitmq_publisher.send_message(
+                body=dict(
+                    action=action,
+                    entity=instance.__class__.__name__.upper(),
+                    entity_name=getattr(instance, "name", None),
+                    project_uuid=str(instance.org.project.project_uuid),
+                    user=instance.modified_by.email,
+                    flow_organization=str(instance.org.uuid),
+                ),
+                exchange="recent-activities.topic",
+                routing_key="",
+            )
 
 @receiver(post_save, sender=Channel)
 def channel_recent_activity_signal(sender, instance: Channel, created: bool, **kwargs):
     update_fields = kwargs.get("update_fields")
     if instance.channel_type not in ["WA", "WAC"] or update_fields != frozenset(
         {
             "config",
```

### Comparing `weni_rp_apps-2.8.0a6/weni/analytics_api/tests.py` & `weni_rp_apps-2.8.0a7/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/analytics_api/views.py` & `weni_rp_apps-2.8.0a7/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/auth/backends.py` & `weni_rp_apps-2.8.0a7/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/auth/urls.py` & `weni_rp_apps-2.8.0a7/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/auth/views.py` & `weni_rp_apps-2.8.0a7/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/channel_stats/serializers.py` & `weni_rp_apps-2.8.0a7/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/channel_stats/views.py` & `weni_rp_apps-2.8.0a7/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/billing/queries.py` & `weni_rp_apps-2.8.0a7/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/billing/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/billing/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/channel/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/channel/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/classifier/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.8.0a7/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/core/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/core/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/core/urls.py` & `weni_rp_apps-2.8.0a7/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/flow/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/flow/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/org/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/org/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/org/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/statistic/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/user/serializers.py` & `weni_rp_apps-2.8.0a7/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/user/services.py` & `weni_rp_apps-2.8.0a7/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/grpc/user/tests.py` & `weni_rp_apps-2.8.0a7/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/backends.py` & `weni_rp_apps-2.8.0a7/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/channel/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/channel/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/channel/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/channel/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/classifier/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/classifier/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.8.0a7/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/clients/connect.py` & `weni_rp_apps-2.8.0a7/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/externals/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/externals/urls.py` & `weni_rp_apps-2.8.0a7/weni/internal/externals/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/externals/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/flows/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/flows/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/flows/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/globals/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/globals/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/globals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.8.0a7/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.8.0a7/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/models.py` & `weni_rp_apps-2.8.0a7/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/msgs/## Índice.md` & `weni_rp_apps-2.8.0a7/weni/internal/msgs/## Índice.md`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/msgs/tasks.py` & `weni_rp_apps-2.8.0a7/weni/internal/msgs/tasks.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/msgs/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/msgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/orgs/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/orgs/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/statistic/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/statistic/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/tests/test_models.py` & `weni_rp_apps-2.8.0a7/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.8.0a7/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/tickets/urls.py` & `weni_rp_apps-2.8.0a7/weni/internal/tickets/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/tickets/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/tickets/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/urls.py` & `weni_rp_apps-2.8.0a7/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/users/serializers.py` & `weni_rp_apps-2.8.0a7/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/users/tests.py` & `weni_rp_apps-2.8.0a7/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/users/urls.py` & `weni_rp_apps-2.8.0a7/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/users/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/users/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/internal/views.py` & `weni_rp_apps-2.8.0a7/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/orgs_api/serializers.py` & `weni_rp_apps-2.8.0a7/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/orgs_api/tests.py` & `weni_rp_apps-2.8.0a7/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/orgs_api/views.py` & `weni_rp_apps-2.8.0a7/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/s3/views.py` & `weni_rp_apps-2.8.0a7/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/serializers/fields.py` & `weni_rp_apps-2.8.0a7/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/success_orgs/business.py` & `weni_rp_apps-2.8.0a7/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/success_orgs/serializers.py` & `weni_rp_apps-2.8.0a7/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.8.0a7/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/success_orgs/views.py` & `weni_rp_apps-2.8.0a7/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/template_message/serializers.py` & `weni_rp_apps-2.8.0a7/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/template_message/tests.py` & `weni_rp_apps-2.8.0a7/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/template_message/views.py` & `weni_rp_apps-2.8.0a7/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/templates/context_processors.py` & `weni_rp_apps-2.8.0a7/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.8.0a7/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/ticketer_queues/views.py` & `weni_rp_apps-2.8.0a7/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/weni/utils/app_config.py` & `weni_rp_apps-2.8.0a7/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.0a6/PKG-INFO` & `weni_rp_apps-2.8.0a7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.8.0a6
+Version: 2.8.0a7
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```
