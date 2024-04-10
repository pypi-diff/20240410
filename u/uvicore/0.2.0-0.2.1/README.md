# Comparing `tmp/uvicore-0.2.0.tar.gz` & `tmp/uvicore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvicore-0.2.0.tar", max compression
+gzip compressed data, was "uvicore-0.2.1.tar", max compression
```

## Comparing `uvicore-0.2.0.tar` & `uvicore-0.2.1.tar`

### file list

```diff
@@ -1,234 +1,241 @@
--rw-r--r--   0        0        0     1072 2024-02-21 06:25:23.852203 uvicore-0.2.0/LICENSE
--rw-r--r--   0        0        0     5013 2024-02-21 06:25:23.852203 uvicore-0.2.0/README.md
--rw-r--r--   0        0        0     6001 2024-02-21 06:25:23.862203 uvicore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2080 2024-02-21 06:25:23.878869 uvicore-0.2.0/uvicore/__init__.py
--rw-r--r--   0        0        0       47 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/__init__.py
--rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.2.0/uvicore/auth/auth.py
--rw-r--r--   0        0        0       61 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/authenticators/__init__.py
--rw-r--r--   0        0        0     2734 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/auth/authenticators/base.py
--rw-r--r--   0        0        0     2709 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/auth/authenticators/basic.py
--rw-r--r--   0        0        0     9888 2022-12-18 06:36:42.753628 uvicore-0.2.0/uvicore/auth/authenticators/jwt.py
--rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.2.0/uvicore/auth/commands/db.py
--rw-r--r--   0        0        0     3805 2024-02-21 06:25:23.878869 uvicore-0.2.0/uvicore/auth/config/package.py
--rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.2.0/uvicore/auth/contractsOLD/__init__.py
--rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.2.0/uvicore/auth/contractsOLD/group.py
--rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.2.0/uvicore/auth/contractsOLD/user.py
--rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.2.0/uvicore/auth/contractsOLD/user_info.py
--rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.2.0/uvicore/auth/database/seeders/__init__.py
--rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.2.0/uvicore/auth/database/seeders/groups.py
--rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.2.0/uvicore/auth/database/seeders/permissions.py
--rw-r--r--   0        0        0      901 2021-03-22 21:25:23.217946 uvicore-0.2.0/uvicore/auth/database/seeders/roles.py
--rw-r--r--   0        0        0      994 2021-03-22 21:25:23.217946 uvicore-0.2.0/uvicore/auth/database/seeders/users.py
--rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.2.0/uvicore/auth/database/tables/__init__.py
--rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/database/tables/group_roles.py
--rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/database/tables/groups.py
--rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/database/tables/permissions.py
--rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/database/tables/role_permissions.py
--rw-r--r--   0        0        0      894 2021-03-22 21:25:23.217946 uvicore-0.2.0/uvicore/auth/database/tables/roles.py
--rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/database/tables/user_groups.py
--rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.2.0/uvicore/auth/database/tables/user_roles.py
--rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.2.0/uvicore/auth/database/tables/users.py
--rw-r--r--   0        0        0        0 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/auth/http/api/userinfo.py
--rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.2.0/uvicore/auth/http/public/assets/js/app.js
--rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.2.0/uvicore/auth/http/public/robots.txt
--rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.2.0/uvicore/auth/http/public/test.txt
--rw-r--r--   0        0        0     1954 2021-08-18 03:36:20.680024 uvicore-0.2.0/uvicore/auth/http/routes/api.py
--rw-r--r--   0        0        0       88 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/middleware/__init__.py
--rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.2.0/uvicore/auth/middleware/auth_OLD.py
--rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.2.0/uvicore/auth/middleware/basic_OLD.py
--rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.2.0/uvicore/auth/middleware/jwt_OLD.py
--rw-r--r--   0        0        0      121 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/models/__init__.py
--rw-r--r--   0        0        0      985 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/models/group.py
--rw-r--r--   0        0        0      671 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/models/permission.py
--rw-r--r--   0        0        0     1050 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/models/role.py
--rw-r--r--   0        0        0     3385 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/models/user.py
--rw-r--r--   0        0        0     4871 2024-02-21 06:25:23.882203 uvicore-0.2.0/uvicore/auth/package/provider.py
--rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/auth/support/password.py
--rw-r--r--   0        0        0     3541 2024-02-21 06:25:23.882203 uvicore-0.2.0/uvicore/auth/user_info.py
--rw-r--r--   0        0        0       57 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/auth/user_providers/__init__.py
--rw-r--r--   0        0        0     3106 2021-08-20 00:01:23.896381 uvicore-0.2.0/uvicore/auth/user_providers/jwt.py
--rw-r--r--   0        0        0     9496 2024-02-21 06:25:23.882203 uvicore-0.2.0/uvicore/auth/user_providers/orm.py
--rw-r--r--   0        0        0     9031 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/cache/backends/array.py
--rw-r--r--   0        0        0     7734 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/cache/backends/redis.py
--rw-r--r--   0        0        0     2115 2021-10-01 23:17:25.701767 uvicore-0.2.0/uvicore/cache/manager.py
--rw-r--r--   0        0        0     2201 2024-02-21 06:25:23.882203 uvicore-0.2.0/uvicore/cache/package/provider.py
--rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.2.0/uvicore/configuration/__init__.py
--rw-r--r--   0        0        0      786 2024-02-21 06:25:23.882203 uvicore-0.2.0/uvicore/configuration/commands/config.py
--rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/configuration/configuration.py
--rw-r--r--   0        0        0     2351 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/configuration/package/provider.py
--rw-r--r--   0        0        0      790 2023-03-06 01:06:43.066631 uvicore-0.2.0/uvicore/console/__init__.py
--rw-r--r--   0        0        0     1475 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/LICENSE.rst
--rw-r--r--   0        0        0      341 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/README.md
--rw-r--r--   0        0        0     2465 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/__init__.py
--rw-r--r--   0        0        0    12412 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_bashcomplete.py
--rw-r--r--   0        0        0    19850 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_compat.py
--rw-r--r--   0        0        0    20701 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_termui_impl.py
--rw-r--r--   0        0        0     1197 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_textwrap.py
--rw-r--r--   0        0        0     3439 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_unicodefun.py
--rw-r--r--   0        0        0     8379 2021-06-30 20:04:15.673495 uvicore-0.2.0/uvicore/console/asyncclick/_winconsole.py
--rw-r--r--   0        0        0    80043 2023-04-16 17:13:46.545521 uvicore-0.2.0/uvicore/console/asyncclick/core.py
--rw-r--r--   0        0        0    11215 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/decorators.py
--rw-r--r--   0        0        0     7744 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/exceptions.py
--rw-r--r--   0        0        0     9281 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/formatting.py
--rw-r--r--   0        0        0     1501 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/globals.py
--rw-r--r--   0        0        0    15697 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/parser.py
--rw-r--r--   0        0        0    23998 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/termui.py
--rw-r--r--   0        0        0    12886 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/testing.py
--rw-r--r--   0        0        0    24845 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/types.py
--rw-r--r--   0        0        0    15642 2021-06-30 20:04:15.676828 uvicore-0.2.0/uvicore/console/asyncclick/utils.py
--rw-r--r--   0        0        0     6189 2023-03-06 01:06:46.553354 uvicore-0.2.0/uvicore/console/click_colors.py
--rw-r--r--   0        0        0     1764 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/console/commands/generators.py
--rw-r--r--   0        0        0     1857 2021-08-19 19:44:45.042716 uvicore-0.2.0/uvicore/console/commands/stubs/command.py
--rw-r--r--   0        0        0     1883 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/console/console.py
--rw-r--r--   0        0        0      756 2023-03-06 01:06:57.420198 uvicore-0.2.0/uvicore/console/decorators.py
--rw-r--r--   0        0        0      717 2023-04-16 17:13:46.545521 uvicore-0.2.0/uvicore/console/events/command.py
--rw-r--r--   0        0        0     2430 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/console/package/bootstrap.py
--rw-r--r--   0        0        0     2938 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/console/package/provider.py
--rw-r--r--   0        0        0     1016 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/console/package/registers.py
--rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.2.0/uvicore/container/__init__.py
--rw-r--r--   0        0        0     2236 2024-02-21 06:25:23.885536 uvicore-0.2.0/uvicore/container/commands/ioc.py
--rw-r--r--   0        0        0    12772 2024-02-21 06:25:23.888869 uvicore-0.2.0/uvicore/container/ioc.py
--rw-r--r--   0        0        0     1122 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/contracts/__init__.py
--rw-r--r--   0        0        0     3449 2021-09-29 18:14:10.395022 uvicore-0.2.0/uvicore/contracts/application.py
--rw-r--r--   0        0        0      657 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/contracts/authenticator.py
--rw-r--r--   0        0        0      390 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/contracts/auto_api.py
--rw-r--r--   0        0        0     4264 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/contracts/builder.py
--rw-r--r--   0        0        0     2085 2021-05-16 03:31:59.322488 uvicore-0.2.0/uvicore/contracts/cache.py
--rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.2.0/uvicore/contracts/config.py
--rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.2.0/uvicore/contracts/connection.py
--rw-r--r--   0        0        0     5514 2023-04-16 17:13:46.548854 uvicore-0.2.0/uvicore/contracts/database.py
--rw-r--r--   0        0        0     2189 2021-09-22 05:15:43.413436 uvicore-0.2.0/uvicore/contracts/dispatcher.py
--rw-r--r--   0        0        0      433 2021-05-16 03:31:59.322488 uvicore-0.2.0/uvicore/contracts/email.py
--rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.2.0/uvicore/contracts/event.py
--rw-r--r--   0        0        0      759 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/contracts/field.py
--rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/contracts/ioc.py
--rw-r--r--   0        0        0     2504 2022-12-18 06:36:42.753628 uvicore-0.2.0/uvicore/contracts/logger.py
--rw-r--r--   0        0        0     1377 2021-04-05 21:28:22.231229 uvicore-0.2.0/uvicore/contracts/mapper.py
--rw-r--r--   0        0        0     3814 2022-02-18 20:14:08.924157 uvicore-0.2.0/uvicore/contracts/model.py
--rw-r--r--   0        0        0     3102 2024-02-21 06:25:23.888869 uvicore-0.2.0/uvicore/contracts/package.py
--rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.2.0/uvicore/contracts/provider.py
--rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.2.0/uvicore/contracts/relation.py
--rw-r--r--   0        0        0     4220 2021-09-22 05:15:43.413436 uvicore-0.2.0/uvicore/contracts/router.py
--rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/contracts/routes-OLD.py
--rw-r--r--   0        0        0      532 2021-03-22 21:25:23.221280 uvicore-0.2.0/uvicore/contracts/server.py
--rw-r--r--   0        0        0      924 2024-02-21 06:25:23.888869 uvicore-0.2.0/uvicore/contracts/template.py
--rw-r--r--   0        0        0     2243 2021-08-20 00:01:23.896381 uvicore-0.2.0/uvicore/contracts/user_info.py
--rw-r--r--   0        0        0     3004 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/contracts/user_provider.py
--rw-r--r--   0        0        0      704 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/database/__init__.py
--rw-r--r--   0        0        0    18719 2023-04-16 17:13:46.548854 uvicore-0.2.0/uvicore/database/builder.py
--rw-r--r--   0        0        0     7979 2024-02-21 06:25:23.888869 uvicore-0.2.0/uvicore/database/commands/db.py
--rw-r--r--   0        0        0     2527 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/commands/generators.py
--rw-r--r--   0        0        0     4721 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/commands/stubs/seeder.py
--rw-r--r--   0        0        0     3012 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/commands/stubs/table.py
--rw-r--r--   0        0        0     9981 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/db.py
--rw-r--r--   0        0        0     1728 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/package/bootstrap.py
--rw-r--r--   0        0        0     3774 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/package/provider.py
--rw-r--r--   0        0        0     3866 2024-02-21 06:25:23.892203 uvicore-0.2.0/uvicore/database/package/registers.py
--rw-r--r--   0        0        0     6117 2024-02-21 06:25:23.895536 uvicore-0.2.0/uvicore/database/query.py
--rw-r--r--   0        0        0     3137 2024-02-10 00:08:36.205626 uvicore-0.2.0/uvicore/database/table.py
--rw-r--r--   0        0        0      302 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/events/__init__.py
--rw-r--r--   0        0        0     1415 2021-09-22 05:15:43.413436 uvicore-0.2.0/uvicore/events/commands/event.py
--rw-r--r--   0        0        0    13029 2021-09-22 05:15:43.413436 uvicore-0.2.0/uvicore/events/dispatcher.py
--rw-r--r--   0        0        0     2180 2021-09-22 05:15:43.413436 uvicore-0.2.0/uvicore/events/event.py
--rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/events/handler.py
--rw-r--r--   0        0        0     2035 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/exceptions/__init__.py
--rw-r--r--   0        0        0       42 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/factories/__init__.py
--rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.2.0/uvicore/factories/logger.py
--rw-r--r--   0        0        0    12711 2024-02-21 06:25:23.895536 uvicore-0.2.0/uvicore/foundation/application.py
--rw-r--r--   0        0        0      306 2024-02-21 06:25:23.895536 uvicore-0.2.0/uvicore/foundation/commands/app.py
--rw-r--r--   0        0        0     3926 2024-02-21 06:25:23.895536 uvicore-0.2.0/uvicore/foundation/config/package.py
--rw-r--r--   0        0        0      270 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/foundation/decorators/__init__.py
--rw-r--r--   0        0        0      435 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/foundation/decorators/composer.py
--rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/controller.py
--rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/event.py
--rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/model.py
--rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/provider.py
--rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/routes.py
--rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/seeder.py
--rw-r--r--   0        0        0      681 2021-09-07 21:04:46.388597 uvicore-0.2.0/uvicore/foundation/decorators/service.py
--rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/foundation/decorators/table.py
--rw-r--r--   0        0        0      893 2021-09-08 13:16:25.207365 uvicore-0.2.0/uvicore/foundation/events/app.py
--rw-r--r--   0        0        0     5691 2024-02-21 06:25:23.895536 uvicore-0.2.0/uvicore/foundation/package/provider.py
--rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.2.0/uvicore/http/OBSOLETE/router.py
--rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/OBSOLETE/routes-OLD.py
--rw-r--r--   0        0        0      762 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/__init__.py
--rw-r--r--   0        0        0     3210 2024-02-21 06:25:23.898870 uvicore-0.2.0/uvicore/http/commands/generators.py
--rw-r--r--   0        0        0      418 2024-02-21 06:25:23.898870 uvicore-0.2.0/uvicore/http/commands/routes.py
--rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.2.0/uvicore/http/commands/serve.py
--rw-r--r--   0        0        0    12279 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/commands/stubs/api_controller.py
--rw-r--r--   0        0        0      913 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/commands/stubs/composer.py
--rw-r--r--   0        0        0    12842 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/commands/stubs/controller.py
--rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/controllers/__init__.py
--rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/controllers/api.py
--rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/controllers/web.py
--rw-r--r--   0        0        0      874 2021-03-24 17:46:21.490777 uvicore-0.2.0/uvicore/http/events/server.py
--rw-r--r--   0        0        0     3972 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/http/exceptions/__init__.py
--rw-r--r--   0        0        0     2851 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/http/exceptions/handlers.py
--rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.2.0/uvicore/http/middleware/__init__.py
--rw-r--r--   0        0        0    13311 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/http/middleware/authentication.py
--rw-r--r--   0        0        0     1968 2024-02-21 06:25:23.898870 uvicore-0.2.0/uvicore/http/openapi/docs.py
--rw-r--r--   0        0        0    29150 2024-02-29 22:04:21.828093 uvicore-0.2.0/uvicore/http/package/bootstrap.py
--rw-r--r--   0        0        0     6524 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/http/package/provider.py
--rw-r--r--   0        0        0     4520 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/http/package/registers.py
--rw-r--r--   0        0        0      138 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/params.py
--rw-r--r--   0        0        0     1269 2021-08-18 03:36:20.680024 uvicore-0.2.0/uvicore/http/request.py
--rw-r--r--   0        0        0     4661 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/http/response.py
--rw-r--r--   0        0        0      455 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/routing/__init__.py
--rw-r--r--   0        0        0    22281 2021-09-22 05:15:43.416770 uvicore-0.2.0/uvicore/http/routing/api_router.py
--rw-r--r--   0        0        0    10476 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/http/routing/auto_api.py
--rw-r--r--   0        0        0     4875 2021-09-07 21:04:46.391931 uvicore-0.2.0/uvicore/http/routing/guard.py
--rw-r--r--   0        0        0    21460 2024-02-21 05:43:11.859354 uvicore-0.2.0/uvicore/http/routing/model_router.py
--rw-r--r--   0        0        0    21451 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/http/routing/router.py
--rw-r--r--   0        0        0    16785 2021-09-22 05:15:43.416770 uvicore-0.2.0/uvicore/http/routing/web_router.py
--rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/server.py
--rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/servers/api.py
--rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/servers/web.py
--rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/static.py
--rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.2.0/uvicore/http/status.py
--rw-r--r--   0        0        0     1609 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/http/templating/context_functions.py
--rw-r--r--   0        0        0     2280 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/http_client/package/provider.py
--rw-r--r--   0        0        0    15001 2021-03-02 19:39:30.886925 uvicore-0.2.0/uvicore/logging/logger.py
--rw-r--r--   0        0        0     2340 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/logging/package/provider.py
--rw-r--r--   0        0        0     2608 2021-05-16 03:31:59.322488 uvicore-0.2.0/uvicore/mail/__init__.py
--rw-r--r--   0        0        0       29 2021-05-16 03:31:59.322488 uvicore-0.2.0/uvicore/mail/backends/__init__.py
--rw-r--r--   0        0        0     2126 2021-05-16 03:31:59.322488 uvicore-0.2.0/uvicore/mail/backends/mailgun.py
--rw-r--r--   0        0        0     1181 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/mail/package/provider.py
--rw-r--r--   0        0        0      181 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/orm/__init__.py
--rw-r--r--   0        0        0     1395 2024-02-21 06:25:23.902203 uvicore-0.2.0/uvicore/orm/commands/generators.py
--rw-r--r--   0        0        0     9719 2023-04-16 17:13:46.552188 uvicore-0.2.0/uvicore/orm/commands/stubs/model.py
--rw-r--r--   0        0        0      447 2021-09-07 21:04:46.391931 uvicore-0.2.0/uvicore/orm/drivers/api.py
--rw-r--r--   0        0        0        0 2021-03-26 15:13:44.398249 uvicore-0.2.0/uvicore/orm/drivers/sqlalchemy.py
--rw-r--r--   0        0        0    13295 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/orm/fields.py
--rw-r--r--   0        0        0     7967 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/orm/mapper.py
--rw-r--r--   0        0        0    18136 2024-02-21 05:44:11.496549 uvicore-0.2.0/uvicore/orm/metaclass.py
--rw-r--r--   0        0        0    32661 2021-10-14 19:51:04.065963 uvicore-0.2.0/uvicore/orm/model.py
--rw-r--r--   0        0        0     3108 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/orm/package/provider.py
--rw-r--r--   0        0        0    49157 2024-03-02 20:17:00.246759 uvicore-0.2.0/uvicore/orm/query.py
--rw-r--r--   0        0        0      458 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/package/__init__.py
--rw-r--r--   0        0        0     1794 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/package/commands/package.py
--rw-r--r--   0        0        0     3490 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/package/package.py
--rw-r--r--   0        0        0     3676 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/package/provider.py
--rw-r--r--   0        0        0       40 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/redis/__init__.py
--rw-r--r--   0        0        0     1218 2024-02-21 06:25:23.905536 uvicore-0.2.0/uvicore/redis/package/bootstrap.py
--rw-r--r--   0        0        0     3287 2024-02-29 20:13:43.996697 uvicore-0.2.0/uvicore/redis/package/provider.py
--rw-r--r--   0        0        0      272 2024-02-21 06:25:23.908870 uvicore-0.2.0/uvicore/redis/package/registers.py
--rw-r--r--   0        0        0     3277 2021-10-14 19:18:41.567853 uvicore-0.2.0/uvicore/redis/redis.py
--rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.2.0/uvicore/support/README.md
--rw-r--r--   0        0        0      296 2021-03-29 16:45:06.822538 uvicore-0.2.0/uvicore/support/classes.py
--rw-r--r--   0        0        0     5162 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/support/collection.py
--rw-r--r--   0        0        0     2419 2021-03-22 21:25:23.221280 uvicore-0.2.0/uvicore/support/concurrency.py
--rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.2.0/uvicore/support/dictionary.py
--rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.2.0/uvicore/support/dumper.py
--rw-r--r--   0        0        0      439 2023-07-16 16:47:20.390563 uvicore-0.2.0/uvicore/support/hash.py
--rw-r--r--   0        0        0     3771 2023-09-26 21:00:07.189986 uvicore-0.2.0/uvicore/support/module.py
--rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.2.0/uvicore/support/path.py
--rw-r--r--   0        0        0     1889 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/support/schematic.py
--rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.2.0/uvicore/support/singleton.py
--rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.2.0/uvicore/support/str.py
--rw-r--r--   0        0        0     5446 2024-02-21 06:25:23.908870 uvicore-0.2.0/uvicore/templating/engine.py
--rw-r--r--   0        0        0     2904 2024-02-21 06:25:23.908870 uvicore-0.2.0/uvicore/templating/package/bootstrap.py
--rw-r--r--   0        0        0     1686 2024-02-21 06:25:23.908870 uvicore-0.2.0/uvicore/templating/package/provider.py
--rw-r--r--   0        0        0     1024 2024-02-21 06:25:23.908870 uvicore-0.2.0/uvicore/templating/package/registers.py
--rw-r--r--   0        0        0     2452 2021-09-29 18:14:10.398356 uvicore-0.2.0/uvicore/typing/__init__.py
--rw-r--r--   0        0        0    12661 2021-10-15 19:36:53.939029 uvicore-0.2.0/uvicore/typing/dictionary.py
--rw-r--r--   0        0        0     7635 1970-01-01 00:00:00.000000 uvicore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 18:24:17.532245 uvicore-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1393 2024-04-10 18:24:17.532245 uvicore-0.2.1/README.md
+-rw-r--r--   0        0        0     6001 2024-04-10 18:24:17.535579 uvicore-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2236 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/__init__.py
+-rw-r--r--   0        0        0       47 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/__init__.py
+-rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.2.1/uvicore/auth/auth.py
+-rw-r--r--   0        0        0       61 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/authenticators/__init__.py
+-rw-r--r--   0        0        0     2809 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/authenticators/base.py
+-rw-r--r--   0        0        0     2709 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/auth/authenticators/basic.py
+-rw-r--r--   0        0        0     9316 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/authenticators/jwt.py
+-rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.2.1/uvicore/auth/commands/db.py
+-rw-r--r--   0        0        0     3805 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/config/package.py
+-rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.2.1/uvicore/auth/contractsOLD/__init__.py
+-rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.2.1/uvicore/auth/contractsOLD/group.py
+-rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.2.1/uvicore/auth/contractsOLD/user.py
+-rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.2.1/uvicore/auth/contractsOLD/user_info.py
+-rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.2.1/uvicore/auth/database/seeders/__init__.py
+-rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.2.1/uvicore/auth/database/seeders/groups.py
+-rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.2.1/uvicore/auth/database/seeders/permissions.py
+-rw-r--r--   0        0        0      901 2021-03-22 21:25:23.217946 uvicore-0.2.1/uvicore/auth/database/seeders/roles.py
+-rw-r--r--   0        0        0      994 2021-03-22 21:25:23.217946 uvicore-0.2.1/uvicore/auth/database/seeders/users.py
+-rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.2.1/uvicore/auth/database/tables/__init__.py
+-rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/database/tables/group_roles.py
+-rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/database/tables/groups.py
+-rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/database/tables/permissions.py
+-rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/database/tables/role_permissions.py
+-rw-r--r--   0        0        0      894 2021-03-22 21:25:23.217946 uvicore-0.2.1/uvicore/auth/database/tables/roles.py
+-rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/database/tables/user_groups.py
+-rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.2.1/uvicore/auth/database/tables/user_roles.py
+-rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.2.1/uvicore/auth/database/tables/users.py
+-rw-r--r--   0        0        0        0 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/auth/http/api/userinfo.py
+-rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.2.1/uvicore/auth/http/public/assets/js/app.js
+-rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.2.1/uvicore/auth/http/public/robots.txt
+-rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.2.1/uvicore/auth/http/public/test.txt
+-rw-r--r--   0        0        0     1954 2021-08-18 03:36:20.680024 uvicore-0.2.1/uvicore/auth/http/routes/api.py
+-rw-r--r--   0        0        0       88 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/middleware/__init__.py
+-rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.2.1/uvicore/auth/middleware/auth_OLD.py
+-rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.2.1/uvicore/auth/middleware/basic_OLD.py
+-rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.2.1/uvicore/auth/middleware/jwt_OLD.py
+-rw-r--r--   0        0        0      121 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/models/__init__.py
+-rw-r--r--   0        0        0      985 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/models/group.py
+-rw-r--r--   0        0        0      671 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/models/permission.py
+-rw-r--r--   0        0        0     1050 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/models/role.py
+-rw-r--r--   0        0        0     3385 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/models/user.py
+-rw-r--r--   0        0        0     4871 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/package/provider.py
+-rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/auth/support/password.py
+-rw-r--r--   0        0        0     3541 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/user_info.py
+-rw-r--r--   0        0        0       57 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/auth/user_providers/__init__.py
+-rw-r--r--   0        0        0     3106 2021-08-20 00:01:23.896381 uvicore-0.2.1/uvicore/auth/user_providers/jwt.py
+-rw-r--r--   0        0        0    11011 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/auth/user_providers/orm.py
+-rw-r--r--   0        0        0     9031 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/cache/backends/array.py
+-rw-r--r--   0        0        0     7734 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/cache/backends/redis.py
+-rw-r--r--   0        0        0     2115 2021-10-01 23:17:25.701767 uvicore-0.2.1/uvicore/cache/manager.py
+-rw-r--r--   0        0        0     2201 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/cache/package/provider.py
+-rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.2.1/uvicore/configuration/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/configuration/commands/config.py
+-rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/configuration/configuration.py
+-rw-r--r--   0        0        0     2351 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/configuration/package/provider.py
+-rw-r--r--   0        0        0      790 2023-03-06 01:06:43.066631 uvicore-0.2.1/uvicore/console/__init__.py
+-rw-r--r--   0        0        0     1475 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/LICENSE.rst
+-rw-r--r--   0        0        0      341 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/README.md
+-rw-r--r--   0        0        0     2465 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/__init__.py
+-rw-r--r--   0        0        0    12412 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_bashcomplete.py
+-rw-r--r--   0        0        0    19850 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_compat.py
+-rw-r--r--   0        0        0    20701 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_termui_impl.py
+-rw-r--r--   0        0        0     1197 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_textwrap.py
+-rw-r--r--   0        0        0     3439 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_unicodefun.py
+-rw-r--r--   0        0        0     8379 2021-06-30 20:04:15.673495 uvicore-0.2.1/uvicore/console/asyncclick/_winconsole.py
+-rw-r--r--   0        0        0    80043 2023-04-16 17:13:46.545521 uvicore-0.2.1/uvicore/console/asyncclick/core.py
+-rw-r--r--   0        0        0    11215 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/decorators.py
+-rw-r--r--   0        0        0     7744 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/exceptions.py
+-rw-r--r--   0        0        0     9281 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/formatting.py
+-rw-r--r--   0        0        0     1501 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/globals.py
+-rw-r--r--   0        0        0    15697 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/parser.py
+-rw-r--r--   0        0        0    23998 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/termui.py
+-rw-r--r--   0        0        0    12886 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/testing.py
+-rw-r--r--   0        0        0    24845 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/types.py
+-rw-r--r--   0        0        0    15642 2021-06-30 20:04:15.676828 uvicore-0.2.1/uvicore/console/asyncclick/utils.py
+-rw-r--r--   0        0        0     6189 2023-03-06 01:06:46.553354 uvicore-0.2.1/uvicore/console/click_colors.py
+-rw-r--r--   0        0        0     1764 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/console/commands/generators.py
+-rw-r--r--   0        0        0     1857 2021-08-19 19:44:45.042716 uvicore-0.2.1/uvicore/console/commands/stubs/command.py
+-rw-r--r--   0        0        0     1933 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/console/console.py
+-rw-r--r--   0        0        0      756 2023-03-06 01:06:57.420198 uvicore-0.2.1/uvicore/console/decorators.py
+-rw-r--r--   0        0        0      717 2023-04-16 17:13:46.545521 uvicore-0.2.1/uvicore/console/events/command.py
+-rw-r--r--   0        0        0     2430 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/console/package/bootstrap.py
+-rw-r--r--   0        0        0     2938 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/console/package/provider.py
+-rw-r--r--   0        0        0     1016 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/console/package/registers.py
+-rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.2.1/uvicore/container/__init__.py
+-rw-r--r--   0        0        0     2236 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/container/commands/ioc.py
+-rw-r--r--   0        0        0    12772 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/container/ioc.py
+-rw-r--r--   0        0        0     1185 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/__init__.py
+-rw-r--r--   0        0        0     3449 2021-09-29 18:14:10.395022 uvicore-0.2.1/uvicore/contracts/application.py
+-rw-r--r--   0        0        0     1089 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/authenticator.py
+-rw-r--r--   0        0        0      390 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/contracts/auto_api.py
+-rw-r--r--   0        0        0     4264 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/contracts/builder.py
+-rw-r--r--   0        0        0     2085 2021-05-16 03:31:59.322488 uvicore-0.2.1/uvicore/contracts/cache.py
+-rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.2.1/uvicore/contracts/config.py
+-rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.2.1/uvicore/contracts/connection.py
+-rw-r--r--   0        0        0     5514 2023-04-16 17:13:46.548854 uvicore-0.2.1/uvicore/contracts/database.py
+-rw-r--r--   0        0        0     2209 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/dispatcher.py
+-rw-r--r--   0        0        0      433 2021-05-16 03:31:59.322488 uvicore-0.2.1/uvicore/contracts/email.py
+-rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.2.1/uvicore/contracts/event.py
+-rw-r--r--   0        0        0      759 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/contracts/field.py
+-rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/contracts/ioc.py
+-rw-r--r--   0        0        0      588 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/job.py
+-rw-r--r--   0        0        0      570 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/job_dispatcher.py
+-rw-r--r--   0        0        0     2504 2022-12-18 06:36:42.753628 uvicore-0.2.1/uvicore/contracts/logger.py
+-rw-r--r--   0        0        0     1377 2021-04-05 21:28:22.231229 uvicore-0.2.1/uvicore/contracts/mapper.py
+-rw-r--r--   0        0        0     3814 2022-02-18 20:14:08.924157 uvicore-0.2.1/uvicore/contracts/model.py
+-rw-r--r--   0        0        0     3102 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/package.py
+-rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.2.1/uvicore/contracts/provider.py
+-rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.2.1/uvicore/contracts/relation.py
+-rw-r--r--   0        0        0     4220 2021-09-22 05:15:43.413436 uvicore-0.2.1/uvicore/contracts/router.py
+-rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/contracts/routes-OLD.py
+-rw-r--r--   0        0        0      532 2021-03-22 21:25:23.221280 uvicore-0.2.1/uvicore/contracts/server.py
+-rw-r--r--   0        0        0      924 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/contracts/template.py
+-rw-r--r--   0        0        0     2243 2021-08-20 00:01:23.896381 uvicore-0.2.1/uvicore/contracts/user_info.py
+-rw-r--r--   0        0        0     3004 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/contracts/user_provider.py
+-rw-r--r--   0        0        0      704 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/database/__init__.py
+-rw-r--r--   0        0        0    18719 2023-04-16 17:13:46.548854 uvicore-0.2.1/uvicore/database/builder.py
+-rw-r--r--   0        0        0     7979 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/commands/db.py
+-rw-r--r--   0        0        0     2527 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/commands/generators.py
+-rw-r--r--   0        0        0     4721 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/commands/stubs/seeder.py
+-rw-r--r--   0        0        0     3012 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/commands/stubs/table.py
+-rw-r--r--   0        0        0     9981 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/db.py
+-rw-r--r--   0        0        0     1728 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/package/bootstrap.py
+-rw-r--r--   0        0        0     3774 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/package/provider.py
+-rw-r--r--   0        0        0     3866 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/package/registers.py
+-rw-r--r--   0        0        0     6117 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/database/query.py
+-rw-r--r--   0        0        0     3137 2024-02-10 00:08:36.205626 uvicore-0.2.1/uvicore/database/table.py
+-rw-r--r--   0        0        0      302 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/events/__init__.py
+-rw-r--r--   0        0        0     1415 2021-09-22 05:15:43.413436 uvicore-0.2.1/uvicore/events/commands/event.py
+-rw-r--r--   0        0        0    13029 2021-09-22 05:15:43.413436 uvicore-0.2.1/uvicore/events/dispatcher.py
+-rw-r--r--   0        0        0     2180 2024-04-02 23:02:52.114042 uvicore-0.2.1/uvicore/events/event.py
+-rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/events/handler.py
+-rw-r--r--   0        0        0     2035 2024-04-04 17:37:46.119796 uvicore-0.2.1/uvicore/exceptions/__init__.py
+-rw-r--r--   0        0        0       42 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/factories/__init__.py
+-rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.2.1/uvicore/factories/logger.py
+-rw-r--r--   0        0        0    12711 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/application.py
+-rw-r--r--   0        0        0      306 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/commands/app.py
+-rw-r--r--   0        0        0     3926 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/config/package.py
+-rw-r--r--   0        0        0      291 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/decorators/__init__.py
+-rw-r--r--   0        0        0      435 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/foundation/decorators/composer.py
+-rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/controller.py
+-rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/event.py
+-rw-r--r--   0        0        0      429 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/decorators/job.py
+-rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/model.py
+-rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/provider.py
+-rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/routes.py
+-rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/seeder.py
+-rw-r--r--   0        0        0      681 2021-09-07 21:04:46.388597 uvicore-0.2.1/uvicore/foundation/decorators/service.py
+-rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/foundation/decorators/table.py
+-rw-r--r--   0        0        0      893 2021-09-08 13:16:25.207365 uvicore-0.2.1/uvicore/foundation/events/app.py
+-rw-r--r--   0        0        0     5691 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/foundation/package/provider.py
+-rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.2.1/uvicore/http/OBSOLETE/router.py
+-rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/OBSOLETE/routes-OLD.py
+-rw-r--r--   0        0        0      762 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/http/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/http/commands/generators.py
+-rw-r--r--   0        0        0      418 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/http/commands/routes.py
+-rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.2.1/uvicore/http/commands/serve.py
+-rw-r--r--   0        0        0    12327 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/http/commands/stubs/api_controller.py
+-rw-r--r--   0        0        0      913 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/http/commands/stubs/composer.py
+-rw-r--r--   0        0        0    12890 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/http/commands/stubs/controller.py
+-rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/controllers/__init__.py
+-rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/controllers/api.py
+-rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/controllers/web.py
+-rw-r--r--   0        0        0      874 2021-03-24 17:46:21.490777 uvicore-0.2.1/uvicore/http/events/server.py
+-rw-r--r--   0        0        0     3972 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/http/exceptions/__init__.py
+-rw-r--r--   0        0        0     2851 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/http/exceptions/handlers.py
+-rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.2.1/uvicore/http/middleware/__init__.py
+-rw-r--r--   0        0        0    13312 2024-04-10 18:24:17.538912 uvicore-0.2.1/uvicore/http/middleware/authentication.py
+-rw-r--r--   0        0        0     1968 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/openapi/docs.py
+-rw-r--r--   0        0        0    29150 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/package/bootstrap.py
+-rw-r--r--   0        0        0     6524 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/package/provider.py
+-rw-r--r--   0        0        0     4520 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/package/registers.py
+-rw-r--r--   0        0        0      124 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/params.py
+-rw-r--r--   0        0        0     1301 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/request.py
+-rw-r--r--   0        0        0     4661 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http/response.py
+-rw-r--r--   0        0        0      455 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/http/routing/__init__.py
+-rw-r--r--   0        0        0    22281 2021-09-22 05:15:43.416770 uvicore-0.2.1/uvicore/http/routing/api_router.py
+-rw-r--r--   0        0        0    10476 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/http/routing/auto_api.py
+-rw-r--r--   0        0        0     4875 2021-09-07 21:04:46.391931 uvicore-0.2.1/uvicore/http/routing/guard.py
+-rw-r--r--   0        0        0    21460 2024-02-21 05:43:11.859354 uvicore-0.2.1/uvicore/http/routing/model_router.py
+-rw-r--r--   0        0        0    21451 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/http/routing/router.py
+-rw-r--r--   0        0        0    16785 2021-09-22 05:15:43.416770 uvicore-0.2.1/uvicore/http/routing/web_router.py
+-rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/server.py
+-rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/servers/api.py
+-rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/servers/web.py
+-rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/static.py
+-rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.2.1/uvicore/http/status.py
+-rw-r--r--   0        0        0     1609 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/http/templating/context_functions.py
+-rw-r--r--   0        0        0     2280 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/http_client/package/provider.py
+-rw-r--r--   0        0        0       88 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/jobs/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/jobs/dispatcher.py
+-rw-r--r--   0        0        0      902 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/jobs/job.py
+-rw-r--r--   0        0        0      332 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/jobs/results.py
+-rw-r--r--   0        0        0    14997 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/logging/logger.py
+-rw-r--r--   0        0        0     2340 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/logging/package/provider.py
+-rw-r--r--   0        0        0     2608 2021-05-16 03:31:59.322488 uvicore-0.2.1/uvicore/mail/__init__.py
+-rw-r--r--   0        0        0       29 2021-05-16 03:31:59.322488 uvicore-0.2.1/uvicore/mail/backends/__init__.py
+-rw-r--r--   0        0        0     2126 2021-05-16 03:31:59.322488 uvicore-0.2.1/uvicore/mail/backends/mailgun.py
+-rw-r--r--   0        0        0     1181 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/mail/package/provider.py
+-rw-r--r--   0        0        0      181 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/orm/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/orm/commands/generators.py
+-rw-r--r--   0        0        0     9719 2023-04-16 17:13:46.552188 uvicore-0.2.1/uvicore/orm/commands/stubs/model.py
+-rw-r--r--   0        0        0      447 2021-09-07 21:04:46.391931 uvicore-0.2.1/uvicore/orm/drivers/api.py
+-rw-r--r--   0        0        0        0 2021-03-26 15:13:44.398249 uvicore-0.2.1/uvicore/orm/drivers/sqlalchemy.py
+-rw-r--r--   0        0        0    13295 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/orm/fields.py
+-rw-r--r--   0        0        0     7967 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/orm/mapper.py
+-rw-r--r--   0        0        0    18144 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/orm/metaclass.py
+-rw-r--r--   0        0        0    32661 2024-03-26 17:38:31.288155 uvicore-0.2.1/uvicore/orm/model.py
+-rw-r--r--   0        0        0     3108 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/orm/package/provider.py
+-rw-r--r--   0        0        0    49157 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/orm/query.py
+-rw-r--r--   0        0        0      458 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/package/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/package/commands/package.py
+-rw-r--r--   0        0        0     3490 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/package/package.py
+-rw-r--r--   0        0        0     3676 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/package/provider.py
+-rw-r--r--   0        0        0       40 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/redis/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/redis/package/bootstrap.py
+-rw-r--r--   0        0        0     3287 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/redis/package/provider.py
+-rw-r--r--   0        0        0      272 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/redis/package/registers.py
+-rw-r--r--   0        0        0     3277 2021-10-14 19:18:41.567853 uvicore-0.2.1/uvicore/redis/redis.py
+-rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.2.1/uvicore/support/README.md
+-rw-r--r--   0        0        0      296 2021-03-29 16:45:06.822538 uvicore-0.2.1/uvicore/support/classes.py
+-rw-r--r--   0        0        0     5162 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/support/collection.py
+-rw-r--r--   0        0        0     2419 2021-03-22 21:25:23.221280 uvicore-0.2.1/uvicore/support/concurrency.py
+-rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.2.1/uvicore/support/dictionary.py
+-rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.2.1/uvicore/support/dumper.py
+-rw-r--r--   0        0        0      439 2023-07-16 16:47:20.390563 uvicore-0.2.1/uvicore/support/hash.py
+-rw-r--r--   0        0        0     3771 2023-09-26 21:00:07.189986 uvicore-0.2.1/uvicore/support/module.py
+-rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.2.1/uvicore/support/path.py
+-rw-r--r--   0        0        0     1889 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/support/schematic.py
+-rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.2.1/uvicore/support/singleton.py
+-rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.2.1/uvicore/support/str.py
+-rw-r--r--   0        0        0     5446 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/templating/engine.py
+-rw-r--r--   0        0        0     2904 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/templating/package/bootstrap.py
+-rw-r--r--   0        0        0     1686 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/templating/package/provider.py
+-rw-r--r--   0        0        0     1024 2024-04-10 18:24:17.542246 uvicore-0.2.1/uvicore/templating/package/registers.py
+-rw-r--r--   0        0        0     2452 2021-09-29 18:14:10.398356 uvicore-0.2.1/uvicore/typing/__init__.py
+-rw-r--r--   0        0        0    12661 2021-10-15 19:36:53.939029 uvicore-0.2.1/uvicore/typing/dictionary.py
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 uvicore-0.2.1/PKG-INFO
```

### Comparing `uvicore-0.2.0/LICENSE` & `uvicore-0.2.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Matthew Reschke
+Copyright (c) 2024 Matthew Reschke
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `uvicore-0.2.0/pyproject.toml` & `uvicore-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uvicore"
-version = "0.2.0"
+version = "0.2.1"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "The Fullstack Async Web, API and CLI Python Framework"
 readme = "README.md"
 homepage = "https://github.com/uvicore/framework"
 documentation = "https://github.com/uvicore/framework"
 repository = "https://github.com/uvicore/framework"
@@ -15,15 +15,15 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Operating System :: MacOS",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Environment :: Web Environment",
     "Environment :: Console",
-    "Framework :: AsyncIO",
+    "Framework :: FastAPI",
     "Typing :: Typed",
 ]
 include = ["LICENSE"]
 
 
 [tool.poetry.dependencies]
 # These packages are mandatory and form the core of the uvicore distribution
```

### Comparing `uvicore-0.2.0/uvicore/__init__.py` & `uvicore-0.2.1/uvicore/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # type: ignore
 from . import contracts
 from uvicore.typing import Dict
-from uvicore.foundation.decorators import event, model, seeder, service, table, provider, routes, controller, composer
+from uvicore.foundation.decorators import event, job, model, seeder, service, table, provider, routes, controller, composer
 
 
 # Uvicore version.  Also available in app.version
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 # Core (non service provider based) singletons as globals
 ioc: contracts.Ioc = None
 events: contracts.Dispatcher = None
+jobs: contracts.JobDispatcher = None
 app: contracts.Application = None
 
 # Core (service provider based) singletons as globals
 config: contracts.Config = None
-#config: Dict()
 log: contracts.Logger = None
 db: contracts.Database = None
 cache: contracts.Cache = None
 
 
 def bootstrap(app_config: Dict, path: str, is_console: bool) -> None:
     """A pre-bootstrap method to setup and call the main uvicore application bootstrap"""
@@ -43,12 +43,16 @@
 
     # Import Event Dispatcher (which is an IoC singleton) and set uvicore.events global
     # This cannot be a service provider because events are fired BEFORE any service providers
     # are ever loaded.
     from uvicore.events.dispatcher import Dispatcher
     uvicore.events = Dispatcher
 
+    # Import Job Dispatcher
+    from uvicore.jobs.dispatcher import Dispatcher as JobDispatcher
+    uvicore.jobs = JobDispatcher
+
     # Why can 'config' be a service provider?  Because it's always the FIRST service provider.
     # So all other providers after that have access to register their own configs.
 
     # Bootstrap the actual uvicore Application
     uvicore.app.bootstrap(app_config, path, is_console)
```

### Comparing `uvicore-0.2.0/uvicore/auth/authenticators/base.py` & `uvicore-0.2.1/uvicore/auth/authenticators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import uvicore
 from uvicore.support import module
 from uvicore.support.dumper import dump, dd
 from uvicore.http.request import HTTPConnection
 from uvicore.contracts import UserInfo, UserProvider
 from uvicore.typing import Dict, Optional, List, Tuple
+from uvicore.contracts import Logger as LoggerInterface
 from uvicore.contracts import Authenticator as AuthenticatorInterface
 
 
 @uvicore.service()
 class Authenticator(AuthenticatorInterface):
     """Base authenticator class"""
 
     def __init__(self, config: Dict):
         self.config = config
 
     @property
-    def log(self):
+    def log(self) -> LoggerInterface:
         return uvicore.log.name('uvicore.auth')
 
     async def retrieve_user(self, username: str, password: str, provider: Dict, request: HTTPConnection, **kwargs) -> Optional[UserInfo]:
         """Retrieve user from User Provider backend"""
 
         # Import user provider defined in auth config
         user_provider: UserProvider = module.load(provider.module).object()
```

### Comparing `uvicore-0.2.0/uvicore/auth/authenticators/basic.py` & `uvicore-0.2.1/uvicore/auth/authenticators/basic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/authenticators/jwt.py` & `uvicore-0.2.1/uvicore/auth/authenticators/jwt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import uvicore
 from jwt import PyJWKClient, decode
+from uvicore.support.hash import md5
+from uvicore.contracts import UserInfo
 from uvicore.support.dumper import dump, dd
 from uvicore.http.request import HTTPConnection
 from uvicore.typing import Dict, Optional, Union, Callable
 from uvicore.auth.authenticators.base import Authenticator
 from uvicore.http.exceptions import NotAuthenticated, InvalidCredentials, HTTPException
-from uvicore.contracts import UserInfo
+
 
 @uvicore.service()
 class Jwt(Authenticator):
     """JWT bearer token authenticator"""
 
     # Notice:  Do not ever throw or return an error from authenticators.
     # If there is any auth problem (no headers, invalid or expired tokens, bad password)
@@ -127,71 +129,49 @@
                         self.log.debug('No audience found in allowed consumers')
                         return True
             except Exception as e:
                 self.log.debug('Issue decoding JWT without signature verification Ruturn True to denote Anonymous user and skip next authenticator')
                 self.log.debug(e)
                 return True
 
+        # Dump JWT to DEBUG log
         self.log.debug('JWT: ' + str(jwt))
-        #self.log.debug(jwt)
+
+        # Map JWT based on our auth configs JWT authenticator auto_create_user_jwt_mapping
+        mapped_jwt = {}
+        for key, value in self.config.auto_create_user_jwt_mapping.items():
+            if isinstance(value, Callable):
+                mapped_jwt[key] = value(jwt)
+            else:
+                mapped_jwt[key] = value
+
+        # Dump Mapped JWT to DEBUG log
+        self.log.debug('Mapped JWT: ' + str(mapped_jwt))
 
         # Get user and validate credentials
-        user: UserInfo = await self.retrieve_user(jwt.email, None, self.config.provider, request, jwt=jwt)
+        user: UserInfo = await self.retrieve_user(mapped_jwt['email'], None, self.config.provider, request, jwt=jwt)
 
         # User from valid JWT not found in uvicore OR not synced for first time (no uuid).
         # Auto create or update user if allowed in config
         if self.config.auto_create_user and (user is None or user.uuid is None):
-            jwt_mapping = self.config.auto_create_user_jwt_mapping
-            #dump(jwt_mapping)
-            new_user = {}
-            for key, value in self.config.auto_create_user_jwt_mapping.items():
-                if isinstance(value, Callable):
-                    new_user[key] = value(jwt)
-                else:
-                    new_user[key] = value
-
-            #dump(new_user)
-
             # User does not exist, create user
             if user is None:
                 # Auto create new user in user provider
-                await self.create_user(self.config.provider, request, **new_user)
-
+                await self.create_user(self.config.provider, request, **mapped_jwt)
             else:
                 # User exists, but needs an initial sync
-                await self.sync_user(self.config.provider, request, **new_user)
-
-            # Get user and validate credentials
-            user: User = await self.retrieve_user(jwt.email, None, self.config.provider, request, jwt=jwt)
+                await self.sync_user(self.config.provider, request, **mapped_jwt)
 
+            # Re-pull user after creation
+            user: UserInfo = await self.retrieve_user(mapped_jwt['email'], None, self.config.provider, request, jwt=jwt)
 
-            # Dict({
-            #     'aud': 'd709a432-5edc-44c7-8721-4cf123473c45',
-            #     'exp': 1616000280,
-            #     'iat': 1615996680,
-            #     'iss': 'https://auth-local.sunfinity.com',
-            #     'sub': '217e27b4-0e0a-464c-84a8-c40312b55801',
-            #     'authenticationType': 'PASSWORD',
-            #     'email': 'it@sunfinity.com',
-            #     'email_verified': True,
-            #     'applicationId': 'd709a432-5edc-44c7-8721-4cf123473c45',
-            #     'roles': ['Administrator'],
-            #     'name': 'Admin|Istrator'
-            # })
-
-
-        # If user is none and auto_create_user is enabled, auto-create user
-        # Link user up to groups table based on JWT roles
-        # Now self.get_user again
-
-        # If no user returned, validation has failed or user not found
-        #if user is None: raise InvalidCredentials()
-
-        # Validate Permissions
-        #self.validate_permissions(user, scopes.scopes)
-
-        # Authentication successful.
-        # Add user to request in case we use it in a decorator, we can pull it out with request.scope.get('user')
-        #request.scope['user'] = user
+        # Periodically sync user and group info from JWT
+        if (self.config.sync_user):
+            # Example cache key mreschke.wiki::cache/users/mreschke@example.com/sync_user_ttl
+            cache_key = "users/" + user.email + "/sync_user_ttl"
+            cache_ttl = self.config.sync_user_ttl
+            #if not await uvicore.cache.has(cache_key):
+            await self.sync_user(self.config.provider, request, **mapped_jwt)
+            await uvicore.cache.put(cache_key, 1, seconds=cache_ttl)
 
         # Return user.  If no user return True to denote Anonymous User and skip next authenticator
         return user or True
```

### Comparing `uvicore-0.2.0/uvicore/auth/config/package.py` & `uvicore-0.2.1/uvicore/auth/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/seeders/groups.py` & `uvicore-0.2.1/uvicore/auth/database/seeders/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/seeders/permissions.py` & `uvicore-0.2.1/uvicore/auth/database/seeders/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/seeders/roles.py` & `uvicore-0.2.1/uvicore/auth/database/seeders/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/seeders/users.py` & `uvicore-0.2.1/uvicore/auth/database/seeders/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/group_roles.py` & `uvicore-0.2.1/uvicore/auth/database/tables/group_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/groups.py` & `uvicore-0.2.1/uvicore/auth/database/tables/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/permissions.py` & `uvicore-0.2.1/uvicore/auth/database/tables/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/role_permissions.py` & `uvicore-0.2.1/uvicore/auth/database/tables/role_permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/roles.py` & `uvicore-0.2.1/uvicore/auth/database/tables/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/user_groups.py` & `uvicore-0.2.1/uvicore/auth/database/tables/user_groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/user_roles.py` & `uvicore-0.2.1/uvicore/auth/database/tables/user_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/database/tables/users.py` & `uvicore-0.2.1/uvicore/auth/database/tables/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/http/routes/api.py` & `uvicore-0.2.1/uvicore/auth/http/routes/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/middleware/auth_OLD.py` & `uvicore-0.2.1/uvicore/auth/middleware/auth_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/middleware/basic_OLD.py` & `uvicore-0.2.1/uvicore/auth/middleware/basic_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/middleware/jwt_OLD.py` & `uvicore-0.2.1/uvicore/auth/middleware/jwt_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/models/group.py` & `uvicore-0.2.1/uvicore/auth/models/group.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/models/permission.py` & `uvicore-0.2.1/uvicore/auth/models/permission.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/models/role.py` & `uvicore-0.2.1/uvicore/auth/models/role.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/models/user.py` & `uvicore-0.2.1/uvicore/auth/models/user.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/package/provider.py` & `uvicore-0.2.1/uvicore/auth/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/support/password.py` & `uvicore-0.2.1/uvicore/auth/support/password.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/user_info.py` & `uvicore-0.2.1/uvicore/auth/user_info.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/user_providers/jwt.py` & `uvicore-0.2.1/uvicore/auth/user_providers/jwt.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/auth/user_providers/orm.py` & `uvicore-0.2.1/uvicore/auth/user_providers/orm.py`

 * *Files 13% similar despite different names*

```diff
@@ -173,14 +173,19 @@
             await uvicore.cache.store(cache_store).put(cache_key, user)
 
         # Return to user
         return user
 
     async def create_user(self, request: HTTPConnection, **kwargs):
         """Create new user in backend"""
+
+        # Consistent kwargs come from our JWT auto_create_user_jwt_mapping config
+        # uuid, username, email, first_name, last_name
+        # title, avatar, creator_id, groups (array)
+
         # Pop groups from kwargs
         groups = kwargs.pop('groups')
 
         # Set other kwargs values
         kwargs['disabled'] = False
         kwargs['login_at'] = datetime.now()
 
@@ -199,20 +204,26 @@
         # Link real_groups
         await user.link('groups', real_groups)
 
         # Return new backend user (not actual Auth user class)
         return user
 
     async def sync_user(self, request: HTTPConnection, **kwargs):
-        """Sync user to backend"""
+        """Sync user and group linkage to backend"""
+        # Sync not only name changes, but also group linkage
+
+        # Consistent kwargs come from our JWT auto_create_user_jwt_mapping config
+        # uuid, username, email, first_name, last_name
+        # title, avatar, creator_id, groups (array)
+
         # Get username
         username = kwargs['username']
 
         # Get actual backend user
-        user = await UserModel.query().show_writeonly(['password']).find(username=username)
+        user = await UserModel.query().show_writeonly(['password']).include('groups').find(username=username)
 
         # If we have successfully logged in, we are not disabled
         user.disabled = False
         user.login_at = datetime.now()
 
         # Pop groups from kwargs
         groups = kwargs.pop('groups')
@@ -223,12 +234,37 @@
         # Translate avatar
         kwargs['avatar_url'] = kwargs.pop('avatar')
 
         # Add all other kwargs to user
         for key, value in kwargs.items():
             setattr(user, key, value)
 
-        # Save user
+        # Save user record
         await user.save()
 
+        # UNLINK any groups from DB that are not listed in groups JWT array
+        if groups and user.groups:
+            unlink_groups = []
+            for g in user.groups:
+                if g.name not in groups:
+                    unlink_groups.append(g)
+            if unlink_groups: await user.unlink('groups', unlink_groups)
+
+        # LINK any groups in JWT that are not linked in DB
+        if groups:
+            # Get actual groups in backend from groups array
+            real_groups = await Group.query().where('name', 'in', groups).get()
+            real_group_names = [x.name for x in real_groups]
+
+            # Convert users existing groups to list of names
+            user_group_names = []
+            if user.groups:
+                user_group_names = [x.name for x in user.groups]
+
+            link_groups = []
+            for g in real_groups:
+                if g.name not in user_group_names:
+                    link_groups.append(g)
+            if link_groups: await user.link('groups', link_groups)
+
         # Return new backend user (not actual Auth user class)
         return user
```

### Comparing `uvicore-0.2.0/uvicore/cache/backends/array.py` & `uvicore-0.2.1/uvicore/cache/backends/array.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/cache/backends/redis.py` & `uvicore-0.2.1/uvicore/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/cache/manager.py` & `uvicore-0.2.1/uvicore/cache/manager.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/cache/package/provider.py` & `uvicore-0.2.1/uvicore/cache/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/configuration/commands/config.py` & `uvicore-0.2.1/uvicore/configuration/commands/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/configuration/configuration.py` & `uvicore-0.2.1/uvicore/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/configuration/package/provider.py` & `uvicore-0.2.1/uvicore/configuration/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/__init__.py` & `uvicore-0.2.1/uvicore/console/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/LICENSE.rst` & `uvicore-0.2.1/uvicore/console/asyncclick/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/__init__.py` & `uvicore-0.2.1/uvicore/console/asyncclick/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_bashcomplete.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_compat.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_compat.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_termui_impl.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_textwrap.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_textwrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_unicodefun.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/_winconsole.py` & `uvicore-0.2.1/uvicore/console/asyncclick/_winconsole.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/core.py` & `uvicore-0.2.1/uvicore/console/asyncclick/core.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/decorators.py` & `uvicore-0.2.1/uvicore/console/asyncclick/decorators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/exceptions.py` & `uvicore-0.2.1/uvicore/console/asyncclick/exceptions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/formatting.py` & `uvicore-0.2.1/uvicore/console/asyncclick/formatting.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/globals.py` & `uvicore-0.2.1/uvicore/console/asyncclick/globals.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/parser.py` & `uvicore-0.2.1/uvicore/console/asyncclick/parser.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/termui.py` & `uvicore-0.2.1/uvicore/console/asyncclick/termui.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/testing.py` & `uvicore-0.2.1/uvicore/console/asyncclick/testing.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/types.py` & `uvicore-0.2.1/uvicore/console/asyncclick/types.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/asyncclick/utils.py` & `uvicore-0.2.1/uvicore/console/asyncclick/utils.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/click_colors.py` & `uvicore-0.2.1/uvicore/console/click_colors.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/commands/generators.py` & `uvicore-0.2.1/uvicore/console/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/commands/stubs/command.py` & `uvicore-0.2.1/uvicore/console/commands/stubs/command.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/console.py` & `uvicore-0.2.1/uvicore/console/console.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import uvicore
 from uvicore.console import click, group
 from uvicore.console.events import command as ConsoleEvents
 
 title_ideas = """
-    The Fullstack Asynchronous API+Web+CLI Python Framework
+    The Full Stack Asynchronous Python Framework with the performance of FastAPI and the elegance of Laravel!
 """
 
 # Must include actual bind name when stacking decorators as it cannot deduce on its own.
 # Bind decorator must come first in the stack
 @uvicore.service('uvicore.console.console.cli', aliases=['Console', 'console', 'cli'])
 @group(help=f"""
     \b
     Uvicore {uvicore.__version__}
     The Fullstack Async Web, API and CLI Python Framework
 
-    Copyright (c) 2023 Matthew Reschke
+    Copyright (c) 2024 Matthew Reschke
     License http://mreschke.com/license/mit
 """)
 @click.version_option(version=uvicore.__version__, prog_name='Uvicore Framework', flag_value='--d')
 @click.pass_context
 async def cli(ctx):
     # Console startup handler
     # This runs before any command.  Even if you don't actually run a command but only display
```

### Comparing `uvicore-0.2.0/uvicore/console/decorators.py` & `uvicore-0.2.1/uvicore/console/decorators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/events/command.py` & `uvicore-0.2.1/uvicore/console/events/command.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/package/bootstrap.py` & `uvicore-0.2.1/uvicore/console/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/package/provider.py` & `uvicore-0.2.1/uvicore/console/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/console/package/registers.py` & `uvicore-0.2.1/uvicore/console/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/container/commands/ioc.py` & `uvicore-0.2.1/uvicore/container/commands/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/container/ioc.py` & `uvicore-0.2.1/uvicore/container/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/__init__.py` & `uvicore-0.2.1/uvicore/contracts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from .config import Config
 from .connection import Connection
 from .database import Database
 from .dispatcher import Dispatcher
 #from .event import Event
 from .field import Field
 from .ioc import Binding, Ioc
+from .job_dispatcher import JobDispatcher
+from .job import Job
 from .logger import Logger
 from .mapper import Mapper
 from .model import Model
 from .package import Package
 from .provider import Provider
 from .relation import Relation
 #from .router import ApiRouter, WebRouter
```

### Comparing `uvicore-0.2.0/uvicore/contracts/application.py` & `uvicore-0.2.1/uvicore/contracts/application.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/authenticator.py` & `uvicore-0.2.1/uvicore/contracts/authenticator.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,12 +11,24 @@
 
     @abstractmethod
     async def authenticate(self, conn: HTTPConnection) -> Union[UserInfo, bool]:
         pass
 
     @abstractmethod
     async def retrieve_user(self, username: str, password: str, provider: Dict) -> Optional[UserInfo]:
+        """Retrieve user from User Provider backend"""
+        pass
+
+    @abstractmethod
+    async def create_user(self, provider: Dict, request: HTTPConnection, **kwargs):
+        """Create new user in backend"""
+        pass
+
+    @abstractmethod
+    async def sync_user(self, provider: Dict, request: HTTPConnection, **kwargs):
+        """Sync user and group linkage to backend"""
         pass
 
     @abstractmethod
     def auth_header(self, request) -> Tuple[str, str, str]:
+        """Extract authorization header parts"""
         pass
```

### Comparing `uvicore-0.2.0/uvicore/contracts/builder.py` & `uvicore-0.2.1/uvicore/contracts/builder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/cache.py` & `uvicore-0.2.1/uvicore/contracts/cache.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/config.py` & `uvicore-0.2.1/uvicore/contracts/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/connection.py` & `uvicore-0.2.1/uvicore/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/database.py` & `uvicore-0.2.1/uvicore/contracts/database.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/dispatcher.py` & `uvicore-0.2.1/uvicore/contracts/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,12 @@
         pass
 
     @abstractmethod
     async def dispatch_async(self, event: Any, payload = {}) -> None:
         """Fire off an event and run all async listener callbacks"""
         pass
 
+    @abstractmethod
     async def codispatch(self, event: Any, payload: Dict = {}) -> None:
         """Alias for dispatch_async()"""
         pass
```

### Comparing `uvicore-0.2.0/uvicore/contracts/event.py` & `uvicore-0.2.1/uvicore/contracts/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/field.py` & `uvicore-0.2.1/uvicore/contracts/field.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/ioc.py` & `uvicore-0.2.1/uvicore/contracts/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/logger.py` & `uvicore-0.2.1/uvicore/contracts/logger.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/mapper.py` & `uvicore-0.2.1/uvicore/contracts/mapper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/model.py` & `uvicore-0.2.1/uvicore/contracts/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/package.py` & `uvicore-0.2.1/uvicore/contracts/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/provider.py` & `uvicore-0.2.1/uvicore/contracts/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/relation.py` & `uvicore-0.2.1/uvicore/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/router.py` & `uvicore-0.2.1/uvicore/contracts/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/routes-OLD.py` & `uvicore-0.2.1/uvicore/contracts/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/server.py` & `uvicore-0.2.1/uvicore/contracts/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/template.py` & `uvicore-0.2.1/uvicore/contracts/template.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/user_info.py` & `uvicore-0.2.1/uvicore/contracts/user_info.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/contracts/user_provider.py` & `uvicore-0.2.1/uvicore/contracts/user_provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/__init__.py` & `uvicore-0.2.1/uvicore/database/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/builder.py` & `uvicore-0.2.1/uvicore/database/builder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/commands/db.py` & `uvicore-0.2.1/uvicore/database/commands/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/commands/generators.py` & `uvicore-0.2.1/uvicore/database/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/commands/stubs/seeder.py` & `uvicore-0.2.1/uvicore/database/commands/stubs/seeder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/commands/stubs/table.py` & `uvicore-0.2.1/uvicore/database/commands/stubs/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/db.py` & `uvicore-0.2.1/uvicore/database/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/package/bootstrap.py` & `uvicore-0.2.1/uvicore/database/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/package/provider.py` & `uvicore-0.2.1/uvicore/database/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/package/registers.py` & `uvicore-0.2.1/uvicore/database/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/query.py` & `uvicore-0.2.1/uvicore/database/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/database/table.py` & `uvicore-0.2.1/uvicore/database/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/events/commands/event.py` & `uvicore-0.2.1/uvicore/events/commands/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/events/dispatcher.py` & `uvicore-0.2.1/uvicore/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/events/event.py` & `uvicore-0.2.1/uvicore/events/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/exceptions/__init__.py` & `uvicore-0.2.1/uvicore/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/application.py` & `uvicore-0.2.1/uvicore/foundation/application.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/config/package.py` & `uvicore-0.2.1/uvicore/foundation/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/decorators/model.py` & `uvicore-0.2.1/uvicore/foundation/decorators/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/decorators/service.py` & `uvicore-0.2.1/uvicore/foundation/decorators/service.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/events/app.py` & `uvicore-0.2.1/uvicore/foundation/events/app.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/foundation/package/provider.py` & `uvicore-0.2.1/uvicore/foundation/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/OBSOLETE/router.py` & `uvicore-0.2.1/uvicore/http/OBSOLETE/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/OBSOLETE/routes-OLD.py` & `uvicore-0.2.1/uvicore/http/OBSOLETE/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/__init__.py` & `uvicore-0.2.1/uvicore/http/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/commands/generators.py` & `uvicore-0.2.1/uvicore/http/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/commands/serve.py` & `uvicore-0.2.1/uvicore/http/commands/serve.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/commands/stubs/api_controller.py` & `uvicore-0.2.1/uvicore/http/commands/stubs/api_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     # Optionally, apply scopes and also grab the current user
     # user: UserInfo = Guard(['authenticated'])
     #   Then in your routes, inject the user with
     #   async def welcome(request: Request, user: UserInfo = self.user):
 
     def register(self, route: ApiRouter):
+        """Register API Controller Endpoints"""
 
         # ----------------------------------------------------------------------
         # Example: Basic route responding with a view dict to JSON blob
         # ----------------------------------------------------------------------
         @route.get('/example1', tags=['Examples'])
         async def example1() -> Dict:
             """This docstring shows up in openapi"""
```

### Comparing `uvicore-0.2.0/uvicore/http/commands/stubs/composer.py` & `uvicore-0.2.1/uvicore/http/commands/stubs/composer.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/commands/stubs/controller.py` & `uvicore-0.2.1/uvicore/http/commands/stubs/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     # Optionally, apply scopes and also grab the current user
     # user: UserInfo = Guard(['authenticated'])
     #   Then in your routes, inject the user with
     #   async def welcome(request: Request, user: UserInfo = self.user):
 
     def register(self, route: WebRouter):
+        """Register Web Controller Endpoints"""
 
         # ----------------------------------------------------------------------
         # Example: Basic route responding with a view template
         # ----------------------------------------------------------------------
         # @route.get('/example1/{id}')
         # async def example1(request: Request, id: int):
         #     # Template should be in http/views/xx_appname/template.j2
```

### Comparing `uvicore-0.2.0/uvicore/http/controllers/api.py` & `uvicore-0.2.1/uvicore/http/controllers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/controllers/web.py` & `uvicore-0.2.1/uvicore/http/controllers/web.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/events/server.py` & `uvicore-0.2.1/uvicore/http/events/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/exceptions/__init__.py` & `uvicore-0.2.1/uvicore/http/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/exceptions/handlers.py` & `uvicore-0.2.1/uvicore/http/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/middleware/__init__.py` & `uvicore-0.2.1/uvicore/http/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/middleware/authentication.py` & `uvicore-0.2.1/uvicore/http/middleware/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         # Next global middleware in stack
         await self.app(scope, receive, send)
 
     async def retrieve_anonymous_user(self, request: HTTPConnection):
         """Retrieve anonymous user from User Provider backend"""
         # Import user provider defined in auth config
         provider_module = self.config.default_provider.module
+
         if provider_module in self.cached_providers:
             #dump('cached provider')
             user_provider = self.cached_providers[provider_module]
         else:
             #dump('UNcached provider')
             # Anonymous user provider is always the 'default_provider'
             # Load and instantiate just once, then cache the results, a huge boost for middleware!
```

### Comparing `uvicore-0.2.0/uvicore/http/openapi/docs.py` & `uvicore-0.2.1/uvicore/http/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/package/bootstrap.py` & `uvicore-0.2.1/uvicore/http/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/package/provider.py` & `uvicore-0.2.1/uvicore/http/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/package/registers.py` & `uvicore-0.2.1/uvicore/http/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/request.py` & `uvicore-0.2.1/uvicore/http/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
+from fastapi import UploadFile
 from fastapi.params import Security
 from uvicore.typing import Sequence, List
 from fastapi.security import SecurityScopes
 from uvicore.support.dumper import dump, dd
 from starlette.requests import Request, HTTPConnection
 from fastapi.params import Path, Query, Header, Cookie, Body, Form, File, Depends, Security
 
+
 class Parameter(Security):
     """Base class for user defined request parameters with infinite kwargs!"""
 
     # Parameters can accept any number of kwargs which are hacked as
     # a single "string" security scope converted to json then converted
     # back to an object before the handler is called
```

### Comparing `uvicore-0.2.0/uvicore/http/response.py` & `uvicore-0.2.1/uvicore/http/response.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/api_router.py` & `uvicore-0.2.1/uvicore/http/routing/api_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/auto_api.py` & `uvicore-0.2.1/uvicore/http/routing/auto_api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/guard.py` & `uvicore-0.2.1/uvicore/http/routing/guard.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/model_router.py` & `uvicore-0.2.1/uvicore/http/routing/model_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/router.py` & `uvicore-0.2.1/uvicore/http/routing/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/routing/web_router.py` & `uvicore-0.2.1/uvicore/http/routing/web_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/server.py` & `uvicore-0.2.1/uvicore/http/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/servers/api.py` & `uvicore-0.2.1/uvicore/http/servers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/static.py` & `uvicore-0.2.1/uvicore/http/static.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/status.py` & `uvicore-0.2.1/uvicore/http/status.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http/templating/context_functions.py` & `uvicore-0.2.1/uvicore/http/templating/context_functions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/http_client/package/provider.py` & `uvicore-0.2.1/uvicore/http_client/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/logging/logger.py` & `uvicore-0.2.1/uvicore/logging/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         self.reset()
 
     def critical(self, message):
         self.logger.critical(str(message))
         self.reset()
 
     def exception(self, message):
-        self.logger.exception(str(message))
+        self.logger.error(str(message))
         self.reset()
 
     def blank(self) -> LoggerInterface:
         self.logger.info('')
         self.reset()
 
     def nl(self) -> LoggerInterface:
```

### Comparing `uvicore-0.2.0/uvicore/logging/package/provider.py` & `uvicore-0.2.1/uvicore/logging/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/mail/__init__.py` & `uvicore-0.2.1/uvicore/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/mail/backends/mailgun.py` & `uvicore-0.2.1/uvicore/mail/backends/mailgun.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/mail/package/provider.py` & `uvicore-0.2.1/uvicore/mail/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/commands/generators.py` & `uvicore-0.2.1/uvicore/orm/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/commands/stubs/model.py` & `uvicore-0.2.1/uvicore/orm/commands/stubs/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/fields.py` & `uvicore-0.2.1/uvicore/orm/fields.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/mapper.py` & `uvicore-0.2.1/uvicore/orm/mapper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/metaclass.py` & `uvicore-0.2.1/uvicore/orm/metaclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
 @uvicore.service()
 class ModelMetaclass(PydanticMetaclass):
 
     # Testing of duplicate field
     # Only works if EACH model sets a metaclass=ModelMetaclass
     # You cannot set the metaclass at the Module.py level
-    def email(entity):
-        return 'email on meta'
+    # def email(entity):
+    #     return 'email on meta'
 
-    def slug(entity):
-        return 'slug on meta'
+    # def slug(entity):
+    #     return 'slug on meta'
 
 
     # Remember all metaclass method ARE @classmethods
     # Remember any method here DO NOT clash with pydantic field names
     # Remember any method here do NOT show up in code intellisense because its a metaclass
     #   If you want it in code intellisense, it must be in model.py and ModelInterface
     #   but then it WILL clash with any pydantic fields of the same name.
```

### Comparing `uvicore-0.2.0/uvicore/orm/model.py` & `uvicore-0.2.1/uvicore/orm/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/package/provider.py` & `uvicore-0.2.1/uvicore/orm/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/orm/query.py` & `uvicore-0.2.1/uvicore/orm/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/package/commands/package.py` & `uvicore-0.2.1/uvicore/package/commands/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/package/package.py` & `uvicore-0.2.1/uvicore/package/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/package/provider.py` & `uvicore-0.2.1/uvicore/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/redis/package/bootstrap.py` & `uvicore-0.2.1/uvicore/redis/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/redis/package/provider.py` & `uvicore-0.2.1/uvicore/redis/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/redis/redis.py` & `uvicore-0.2.1/uvicore/redis/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/collection.py` & `uvicore-0.2.1/uvicore/support/collection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/concurrency.py` & `uvicore-0.2.1/uvicore/support/concurrency.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/dictionary.py` & `uvicore-0.2.1/uvicore/support/dictionary.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/dumper.py` & `uvicore-0.2.1/uvicore/support/dumper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/module.py` & `uvicore-0.2.1/uvicore/support/module.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/path.py` & `uvicore-0.2.1/uvicore/support/path.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/schematic.py` & `uvicore-0.2.1/uvicore/support/schematic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/singleton.py` & `uvicore-0.2.1/uvicore/support/singleton.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/support/str.py` & `uvicore-0.2.1/uvicore/support/str.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/templating/engine.py` & `uvicore-0.2.1/uvicore/templating/engine.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/templating/package/bootstrap.py` & `uvicore-0.2.1/uvicore/templating/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/templating/package/provider.py` & `uvicore-0.2.1/uvicore/templating/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/templating/package/registers.py` & `uvicore-0.2.1/uvicore/templating/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/typing/__init__.py` & `uvicore-0.2.1/uvicore/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.0/uvicore/typing/dictionary.py` & `uvicore-0.2.1/uvicore/typing/dictionary.py`

 * *Files identical despite different names*

