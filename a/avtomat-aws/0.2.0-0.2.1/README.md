# Comparing `tmp/avtomat_aws-0.2.0.tar.gz` & `tmp/avtomat_aws-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.2.0.tar", max compression
+gzip compressed data, was "avtomat_aws-0.2.1.tar", max compression
```

## Comparing `avtomat_aws-0.2.0.tar` & `avtomat_aws-0.2.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1285 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/LICENSE
--rw-r--r--   0        0        0     3838 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/README.md
--rw-r--r--   0        0        0       69 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      864 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      928 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1156 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1145 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1300 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      874 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_images.py
--rw-r--r--   0        0        0      711 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_snapshots.py
--rw-r--r--   0        0        0      855 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0     1020 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_instances.py
--rw-r--r--   0        0        0      718 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      688 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      834 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      513 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      522 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1244 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1410 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      675 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1442 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1203 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      522 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1389 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      960 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      884 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1251 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1131 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      824 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      887 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      791 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      781 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      509 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      732 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      763 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      766 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      746 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1262 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1364 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      583 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     4829 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1242 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      895 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1225 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1418 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      462 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      789 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      615 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/__init__.py
--rw-r--r--   0        0        0      203 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/set_output.py
--rw-r--r--   0        0        0     2083 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/table.py
--rw-r--r--   0        0        0      858 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/format_tags.py
--rw-r--r--   0        0        0      288 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2636 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      728 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3420 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3289 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1187 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2625 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     2512 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_images.py
--rw-r--r--   0        0        0     1988 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0    11038 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_instances.py
--rw-r--r--   0        0        0     1532 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     3012 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3599 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3330 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5204 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     3322 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4403 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3514 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      497 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1743 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1733 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/README.md
+-rw-r--r--   0        0        0       69 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      864 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      928 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1156 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1145 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1300 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      874 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_images.py
+-rw-r--r--   0        0        0      711 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      855 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0     1265 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_instances.py
+-rw-r--r--   0        0        0      718 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      688 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      834 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      513 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      522 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1244 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1410 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      675 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1442 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1203 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      522 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1389 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      960 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      884 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1251 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1131 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      824 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      887 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      791 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      781 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      509 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      732 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      763 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      766 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1262 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1364 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      583 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     4829 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1242 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      895 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1225 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1418 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      462 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/set_output.py
+-rw-r--r--   0        0        0     2083 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/table.py
+-rw-r--r--   0        0        0      858 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/format_tags.py
+-rw-r--r--   0        0        0      288 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3420 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3289 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1187 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     2512 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_images.py
+-rw-r--r--   0        0        0     1988 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0    12176 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_instances.py
+-rw-r--r--   0        0        0     1532 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     3012 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3599 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3330 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5204 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4403 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3514 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-10 20:09:13.234189 avtomat_aws-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.2.1/PKG-INFO
```

### Comparing `avtomat_aws-0.2.0/CHANGELOG.md` & `avtomat_aws-0.2.1/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## 0.2.1 (2024-04-10)
+
+### Fix
+
+- **ec2.delete_instances.discover_image_snapshots.exception**: Change image.image_id to image.id
+- **ec2.delete_instances.cli**: Revert the original cli interface
+- **ec2.delete_instances.discover_image_snapshots**: Skip snapshot retrieval for images not in 'available' state
+- **ec2.delete_instances**: Add 'disable_protections' parameter allowing disabling of termination and stop API protections before deletion
+
 ## 0.2.0 (2024-04-09)
 
 ### Feat
 
 - **ec2.delete_instances**: Add new action
 - **ec2.create_images**: Add new action
```

### Comparing `avtomat_aws-0.2.0/LICENSE` & `avtomat_aws-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/README.md` & `avtomat_aws-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_images.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 from avtomat_aws.helpers.cli.set_output import set_output
-from avtomat_aws.services.ec2 import delete_instances
+from avtomat_aws.services.ec2 import delete_volumes
 
-ACTION_DESCRIPTION = "Delete EC2 instances."
+ACTION_DESCRIPTION = "Delete EBS volumes."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
-        "--instance_ids",
+        "--volume_ids",
         nargs="+",
-        help="Instance IDs to delete, separated by space.",
+        help="Volume IDs to delete, separated by space.",
         required=True,
     )
     parser.add_argument(
-        "--include",
-        nargs="+",
-        help="Associated resource types to delete, separated by space.",
-        required=False,
-    )
-    parser.add_argument(
-        "--final_image",
+        "--snapshot",
         action="store_true",
-        help="Create an image (AMI) before deletion.",
+        help="Create snapshots before deletion.",
         required=False,
     )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = delete_instances(**inputs)
+        result = delete_volumes(**inputs)
         set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/s3/delete_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from avtomat_aws.helpers.cli.set_output import set_output
-from avtomat_aws.services.ec2 import delete_volumes
+from avtomat_aws.services.s3 import delete_objects
 
-ACTION_DESCRIPTION = "Delete EBS volumes."
+ACTION_DESCRIPTION = "Delete objects from an S3 bucket."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
-        "--volume_ids",
+        "--bucket", help="Name of the S3 bucket to delete objects from.", required=True
+    )
+    required.add_argument(
+        "--objects",
         nargs="+",
-        help="Volume IDs to delete, separated by space.",
+        help="Objects to delete, separated by space.",
         required=True,
     )
-    parser.add_argument(
-        "--snapshot",
-        action="store_true",
-        help="Create snapshots before deletion.",
-        required=False,
-    )
+    parser.add_argument("--prefix", help="Prefix to filter objects by.", required=False)
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = delete_volumes(**inputs)
+        result = delete_objects(**inputs)
         set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_active_regions.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/main.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/s3/discover_objects.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 from avtomat_aws.helpers.cli.set_output import set_output
-from avtomat_aws.services.s3 import delete_objects
+from avtomat_aws.services.s3 import discover_objects
 
-ACTION_DESCRIPTION = "Delete objects from an S3 bucket."
+ACTION_DESCRIPTION = "Discover objects in an S3 bucket."
 
 
 def add_cli_arguments(parser):
     """Argument parsing"""
 
     required = parser.add_argument_group("required")
 
     required.add_argument(
-        "--bucket", help="Name of the S3 bucket to delete objects from.", required=True
-    )
-    required.add_argument(
-        "--objects",
-        nargs="+",
-        help="Objects to delete, separated by space.",
-        required=True,
+        "--bucket", help="Name of the S3 bucket to discover objects in.", required=True
     )
     parser.add_argument("--prefix", help="Prefix to filter objects by.", required=False)
+    parser.add_argument(
+        "--modified_before",
+        help="Get objects last modified before date (YYYY/MM//DD).",
+        required=False,
+    )
+    parser.add_argument(
+        "--modified_after",
+        help="Get objects last modified after date (YYYY/MM//DD).",
+        required=False,
+    )
+    parser.add_argument(
+        "--name_only",
+        action="store_true",
+        help="Return only the object name, not the entire path.",
+        required=False,
+    )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
 
     try:
-        result = delete_objects(**inputs)
+        result = discover_objects(**inputs)
         set_output(result, inputs)
     except Exception as e:
         print(f"Action failed - {e}")
         exit(1)
```

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/services.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/services.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.2.1/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.2.1/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.2.1/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.2.1/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/helpers/cli/table.py` & `avtomat_aws-0.2.1/avtomat_aws/helpers/cli/table.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/helpers/format_tags.py` & `avtomat_aws-0.2.1/avtomat_aws/helpers/format_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.2.1/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.2.1/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.2.1/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.2.1/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_images.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "include": None,
     "final_image": False,
+    "disable_protections": False,
     "region": None,
     "debug": False,
     "silent": False,
 }
 RULES = [
     {"required": ["instance_ids"]},
     {
@@ -61,48 +62,54 @@
     # Gatekeeper: If no instances remain, return early
     if not instances:
         return failed
 
     # Discover associated resources before deletion
     associated_resources = {"Volumes": [], "Images": [], "Snapshots": []}
     if kwargs.get("include"):
+        logger.info(f"Discovering associated resources: {kwargs.get('include')}")
         if "volume" in kwargs.get("include"):
             associated_resources["Volumes"] = discover_volumes(instances)
         if "image" in kwargs.get("include"):
             associated_resources["Images"], associated_resources["Snapshots"] = (
                 discover_images(instances, session_objects["ec2_resource"])
             )
         if "snapshot" in kwargs.get("include"):
             if not associated_resources[
                 "Volumes"
             ]:  # If volume deletion wasn't requested (we still need volumes for snapshots)
                 associated_resources["Volumes"] = discover_volumes(instances)
             associated_resources["Snapshots"] += discover_snapshots(
                 associated_resources["Volumes"], session_objects["ec2_resource"]
             )  # We append instead of assign to avoid overwriting snapshots associated with images
-
-    logger.info(f"Deleting instances")
-    if kwargs.get("final_image"):
-        logger.info("Creating images before deletion")
+            associated_resources["Snapshots"] = list(
+                set(associated_resources["Snapshots"])
+            )  # Deduplicate
+
+    if kwargs.get("disable_protections"):
+        logger.info("Disabling API protections")
+        disable_protections(instances)
 
     running_instances_to_stop = []
+    logger.info("Stopping any running instances")
     for instance in instances:  # First concurrently stop all running instances.
         if instance.state["Name"] == "running":
             logger.info(f"{instance.id} - running, stopping before deletion")
             instance.stop()
             running_instances_to_stop.append(instance)
     for (
         instance
     ) in (
         running_instances_to_stop
     ):  # Then wait for them to stop. Avoids waiting per instance.
         instance.wait_until_stopped()
 
     images_to_wait = []
     if kwargs.get("final_image"):
+        logger.info("Creating images before deletion")
         for instance in instances[:]:  # Iterate over a shallow copy
             try:
                 # Generate random uuid as image names must be unique
                 uuid_str = str(uuid.uuid4())
                 image = instance.create_image(
                     Name=f"source_{instance.id}_{uuid_str}",
                     Description=f"Pre-deletion image of {instance.id}",
@@ -141,14 +148,15 @@
             )
             continue
 
     # Gatekeeper: If no instances remain, return early
     if not instances:
         return failed
 
+    logger.info(f"Deleting instances")
     for instance in instances[:]:  # Iterate over a shallow copy
         try:
             instance.terminate()
             logger.info(f"{instance.id} - deleted")
         except Exception as e:
             failed["Instances"].append(instance.id)
             instances.remove(instance)  # Modify the original list
@@ -166,49 +174,54 @@
                         logger.warning(f"{instance.id} - cleaned up {image.id}")
             continue
 
     # Gatekeeper: If no instances remain, return early
     if not instances:
         return failed
 
-    logger.info(f"{len(instances)} instances deleted")
-
-    if failed["Instances"]:
-        logger.warning(f"{len(failed['Instances'])} instances failed to delete")
-        logger.debug(failed["Instances"])
-
     time.sleep(
         5
     )  # Wait for a few seconds before attempting to delete associated resources
 
+    volumes_counter = 0
+    images_counter = 0
+    snapshots_counter = 0
     if kwargs.get("include"):
         logger.info(f"Deleting associated resources: {kwargs.get('include')}")
         if "volume" in kwargs.get("include"):
-            counter, volumes_failed = delete_volumes(associated_resources["Volumes"])
-            logger.info(f"{counter} volumes deleted")
-            if volumes_failed:
-                failed["Volumes"] = volumes_failed
-                logger.warning(f"{len(volumes_failed)} volumes failed to delete")
-                logger.debug(volumes_failed)
+            volumes_counter, failed["Volumes"] = delete_volumes(
+                associated_resources["Volumes"]
+            )
         if "image" in kwargs.get("include"):
-            counter, images_failed = delete_images(associated_resources["Images"])
-            logger.info(f"{counter} images deleted")
-            if images_failed:
-                failed["Images"] = images_failed
-                logger.warning(f"{len(images_failed)} images failed to delete")
-                logger.debug(images_failed)
+            images_counter, failed["Images"] = delete_images(
+                associated_resources["Images"]
+            )
         if "image" in kwargs.get("include") or "snapshot" in kwargs.get("include"):
-            counter, snapshots_failed = delete_snapshots(
+            snapshots_counter, failed["Snapshots"] = delete_snapshots(
                 associated_resources["Snapshots"]
             )
-            logger.info(f"{counter} snapshots deleted")
-            if snapshots_failed:
-                failed["Snapshots"] = snapshots_failed
-                logger.warning(f"{len(snapshots_failed)} snapshots failed to delete")
-                logger.debug(snapshots_failed)
+
+        # Provide a summary of deleted resources
+        logger.info(f"{len(instances)} instances deleted")
+        logger.info(f"{volumes_counter} volumes deleted")
+        logger.info(f"{images_counter} images deleted")
+        logger.info(f"{snapshots_counter} snapshots deleted")
+
+        if failed["Instances"]:
+            logger.warning(f"{len(failed['Instances'])} instances failed to delete")
+            logger.debug(failed["Instances"])
+        if failed["Volumes"]:
+            logger.warning(f"{len(failed['Volumes'])} volumes failed to delete")
+            logger.debug(failed["Volumes"])
+        if failed["Images"]:
+            logger.warning(f"{len(failed['Images'])} images failed to delete")
+            logger.debug(failed["Images"])
+        if failed["Snapshots"]:
+            logger.warning(f"{len(failed['Snapshots'])} snapshots failed to delete")
+            logger.debug(failed["Snapshots"])
 
     return failed
 
 
 def delete_volumes(volumes):
     """Delete all volumes associated with an instance"""
     counter = 0
@@ -275,15 +288,20 @@
     for image in ec2_resource.images.filter(
         Owners=["self"],
         Filters=[{"Name": "source-instance-id", "Values": instance_ids}],
     ):
         images.append(image)
     snapshots = []
     for image in images:
-        snapshots += discover_image_snapshots(image, ec2_resource)
+        if image.state == "available":
+            snapshots += discover_image_snapshots(image, ec2_resource)
+        else:
+            logger.warning(
+                f"{image.id} - not fully available, will skip snapshot deletion"
+            )
     return images, snapshots
 
 
 def discover_snapshots(volumes, ec2_resource):
     """Discover snapshots associated with volumes"""
     volume_ids = [volume.id for volume in volumes]
     snapshots = []
@@ -297,11 +315,22 @@
 def discover_image_snapshots(image, ec2_resource):
     """Discover snapshots associated with images"""
     snapshots = []
     for snapshot_id in image.block_device_mappings:
         try:
             snapshot = ec2_resource.Snapshot(snapshot_id["Ebs"]["SnapshotId"])
             snapshots.append(snapshot)
-        except ClientError as e:
-            logger.error(f"{snapshot_id} - failed to discover snapshot - {e}")
+        except Exception as e:
+            logger.error(f"{image.id} - failed to discover snapshots - {e}")
             continue
     return snapshots
+
+
+def disable_protections(instances):
+    """Disable termination and stop protections for instances"""
+    for instance in instances:
+        try:
+            instance.modify_attribute(DisableApiTermination={"Value": False})
+            instance.modify_attribute(DisableApiStop={"Value": False})
+            logger.info(f"{instance.id} - api protections disabled")
+        except Exception as e:
+            logger.error(f"{instance.id} - failed to disable api protections - {e}")
```

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.2.1/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.2.1/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.2.1/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.2.1/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.2.1/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.2.1/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/avtomat_aws/validations/rules.py` & `avtomat_aws-0.2.1/avtomat_aws/validations/rules.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.0/pyproject.toml` & `avtomat_aws-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.2.0"
+version = "0.2.1"
 description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.2.0/PKG-INFO` & `avtomat_aws-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.2.1 Summary: A collection of
 reusable Amazon Web Services actions, bringing speed and certainty to cloud
 operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

