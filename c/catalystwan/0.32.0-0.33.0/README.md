# Comparing `tmp/catalystwan-0.32.0.tar.gz` & `tmp/catalystwan-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.32.0.tar", max compression
+gzip compressed data, was "catalystwan-0.33.0.tar", max compression
```

## Comparing `catalystwan-0.32.0.tar` & `catalystwan-0.33.0.tar`

### file list

```diff
@@ -1,334 +1,334 @@
--rw-r--r--   0        0        0    11375 2024-04-08 14:34:01.363267 catalystwan-0.32.0/LICENSE
--rw-r--r--   0        0        0    12394 2024-04-08 14:34:01.363267 catalystwan-0.32.0/README.md
--rw-r--r--   0        0        0     2524 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6369 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3105 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4301 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     4645 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    15767 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    28976 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    29260 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-04-08 14:34:01.363267 catalystwan-0.32.0/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3107 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5235 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-04-08 14:34:01.367267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1446 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4400 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5089 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    13671 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0    21558 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    26501 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1274 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     2554 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2770 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     4037 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2064 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4836 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     2028 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2091 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2092 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2247 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2324 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2174 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2032 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     2073 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2132 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     2039 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2159 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2104 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2263 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2186 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1793 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1950 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1870 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1827 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1911 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     2016 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1932 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2079 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1953 2024-04-08 14:34:01.371267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1974 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1932 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1890 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1953 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1874 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2115 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1848 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1974 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1781 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1946 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1845 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1926 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1926 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1787 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1806 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2672 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     3711 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    10675 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13948 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      819 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     4698 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    22618 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14040 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     6311 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/monitoring_device_details.py
--rw-r--r--   0        0        0     1929 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/monitoring_status.py
--rw-r--r--   0        0        0     1446 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1085 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1050 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     5929 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     2792 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     5747 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1902 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/logging.conf
--rw-r--r--   0        0        0     3079 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     1090 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0    10043 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9117 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0     5553 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1342 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1121 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      577 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1033 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      885 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      731 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1034 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1034 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1268 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
--rw-r--r--   0        0        0     2867 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1028 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5197 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0      925 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1581 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1177 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      759 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      738 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1182 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1496 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      801 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      691 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1131 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0      883 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1384 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0    14665 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     8961 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     3448 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-04-08 14:34:01.375267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0    13826 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0     2179 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      167 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1041 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      342 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0     4567 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     7598 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5540 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list.py
--rw-r--r--   0        0        0     5726 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py
--rw-r--r--   0        0        0    11851 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/control.py
--rw-r--r--   0        0        0     3861 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access.py
--rw-r--r--   0        0        0     3961 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access_ipv6.py
--rw-r--r--   0        0        0     3004 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/hub_and_spoke.py
--rw-r--r--   0        0        0     1184 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/mesh.py
--rw-r--r--   0        0        0     3454 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/qos_map.py
--rw-r--r--   0        0        0     1193 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/rewrite.py
--rw-r--r--   0        0        0    12252 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/rule_set.py
--rw-r--r--   0        0        0     2948 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/security_group.py
--rw-r--r--   0        0        0    13309 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/traffic_data.py
--rw-r--r--   0        0        0     1074 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/vpn_membership.py
--rw-r--r--   0        0        0     9345 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/definitions/zone_based_firewall.py
--rw-r--r--   0        0        0    10893 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/lists.py
--rw-r--r--   0        0        0    14613 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/lists_entries.py
--rw-r--r--   0        0        0     5558 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3525 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    31904 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1274 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     7100 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     2908 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9590 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/response.py
--rw-r--r--   0        0        0    19161 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/session.py
--rw-r--r--   0        0        0      401 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-04-08 14:34:01.379267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     4598 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     7945 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28154 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    34937 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0      894 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     5489 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7335 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14851 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6063 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4721 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    11346 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     8719 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      154 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     5066 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0    17168 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     9946 2024-04-08 14:34:01.383267 catalystwan-0.32.0/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      862 2024-04-08 14:34:01.387267 catalystwan-0.32.0/pyproject.toml
--rw-r--r--   0        0        0    15920 1970-01-01 00:00:00.000000 catalystwan-0.32.0/setup.py
--rw-r--r--   0        0        0    13521 1970-01-01 00:00:00.000000 catalystwan-0.32.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-04-10 08:01:34.170286 catalystwan-0.33.0/LICENSE
+-rw-r--r--   0        0        0    12406 2024-04-10 08:01:34.170286 catalystwan-0.33.0/README.md
+-rw-r--r--   0        0        0     2524 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3105 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0     2053 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4301 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     4645 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     1290 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py
+-rw-r--r--   0        0        0     7315 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    15767 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    28976 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    29260 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3107 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5235 2024-04-10 08:01:34.170286 catalystwan-0.33.0/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1446 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13671 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    25601 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     4037 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2064 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     4836 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     2028 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2091 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2092 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2247 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2324 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     2174 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2032 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     2073 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2132 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     2039 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2159 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     2104 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2263 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2186 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1793 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1950 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1848 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1870 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1827 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1911 2024-04-10 08:01:34.174286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     2016 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1932 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2079 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1806 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1953 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1974 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1932 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1890 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1953 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1848 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1874 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1806 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2115 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1848 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1974 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1781 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1946 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1845 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1806 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1926 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1926 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1787 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1806 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1782 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13948 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     5158 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    24922 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14040 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8132 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/monitoring_device_details.py
+-rw-r--r--   0        0        0     1929 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/monitoring_status.py
+-rw-r--r--   0        0        0     1446 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3582 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     5747 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1902 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/logging.conf
+-rw-r--r--   0        0        0     3079 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/common.py
+-rw-r--r--   0        0        0      171 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0     1090 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0    10043 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0     9117 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     1086 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
+-rw-r--r--   0        0        0     5553 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1342 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1121 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      577 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1033 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      885 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      731 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1034 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1268 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
+-rw-r--r--   0        0        0     2867 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1028 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5197 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0      925 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1581 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1177 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      759 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      738 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1182 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1496 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      801 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      691 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1131 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0      883 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     1384 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0    14665 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0     8961 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14020 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     3448 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     3835 2024-04-10 08:01:34.178286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     2777 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    14424 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     9128 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6575 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     7971 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24489 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10081 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3294 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     6725 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    11900 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     6391 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6993 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5179 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3790 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5294 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0    13826 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0     2179 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0      167 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1041 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0     4567 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     7598 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5540 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/access_control_list.py
+-rw-r--r--   0        0        0     5726 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py
+-rw-r--r--   0        0        0    11851 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/control.py
+-rw-r--r--   0        0        0     3861 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/device_access.py
+-rw-r--r--   0        0        0     3961 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/device_access_ipv6.py
+-rw-r--r--   0        0        0     3004 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/hub_and_spoke.py
+-rw-r--r--   0        0        0     1184 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/mesh.py
+-rw-r--r--   0        0        0     3454 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/qos_map.py
+-rw-r--r--   0        0        0     1193 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/rewrite.py
+-rw-r--r--   0        0        0    12252 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/rule_set.py
+-rw-r--r--   0        0        0     2948 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/security_group.py
+-rw-r--r--   0        0        0    13309 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/traffic_data.py
+-rw-r--r--   0        0        0     1074 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/vpn_membership.py
+-rw-r--r--   0        0        0     9345 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/definitions/zone_based_firewall.py
+-rw-r--r--   0        0        0    10893 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/lists.py
+-rw-r--r--   0        0        0    14613 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/lists_entries.py
+-rw-r--r--   0        0        0     5558 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3525 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    31904 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1274 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     7100 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     5239 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9300 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/response.py
+-rw-r--r--   0        0        0    19161 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/session.py
+-rw-r--r--   0        0        0      401 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-04-10 08:01:34.182286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     4598 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1756 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     7945 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28154 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    33583 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0      894 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     5489 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16472 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     5883 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15050 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    11346 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     8547 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      154 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     5066 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0    17168 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0     9946 2024-04-10 08:01:34.186286 catalystwan-0.33.0/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      862 2024-04-10 08:01:34.190286 catalystwan-0.33.0/pyproject.toml
+-rw-r--r--   0        0        0    15932 1970-01-01 00:00:00.000000 catalystwan-0.33.0/setup.py
+-rw-r--r--   0        0        0    13533 1970-01-01 00:00:00.000000 catalystwan-0.33.0/PKG-INFO
```

### Comparing `catalystwan-0.32.0/LICENSE` & `catalystwan-0.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/README.md` & `catalystwan-0.33.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -284,21 +284,21 @@
 
 ```python
 api = session.api.tenant_management
 # create tenants
 tenants = [
     Tenant(
         name="tenant1",
-        orgName="CiscoDevNet",
-        subDomain="alpha.bravo.net",
+        org_name="CiscoDevNet",
+        subdomain="alpha.bravo.net",
         desc="This is tenant for unit tests",
-        edgeConnectorEnable=True,
-        edgeConnectorSystemIp="172.16.255.81",
-        edgeConnectorTunnelInterfaceName="GigabitEthernet1",
-        wanEdgeForecast=1,
+        edge_connector_enable=True,
+        edge_connector_system_ip="172.16.255.81",
+        edge_connector_tunnel_interface_name="GigabitEthernet1",
+        wan_edge_forecast=1,
     )
 ]
 create_task = api.create(tenants)
 create_task.wait_for_completed()
 # list all tenants
 tenants_data = api.get_all()
 # pick tenant from list by name
```

#### html2text {}

```diff
@@ -92,19 +92,19 @@
 (name="new_resource_group").single_or_default() updated_resource_group =
 ResourceGroupUpdateRequest( id=resource_group.id, name=resource_group.name,
 desc="Custom Resource Group #1 with updated description and site ids", siteIds=
 [200] ) # switch to resource group view session.api.resource_groups.switch
 ("new_resource_group") # delete resource group
 session.api.resource_groups.delete(resource_group.id) ``` TTeennaanntt mmaannaaggeemmeenntt
 (click to expand) ```python api = session.api.tenant_management # create
-tenants tenants = [ Tenant( name="tenant1", orgName="CiscoDevNet",
-subDomain="alpha.bravo.net", desc="This is tenant for unit tests",
-edgeConnectorEnable=True, edgeConnectorSystemIp="172.16.255.81",
-edgeConnectorTunnelInterfaceName="GigabitEthernet1", wanEdgeForecast=1, ) ]
-create_task = api.create(tenants) create_task.wait_for_completed() # list all
+tenants tenants = [ Tenant( name="tenant1", org_name="CiscoDevNet",
+subdomain="alpha.bravo.net", desc="This is tenant for unit tests",
+edge_connector_enable=True, edge_connector_system_ip="172.16.255.81",
+edge_connector_tunnel_interface_name="GigabitEthernet1", wan_edge_forecast=1, )
+] create_task = api.create(tenants) create_task.wait_for_completed() # list all
 tenants tenants_data = api.get_all() # pick tenant from list by name tenant =
 tenants_data.filter(name="tenant1").single_or_default() # get selected tenant
 id tenant_id = tenant.tenant_id # get vsession id of selected tenant vsessionid
 = api.vsession_id(tenant_id) # delete tenant by ids delete_task = api.delete(
 [tenant_id]) delete_task.wait_for_completed() # others
 api.get_hosting_capacity_on_vsmarts() api.get_statuses() api.get_vsmart_mapping
 () ``` TTeennaanntt mmiiggrraattiioonn (click to expand) ```python from pathlib import Path
```

### Comparing `catalystwan-0.32.0/catalystwan/__init__.py` & `catalystwan-0.33.0/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/abstractions.py` & `catalystwan-0.33.0/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.0/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/administration.py` & `catalystwan-0.33.0/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/alarms_api.py` & `catalystwan-0.33.0/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/api_container.py` & `catalystwan-0.33.0/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/basic_api.py` & `catalystwan-0.33.0/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.0/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/config_group_api.py` & `catalystwan-0.33.0/catalystwan/api/config_group_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.0/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py` & `catalystwan-0.33.0/catalystwan/api/configuration_groups/parcels/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.0/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/device_action_api.py` & `catalystwan-0.33.0/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.0/catalystwan/api/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/logs_api.py` & `catalystwan-0.33.0/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.0/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.0/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/omp_api.py` & `catalystwan-0.33.0/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.0/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/parcel_api.py` & `catalystwan-0.33.0/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.0/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/policy_api.py` & `catalystwan-0.33.0/catalystwan/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.0/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/software_action_api.py` & `catalystwan-0.33.0/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.0/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/task_status_api.py` & `catalystwan-0.33.0/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/template_api.py` & `catalystwan-0.33.0/catalystwan/api/template_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/README.md` & `catalystwan-0.33.0/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.0/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.0/catalystwan/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.0/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.0/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.0/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.0/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.0/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.0/catalystwan/api/tenant_management_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             password (Optional[str]): Provider password if not provided current session password will be used
 
         Returns:
             Task: Object representing tenant deletion process
         """
         if password is None:
             password = self.session.password
-        delete_request = TenantBulkDeleteRequest(tenantIdList=tenant_id_list, password=password)
+        delete_request = TenantBulkDeleteRequest(tenant_id_list=tenant_id_list, password=password)
         task_id = self._endpoints.delete_tenant_async_bulk(delete_request).id
         return Task(self.session, task_id)
 
     def get_statuses(self) -> DataSequence[TenantStatus]:
         """Gets tenant statuses from vManage
 
         Returns:
@@ -101,15 +101,15 @@
             tenant_id (str): Tenant ID
             src_vsmart_uuid (str): Source vSmart uuid
             dst_vsmart_uuid (str): Destination vSmart uuid
         """
         self._endpoints.update_tenant_vsmart_placement(
             tenant_id=tenant_id,
             vsmart_placement_update_request=vSmartPlacementUpdateRequest(
-                srcvSmartUuid=src_vsmart_uuid, destvSmartUuid=dst_vsmart_uuid
+                src_vsmart_uuid=src_vsmart_uuid, dest_vsmart_uuid=dst_vsmart_uuid
             ),
         )
 
     def get_vsmart_mapping(self) -> vSmartTenantMap:
         """Gets vSmart to tenant mapping
 
         Returns:
```

### Comparing `catalystwan-0.32.0/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.0/catalystwan/api/tenant_migration_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         """Stores migration token as text file for given migration identifier.
         Should be executed on migration target.
 
         Args:
             migration_id (str): migration identifier (it is obtained after import tenant task is finished)
             download_path (Path): full download path containing a filename eg.: Path("/home/user/import-token.txt")
         """
-        params = MigrationTokenQueryParams(migrationId=migration_id)
+        params = MigrationTokenQueryParams(migration_id=migration_id)
         token = self.session.endpoints.tenant_migration.get_migration_token(params)
         with open(download_path, "w") as file:
             file.write(token)
 
     def migrate_network(self, token_file: Path) -> Task:
         """Starts migration procedure on migration origin.
```

### Comparing `catalystwan-0.32.0/catalystwan/api/versions_utils.py` & `catalystwan-0.33.0/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/dataclasses.py` & `catalystwan-0.33.0/catalystwan/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Cisco Systems, Inc. and its affiliates
 
 import datetime as dt
 from typing import List, Optional
 
 from attr import define, field  # type: ignore
-from pydantic.v1 import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.exceptions import RetrieveIntervalOutOfRange
 from catalystwan.utils.alarm_status import Severity
 from catalystwan.utils.certificate_status import ValidityPeriod
 from catalystwan.utils.colors import PrintColors
 from catalystwan.utils.creation_tools import FIELD_NAME, asdict, convert_attributes
 from catalystwan.utils.personality import Personality
@@ -500,24 +500,25 @@
 @define
 class SoftwareInstallTimeout(DataclassBase):
     download_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "downloadTimeoutInMin"})
     activate_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "activateTimeoutInMin"})
 
 
 class FeatureTemplatesTypes(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
     parent: str
     default: str
-    display_name: str = Field(alias="displayName")
+    display_name: str = Field(serialization_alias="displayName", validation_alias="displayName")
     name: str
-    type_class: str = Field(alias="typeClass")
+    type_class: str = Field(serialization_alias="typeClass", validation_alias="typeClass")
     description: str
     write_permission: bool
     read_permission: bool
-    helper_type: List[str] = Field(default=[], alias="helperType")
-    device_models: List[dict] = Field(default=[], alias="deviceModels")
+    helper_type: List[str] = Field(default=[], serialization_alias="helperType", validation_alias="helperType")
+    device_models: List[dict] = Field(default=[], serialization_alias="deviceModels", validation_alias="deviceModels")
 
 
 @define
 class ResourcePoolData(DataclassBase):
     """Endpoint: /resourcepool/resource/vpn"""
 
     tenant_id: str = field(metadata={FIELD_NAME: "tenantId"})
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.0/catalystwan/endpoints/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,15 @@
     Union,
     runtime_checkable,
 )
 from uuid import UUID
 
 from packaging.specifiers import SpecifierSet  # type: ignore
 from packaging.version import Version  # type: ignore
-from pydantic import BaseModel as BaseModelV2
-from pydantic.v1 import BaseModel as BaseModelV1
+from pydantic import BaseModel
 from typing_extensions import Annotated, get_args, get_origin
 
 from catalystwan.abstractions import APIEndpointClient, APIEndpointClientResponse
 from catalystwan.exceptions import APIEndpointError, APIRequestPayloadTypeError, APIVersionError, APIViewError
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.session_type import SessionType
 
@@ -77,20 +76,18 @@
 @runtime_checkable
 class CustomPayloadType(Protocol):
     def prepared(self) -> PreparedPayload:
         ...
 
 
 JSON = Union[str, int, float, bool, None, Dict[str, "JSON"], List["JSON"]]
-ModelPayloadType = Union[BaseModelV1, BaseModelV2, Sequence[BaseModelV1], Sequence[BaseModelV2]]
+ModelPayloadType = Union[BaseModel, Sequence[BaseModel]]
 PayloadType = Union[None, JSON, str, bytes, dict, ModelPayloadType, CustomPayloadType]
-ReturnType = Union[
-    None, JSON, bytes, str, dict, BaseModelV1, BaseModelV2, DataSequence[BaseModelV1], DataSequence[BaseModelV2]
-]
-RequestParamsType = Union[Dict[str, str], BaseModelV1, BaseModelV2]
+ReturnType = Union[None, JSON, bytes, str, dict, BaseModel, DataSequence[BaseModel]]
+RequestParamsType = Union[Dict[str, str], BaseModel]
 
 
 @dataclass
 class TypeSpecifier:
     """Holds type information extracted from signature. Common for payload and return values. Used for documentation"""
 
     present: bool
@@ -166,53 +163,44 @@
     @classmethod
     def _prepare_payload(cls, payload: PayloadType, force_json: bool = False) -> PreparedPayload:
         """Helper method to prepare data for sending based on type"""
         if force_json or isinstance(payload, dict):
             return PreparedPayload(data=json.dumps(payload), headers={"content-type": "application/json"})
         if isinstance(payload, (str, bytes)):
             return PreparedPayload(data=payload)
-        elif isinstance(payload, (BaseModelV1, BaseModelV2)):
+        elif isinstance(payload, (BaseModel)):
             return cls._prepare_basemodel_payload(payload)
         elif isinstance(payload, Sequence) and not isinstance(payload, (str, bytes)):
             return cls._prepare_sequence_payload(payload)  # type: ignore[arg-type]
             # offender is List[JSON] which is also a Sequence can be ignored as long as force_json is passed correctly
         elif isinstance(payload, CustomPayloadType):
             return payload.prepared()
         else:
             raise APIRequestPayloadTypeError(payload)
 
     @classmethod
-    def _prepare_basemodel_payload(cls, payload: Union[BaseModelV1, BaseModelV2]) -> PreparedPayload:
+    def _prepare_basemodel_payload(cls, payload: BaseModel) -> PreparedPayload:
         """Helper method to prepare BaseModel instance for sending"""
-        if isinstance(payload, BaseModelV1):
-            return PreparedPayload(
-                data=payload.json(exclude_none=True, by_alias=True), headers={"content-type": "application/json"}
-            )
         return PreparedPayload(
             data=payload.model_dump_json(exclude_none=True, by_alias=True), headers={"content-type": "application/json"}
         )
 
     @classmethod
-    def _prepare_sequence_payload(cls, payload: Iterable[Union[BaseModelV1, BaseModelV2]]) -> PreparedPayload:
+    def _prepare_sequence_payload(cls, payload: Iterable[BaseModel]) -> PreparedPayload:
         """Helper method to prepare sequences for sending"""
         items = []
         for item in payload:
-            if isinstance(item, BaseModelV1):
-                items.append(item.dict(exclude_none=True, by_alias=True))
-            elif isinstance(item, BaseModelV2):
-                items.append(item.model_dump(exclude_none=True, by_alias=True))
+            items.append(item.model_dump(exclude_none=True, by_alias=True))
         data = json.dumps(items)
         return PreparedPayload(data=data, headers={"content-type": "application/json"})
 
     @classmethod
     def _prepare_params(cls, params: RequestParamsType) -> Dict[str, Any]:
         """Helper method to prepare params for sending"""
-        if isinstance(params, BaseModelV1):
-            return params.dict(exclude_none=True, by_alias=True)
-        elif isinstance(params, BaseModelV2):
+        if isinstance(params, BaseModel):
             return params.model_dump(exclude_none=True, by_alias=True)
         return params
 
     def __init__(self, client: APIEndpointClient):
         self._client = client
         self._basepath = BASE_PATH
 
@@ -387,21 +375,21 @@
                 "use None annotation if function does not return any value"
             )
         if (type_origin := get_origin(annotation)) and isclass(type_origin) and issubclass(type_origin, DataSequence):
             if (
                 (type_args := get_args(annotation))
                 and (len(type_args) == 1)
                 and isclass(type_args[0])
-                and issubclass(type_args[0], (BaseModelV1, BaseModelV2))
+                and issubclass(type_args[0], BaseModel)
             ):
                 return TypeSpecifier(True, DataSequence, type_args[0])
             raise APIEndpointError(f"Expected: {ReturnType} but return type {annotation}")
         elif isclass(annotation):
             try:
-                if issubclass(annotation, (bytes, str, dict, BinaryIO, (BaseModelV1, BaseModelV2))):
+                if issubclass(annotation, (bytes, str, dict, BinaryIO, BaseModel)):
                     return TypeSpecifier(True, None, annotation)
                 raise APIEndpointError(f"Expected: {ReturnType} but return type {annotation}")
             except TypeError:
                 raise APIEndpointError(f"Expected: {ReturnType} but return type {annotation}")
         raise APIEndpointError(f"Expected: {ReturnType} but return type {annotation}")
 
     def specify_payload_type(self) -> TypeSpecifier:
@@ -433,46 +421,46 @@
                 # flake suggest using isinstance(arg, type(None)) above, but it doesn't match NoneType
                 if len(optional_type_args) == 1:
                     is_optional = True
                     annotation = optional_type_args[0]
 
         # Check if regular class
         if isclass(annotation):
-            if issubclass(annotation, (bytes, str, dict, BinaryIO, BaseModelV1, BaseModelV2, CustomPayloadType)):
+            if issubclass(annotation, (bytes, str, dict, BinaryIO, BaseModel, CustomPayloadType)):
                 return TypeSpecifier(True, None, annotation, None, False, is_optional)
             else:
                 raise APIEndpointError(f"'payload' param must be annotated with supported type: {PayloadType}")
 
         # Check for accepted alias types like List[...] and Union[...]
         elif type_origin := get_origin(annotation):
             # Check if Sequence[PayloadModelType] like List or DataSequence
             if isclass(type_origin) and issubclass(type_origin, Sequence):
                 if (
                     (type_args := get_args(annotation))
                     and (len(type_args) == 1)
                     and isclass(type_args[0])
-                    and issubclass(type_args[0], (BaseModelV1, BaseModelV2))
+                    and issubclass(type_args[0], BaseModel)
                 ):
                     return TypeSpecifier(True, type_origin, type_args[0], None, False, is_optional)
             # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
             elif type_origin == Annotated:
                 if annotated_origin := get_args(annotation):
                     if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
                         if (
                             (type_args := get_args(annotated_origin[0]))
                             and all(isclass(t) for t in type_args)
-                            and all(issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args)
+                            and all(issubclass(t, BaseModel) for t in type_args)
                         ):
                             return TypeSpecifier.model_union(models=list(type_args))
             # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
             elif type_origin == Union:
                 if (
                     (type_args := get_args(annotation))
                     and all(isclass(t) for t in type_args)
-                    and all(issubclass(t, (BaseModelV1, BaseModelV2)) for t in type_args)
+                    and all(issubclass(t, BaseModel) for t in type_args)
                 ):
                     return TypeSpecifier.model_union(models=list(type_args))
             raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
         else:
             raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
 
     def check_params(self):
@@ -480,18 +468,15 @@
 
         Raises:
             APIEndpointError: when decorated params not matching specification
         """
         parameters = self.sig.parameters
 
         if params_param := parameters.get("params"):
-            if not (
-                isclass(params_param.annotation)
-                and issubclass(params_param.annotation, (BaseModelV1, BaseModelV2, Dict))
-            ):
+            if not (isclass(params_param.annotation) and issubclass(params_param.annotation, (BaseModel, Dict))):
                 raise APIEndpointError(f"'params' param must be annotated with supported type: {RequestParamsType}")
 
         general_purpose_arg_names = {
             key for key in self.sig.parameters.keys() if key not in self.forbidden_url_field_names
         }
         if missing := self.url_field_names.difference(general_purpose_arg_names):
             raise APIEndpointError(f"Missing parameters: {missing} to format url: {self.url}")
@@ -574,15 +559,15 @@
                         if isinstance(full_json, dict):
                             return full_json.get(self.resp_json_key)
                         else:
                             raise TypeError(f"Expected dictionary as json payload but found: {type(full_json)}")
                     return full_json
                 if self.return_spec.payload_type is None:
                     pass
-                elif issubclass(self.return_spec.payload_type, (BaseModelV1, BaseModelV2)):
+                elif issubclass(self.return_spec.payload_type, BaseModel):
                     if self.return_spec.sequence_type == DataSequence:
                         return response.dataseq(self.return_spec.payload_type, self.resp_json_key)
                     else:
                         return response.dataobj(self.return_spec.payload_type, self.resp_json_key)
                 elif issubclass(self.return_spec.payload_type, str):
                     return response.text
                 elif issubclass(self.return_spec.payload_type, bytes):
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.0/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.0/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.0/catalystwan/endpoints/cluster_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
+from typing import Literal, Optional
 
-from enum import Enum
-from typing import Optional
-
-from pydantic.v1 import BaseModel
+from pydantic import BaseModel
 
 from catalystwan.endpoints import APIEndpoints, get
 from catalystwan.typed_list import DataSequence
 
-
-class TenancyModeEnum(str, Enum):
-    st = "SingleTenant"
-    mt = "MultiTenant"
+TenancyModes = Literal["SingleTenant", "MultiTenant"]
 
 
 class TenancyMode(BaseModel):
-    mode: TenancyModeEnum
+    mode: TenancyModes
     deploymentmode: str
     domain: Optional[str] = None
     clusterid: Optional[str] = None
 
 
 class VManageDetails(BaseModel):
     service: str
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from datetime import datetime
 from typing import List, Optional
 
-from pydantic.v1 import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.common import Solution
 from catalystwan.models.configuration.feature_profile.common import ProfileType
 from catalystwan.typed_list import DataSequence
 
 
@@ -21,23 +21,24 @@
     name: str
     description: str
     solution: Solution
     profiles: Optional[List[ProfileId]]
 
 
 class FeatureProfile(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
     id: str
     name: str
     description: Optional[str]
     solution: str
     type: ProfileType
-    created_by: str = Field(alias="createdBy")
-    last_updated_by: str = Field(alias="lastUpdatedBy")
-    created_on: datetime = Field(alias="createdOn")
-    last_updated_on: datetime = Field(alias="lastUpdatedOn")
+    created_by: str = Field(serialization_alias="createdBy", validation_alias="createdBy")
+    last_updated_by: str = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
+    created_on: datetime = Field(serialization_alias="createdOn", validation_alias="createdOn")
+    last_updated_on: datetime = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
 
 
 class ConfigGroup(BaseModel):
     name: str
     description: Optional[str]
     solution: Solution
     profiles: Optional[List[FeatureProfile]]
@@ -69,21 +70,25 @@
 
 class VariableData(BaseModel):
     name: str
     value: str
 
 
 class DeviceVariables(BaseModel):
-    device_id: str = Field(alias="device-id")
+    model_config = ConfigDict(populate_by_name=True)
+    device_id: str = Field(serialization_alias="device-id", validation_alias="device-id")
     variables: List[VariableData]
 
 
 class GroupVariables(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
     name: str
-    group_variables: List[VariableData] = Field(alias="group-variables")
+    group_variables: List[VariableData] = Field(
+        serialization_alias="group-variables", validation_alias="group-variables"
+    )
 
 
 class ConfigGroupVariablesCreateResponse(BaseModel):
     family: Solution
     devices: List[DeviceVariables]
     groups: List[GroupVariables]
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.0/catalystwan/endpoints/configuration_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,339 +1,337 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 import datetime
-from enum import Enum
 from typing import List, Literal, Optional, Union
 
-from pydantic.v1 import BaseModel, Field, IPvAnyAddress, validator
+from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, field_validator
 
 from catalystwan.endpoints import JSON, APIEndpoints, get, post, put, view
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.session_type import ProviderView, SingleTenantView
 
-
-class ModeEnum(str, Enum):
-    ON = "on"
-    OFF = "off"
-
-
-class DataStreamIPTypeEnum(str, Enum):
-    SYSTEM = "systemIp"
-    MGMT = "mgmtIp"
-    TRANSPORT = "transportIp"
-
-
-class PasswordPolicyEnum(str, Enum):
-    DISABLED = "disabled"
-    MEDIUM = "mediumSecurity"
-    HIGH = "highSecurity"
-
-
-class SmartLicensingSettingModeEnum(str, Enum):
-    ONPREM = "on-prem"
-    OFFLINE = "offline"
-    ONLINE = "online"
-
-
-class CRLActionEnum(str, Enum):
-    DISABLE = "disable"
-    REVOKE = "revoke"
-    QUARANTINE = "quarantine"
+OnOffMode = Literal["on", "off"]
+DataStreamIPTypes = Literal["systemIp", "mgmtIp", "transportIp"]
+PasswordPolicies = Literal["disabled", "mediumSecurity", "highSecurity"]
+SmartLicensingSettingModes = Literal["on-prem", "offline", "online"]
+CRLActions = Literal["disable", "revoke", "quarantine"]
 
 
 class Organization(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     org: Optional[str] = Field(default=None)
-    domain_id: Optional[str] = Field(alias="domain-id")
-    control_connection_up: Optional[bool] = Field(alias="controlConnectionUp")
+    domain_id: Optional[str] = Field(serialization_alias="domain-id", validation_alias="domain-id")
+    control_connection_up: Optional[bool] = Field(
+        serialization_alias="controlConnectionUp", validation_alias="controlConnectionUp"
+    )
 
 
 class Device(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    domain_ip: Optional[str] = Field(default=None, alias="domainIp")
+    model_config = ConfigDict(populate_by_name=True)
+    domain_ip: Optional[str] = Field(default=None, serialization_alias="domainIp", validation_alias="domainIp")
     port: Optional[str] = Field(default="12346")
 
 
 class EmailNotificationSettings(BaseModel):
     enabled: Optional[bool] = False
 
 
 class HardwareRootCA(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    hardware_certificate: Optional[str] = Field(default=None, alias="hardwareCertificate")
-    control_connection_up: Optional[bool] = Field(default=False, alias="controlConnectionUp")
+    model_config = ConfigDict(populate_by_name=True)
+    hardware_certificate: Optional[str] = Field(
+        default=None, serialization_alias="hardwareCertificate", validation_alias="hardwareCertificate"
+    )
+    control_connection_up: Optional[bool] = Field(
+        default=False, serialization_alias="controlConnectionUp", validation_alias="controlConnectionUp"
+    )
 
 
 class Certificate(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    certificate_signing: str = Field(alias="certificateSigning")
-    validity_period: str = Field(alias="validityPeriod")
-    retrieve_interval: str = Field(alias="retrieveInterval")
-    first_name: Optional[str] = Field(default=None, alias="firstName")
-    last_name: Optional[str] = Field(default=None, alias="lastName")
+    model_config = ConfigDict(populate_by_name=True)
+    certificate_signing: str = Field(serialization_alias="certificateSigning", validation_alias="certificateSigning")
+    validity_period: str = Field(serialization_alias="validityPeriod", validation_alias="validityPeriod")
+    retrieve_interval: str = Field(serialization_alias="retrieveInterval", validation_alias="retrieveInterval")
+    first_name: Optional[str] = Field(default=None, serialization_alias="firstName", validation_alias="firstName")
+    last_name: Optional[str] = Field(default=None, serialization_alias="lastName", validation_alias="lastName")
     email: Optional[str] = Field(default=None)
 
 
 class VEdgeCloud(BaseModel):
     certificateauthority: Optional[str] = None
 
 
 class Banner(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    mode: Optional[ModeEnum] = ModeEnum.OFF
-    banner_detail: Optional[str] = Field(alias="bannerDetail")
+    model_config = ConfigDict(populate_by_name=True)
+    mode: Optional[OnOffMode] = "off"
+    banner_detail: Optional[str] = Field(serialization_alias="bannerDetail", validation_alias="bannerDetail")
 
 
 class ProxyHTTPServer(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     proxy: bool
-    proxy_ip: str = Field(default="", alias="proxyIp")
-    proxy_port: str = Field(default="", alias="proxyPort")
+    proxy_ip: str = Field(default="", serialization_alias="proxyIp", validation_alias="proxyIp")
+    proxy_port: str = Field(default="", serialization_alias="proxyPort", validation_alias="proxyPort")
 
 
 class ReverseProxy(BaseModel):
-    mode: Optional[ModeEnum] = ModeEnum.OFF
+    mode: Optional[OnOffMode] = "off"
 
 
 class CloudX(BaseModel):
-    mode: Optional[ModeEnum] = ModeEnum.OFF
+    mode: Optional[OnOffMode] = "off"
 
 
 class ManageEncryptedPassword(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    manage_type8_password: Optional[bool] = Field(default=False, alias="manageType8Password")
+    model_config = ConfigDict(populate_by_name=True)
+    manage_type8_password: Optional[bool] = Field(
+        default=False, serialization_alias="manageType8Password", validation_alias="manageType8Password"
+    )
 
 
 class CloudServices(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     enabled: Optional[bool] = False
-    vanalytics_enabled: Optional[bool] = Field(default=False, alias="vanalyticsEnabled")
-    vmonitoring_enabled: Optional[bool] = Field(default=False, alias="vmonitoringEnabled")
+    vanalytics_enabled: Optional[bool] = Field(
+        default=False, serialization_alias="vanalyticsEnabled", validation_alias="vanalyticsEnabled"
+    )
+    vmonitoring_enabled: Optional[bool] = Field(
+        default=False, serialization_alias="vmonitoringEnabled", validation_alias="vmonitoringEnabled"
+    )
     otp: Optional[str] = None
-    cloud_gateway_url: Optional[str] = Field(default=None, alias="cloudGatewayUrl")
-    vanalytics_enabled_time: Optional[datetime.datetime] = Field(default=None, alias="vanalyticsEnabledTime")
-    vmonitoring_enabled_time: Optional[datetime.datetime] = Field(default=None, alias="vmonitoringEnabledTime")
+    cloud_gateway_url: Optional[str] = Field(
+        default=None, serialization_alias="cloudGatewayUrl", validation_alias="cloudGatewayUrl"
+    )
+    vanalytics_enabled_time: Optional[datetime.datetime] = Field(
+        default=None, serialization_alias="vanalyticsEnabledTime", validation_alias="vanalyticsEnabledTime"
+    )
+    vmonitoring_enabled_time: Optional[datetime.datetime] = Field(
+        default=None, serialization_alias="vmonitoringEnabledTime", validation_alias="vmonitoringEnabledTime"
+    )
 
 
 class ClientSessionTimeout(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    is_enabled: Optional[bool] = Field(default=False, alias="isEnabled")
+    model_config = ConfigDict(populate_by_name=True)
+    is_enabled: Optional[bool] = Field(default=False, serialization_alias="isEnabled", validation_alias="isEnabled")
     timeout: Optional[int] = Field(default=None, ge=10, description="timeout in minutes")
 
 
 class SessionLifeTime(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    session_life_time: int = Field(alias="sessionLifeTime", ge=30, le=10080, description="lifetime in minutes")
+    model_config = ConfigDict(populate_by_name=True)
+    session_life_time: int = Field(
+        serialization_alias="sessionLifeTime",
+        validation_alias="sessionLifeTime",
+        ge=30,
+        le=10080,
+        description="lifetime in minutes",
+    )
 
 
 class ServerSessionTimeout(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    server_session_timeout: int = Field(alias="serverSessionTimeout", ge=10, le=30, description="timeout in minutes")
+    model_config = ConfigDict(populate_by_name=True)
+    server_session_timeout: int = Field(
+        serialization_alias="serverSessionTimeout",
+        validation_alias="serverSessionTimeout",
+        ge=10,
+        le=30,
+        description="timeout in minutes",
+    )
 
 
 class MaxSessionsPerUser(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    max_sessions_per_user: int = Field(alias="maxSessionsPerUser", ge=1, le=8)
+    model_config = ConfigDict(populate_by_name=True)
+    max_sessions_per_user: int = Field(
+        serialization_alias="maxSessionsPerUser", validation_alias="maxSessionsPerUser", ge=1, le=8
+    )
 
 
 class PasswordPolicy(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    password_policy: Union[bool, PasswordPolicyEnum] = Field(alias="passwordPolicy")
+    model_config = ConfigDict(populate_by_name=True)
+    password_policy: Union[bool, PasswordPolicies] = Field(
+        serialization_alias="passwordPolicy", validation_alias="passwordPolicy"
+    )
     password_expiration_time: Optional[int] = Field(
-        default=False, alias="passwordExpirationTime", ge=1, le=90, description="timeout in days"
+        default=False,
+        serialization_alias="passwordExpirationTime",
+        validation_alias="passwordExpirationTime",
+        ge=1,
+        le=90,
+        description="timeout in days",
     )
 
 
 class VManageDataStream(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     enable: Optional[bool] = False
-    ip_type: Optional[DataStreamIPTypeEnum] = Field(default=None, alias="ipType")
-    server_host_name: Union[IPvAnyAddress, DataStreamIPTypeEnum, None] = Field(default=None, alias="serverHostName")
+    ip_type: Optional[DataStreamIPTypes] = Field(default=None, serialization_alias="ipType", validation_alias="ipType")
+    server_host_name: Union[IPvAnyAddress, DataStreamIPTypes, None] = Field(
+        default=None, serialization_alias="serverHostName", validation_alias="serverHostName"
+    )
     vpn: Optional[int] = Field(default=None, le=512)
 
 
 class DataCollectionOnNotification(BaseModel):
     enabled: bool
 
 
 class SDWANTelemetry(BaseModel):
     enabled: bool
 
 
 class StatsOperation(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    stats_operation: str = Field(alias="statsOperation")
-    rid: int = Field(alias="@rid")
-    operation_interval: int = Field(alias="operationInterval", ge=1, description="interval in minutes")
-    default_interval: int = Field(alias="defaultInterval", ge=1, description="interval in minutes")
+    model_config = ConfigDict(populate_by_name=True)
+    stats_operation: str = Field(serialization_alias="statsOperation", validation_alias="statsOperation")
+    rid: int = Field(serialization_alias="@rid", validation_alias="@rid")
+    operation_interval: int = Field(
+        serialization_alias="operationInterval",
+        validation_alias="operationInterval",
+        ge=1,
+        description="interval in minutes",
+    )
+    default_interval: int = Field(
+        serialization_alias="defaultInterval",
+        validation_alias="defaultInterval",
+        ge=1,
+        description="interval in minutes",
+    )
 
 
 class MaintenanceWindow(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     enabled: Optional[bool] = False
     message: Optional[str] = ""
-    start: Optional[int] = Field(default=None, alias="epochStartTimeInMillis")
-    end: Optional[int] = Field(default=None, alias="epochEndTimeInMillis")
+    start: Optional[int] = Field(
+        default=None, serialization_alias="epochStartTimeInMillis", validation_alias="epochStartTimeInMillis"
+    )
+    end: Optional[int] = Field(
+        default=None, serialization_alias="epochEndTimeInMillis", validation_alias="epochEndTimeInMillis"
+    )
 
 
 class ElasticSearchDBSize(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    index_name: str = Field(alias="indexName")
-    size_in_gb: int = Field(alias="sizeInGB")
+    model_config = ConfigDict(populate_by_name=True)
+    index_name: str = Field(serialization_alias="indexName", validation_alias="indexName")
+    size_in_gb: int = Field(serialization_alias="sizeInGB", validation_alias="sizeInGB")
 
 
 class GoogleMapKey(BaseModel):
     key: str
 
 
 class SoftwareInstallTimeout(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    download_timeout: str = Field(alias="downloadTimeoutInMin")
-    activate_timeout: str = Field(alias="activateTimeoutInMin")
-    control_pps: Optional[str] = Field(alias="controlPps")
+    model_config = ConfigDict(populate_by_name=True)
+    download_timeout: str = Field(serialization_alias="downloadTimeoutInMin", validation_alias="downloadTimeoutInMin")
+    activate_timeout: str = Field(serialization_alias="activateTimeoutInMin", validation_alias="activateTimeoutInMin")
+    control_pps: Optional[str] = Field(serialization_alias="controlPps", validation_alias="controlPps")
 
-    @validator("download_timeout")
+    @field_validator("download_timeout")
     def check_download_timeout(cls, download_timeout_str: str):
         download_timeout = int(download_timeout_str)
         if download_timeout < 60 or download_timeout > 360:
             raise ValueError("download timeout should be in range 60-360")
         return download_timeout_str
 
-    @validator("activate_timeout")
+    @field_validator("activate_timeout")
     def check_activate_timeout(cls, activate_timeout_str: str):
         activate_timeout = int(activate_timeout_str)
         if activate_timeout < 30 or activate_timeout > 180:
             raise ValueError("activate timeout should be in range 30-180")
         return activate_timeout_str
 
-    @validator("control_pps")
+    @field_validator("control_pps")
     def check_control_pps(cls, control_pps_str: str):
         control_pps = int(control_pps_str)
         if control_pps < 300 or control_pps > 65535:
             raise ValueError("control pps should be in range 300-65535")
         return control_pps_str
 
 
 class IPSSignatureSettings(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    is_enabled: Optional[bool] = Field(default=False, alias="isEnabled")
+    model_config = ConfigDict(populate_by_name=True)
+    is_enabled: Optional[bool] = Field(default=False, serialization_alias="isEnabled", validation_alias="isEnabled")
     username: Optional[str] = None
     update_interval: Optional[int] = Field(
-        default=None, alias="updateInterval", description="interval in minutes", ge=1, le=1440
+        default=None,
+        serialization_alias="updateInterval",
+        validation_alias="updateInterval",
+        description="interval in minutes",
+        ge=1,
+        le=1440,
     )
 
 
 class SmartAccountCredentials(BaseModel):
     username: Optional[str] = None
     password: Optional[str] = None
 
 
 class PnPConnectSync(BaseModel):
-    mode: Optional[ModeEnum] = ModeEnum.OFF
+    mode: Optional[OnOffMode] = "off"
 
 
 class ClaimDevice(BaseModel):
     enabled: bool
 
 
 class WalkMe(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
+    model_config = ConfigDict(populate_by_name=True)
     walkme: bool
-    walkme_analytics: bool = Field(alias="walkmeAnalytics")
+    walkme_analytics: bool = Field(serialization_alias="walkmeAnalytics", validation_alias="walkmeAnalytics")
 
 
 class SmartLicensingSetting(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    mode: Optional[SmartLicensingSettingModeEnum] = None
-    ssm_server_url: Optional[str] = Field(None, alias="ssmServerUrl")
-    ssm_client_id: Optional[str] = Field(None, alias="ssmClientId")
-    ssm_client_secret: Optional[str] = Field(None, alias="ssmClientSecret")
+    model_config = ConfigDict(populate_by_name=True)
+    mode: Optional[SmartLicensingSettingModes] = None
+    ssm_server_url: Optional[str] = Field(None, serialization_alias="ssmServerUrl", validation_alias="ssmServerUrl")
+    ssm_client_id: Optional[str] = Field(None, serialization_alias="ssmClientId", validation_alias="ssmClientId")
+    ssm_client_secret: Optional[str] = Field(
+        None, serialization_alias="ssmClientSecret", validation_alias="ssmClientSecret"
+    )
 
 
 class StatsCollectionInterval(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    config_name: Literal["statsCollection"] = Field(default="statsCollection", alias="configName")
+    model_config = ConfigDict(populate_by_name=True)
+    config_name: Literal["statsCollection"] = Field(
+        default="statsCollection", serialization_alias="configName", validation_alias="configName"
+    )
     operation_interval: int = Field(
-        ge=5, le=180, alias="operationInterval", desctiption="collecion interval in minutes"
+        ge=5,
+        le=180,
+        serialization_alias="operationInterval",
+        validation_alias="operationInterval",
+        description="collecion interval in minutes",
     )
 
 
 StatsConfigItem = Union[StatsCollectionInterval, None]  # open for extension for now only one option could be deduced
 
 
 class StatsConfig(BaseModel):
     config: List[StatsConfigItem]
 
     @staticmethod
     def from_collection_interval(interval: int) -> "StatsConfig":
-        return StatsConfig(config=[StatsCollectionInterval(operationInterval=interval)])
+        return StatsConfig(config=[StatsCollectionInterval(operation_interval=interval)])
 
 
 class CRLSettings(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-
-    action: CRLActionEnum
-    crl_url: Optional[str] = Field(None, alias="crlUrl")
+    model_config = ConfigDict(populate_by_name=True)
+    action: CRLActions
+    crl_url: Optional[str] = Field(None, serialization_alias="crlUrl", validation_alias="crlUrl")
     polling_interval: Optional[str] = Field(description="Retrieval interval (1-24 hours)")
     vpn: Optional[str]
 
-    @validator("polling_interval")
+    @field_validator("polling_interval")
     def check_polling_interval(cls, polling_interval_str: str):
         polling_interval = int(polling_interval_str)
         if polling_interval < 1 or polling_interval > 24:
             raise ValueError("Polling interval should be in range 1-24")
         return polling_interval_str
 
-    @validator("vpn")
+    @field_validator("vpn")
     def check_vpn(cls, vpn_str: str):
         vpn = int(vpn_str)
         if vpn < 0 or vpn > 65530:
             raise ValueError("vpn should be in range 0-65530")
         return vpn_str
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.0/catalystwan/endpoints/endpoints_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/misc.py` & `catalystwan-0.33.0/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/monitoring_status.py` & `catalystwan-0.33.0/catalystwan/endpoints/monitoring_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.0/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.0/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 
 from typing import Optional
 
-from pydantic.v1 import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints import APIEndpoints, get
 
 
 class CloudConnector(BaseModel):
-    cloud_enabled: Optional[bool] = Field(default=False, alias="cloudEnabled")
-    client_id: Optional[str] = Field(default=None, alias="clientId")
-    client_secret: Optional[str] = Field(default=None, alias="clientSecret")
-    org_name: Optional[str] = Field(default=None, alias="orgName")
+    model_config = ConfigDict(populate_by_name=True)
+    cloud_enabled: Optional[bool] = Field(
+        default=False, serialization_alias="cloudEnabled", validation_alias="cloudEnabled"
+    )
+    client_id: Optional[str] = Field(default=None, serialization_alias="clientId", validation_alias="clientId")
+    client_secret: Optional[str] = Field(
+        default=None, serialization_alias="clientSecret", validation_alias="clientSecret"
+    )
+    org_name: Optional[str] = Field(default=None, serialization_alias="orgName", validation_alias="orgName")
     affinity: Optional[str] = None
-    telemetry_enabled: Optional[bool] = Field(default=None, alias="telemetryEnabled")
+    telemetry_enabled: Optional[bool] = Field(
+        default=None, serialization_alias="telemetryEnabled", validation_alias="telemetryEnabled"
+    )
 
 
 class SDAVCCloudConnector(APIEndpoints):
     def disable_cloud_connector(self):
         # PUT /sdavc/cloudconnector
         ...
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.0/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import List
 
-from pydantic.v1 import BaseModel
+from pydantic import BaseModel
 
 from catalystwan.endpoints import APIEndpoints, get, view
 from catalystwan.utils.session_type import ProviderAsTenantView, TenantView
 
 
 class BackupFiles(BaseModel):
     backup_files: List[str]
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.0/catalystwan/endpoints/tenant_migration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from pathlib import Path
-from urllib.parse import parse_qsl, urlsplit
+from typing import Any
+from urllib.parse import parse_qs, urlsplit
 
-from pydantic.v1 import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.endpoints import APIEndpoints, CustomPayloadType, PreparedPayload, get, post, versions, view
 from catalystwan.models.tenant import TenantExport
 from catalystwan.utils.session_type import ProviderView, SingleTenantView
 
 
 class MigrationTokenQueryParams(BaseModel):
-    migration_id: str = Field(alias="migrationId")
+    model_config = ConfigDict(populate_by_name=True, extra="allow")
+    migration_id: str = Field(serialization_alias="migrationId", validation_alias="migrationId")
+
+    @model_validator(mode="before")
+    @classmethod
+    def single_migration_id_required(cls, values: Any):
+        migration_id = values.get("migrationId")
+        if isinstance(migration_id, list) and len(migration_id) == 1:
+            values["migrationId"] = migration_id[0]
+        return values
 
 
 class ExportInfo(BaseModel):
-    process_id: str = Field(alias="processId")
+    model_config = ConfigDict(populate_by_name=True)
+    process_id: str = Field(serialization_alias="processId", validation_alias="processId")
 
 
 class ImportInfo(BaseModel):
-    process_id: str = Field(alias="processId")
-    migration_token_url: str = Field(alias="migrationTokenURL")
+    model_config = ConfigDict(populate_by_name=True)
+    process_id: str = Field(serialization_alias="processId", validation_alias="processId")
+    migration_token_url: str = Field(serialization_alias="migrationTokenURL", validation_alias="migrationTokenURL")
 
     @property
     def migration_token_query(self) -> str:
         return urlsplit(self.migration_token_url).query
 
     @property
     def migration_token_query_params(self) -> MigrationTokenQueryParams:
-        query = self.migration_token_query
-        return MigrationTokenQueryParams.parse_obj(parse_qsl(query))
+        return MigrationTokenQueryParams.model_validate(parse_qs(self.migration_token_query))
 
 
 class MigrationInfo(BaseModel):
-    process_id: str = Field(alias="processId")
+    model_config = ConfigDict(populate_by_name=True)
+    process_id: str = Field(serialization_alias="processId", validation_alias="processId")
 
 
 class MigrationFile(CustomPayloadType):
     def __init__(self, filename: Path):
         self.filename = filename
 
     def prepared(self) -> PreparedPayload:
```

### Comparing `catalystwan-0.32.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/exceptions.py` & `catalystwan-0.33.0/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.0/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/logging.conf` & `catalystwan-0.33.0/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/common.py` & `catalystwan-0.33.0/catalystwan/models/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.33.0/catalystwan/models/configuration/config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/device_inventory.py` & `catalystwan-0.33.0/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.0/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.0/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.0/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/control.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/device_access_ipv6.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/hub_and_spoke.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/mesh.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/qos_map.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/rewrite.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/rule_set.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/security_group.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/traffic_data.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/vpn_membership.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/definitions/zone_based_firewall.py` & `catalystwan-0.33.0/catalystwan/models/policy/definitions/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/lists.py` & `catalystwan-0.33.0/catalystwan/models/policy/lists.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/lists_entries.py` & `catalystwan-0.33.0/catalystwan/models/policy/lists_entries.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/localized.py` & `catalystwan-0.33.0/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/policy.py` & `catalystwan-0.33.0/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.0/catalystwan/models/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.0/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/models/policy/security.py` & `catalystwan-0.33.0/catalystwan/models/policy/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/response.py` & `catalystwan-0.33.0/catalystwan/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from datetime import datetime
 from email.utils import parsedate_to_datetime
 from functools import wraps
 from pprint import pformat
 from typing import Any, Callable, Dict, Optional, Sequence, Type, TypeVar, Union, cast
 from urllib.parse import urlparse
 
-from pydantic import BaseModel as BaseModelV2
-from pydantic.v1 import BaseModel as BaseModelV1
+from pydantic import BaseModel
 from requests import PreparedRequest, Request, Response
 from requests.cookies import RequestsCookieJar
 from requests.exceptions import JSONDecodeError
 
 from catalystwan import with_proc_info_header
 from catalystwan.abstractions import APIEndpointClientResponse
 from catalystwan.exceptions import ManagerErrorInfo
@@ -174,15 +173,15 @@
         if history:
             return response_history_debug(self, None)
         return response_debug(self, None)
 
     def dataseq(self, cls: Type[T], sourcekey: Optional[str] = "data") -> DataSequence[T]:
         """Returns data contents from JSON payload parsed as DataSequence of Dataclass/BaseModel instances
         Args:
-            cls: Dataclass/BaseModelV1 subtype (eg. Devices)
+            cls: Dataclass/BaseModel subtype (eg. Devices)
             sourcekey: name of the JSON key from response payload to be parsed. If None whole JSON payload will be used
 
         Returns:
             DataSequence[T] of given type T which is subclassing from Dataclass/BaseModel,
             in case JSON payload was containing a single Object - sequence with one element is returned
         """
         if sourcekey is None:
@@ -191,17 +190,15 @@
             data = self.payload.json.get(sourcekey)
 
         if isinstance(data, Sequence):
             sequence = data
         else:
             sequence = [cast(dict, data)]
 
-        if issubclass(cls, BaseModelV1):
-            return DataSequence(cls, [cls.parse_obj(item) for item in sequence])  # type: ignore
-        if issubclass(cls, BaseModelV2):
+        if issubclass(cls, BaseModel):
             return DataSequence(cls, [cls.model_validate(item) for item in sequence])  # type: ignore
         return DataSequence(cls, [create_dataclass(cls, item) for item in sequence])
 
     def dataobj(self, cls: Type[T], sourcekey: Optional[str] = "data") -> T:
         """Returns data contents from JSON payload parsed as Dataclass/BaseModel instance
         Args:
             cls: Dataclass/BaseModel subtype (eg. Devices)
@@ -212,18 +209,16 @@
 
         """
         if sourcekey is None:
             data = self.payload.json
         else:
             data = self.payload.json.get(sourcekey)
 
-        if issubclass(cls, BaseModelV1):
-            return cls.parse_obj(data)  # type: ignore
-        if issubclass(cls, BaseModelV2):
-            return cls.model_validate(data)  # type: ignore
+        if issubclass(cls, BaseModel):
+            return cls.model_validate(data)  # type: ignore[return-value]
         return create_dataclass(cls, data)
 
     def get_error_info(self) -> ManagerErrorInfo:
         """Returns error information from JSON payload"""
 
         if self.payload.error is None:
             return ManagerErrorInfo(
```

### Comparing `catalystwan-0.32.0/catalystwan/session.py` & `catalystwan-0.33.0/catalystwan/session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.0/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.0/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.0/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.0/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.0/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.0/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.0/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.0/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.0/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_administration.py` & `catalystwan-0.33.0/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.0/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.0/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.0/catalystwan/tests/test_endpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from typing import Dict, List, Literal, Optional, Union
 from unittest.mock import MagicMock
 from uuid import UUID, uuid4
 
 import pytest  # type: ignore
 from packaging.version import Version  # type: ignore
 from parameterized import parameterized  # type: ignore
-from pydantic import BaseModel as BaseModelV2
-from pydantic import Field as FieldV2
-from pydantic.v1 import BaseModel as BaseModelV1
+from pydantic import BaseModel, Field
 from typing_extensions import Annotated
 
 from catalystwan.endpoints import (
     BASE_PATH,
     JSON,
     APIEndpoints,
     CustomPayloadType,
@@ -31,39 +29,27 @@
 from catalystwan.endpoints import logger as endpoints_logger
 from catalystwan.endpoints import post, put, request, versions, view
 from catalystwan.exceptions import APIEndpointError, APIRequestPayloadTypeError, APIVersionError, APIViewError
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.session_type import ProviderAsTenantView, ProviderView, TenantView
 
 
-class BaseModelV1Example(BaseModelV1):
+class BaseModelExample(BaseModel):
     id: str
     size: int
     capacity: float
     active: bool
 
 
-class ParamsModelV1Example(BaseModelV1):
-    name: str
-    color: str
-
-
-class BaseModelV2Example(BaseModelV2):
-    id: str
-    size: int
-    capacity: float
-    active: bool
-
-
-class BaseModelV2Example2(BaseModelV2):
+class BaseModelExample2(BaseModel):
     other_id: str
     active: bool
 
 
-class ParamsModelV2Example(BaseModelV2):
+class ParamsModelExample(BaseModel):
     name: str
     color: str
 
 
 class CustomTypeExample(CustomPayloadType):
     def __init__(self, filename: Path):
         self.filename = filename
@@ -84,25 +70,22 @@
         self.dict_payload = {
             "id": "XYZ-189",
             "size": 100,
             "capacity": 1.7,
             "active": True,
         }
         self.json_payload = json.dumps(self.dict_payload)
-        self.basemodel_v1_payload = BaseModelV1Example.parse_obj(self.dict_payload)
-        self.basemodel_v2_payload = BaseModelV2Example.model_validate(self.dict_payload)
+        self.basemodel_payload = BaseModelExample.model_validate(self.dict_payload)
         self.list_dict_payload = [self.dict_payload] * 2
         self.dict_params = {
             "name": "purple",
             "color": "haze",
         }
-        self.basemodel_v1_params = ParamsModelV1Example.parse_obj(self.dict_params)
-        self.basemodel_v2_params = ParamsModelV2Example.model_validate(self.dict_params)
-        self.basemodel_v1_sequence_payload = [self.basemodel_v1_payload] * 2
-        self.basemodel_v2_sequence_payload = [self.basemodel_v2_payload] * 2
+        self.basemodel_params = ParamsModelExample.model_validate(self.dict_params)
+        self.basemodel_sequence_payload = [self.basemodel_payload] * 2
 
     @parameterized.expand(
         [
             ("<2.0", "1.9.9"),
             (">=1.9, !=3.0", "3.1"),
             (">0.9, <=1.3", "1.3"),
         ]
@@ -199,33 +182,23 @@
         api = ExampleAPI(self.session_mock)
         with self.assertLogs(endpoints_logger, level="WARNING") as log:
             api.versions_decorated_method()
             for allowed in allowed_sessions:
                 assert str(allowed) in log.output[0]
             assert str(current_session) in log.output[0]
 
-    def test_basemodel_v1_payload(self):
-        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_v1_payload)
-        _, kwargs = self.session_mock.request.call_args
-        assert json.loads(kwargs.get("data")) == self.dict_payload
-
     @pytest.mark.filterwarnings("ignore::DeprecationWarning")
-    def test_basemodel_v2_payload(self):
-        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_v2_payload)
+    def test_basemodel_payload(self):
+        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_payload)
         _, kwargs = self.session_mock.request.call_args
         assert json.loads(kwargs.get("data")) == self.dict_payload
 
-    def test_basemodel_v1_sequence_payload(self):
-        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_v1_sequence_payload)
-        _, kwargs = self.session_mock.request.call_args
-        assert json.loads(kwargs.get("data")) == self.list_dict_payload
-
     @pytest.mark.filterwarnings("ignore::DeprecationWarning")
-    def test_basemodel_v2_sequence_payload(self):
-        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_v2_sequence_payload)
+    def test_basemodel_sequence_payload(self):
+        self.endpoints._request("GET", f"/{__name__}", payload=self.basemodel_sequence_payload)
         _, kwargs = self.session_mock.request.call_args
         assert json.loads(kwargs.get("data")) == self.list_dict_payload
 
     def test_custom_payload(self):
         expected_data = b"\xFFsomething\x00"
         with tempfile.TemporaryDirectory() as tempdir:
             tempdir_path = Path(tempdir)
@@ -277,22 +250,17 @@
             self.endpoints._request("GET", f"/{__name__}", payload={1, 2, 3})
 
     def test_dict_params(self):
         self.endpoints._request("POST", f"/{__name__}", params=self.dict_params)
         _, kwargs = self.session_mock.request.call_args
         assert kwargs.get("params") == self.dict_params
 
-    def test_basemodel_v1_params(self):
-        self.endpoints._request("POST", f"/{__name__}", params=self.basemodel_v1_params)
-        _, kwargs = self.session_mock.request.call_args
-        assert kwargs.get("params") == self.dict_params
-
     @pytest.mark.filterwarnings("ignore::DeprecationWarning")
-    def test_basemodel_v2_params(self):
-        self.endpoints._request("POST", f"/{__name__}", params=self.basemodel_v2_params)
+    def test_basemodel_params(self):
+        self.endpoints._request("POST", f"/{__name__}", params=self.basemodel_params)
         _, kwargs = self.session_mock.request.call_args
         assert kwargs.get("params") == self.dict_params
 
     def test_request_decorator_forbidden_url_field_name(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
@@ -317,15 +285,15 @@
                     ...
 
     def test_request_decorator_unsupported_composite_return_type(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("GET", "/v1/data")
-                def get_data(self) -> List[BaseModelV1Example]:  # type: ignore [empty-body]
+                def get_data(self) -> List[BaseModelExample]:  # type: ignore [empty-body]
                     ...
 
     def test_request_decorator_unsupported_payload_type(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("POST", "/v1/data")
@@ -341,48 +309,48 @@
                     ...
 
     def test_request_decorator_unsupported_payload_composite_type(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("POST", "/v1/data")
-                def get_data(self, payload: Dict[str, BaseModelV1Example]) -> None:  # type: ignore [empty-body]
+                def get_data(self, payload: Dict[str, BaseModelExample]) -> None:  # type: ignore [empty-body]
                     ...
 
     @parameterized.expand(
         [
-            (BaseModelV1Example, False, TypeSpecifier(True, None, BaseModelV1Example, None, False, False)),
-            (List[BaseModelV1Example], False, TypeSpecifier(True, list, BaseModelV1Example, None, False, False)),
-            (Optional[BaseModelV1Example], False, TypeSpecifier(True, None, BaseModelV1Example, None, False, True)),
+            (BaseModelExample, False, TypeSpecifier(True, None, BaseModelExample, None, False, False)),
+            (List[BaseModelExample], False, TypeSpecifier(True, list, BaseModelExample, None, False, False)),
+            (Optional[BaseModelExample], False, TypeSpecifier(True, None, BaseModelExample, None, False, True)),
             (
-                Optional[List[BaseModelV1Example]],
+                Optional[List[BaseModelExample]],
                 False,
-                TypeSpecifier(True, list, BaseModelV1Example, None, False, True),
+                TypeSpecifier(True, list, BaseModelExample, None, False, True),
             ),
-            (List[Optional[BaseModelV1Example]], True, None),
-            (List[BaseModelV2Example], False, TypeSpecifier(True, list, BaseModelV2Example, None, False, False)),
-            (Optional[BaseModelV2Example], False, TypeSpecifier(True, None, BaseModelV2Example, None, False, True)),
+            (List[Optional[BaseModelExample]], True, None),
+            (List[BaseModelExample], False, TypeSpecifier(True, list, BaseModelExample, None, False, False)),
+            (Optional[BaseModelExample], False, TypeSpecifier(True, None, BaseModelExample, None, False, True)),
             (
-                Optional[List[BaseModelV2Example]],
+                Optional[List[BaseModelExample]],
                 False,
-                TypeSpecifier(True, list, BaseModelV2Example, None, False, True),
+                TypeSpecifier(True, list, BaseModelExample, None, False, True),
             ),
-            (List[Optional[BaseModelV2Example]], True, None),
+            (List[Optional[BaseModelExample]], True, None),
             (JSON, False, TypeSpecifier(True, None, None, None, True, False)),
             (str, False, TypeSpecifier(True, None, str, None, False, False)),
             (bytes, False, TypeSpecifier(True, None, bytes, None, False, False)),
             (
-                Union[BaseModelV2Example, BaseModelV2Example2],
+                Union[BaseModelExample, BaseModelExample2],
                 False,
-                TypeSpecifier(True, None, None, [BaseModelV2Example, BaseModelV2Example2], False, False),
+                TypeSpecifier(True, None, None, [BaseModelExample, BaseModelExample2], False, False),
             ),
             (
-                Annotated[Union[BaseModelV2Example, BaseModelV2Example2], None],
+                Annotated[Union[BaseModelExample, BaseModelExample2], None],
                 False,
-                TypeSpecifier(True, None, None, [BaseModelV2Example, BaseModelV2Example2], False, False),
+                TypeSpecifier(True, None, None, [BaseModelExample, BaseModelExample2], False, False),
             ),
             (None, True, None),
         ]
     )
     def test_request_decorator_payload_spec(self, payload_type, raises, expected_payload_spec):
         # Arrange
         class TestAPI(APIEndpoints):
@@ -423,32 +391,32 @@
                     ...
 
     def test_request_decorator_bogus_params(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("POST", "/v1/data/{id}")  # type: ignore [empty-body]
-                def get_data(self, id: str, payload: BaseModelV1Example, bogus: str) -> None:
+                def get_data(self, id: str, payload: BaseModelExample, bogus: str) -> None:
                     ...
 
     def test_request_decorator_accepts_optional_payload(self):
         # Arrange
         class TestAPIOptional(APIEndpoints):
             @request("GET", "/v1/data")
-            def get_data1(self, payload: Optional[BaseModelV1Example]) -> None:  # type: ignore [empty-body]
+            def get_data1(self, payload: Optional[BaseModelExample]) -> None:  # type: ignore [empty-body]
                 ...
 
         class TestAPIUnion(APIEndpoints):
             @request("GET", "/v2/data")
-            def get_data2(self, payload: Union[None, BaseModelV1Example]) -> None:  # type: ignore [empty-body]
+            def get_data2(self, payload: Union[None, BaseModelExample]) -> None:  # type: ignore [empty-body]
                 ...
 
         class TestAPIOptionalModelSequence(APIEndpoints):
             @request("GET", "/v3/data")
-            def get_data3(self, payload: Optional[List[BaseModelV1Example]]) -> None:  # type: ignore [empty-body]
+            def get_data3(self, payload: Optional[List[BaseModelExample]]) -> None:  # type: ignore [empty-body]
                 ...
 
     def test_request_decorator_call_from_unsuitable_base_class(self):
         class TestAPI:
             @request("GET", "/v1/data")
             def get_data(self) -> None:  # type: ignore [empty-body]
                 ...
@@ -457,68 +425,68 @@
         with self.assertRaises(APIEndpointError):
             api.get_data()
 
     def test_request_decorator_call_with_positional_arguments(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v1/data/{id}")
-            def get_data(self, id: str, payload: BaseModelV2Example) -> None:  # type: ignore [empty-body]
+            def get_data(self, id: str, payload: BaseModelExample) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
-        api.get_data("ID123", self.basemodel_v1_payload)
+        api.get_data("ID123", self.basemodel_payload)
         # Assert
         self.session_mock.request.assert_called_once_with(
             "GET",
             self.base_path + "/v1/data/ID123",
-            data=self.json_payload,
+            data=self.basemodel_payload.model_dump_json(),
             headers={"content-type": "application/json"},
         )
 
     def test_request_decorator_call_with_mixed_positional_arguments(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             def get_data(
-                self, payload: BaseModelV2Example, category: str, params: ParamsModelV1Example
+                self, payload: BaseModelExample, category: str, params: ParamsModelExample
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
-        api.get_data(self.basemodel_v1_payload, "clothes", self.basemodel_v1_params)
+        api.get_data(self.basemodel_payload, "clothes", self.basemodel_params)
         # Assert
         self.session_mock.request.assert_called_once_with(
             "GET",
             self.base_path + "/v2/clothes/items",
-            data=self.json_payload,
+            data=self.basemodel_payload.model_dump_json(),
             headers={"content-type": "application/json"},
-            params=self.basemodel_v1_params,
+            params=self.basemodel_params.model_dump(),
         )
 
     def test_request_decorator_call_with_keyword_arguments(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             def get_data(
-                self, payload: BaseModelV2Example, category: str, params: ParamsModelV1Example
+                self, payload: BaseModelExample, category: str, params: ParamsModelExample
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
-        api.get_data(category="clothes", params=self.basemodel_v1_params, payload=self.basemodel_v1_payload)
+        api.get_data(category="clothes", params=self.basemodel_params, payload=self.basemodel_payload)
         # Assert
         self.session_mock.request.assert_called_once_with(
             "GET",
             self.base_path + "/v2/clothes/items",
-            data=self.json_payload,
+            data=self.basemodel_payload.model_dump_json(),
             headers={"content-type": "application/json"},
-            params=self.basemodel_v1_params,
+            params=self.basemodel_params.model_dump(),
         )
 
     def test_request_decorator_call_with_json_payload(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/aaa/bbb/ccc")
             def get_data(self, payload: JSON) -> None:  # type: ignore [empty-body]
@@ -536,15 +504,15 @@
             headers={"content-type": "application/json"},
         )
 
     def test_request_decorator_call_optional_model_payload(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("PUT", "/v1/data/{id}")
-            def put_data(self, id: str, payload: Optional[BaseModelV1Example]) -> None:  # type: ignore [empty-body]
+            def put_data(self, id: str, payload: Optional[BaseModelExample]) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
         api.put_data("ID123", None)
         # Assert
         self.session_mock.request.assert_called_once_with(
@@ -552,39 +520,39 @@
             self.base_path + "/v1/data/ID123",
         )
 
     def test_request_decorator_call_and_return_model(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v1/items")
-            def get_data(self) -> BaseModelV1Example:  # type: ignore [empty-body]
+            def get_data(self) -> BaseModelExample:  # type: ignore [empty-body]
                 ...
 
-        self.session_mock.request.return_value.dataobj = MagicMock(return_value=self.basemodel_v1_payload)
+        self.session_mock.request.return_value.dataobj = MagicMock(return_value=self.basemodel_payload)
         api = TestAPI(self.session_mock)
         # Act
         retval = api.get_data()
         # Assert
         self.session_mock.request.return_value.dataobj.assert_called_once()
-        assert retval == self.basemodel_v1_payload
+        assert retval == self.basemodel_payload
 
     def test_request_decorator_call_and_return_model_datasequece(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v1/items")
-            def get_data(self) -> DataSequence[BaseModelV1Example]:  # type: ignore [empty-body]
+            def get_data(self) -> DataSequence[BaseModelExample]:  # type: ignore [empty-body]
                 ...
 
-        self.session_mock.request.return_value.dataseq = MagicMock(return_value=self.basemodel_v1_sequence_payload)
+        self.session_mock.request.return_value.dataseq = MagicMock(return_value=self.basemodel_sequence_payload)
         api = TestAPI(self.session_mock)
         # Act
         retval = api.get_data()
         # Assert
         self.session_mock.request.return_value.dataseq.assert_called_once()
-        assert retval == self.basemodel_v1_sequence_payload
+        assert retval == self.basemodel_sequence_payload
 
     def test_request_decorator_call_and_return_str(self):
         # Arrange
         expected = "This is String!"
 
         class TestAPI(APIEndpoints):
             @request("GET", "/v1/items")
@@ -713,108 +681,108 @@
         decorator.http_method = "DELETE"
 
     def test_no_mutable_state_when_calling_endpoint(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             def get_data(
-                self, payload: BaseModelV1Example, category: str, params: ParamsModelV1Example
+                self, payload: BaseModelExample, category: str, params: ParamsModelExample
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         for category in ["clothes", "food"]:
             for dict_payload in [
                 {"id": "id1", "size": 100, "capacity": 1.7, "active": True},
                 {"id": "id2", "size": 120, "capacity": 1.9, "active": False},
             ]:
                 for params in [
-                    ParamsModelV1Example(name="submarine", color="yellow"),
-                    ParamsModelV1Example(name="oyster", color="blue"),
+                    ParamsModelExample(name="submarine", color="yellow"),
+                    ParamsModelExample(name="oyster", color="blue"),
                 ]:
                     # Act
-                    payload = BaseModelV1Example.parse_obj(dict_payload)
+                    payload = BaseModelExample.model_validate(dict_payload)
                     api.get_data(category=category, params=params, payload=payload)
                     # Assert
                     self.session_mock.request.assert_called_once_with(
                         "GET",
                         self.base_path + f"/v2/{category}/items",
-                        data=json.dumps(dict_payload),
+                        data=payload.model_dump_json(),
                         headers={"content-type": "application/json"},
-                        params=params,
+                        params=params.model_dump(),
                     )
                     self.session_mock.reset_mock()
 
-    def test_request_decorator_call_with_defaults_arguments(self):
+    def test_request_decorator_call_with_default_arguments(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             def get_data(
                 self,
-                payload: BaseModelV1Example = self.basemodel_v1_payload,
+                payload: BaseModelExample = self.basemodel_payload,
                 category: str = "default-category",
-                params: ParamsModelV1Example = self.basemodel_v1_params,
+                params: ParamsModelExample = self.basemodel_params,
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
         api.get_data()
         # Assert
         self.session_mock.request.assert_called_once_with(
             "GET",
             self.base_path + "/v2/default-category/items",
-            data=self.json_payload,
+            data=self.basemodel_payload.model_dump_json(),
             headers={"content-type": "application/json"},
-            params=self.basemodel_v1_params,
+            params=self.dict_params,
         )
 
     def test_request_decorator_call_with_defaults_arguments_override(self):
         # Arrange
         class TestAPI(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             def get_data(
                 self,
-                payload: BaseModelV1Example = self.basemodel_v1_payload,
+                payload: BaseModelExample = self.basemodel_payload,
                 category: str = "default",
-                params: ParamsModelV1Example = self.basemodel_v1_params,
+                params: ParamsModelExample = self.basemodel_params,
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         api = TestAPI(self.session_mock)
         # Act
-        payload_override = BaseModelV1Example(id="override-id", size=500, capacity=9.0001, active=False)
+        payload_override = BaseModelExample(id="override-id", size=500, capacity=9.0001, active=False)
         category_override = "override-category!"
-        params_override = ParamsModelV1Example(name="override-Name", color="override with orange!")
+        params_override = ParamsModelExample(name="override-Name", color="override with orange!")
         api.get_data(payload_override, category_override, params_override)
         # Assert
         self.session_mock.request.assert_called_once_with(
             "GET",
             self.base_path + f"/v2/{category_override}/items",
-            data=payload_override.json(),
+            data=payload_override.model_dump_json(),
             headers={"content-type": "application/json"},
-            params=params_override,
+            params=params_override.model_dump(),
         )
 
     def test_decorator_chaining_order(self):
         # Expected @request can access original function signature (it will raise otherwise)
         class TestAPIMixedOrder1(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             @versions("<2")
             def get_data(
-                self, payload: BaseModelV1Example, category: str, params: ParamsModelV1Example
+                self, payload: BaseModelExample, category: str, params: ParamsModelExample
             ) -> None:  # type: ignore [empty-body]
                 ...
 
         class TestAPIMixedOrder2(APIEndpoints):
             @request("GET", "/v2/{category}/items")
             @versions("<2")
             @view({ProviderView})
             def get_data(
-                self, payload: BaseModelV1Example, category: str, params: ParamsModelV1Example
+                self, payload: BaseModelExample, category: str, params: ParamsModelExample
             ) -> None:  # type: ignore [empty-body]
                 ...
 
     def test_request_decorator_format_url_with_str_enum(self):
         class FruitEnum(str, Enum):
             BANANA = "banana"
             ORANGE = "orange"
@@ -883,26 +851,26 @@
                 def get_data(self, fruit_type: FruitType) -> None:  # type: ignore [empty-body]
                     ...
 
     def test_request_decorator_accept_union_of_models(self):
         class TestAPI(APIEndpoints):
             @request("GET", "/v1/data")
             def get_data(
-                self, payload: Union[BaseModelV2Example, BaseModelV2Example2]
+                self, payload: Union[BaseModelExample, BaseModelExample2]
             ) -> None:  # type: ignore [empty-body]
                 ...
 
     def test_request_decorator_accept_annotated_union_of_models(self):
-        class BaseModelV2_A(BaseModelV2):
+        class BaseModel_A(BaseModel):
             field: Literal["number"] = "number"
             num: float
 
-        class BaseModelV2_B(BaseModelV2):
+        class BaseModel_B(BaseModel):
             field: Literal["name"] = "name"
             name: str
 
-        AnyBaseModel = Annotated[Union[BaseModelV2_A, BaseModelV2_B], FieldV2(discriminator="field")]
+        AnyBaseModel = Annotated[Union[BaseModel_A, BaseModel_B], Field(discriminator="field")]
 
         class TestAPI(APIEndpoints):
             @request("POST", "/v1/data")
             def create(self, payload: AnyBaseModel) -> None:  # type: ignore [empty-body]
                 ...
```

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.0/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.0/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_response.py` & `catalystwan-0.33.0/catalystwan/tests/test_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,41 +2,32 @@
 
 import unittest
 from typing import Any, List, Optional
 from unittest.mock import patch
 
 from attr import define, field  # type: ignore
 from parameterized import parameterized  # type: ignore
-from pydantic import BaseModel as BaseModelV2
-from pydantic import Field as FieldV2
-from pydantic.v1 import BaseModel as BaseModelV1
-from pydantic.v1 import Field as FieldV1
+from pydantic import BaseModel, Field
 
 from catalystwan.dataclasses import DataclassBase
 from catalystwan.response import ManagerErrorInfo, ManagerResponse
 from catalystwan.typed_list import DataSequence
 
 
 @define
 class ParsedDataTypeAttrs(DataclassBase):
     key1: str
     key2: int
     key3: Optional[float] = field(default=None)
 
 
-class ParsedDataTypePydanticV1(BaseModelV1):
+class ParsedDataTypePydanticV2(BaseModel):
     key1: str
     key2: int
-    key3: Optional[float] = FieldV1(default=None)
-
-
-class ParsedDataTypePydanticV2(BaseModelV2):
-    key1: str
-    key2: int
-    key3: Optional[float] = FieldV2(default=None)
+    key3: Optional[float] = Field(default=None)
 
 
 PARSE_DATASEQ_TEST_DATA: List = [
     (True, None, 0, "data"),
     (True, "string", 0, "data"),
     (True, {}, 0, "data"),
     (True, {"key1": "string", "key2": 12, "key3": 4.5}, 0, "data"),
@@ -83,27 +74,15 @@
             assert isinstance(data_sequence, DataSequence)
             assert len(data_sequence) == expected_len
         else:
             with self.assertRaises(Exception):
                 vmng_response.dataseq(ParsedDataTypeAttrs, sourcekey)
 
     @parameterized.expand(PARSE_DATASEQ_TEST_DATA)
-    def test_dataseq_pydantic_v1(self, raises: bool, json: Any, expected_len: int, sourcekey: str):
-        self.response_mock.json.return_value = json
-        vmng_response = ManagerResponse(self.response_mock)
-        if not raises:
-            data_sequence = vmng_response.dataseq(ParsedDataTypePydanticV1, sourcekey)
-            assert isinstance(data_sequence, DataSequence)
-            assert len(data_sequence) == expected_len
-        else:
-            with self.assertRaises(Exception):
-                vmng_response.dataseq(ParsedDataTypePydanticV1, sourcekey)
-
-    @parameterized.expand(PARSE_DATASEQ_TEST_DATA)
-    def test_dataseq_pydantic_v2(self, raises: bool, json: Any, expected_len: int, sourcekey: str):
+    def test_dataseq_pydantic(self, raises: bool, json: Any, expected_len: int, sourcekey: str):
         self.response_mock.json.return_value = json
         vmng_response = ManagerResponse(self.response_mock)
         if not raises:
             data_sequence = vmng_response.dataseq(ParsedDataTypePydanticV2, sourcekey)
             assert isinstance(data_sequence, DataSequence)
             assert len(data_sequence) == expected_len
         else:
@@ -118,26 +97,15 @@
             data_object = vmng_response.dataobj(ParsedDataTypeAttrs, sourcekey)
             assert isinstance(data_object, ParsedDataTypeAttrs)
         else:
             with self.assertRaises(Exception):
                 vmng_response.dataobj(ParsedDataTypeAttrs, sourcekey)
 
     @parameterized.expand(PARSE_DATAOBJ_TEST_DATA)
-    def test_dataobj_pydantic_v1(self, raises: bool, json: Any, sourcekey: str):
-        self.response_mock.json.return_value = json
-        vmng_response = ManagerResponse(self.response_mock)
-        if not raises:
-            data_object = vmng_response.dataobj(ParsedDataTypePydanticV1, sourcekey)
-            assert isinstance(data_object, ParsedDataTypePydanticV1)
-        else:
-            with self.assertRaises(Exception):
-                vmng_response.dataobj(ParsedDataTypePydanticV1, sourcekey)
-
-    @parameterized.expand(PARSE_DATAOBJ_TEST_DATA)
-    def test_dataobj_pydantic_v2(self, raises: bool, json: Any, sourcekey: str):
+    def test_dataobj_pydantic(self, raises: bool, json: Any, sourcekey: str):
         self.response_mock.json.return_value = json
         vmng_response = ManagerResponse(self.response_mock)
         if not raises:
             data_object = vmng_response.dataobj(ParsedDataTypePydanticV2, sourcekey)
             assert isinstance(data_object, ParsedDataTypePydanticV2)
         else:
             with self.assertRaises(Exception):
```

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_session.py` & `catalystwan-0.33.0/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_task_status_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -303,76 +303,79 @@
             "isParallelExecutionEnabled": True,
         }
 
     @patch.object(Task, "_Task__check_validation_status")
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_success(self, mock_task_response, mock_validation):
         # Arrange
-        mock_task_response.return_value = TaskData.parse_obj(self.success_response)
+        mock_task_response.return_value = TaskData.model_validate(self.success_response)
 
         # Act
         answer = self.task.wait_for_completed(interval_seconds=1).result
 
         # Assert
         self.assertEqual(answer, True)
 
     @patch.object(Task, "_Task__check_validation_status")
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_empty_data(self, mock_task_response, mock_validation):
         # Data is empty, and then response is success
 
         # Arrange
         mock_task_response.side_effect = [
-            TaskData.parse_obj(self.empty_data),
-            TaskData.parse_obj(self.success_response),
+            TaskData.model_validate(self.empty_data),
+            TaskData.model_validate(self.success_response),
         ]
 
         # Act
         answer = self.task.wait_for_completed(timeout_seconds=2, interval_seconds=1).result
 
         # Assert
         self.assertEqual(answer, True)
 
     @patch.object(Task, "_Task__check_validation_status")
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_with_action_config_as_dict(self, mock_task_response, mock_validation):
         # Arrange
-        mock_task_response.return_value = TaskData.parse_obj(self.response_with_action_config_as_dict)
+        mock_task_response.return_value = TaskData.model_validate(self.response_with_action_config_as_dict)
 
         # Act
         answer = self.task.wait_for_completed(interval_seconds=1).result
 
         # Assert
         self.assertEqual(answer, True)
 
     @patch.object(Task, "_Task__check_validation_status")
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_no_data(self, mock_task_response, mock_validation):
         # No data in first call, and then response is success
 
         # Arrange
-        mock_task_response.side_effect = [TaskData.parse_obj(self.no_data), TaskData.parse_obj(self.success_response)]
+        mock_task_response.side_effect = [
+            TaskData.model_validate(self.no_data),
+            TaskData.model_validate(self.success_response),
+        ]
 
         # Act
         answer = self.task.wait_for_completed(timeout_seconds=2, interval_seconds=1).result
 
         # Assert
         self.assertEqual(answer, True)
 
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_no_validation_field(self, mock_task_response_response):
         # Arrange
-        mock_task_response_response.return_value = TaskData.parse_obj(self.no_validation)
+        mock_task_response_response.return_value = TaskData.model_validate(self.no_validation)
 
         # Act
         answer = self.task.wait_for_completed(interval_seconds=1).result
 
         # Assert
         self.assertEqual(answer, True)
 
     @patch.object(ConfigurationDashboardStatus, "find_status")
     def test_wait_for_completed_raise_TaskValidationError(self, mock_task_response_response):
         # Arrange
-        mock_task_response_response.return_value = TaskData.parse_obj(self.validation_failure)
+        mock_task_response_response.return_value = TaskData.model_validate(self.validation_failure)
 
         # Act&Assert
         self.assertRaises(TaskValidationError, self.task.wait_for_completed)
```

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_templates.py` & `catalystwan-0.33.0/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_tenant_management_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,51 +29,51 @@
         self.session.session_type = None
         self.api = TenantManagementAPI(self.session)
 
     def test_get(self):
         expected_tenants = [
             Tenant(
                 name="tenant1",
-                orgName="CiscoDevNet",
-                subDomain="alpha.bravo.net",
+                org_name="CiscoDevNet",
+                subdomain="alpha.bravo.net",
                 desc="This is tenant for unit tests",
-                edgeConnectorEnable=True,
-                edgeConnectorSystemIp="172.16.255.81",
-                edgeConnectorTunnelInterfaceName="GigabitEthernet1",
-                wanEdgeForecast=1,
+                edge_connector_enable=True,
+                edge_connector_system_ip="172.16.255.81",
+                edge_connector_tunnel_interface_name="GigabitEthernet1",
+                wan_edge_forecast=1,
             )
         ]
         self.api._endpoints.get_all_tenants = MagicMock(return_value=expected_tenants)
         observed_tenants = self.api.get()
         assert expected_tenants == observed_tenants
 
     def test_create(self):
         tenants = [
             Tenant(
                 name="tenant1",
-                orgName="CiscoDevNet",
-                subDomain="alpha.bravo.net",
+                org_name="CiscoDevNet",
+                subdomain="alpha.bravo.net",
                 desc="This is tenant for unit tests",
-                edgeConnectorEnable=True,
-                edgeConnectorSystemIp="172.16.255.81",
-                edgeConnectorTunnelInterfaceName="GigabitEthernet1",
-                wanEdgeForecast=1,
+                edge_connector_enable=True,
+                edge_connector_system_ip="172.16.255.81",
+                edge_connector_tunnel_interface_name="GigabitEthernet1",
+                wan_edge_forecast=1,
             )
         ]
         task = self.api.create(tenants)
         self.assertIsInstance(task, Task)
 
     def test_update(self):
         # Arrange
         tenant_update_request = TenantUpdateRequest(
-            tenantId="apo605#",
-            subDomain="doamin.tenant.net",
+            tenant_id="apo605#",
+            subdomain="doamin.tenant.net",
             desc="Tenant1 description",
-            wanEdgeForecast=1,
-            edgeConnectorEnable=False,
+            wan_edge_forecast=1,
+            edge_connector_enable=False,
         )
         self.api._endpoints.update_tenant = MagicMock()
         # Act
         self.api.update(tenant_update_request=tenant_update_request)
         # Assert
         self.api._endpoints.update_tenant.assert_called_once_with(
             tenant_id=tenant_update_request.tenant_id, tenant_update_request=tenant_update_request
@@ -81,16 +81,16 @@
 
     def test_update_vsmart_placement(self):
         # Arrange
         src_uuid = "123190GDS*!"
         dst_uuid = "!_0ac%$asfDS"
         tenant_id = "apo605#"
         vsmart_placement_update = vSmartPlacementUpdateRequest(
-            srcvSmartUuid=src_uuid,
-            destvSmartUuid=dst_uuid,
+            src_vsmart_uuid=src_uuid,
+            dest_vsmart_uuid=dst_uuid,
         )
         self.api._endpoints.update_tenant_vsmart_placement = MagicMock()
         # Act
         self.api.update_vsmart_placement(tenant_id=tenant_id, src_vsmart_uuid=src_uuid, dst_vsmart_uuid=dst_uuid)
         # Assert
         self.api._endpoints.update_tenant_vsmart_placement.assert_called_once_with(
             tenant_id=tenant_id, vsmart_placement_update_request=vsmart_placement_update
@@ -106,49 +106,49 @@
         tenant_id_list = ["1"]
         self.session.password = "p4s$w0rD"  # pragma: allowlist secret
         task = self.api.delete(tenant_id_list)
         self.assertIsInstance(task, Task)
 
     def test_get_statuses(self):
         tenant_status = TenantStatus(
-            tenantId="tenant2",
-            tenantName="TeanantTwo",
-            controlStatus=ControlStatus(controlUp=1, controlDown=0, partial=1),
-            siteHealth=SiteHealth(fullConnectivity=2, partialConnectivity=1, noConnectivity=0),
-            vEdgeHealth=vEdgeHealth(normal=3, warning=1, error=0),
-            vSmartStatus=vSmartStatus(up=1, down=0),
+            tenant_id="tenant2",
+            tenant_name="TeanantTwo",
+            control_status=ControlStatus(control_up=1, control_down=0, partial=1),
+            site_health=SiteHealth(full_connectivity=2, partial_connectivity=1, no_connectivity=0),
+            vedge_health=vEdgeHealth(normal=3, warning=1, error=0),
+            vsmart_status=vSmartStatus(up=1, down=0),
         )
         expected_statuses = DataSequence(TenantStatus, [tenant_status])
         self.api._endpoints.get_all_tenant_statuses = MagicMock(return_value=expected_statuses)
         observed_statuses = self.api.get_statuses()
         assert expected_statuses == observed_statuses
 
     def test_get_hosting_capacity_on_vsmarts(self):
-        capacity = vSmartTenantCapacity(vSmartUuid="ABCD-1234", totalTenantCapacity=12, currentTenantCount=5)
+        capacity = vSmartTenantCapacity(vsmart_uuid="ABCD-1234", total_tenant_capacity=12, current_tenant_count=5)
         expected_capacities = DataSequence(vSmartTenantCapacity, [capacity])
         self.api._endpoints.get_tenant_hosting_capacity_on_vsmarts = MagicMock(return_value=expected_capacities)
         observed_capacities = self.api.get_hosting_capacity_on_vsmarts()
         assert expected_capacities == observed_capacities
 
     def test_get_vsmart_mapping(self):
         expected_mapping = vSmartTenantMap(
             data={
                 "vsmart1": [
                     Tenant(
                         name="tenant1",
-                        orgName="Tenant1-organization",
+                        org_name="Tenant1-organization",
                         desc="Tenant1 description",
-                        subDomain="tenant1.organization.org",
-                        flakeId=9987,
+                        subdomain="tenant1.organization.org",
+                        flake_id=9987,
                     )
                 ]
             }
         )
         self.api._endpoints.get_tenant_vsmart_mapping = MagicMock(return_value=expected_mapping)
         observed_mapping = self.api.get_vsmart_mapping()
         assert expected_mapping == observed_mapping
 
     def test_vsession_id(self):
         expected_vsession_id = "567-DEF"
-        self.api._endpoints.vsession_id = MagicMock(return_value=vSessionId(VSessionId=expected_vsession_id))
+        self.api._endpoints.vsession_id = MagicMock(return_value=vSessionId(vsessionid=expected_vsession_id))
         observed_vsession_id = self.api.vsession_id("1")
         assert expected_vsession_id == observed_vsession_id
```

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.0/catalystwan/tests/test_tenant_migration_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 import tempfile
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
+from uuid import uuid4
 
 from packaging.version import Version  # type: ignore
 
 from catalystwan.api.task_status_api import Task
 from catalystwan.api.tenant_migration_api import ImportTask, TenantMigrationAPI
 from catalystwan.endpoints.tenant_migration import ImportInfo, MigrationInfo
 from catalystwan.models.tenant import Tenant, TenantExport
@@ -42,48 +43,42 @@
             download_path = Path(tmpdir) / "test.tar.gz"
             self.session.endpoints.tenant_migration.download_tenant_data = MagicMock(return_value=content)
             self.api.download(download_path)
             assert open(download_path, "rb").read() == content
 
     def test_import_tenant(self):
         self.session.api_version = Version("20.12")
-        migration_key = "Cisco12345"
-        migration_id = "dcbed267-eb0d-4dcd-9c12-2536e8562f75"
+        migration_key = "mkey1"
+        migration_id = str(uuid4())
         with tempfile.TemporaryDirectory() as tmpdir:
             import_file = Path(tmpdir) / "tenant.tar.gz"
             with open(import_file, "wb") as f:
                 f.write(b"\xFEtest_data")
             self.session.endpoints.tenant_migration.import_tenant_data = MagicMock(
                 return_value=ImportInfo(
-                    processId="123",
-                    migrationTokenURL=(
-                        "/dataservice/tenantmigration/migrationToken?"
-                        "migrationId=dcbed267-eb0d-4dcd-9c12-2536e8562f75"
-                    ),
+                    process_id="123",
+                    migration_token_url=("/dataservice/tenantmigration/migrationToken?" f"migrationId={migration_id}"),
                 )
             )
             task = self.api.import_tenant(import_file, migration_key)
             self.assertIsInstance(task, ImportTask)
             assert task.import_info.migration_token_query_params.migration_id == migration_id
 
     def test_import_tenant_with_key(self):
         self.session.api_version = Version("20.13")
-        migration_key = "Cisco12345"
-        migration_id = "dcbed267-eb0d-4dcd-9c12-2536e8562f75"
+        migration_key = "mkey2"
+        migration_id = str(uuid4())
         with tempfile.TemporaryDirectory() as tmpdir:
             import_file = Path(tmpdir) / "tenant.tar.gz"
             with open(import_file, "wb") as f:
                 f.write(b"\xFEtest_data")
             self.session.endpoints.tenant_migration.import_tenant_data_with_key = MagicMock(
                 return_value=ImportInfo(
-                    processId="123",
-                    migrationTokenURL=(
-                        "/dataservice/tenantmigration/migrationToken?"
-                        "migrationId=dcbed267-eb0d-4dcd-9c12-2536e8562f75"
-                    ),
+                    process_id="123",
+                    migration_token_url=("/dataservice/tenantmigration/migrationToken?" f"migrationId={migration_id}"),
                 )
             )
             task = self.api.import_tenant(import_file, migration_key)
             self.assertIsInstance(task, ImportTask)
             assert task.import_info.migration_token_query_params.migration_id == migration_id
 
     def test_store_token(self):
```

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.0/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_version.py` & `catalystwan-0.33.0/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.0/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.0/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/typed_list.py` & `catalystwan-0.33.0/catalystwan/typed_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
 from typing import Any, Generic, Iterable, MutableSequence, Type, TypeVar, overload
 
-from pydantic import BaseModel as BaseModelV2
-from pydantic.v1 import BaseModel as BaseModelV1
+from pydantic import BaseModel
 
 from catalystwan.exceptions import InvalidOperationError
 from catalystwan.utils.creation_tools import AttrsInstance, asdict
 
 T = TypeVar("T")
 D = TypeVar("D")
 
@@ -148,21 +147,17 @@
         ...
 
     @overload
     def __init__(self, _type: Type[T], _iterable: Iterable[T], /) -> None:
         ...
 
     def __init__(self, _type, _iterable=None, /):
-        if (
-            not isinstance(_type, AttrsInstance)
-            and not issubclass(_type, BaseModelV1)
-            and not issubclass(_type, BaseModelV2)
-        ):
+        if not isinstance(_type, AttrsInstance) and not issubclass(_type, BaseModel):
             raise TypeError(
-                f"Expected {AttrsInstance.__name__} or {BaseModelV1.__name__} item type, got {_type.__name__}."
+                f"Expected {AttrsInstance.__name__} or {BaseModel.__name__} item type, got {_type.__name__}."
             )
 
         super().__init__(_type, _iterable)
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, DataSequence):
             if len(self) != len(__o):
@@ -172,15 +167,15 @@
 
     def __repr__(self) -> str:
         return f"DataSequence({self._type.__name__}, {repr(self.data)})"
 
     def __str__(self) -> str:
         pretty_message = ""
         for element in self:
-            if issubclass(element.__class__, (BaseModelV1, BaseModelV2)):
+            if issubclass(element.__class__, BaseModel):
                 pprint = "\n".join(f"    {attr[0]}: {attr[1]}, " for attr in element.dict().items())  # type: ignore
             else:
                 pprint = "\n".join(f"    {attr[0]}: {attr[1]}, " for attr in asdict(element).items())  # type: ignore
 
             pretty_message += f"\n{element.__class__.__name__}(\n" + pprint + "\n)"  # type: ignore
         return pretty_message
```

### Comparing `catalystwan-0.32.0/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.0/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/dashboard.py` & `catalystwan-0.33.0/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/device_model.py` & `catalystwan-0.33.0/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/dict.py` & `catalystwan-0.33.0/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.0/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.0/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/operation_status.py` & `catalystwan-0.33.0/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/timezone.py` & `catalystwan-0.33.0/catalystwan/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.0/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/version.py` & `catalystwan-0.33.0/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/vmanage_auth.py` & `catalystwan-0.33.0/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.0/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.32.0/pyproject.toml` & `catalystwan-0.33.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.32.0"
+version = "0.33.0"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.32.0/setup.py` & `catalystwan-0.33.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.32.0',
+    'version': '0.33.0',
     'description': 'Cisco Catalyst WAN SDK for Python',
-    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any Manager.\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        orgName="CiscoDevNet",\n        subDomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edgeConnectorEnable=True,\n        edgeConnectorSystemIp="172.16.255.81",\n        edgeConnectorTunnelInterfaceName="GigabitEthernet1",\n        wanEdgeForecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on vmngclient@cisco.com.\n',
+    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any Manager.\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -33,15 +33,15 @@
 'catalystwan.tests.templates': ['definitions/*', 'definitions/basic/*',
 'schemas/*', 'schemas/basic/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
 'attrs>=21.4.0,<22.0.0', 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0',
 'flake8-quotes>=3.3.1,<4.0.0', 'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0',
 'python-dateutil>=2.8.2,<3.0.0', 'requests-toolbelt>=1.0.0,<2.0.0',
 'requests>=2.27.1,<3.0.0', 'tenacity>=8.1.0,<9.0.0', 'typing-
 extensions>=4.6.1,<5.0.0'] setup_kwargs = { 'name': 'catalystwan', 'version':
-'0.32.0', 'description': 'Cisco Catalyst WAN SDK for Python',
+'0.33.0', 'description': 'Cisco Catalyst WAN SDK for Python',
 'long_description': '
                       \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
 \n\n[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official Manager API. It is intended
 to serve as a multiple session handler (provider, provider as a tenant,
@@ -144,24 +144,25 @@
 ResourceGroupUpdateRequest(\n id=resource_group.id,\n
 name=resource_group.name,\n desc="Custom Resource Group #1 with updated
 description and site ids",\n siteIds=[200]\n)\n\n# switch to resource group
 view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete
 resource group\nsession.api.resource_groups.delete
 (resource_group.id)\n```\n\n\n\n\n TTeennaanntt mmaannaaggeemmeenntt (click to
 expand)\n\n```python\napi = session.api.tenant_management\n# create
-tenants\ntenants = [\n Tenant(\n name="tenant1",\n orgName="CiscoDevNet",\n
-subDomain="alpha.bravo.net",\n desc="This is tenant for unit tests",\n
-edgeConnectorEnable=True,\n edgeConnectorSystemIp="172.16.255.81",\n
-edgeConnectorTunnelInterfaceName="GigabitEthernet1",\n wanEdgeForecast=1,\n
-)\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n#
-list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by
-name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get
-selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected
-tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by
-ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n#
+tenants\ntenants = [\n Tenant(\n name="tenant1",\n org_name="CiscoDevNet",\n
+subdomain="alpha.bravo.net",\n desc="This is tenant for unit tests",\n
+edge_connector_enable=True,\n edge_connector_system_ip="172.16.255.81",\n
+edge_connector_tunnel_interface_name="GigabitEthernet1",\n
+wan_edge_forecast=1,\n )\n]\ncreate_task = api.create
+(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data =
+api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter
+(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id =
+tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid =
+api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete(
+[tenant_id])\ndelete_task.wait_for_completed()\n#
 others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses
 ()\napi.get_vsmart_mapping()\n```\n\n\n\n TTeennaanntt mmiiggrraattiioonn (click to
 expand)\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import
 create_manager_session\nfrom catalystwan.models.tenant import
 TenantExport\nfrom catalystwan.workflows.tenant_migration import
 migration_workflow\n\ntenant = TenantExport(\n name="mango",\n desc="Mango
 tenant description",\n org_name="Provider Org-Mango Inc",\n
```

### Comparing `catalystwan-0.32.0/PKG-INFO` & `catalystwan-0.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.32.0
+Version: 0.33.0
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -312,21 +312,21 @@
 
 ```python
 api = session.api.tenant_management
 # create tenants
 tenants = [
     Tenant(
         name="tenant1",
-        orgName="CiscoDevNet",
-        subDomain="alpha.bravo.net",
+        org_name="CiscoDevNet",
+        subdomain="alpha.bravo.net",
         desc="This is tenant for unit tests",
-        edgeConnectorEnable=True,
-        edgeConnectorSystemIp="172.16.255.81",
-        edgeConnectorTunnelInterfaceName="GigabitEthernet1",
-        wanEdgeForecast=1,
+        edge_connector_enable=True,
+        edge_connector_system_ip="172.16.255.81",
+        edge_connector_tunnel_interface_name="GigabitEthernet1",
+        wan_edge_forecast=1,
     )
 ]
 create_task = api.create(tenants)
 create_task.wait_for_completed()
 # list all tenants
 tenants_data = api.get_all()
 # pick tenant from list by name
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.32.0 Summary: Cisco Catalyst
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.0 Summary: Cisco Catalyst
 WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-catalyst-wan-
 sdk Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist: ciscoconfparse
@@ -107,19 +107,19 @@
 (name="new_resource_group").single_or_default() updated_resource_group =
 ResourceGroupUpdateRequest( id=resource_group.id, name=resource_group.name,
 desc="Custom Resource Group #1 with updated description and site ids", siteIds=
 [200] ) # switch to resource group view session.api.resource_groups.switch
 ("new_resource_group") # delete resource group
 session.api.resource_groups.delete(resource_group.id) ``` TTeennaanntt mmaannaaggeemmeenntt
 (click to expand) ```python api = session.api.tenant_management # create
-tenants tenants = [ Tenant( name="tenant1", orgName="CiscoDevNet",
-subDomain="alpha.bravo.net", desc="This is tenant for unit tests",
-edgeConnectorEnable=True, edgeConnectorSystemIp="172.16.255.81",
-edgeConnectorTunnelInterfaceName="GigabitEthernet1", wanEdgeForecast=1, ) ]
-create_task = api.create(tenants) create_task.wait_for_completed() # list all
+tenants tenants = [ Tenant( name="tenant1", org_name="CiscoDevNet",
+subdomain="alpha.bravo.net", desc="This is tenant for unit tests",
+edge_connector_enable=True, edge_connector_system_ip="172.16.255.81",
+edge_connector_tunnel_interface_name="GigabitEthernet1", wan_edge_forecast=1, )
+] create_task = api.create(tenants) create_task.wait_for_completed() # list all
 tenants tenants_data = api.get_all() # pick tenant from list by name tenant =
 tenants_data.filter(name="tenant1").single_or_default() # get selected tenant
 id tenant_id = tenant.tenant_id # get vsession id of selected tenant vsessionid
 = api.vsession_id(tenant_id) # delete tenant by ids delete_task = api.delete(
 [tenant_id]) delete_task.wait_for_completed() # others
 api.get_hosting_capacity_on_vsmarts() api.get_statuses() api.get_vsmart_mapping
 () ``` TTeennaanntt mmiiggrraattiioonn (click to expand) ```python from pathlib import Path
```

