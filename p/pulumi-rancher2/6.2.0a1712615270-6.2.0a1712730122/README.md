# Comparing `tmp/pulumi_rancher2-6.2.0a1712615270.tar.gz` & `tmp/pulumi_rancher2-6.2.0a1712730122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-6.2.0a1712615270.tar", last modified: Mon Apr  8 22:30:19 2024, max compression
+gzip compressed data, was "pulumi_rancher2-6.2.0a1712730122.tar", last modified: Wed Apr 10 06:46:25 2024, max compression
```

## Comparing `pulumi_rancher2-6.2.0a1712615270.tar` & `pulumi_rancher2-6.2.0a1712730122.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1391177 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    41229 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    27436 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45542 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)   167286 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    39652 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    31618 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/custom_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21643 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34584 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)  1818101 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    37937 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31939 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-08 22:30:19.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-08 22:30:19.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:30:19.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 22:30:19.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 22:30:19.000000 pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 22:30:11.000000 pulumi_rancher2-6.2.0a1712615270/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:30:19.357216 pulumi_rancher2-6.2.0a1712615270/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:46:25.369752 pulumi_rancher2-6.2.0a1712730122/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-10 06:46:25.369752 pulumi_rancher2-6.2.0a1712730122/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:46:25.369752 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1391177 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41229 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27436 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45542 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167286 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39652 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31618 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:46:25.369752 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21643 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34584 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1818101 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37937 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31939 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:46:25.369752 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-10 06:46:25.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-10 06:46:25.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:46:25.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 06:46:25.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 06:46:25.000000 pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 06:46:17.000000 pulumi_rancher2-6.2.0a1712730122/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:46:25.373752 pulumi_rancher2-6.2.0a1712730122/setup.cfg
```

### Comparing `pulumi_rancher2-6.2.0a1712615270/PKG-INFO` & `pulumi_rancher2-6.2.0a1712730122/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1712615270
+Version: 6.2.0a1712730122
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1712615270/README.md` & `pulumi_rancher2-6.2.0a1712730122/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/__init__.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/app.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/catalog.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/certificate.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/__init__.pyi` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/custom_user_token.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/custom_user_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/feature.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_app.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/get_user.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_role.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/namespace.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/node_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/notifier.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/outputs.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/provider.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/registry.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/role_template.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/secret.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/setting.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/token.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2/user.py` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1712615270
+Version: 6.2.0a1712730122
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1712615270/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-6.2.0a1712730122/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1712615270/pyproject.toml` & `pulumi_rancher2-6.2.0a1712730122/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rancher2"
   description = "A Pulumi package for creating and managing rancher2 resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rancher2"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1712615270"
+  version = "6.2.0a1712730122"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rancher2"
 
 [build-system]
```

