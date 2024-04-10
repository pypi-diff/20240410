# Comparing `tmp/zscaler_pulumi_zia-0.0.5.tar.gz` & `tmp/zscaler_pulumi_zia-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_pulumi_zia-0.0.5.tar", last modified: Thu Mar 28 17:08:59 2024, max compression
+gzip compressed data, was "zscaler_pulumi_zia-0.0.6.tar", last modified: Wed Apr 10 07:00:14 2024, max compression
```

## Comparing `zscaler_pulumi_zia-0.0.5.tar` & `zscaler_pulumi_zia-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108384 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/activation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    56587 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/admin_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/auth_settings_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    50909 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_notification_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)   113986 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_web_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15037 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_application_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    26137 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    37263 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_network_services.py
--rw-r--r--   0 runner    (1001) docker     (127)   105422 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_source_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)   102057 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/forwarding_control_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/forwarding_control_zpa_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_activation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_admin_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_auth_settings_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_cbi_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_department_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_device_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_incident_receiver_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_notification_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_web_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpedm_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpidm_profile_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpidm_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_app_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_app_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_application_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_network_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_network_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    25304 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_source_ip_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    26783 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_forwarding_control_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_forwarding_control_zpa_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_group_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_icap_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_sandbox_behavioral_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_sandbox_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_security_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_time_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_internal_ip_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_node_vips.py
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_vip_recommended_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_vpn_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_url_filtering_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_workload_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)   107204 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)   259157 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/sandbox_behavioral_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/sandbox_file_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/security_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    37992 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    23784 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_vpn_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    59635 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)   105181 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/url_filtering_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    28305 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:08:59.704892 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 17:08:59.000000 zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:00:14.743365 zscaler_pulumi_zia-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-10 07:00:14.743365 zscaler_pulumi_zia-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:00:14.743365 zscaler_pulumi_zia-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:00:14.739365 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108384 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/activation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56587 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/auth_settings_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:00:14.743365 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50846 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_notification_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113986 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_web_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15037 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_application_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26137 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_destination_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37263 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_network_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105422 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_source_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102057 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/forwarding_control_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/forwarding_control_zpa_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_activation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_auth_settings_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_cbi_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_department_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_device_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_incident_receiver_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_notification_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_web_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpedm_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpidm_profile_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpidm_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_app_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_app_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_application_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_destination_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_network_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_network_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25304 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_source_ip_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26783 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_forwarding_control_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_forwarding_control_zpa_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_group_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_icap_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_rule_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_sandbox_behavioral_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_sandbox_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_security_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_time_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_internal_ip_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_node_vips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_vip_recommended_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_vpn_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_url_filtering_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_workload_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107204 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/location_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)   259157 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/rule_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/sandbox_behavioral_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/sandbox_file_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/security_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37992 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_gre_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23784 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_vpn_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59635 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105181 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/url_filtering_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28305 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:00:14.743365 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 07:00:14.000000 zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/top_level.txt
```

### Comparing `zscaler_pulumi_zia-0.0.5/PKG-INFO` & `zscaler_pulumi_zia-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler_pulumi_zia
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Pulumi package for creating and managing zia cloud resources.
 Home-page: https://www.zscaler.com
 License: MIT
 Project-URL: Repository, https://github.com/zscaler/pulumi-zia
 Keywords: pulumi zia zscaler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zscaler_pulumi_zia-0.0.5/README.md` & `zscaler_pulumi_zia-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/setup.py` & `zscaler_pulumi_zia-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "zia Pulumi Package - Development Version"
```

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/__init__.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/_inputs.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/_inputs.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/_utilities.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/_utilities.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/activation_status.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/activation_status.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/admin_users.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/admin_users.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/auth_settings_urls.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/auth_settings_urls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/config/vars.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/config/vars.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_dictionaries.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_dictionaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         :param pulumi.Input[str] confidence_threshold: The DLP confidence threshold. The following values are supported:
         :param pulumi.Input[str] custom_phrase_match_type: The DLP custom phrase match type. Supported values are:
         :param pulumi.Input[str] description: The desciption of the DLP dictionary
         :param pulumi.Input[int] dict_template_id: ID of the predefined dictionary (original source dictionary) that is used for cloning. This field is applicable only to cloned dictionaries. Only a limited set of identification-based predefined dictionaries (e.g., Credit Cards, Social Security Numbers, National Identification Numbers, etc.) can be cloned. Up to 4 clones can be created from a predefined dictionary.
         :param pulumi.Input[str] dictionary_type: The DLP dictionary type. The following values are supported:
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesExactDataMatchDetailArgs']]] exact_data_match_details: Exact Data Match (EDM) related information for custom DLP dictionaries.
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesIdmProfileMatchAccuracyArgs']]] idm_profile_match_accuracies: List of Indexed Document Match (IDM) profiles and their corresponding match accuracy for custom DLP dictionaries.
-        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         :param pulumi.Input[bool] include_bin_numbers: A true value denotes that the specified Bank Identification Number (BIN) values are included in the Credit Cards dictionary. A false value denotes that the specified BIN values are excluded from the Credit Cards dictionary. Note: This field is applicable only to the predefined Credit Cards dictionary and its clones.
         :param pulumi.Input[str] name: The DLP dictionary's name
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesPatternArgs']]] patterns: List containing the patterns used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesPhraseArgs']]] phrases: List containing the phrases used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[int] proximity: The DLP dictionary proximity length.
         """
         if bin_numbers is not None:
@@ -172,15 +172,15 @@
     def idm_profile_match_accuracies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DLPDictionariesIdmProfileMatchAccuracyArgs']]]]):
         pulumi.set(self, "idm_profile_match_accuracies", value)
 
     @property
     @pulumi.getter(name="ignoreExactMatchIdmDict")
     def ignore_exact_match_idm_dict(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         """
         return pulumi.get(self, "ignore_exact_match_idm_dict")
 
     @ignore_exact_match_idm_dict.setter
     def ignore_exact_match_idm_dict(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_exact_match_idm_dict", value)
 
@@ -269,15 +269,15 @@
         :param pulumi.Input[str] confidence_threshold: The DLP confidence threshold. The following values are supported:
         :param pulumi.Input[str] custom_phrase_match_type: The DLP custom phrase match type. Supported values are:
         :param pulumi.Input[str] description: The desciption of the DLP dictionary
         :param pulumi.Input[int] dict_template_id: ID of the predefined dictionary (original source dictionary) that is used for cloning. This field is applicable only to cloned dictionaries. Only a limited set of identification-based predefined dictionaries (e.g., Credit Cards, Social Security Numbers, National Identification Numbers, etc.) can be cloned. Up to 4 clones can be created from a predefined dictionary.
         :param pulumi.Input[str] dictionary_type: The DLP dictionary type. The following values are supported:
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesExactDataMatchDetailArgs']]] exact_data_match_details: Exact Data Match (EDM) related information for custom DLP dictionaries.
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesIdmProfileMatchAccuracyArgs']]] idm_profile_match_accuracies: List of Indexed Document Match (IDM) profiles and their corresponding match accuracy for custom DLP dictionaries.
-        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         :param pulumi.Input[bool] include_bin_numbers: A true value denotes that the specified Bank Identification Number (BIN) values are included in the Credit Cards dictionary. A false value denotes that the specified BIN values are excluded from the Credit Cards dictionary. Note: This field is applicable only to the predefined Credit Cards dictionary and its clones.
         :param pulumi.Input[str] name: The DLP dictionary's name
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesPatternArgs']]] patterns: List containing the patterns used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[Sequence[pulumi.Input['DLPDictionariesPhraseArgs']]] phrases: List containing the phrases used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[int] proximity: The DLP dictionary proximity length.
         """
         if bin_numbers is not None:
@@ -416,15 +416,15 @@
     def idm_profile_match_accuracies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DLPDictionariesIdmProfileMatchAccuracyArgs']]]]):
         pulumi.set(self, "idm_profile_match_accuracies", value)
 
     @property
     @pulumi.getter(name="ignoreExactMatchIdmDict")
     def ignore_exact_match_idm_dict(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         """
         return pulumi.get(self, "ignore_exact_match_idm_dict")
 
     @ignore_exact_match_idm_dict.setter
     def ignore_exact_match_idm_dict(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_exact_match_idm_dict", value)
 
@@ -560,15 +560,15 @@
         :param pulumi.Input[str] confidence_threshold: The DLP confidence threshold. The following values are supported:
         :param pulumi.Input[str] custom_phrase_match_type: The DLP custom phrase match type. Supported values are:
         :param pulumi.Input[str] description: The desciption of the DLP dictionary
         :param pulumi.Input[int] dict_template_id: ID of the predefined dictionary (original source dictionary) that is used for cloning. This field is applicable only to cloned dictionaries. Only a limited set of identification-based predefined dictionaries (e.g., Credit Cards, Social Security Numbers, National Identification Numbers, etc.) can be cloned. Up to 4 clones can be created from a predefined dictionary.
         :param pulumi.Input[str] dictionary_type: The DLP dictionary type. The following values are supported:
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesExactDataMatchDetailArgs']]]] exact_data_match_details: Exact Data Match (EDM) related information for custom DLP dictionaries.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesIdmProfileMatchAccuracyArgs']]]] idm_profile_match_accuracies: List of Indexed Document Match (IDM) profiles and their corresponding match accuracy for custom DLP dictionaries.
-        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         :param pulumi.Input[bool] include_bin_numbers: A true value denotes that the specified Bank Identification Number (BIN) values are included in the Credit Cards dictionary. A false value denotes that the specified BIN values are excluded from the Credit Cards dictionary. Note: This field is applicable only to the predefined Credit Cards dictionary and its clones.
         :param pulumi.Input[str] name: The DLP dictionary's name
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesPatternArgs']]]] patterns: List containing the patterns used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesPhraseArgs']]]] phrases: List containing the phrases used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[int] proximity: The DLP dictionary proximity length.
         """
         ...
@@ -711,15 +711,15 @@
         :param pulumi.Input[str] confidence_threshold: The DLP confidence threshold. The following values are supported:
         :param pulumi.Input[str] custom_phrase_match_type: The DLP custom phrase match type. Supported values are:
         :param pulumi.Input[str] description: The desciption of the DLP dictionary
         :param pulumi.Input[int] dict_template_id: ID of the predefined dictionary (original source dictionary) that is used for cloning. This field is applicable only to cloned dictionaries. Only a limited set of identification-based predefined dictionaries (e.g., Credit Cards, Social Security Numbers, National Identification Numbers, etc.) can be cloned. Up to 4 clones can be created from a predefined dictionary.
         :param pulumi.Input[str] dictionary_type: The DLP dictionary type. The following values are supported:
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesExactDataMatchDetailArgs']]]] exact_data_match_details: Exact Data Match (EDM) related information for custom DLP dictionaries.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesIdmProfileMatchAccuracyArgs']]]] idm_profile_match_accuracies: List of Indexed Document Match (IDM) profiles and their corresponding match accuracy for custom DLP dictionaries.
-        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        :param pulumi.Input[bool] ignore_exact_match_idm_dict: Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         :param pulumi.Input[bool] include_bin_numbers: A true value denotes that the specified Bank Identification Number (BIN) values are included in the Credit Cards dictionary. A false value denotes that the specified BIN values are excluded from the Credit Cards dictionary. Note: This field is applicable only to the predefined Credit Cards dictionary and its clones.
         :param pulumi.Input[str] name: The DLP dictionary's name
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesPatternArgs']]]] patterns: List containing the patterns used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DLPDictionariesPhraseArgs']]]] phrases: List containing the phrases used within a custom DLP dictionary. This attribute is not applicable to predefined DLP dictionaries. Required when `dictionary_type` is `PATTERNS_AND_PHRASES`
         :param pulumi.Input[int] proximity: The DLP dictionary proximity length.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -812,15 +812,15 @@
         """
         return pulumi.get(self, "idm_profile_match_accuracies")
 
     @property
     @pulumi.getter(name="ignoreExactMatchIdmDict")
     def ignore_exact_match_idm_dict(self) -> pulumi.Output[Optional[bool]]:
         """
-        Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         """
         return pulumi.get(self, "ignore_exact_match_idm_dict")
 
     @property
     @pulumi.getter(name="includeBinNumbers")
     def include_bin_numbers(self) -> pulumi.Output[bool]:
         """
```

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_engines.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_engines.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_notification_templates.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_notification_templates.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/dlp_web_rules.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/dlp_web_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_application_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_application_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_destination_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_destination_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_network_services.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_network_services.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_rule.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_service_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_service_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/firewall_filtering_source_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/firewall_filtering_source_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/forwarding_control_rule.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/forwarding_control_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/forwarding_control_zpa_gateway.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/forwarding_control_zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_activation_status.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_activation_status.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_admin_roles.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_admin_roles.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_admin_users.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_admin_users.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_auth_settings_urls.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_auth_settings_urls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_cbi_profile.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_cbi_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_department_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_department_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_device_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_device_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_devices.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_devices.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_dictionaries.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_dictionaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     def idm_profile_match_accuracies(self) -> Sequence['outputs.GetDLPDictionariesIdmProfileMatchAccuracyResult']:
         return pulumi.get(self, "idm_profile_match_accuracies")
 
     @property
     @pulumi.getter(name="ignoreExactMatchIdmDict")
     def ignore_exact_match_idm_dict(self) -> bool:
         """
-        (Boolean) Indicates whether to exclude documents that are a 100%!m(MISSING)atch to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
+        (Boolean) Indicates whether to exclude documents that are a 100% match to already-indexed documents from triggering an Indexed Document Match (IDM) Dictionary.
         """
         return pulumi.get(self, "ignore_exact_match_idm_dict")
 
     @property
     @pulumi.getter(name="includeBinNumbers")
     def include_bin_numbers(self) -> bool:
         """
```

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_engines.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_engines.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_incident_receiver_servers.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_incident_receiver_servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_notification_templates.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_notification_templates.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlp_web_rules.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlp_web_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpedm_schema.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpedm_schema.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpidm_profile_lite.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpidm_profile_lite.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_dlpidm_profiles.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_dlpidm_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_app_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_app_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_app_services.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_app_services.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_application.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_application.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_application_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_application_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_destination_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_destination_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_network_service_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_network_service_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_network_services.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_network_services.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_rule.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_firewall_filtering_source_ip_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_firewall_filtering_source_ip_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_forwarding_control_rule.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_forwarding_control_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_forwarding_control_zpa_gateway.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_forwarding_control_zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_group_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_group_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_icap_servers.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_icap_servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_lite.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_lite.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_location_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_location_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_rule_labels.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_rule_labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_sandbox_behavioral_analysis.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_sandbox_behavioral_analysis.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_sandbox_report.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_sandbox_report.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_security_settings.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_security_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_time_window.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_time_window.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_internal_ip_range.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_internal_ip_range.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel_info.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_gre_tunnel_info.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_node_vips.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_node_vips.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_static_ip.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_static_ip.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_vip_recommended_list.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_vip_recommended_list.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_traffic_forwarding_vpn_credentials.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_traffic_forwarding_vpn_credentials.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_url_categories.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_url_filtering_rules.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_url_filtering_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_user_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_user_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/get_workload_groups.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/get_workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/location_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/location_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/outputs.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/outputs.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/provider.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/provider.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/rule_labels.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/rule_labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/sandbox_behavioral_analysis.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/sandbox_behavioral_analysis.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/sandbox_file_submission.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/sandbox_file_submission.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/security_settings.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/security_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_gre_tunnel.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_gre_tunnel.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_static_ip.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_static_ip.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/traffic_forwarding_vpn_credentials.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/traffic_forwarding_vpn_credentials.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/url_categories.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/url_filtering_rules.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/url_filtering_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia/user_management.py` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia/user_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/PKG-INFO` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-pulumi-zia
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Pulumi package for creating and managing zia cloud resources.
 Home-page: https://www.zscaler.com
 License: MIT
 Project-URL: Repository, https://github.com/zscaler/pulumi-zia
 Keywords: pulumi zia zscaler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zscaler_pulumi_zia-0.0.5/zscaler_pulumi_zia.egg-info/SOURCES.txt` & `zscaler_pulumi_zia-0.0.6/zscaler_pulumi_zia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

