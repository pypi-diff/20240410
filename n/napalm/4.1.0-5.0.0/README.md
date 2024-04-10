# Comparing `tmp/napalm-4.1.0.tar.gz` & `tmp/napalm-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-4.1.0.tar", last modified: Tue May 23 17:42:28 2023, max compression
+gzip compressed data, was "napalm-5.0.0.tar", last modified: Wed Apr 10 12:01:20 2024, max compression
```

## Comparing `napalm-4.1.0.tar` & `napalm-5.0.0.tar`

### file list

```diff
@@ -1,179 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 17:42:19.000000 napalm-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 17:42:19.000000 napalm-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-23 17:42:28.085401 napalm-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-23 17:42:19.000000 napalm-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/_SUPPORTED_DRIVERS.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67796 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/canonical_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/clitools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8542 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/netmiko_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/double.py
--rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/getters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/string_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    93647 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/pyeapi_syntax_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/cli_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/ntp_peers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/vrf.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   153235 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/ios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.069401 napalm-4.1.0/napalm/ios/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/iosxr/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    95462 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/iosxr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/iosxr/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/schedule_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/iosxr_netconf/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   119196 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/iosxr_netconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   103749 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/junos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/schedule_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_probes.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/junos_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/junos_views.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxapi_plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66020 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/nxos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/users.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69493 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/nxos_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/system_resources.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/users.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/pyIOSXR/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27426 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/iosxr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 17:42:19.000000 napalm-4.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 17:42:19.000000 napalm-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-23 17:42:28.085401 napalm-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-23 17:42:19.000000 napalm-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.047799 napalm-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:01:16.000000 napalm-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 12:01:16.000000 napalm-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-10 12:01:20.047799 napalm-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-10 12:01:16.000000 napalm-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.019799 napalm-5.0.0/napalm/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/_SUPPORTED_DRIVERS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.023799 napalm-5.0.0/napalm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67927 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/canonical_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.023799 napalm-5.0.0/napalm/base/clitools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8542 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/cl_napalm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/cl_napalm_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/cl_napalm_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1315 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/cl_napalm_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/clitools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/netmiko_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.027799 napalm-5.0.0/napalm/base/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22905 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.027799 napalm-5.0.0/napalm/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/utils/jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/utils/string_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/base/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.027799 napalm-5.0.0/napalm/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92288 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.027799 napalm-5.0.0/napalm/eos/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.027799 napalm-5.0.0/napalm/eos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.031799 napalm-5.0.0/napalm/eos/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/textfsm_templates/ntp_peers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/textfsm_templates/vrf.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/eos/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.031799 napalm-5.0.0/napalm/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154210 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/ios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.031799 napalm-5.0.0/napalm/ios/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.015799 napalm-5.0.0/napalm/ios/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.031799 napalm-5.0.0/napalm/ios/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.031799 napalm-5.0.0/napalm/iosxr/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95905 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/iosxr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.035799 napalm-5.0.0/napalm/iosxr/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/delete_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/schedule_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/set_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/templates/snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.035799 napalm-5.0.0/napalm/iosxr_netconf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr_netconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr_netconf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119283 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/iosxr_netconf/iosxr_netconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.035799 napalm-5.0.0/napalm/junos/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104187 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/junos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.039799 napalm-5.0.0/napalm/junos/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/delete_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/schedule_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/set_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.039799 napalm-5.0.0/napalm/junos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      622 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/utils/junos_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25648 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/junos/utils/junos_views.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.039799 napalm-5.0.0/napalm/nxapi_plumbing/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxapi_plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxapi_plumbing/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxapi_plumbing/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxapi_plumbing/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxapi_plumbing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.039799 napalm-5.0.0/napalm/nxos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67415 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/nxos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.039799 napalm-5.0.0/napalm/nxos/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos/utils/textfsm_templates/users.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69891 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/nxos_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos_ssh/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos_ssh/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/nxos_ssh/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/utils/textfsm_templates/system_resources.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/nxos_ssh/utils/textfsm_templates/users.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm/pyIOSXR/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/pyIOSXR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/pyIOSXR/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-04-10 12:01:16.000000 napalm-5.0.0/napalm/pyIOSXR/iosxr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:01:20.043799 napalm-5.0.0/napalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 12:01:20.000000 napalm-5.0.0/napalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 12:01:16.000000 napalm-5.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-10 12:01:16.000000 napalm-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-10 12:01:20.047799 napalm-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 12:01:16.000000 napalm-5.0.0/setup.py
```

### Comparing `napalm-4.1.0/LICENSE` & `napalm-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/PKG-INFO` & `napalm-5.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: napalm
-Version: 4.1.0
-Summary: Network Automation and Programmability Abstraction Layer with Multivendor support
-Home-page: https://github.com/napalm-automation/napalm
-Author: David Barroso, Kirk Byers, Mircea Ulinic
-Author-email: dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com
-License: Apache 2.0
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI](https://img.shields.io/pypi/v/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![Actions Build](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml/badge.svg?branch=develop)](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
 NAPALM
@@ -48,14 +27,17 @@
 Install
 =======
 
 ```
 pip install napalm
 ```
 
+*Note*: Beginning with release 5.0.0 and later, NAPALM offers support for
+Python 3.8+ only.
+
 *Note*: Beginning with release 4.0.0 and later, NAPALM offers support for
 Python 3.7+ only.
 
 *Note*: Beginning with release 3.0.0 and later, NAPALM offers support for
 Python 3.6+ only.
```

### Comparing `napalm-4.1.0/README.md` & `napalm-5.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,47 @@
+Metadata-Version: 2.1
+Name: napalm
+Version: 5.0.0
+Summary: Network Automation and Programmability Abstraction Layer with Multivendor support
+Home-page: https://github.com/napalm-automation/napalm
+Author: David Barroso, Kirk Byers, Mircea Ulinic
+Author-email: dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com
+License: Apache 2.0
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: setuptools>=38.4.0
+Requires-Dist: cffi>=1.11.3
+Requires-Dist: paramiko>=2.6.0
+Requires-Dist: requests>=2.7.0
+Requires-Dist: textfsm
+Requires-Dist: jinja2
+Requires-Dist: netaddr
+Requires-Dist: pyYAML
+Requires-Dist: pyeapi>=1.0.2
+Requires-Dist: netmiko>=4.1.0
+Requires-Dist: junos-eznc>=2.7.0
+Requires-Dist: scp
+Requires-Dist: lxml>=4.3.0
+Requires-Dist: ncclient
+Requires-Dist: ttp
+Requires-Dist: ttp_templates
+Requires-Dist: netutils>=1.0.0
+Requires-Dist: typing-extensions>=4.3.0
+
 [![PyPI](https://img.shields.io/pypi/v/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![Actions Build](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml/badge.svg?branch=develop)](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
 NAPALM
@@ -27,14 +67,17 @@
 Install
 =======
 
 ```
 pip install napalm
 ```
 
+*Note*: Beginning with release 5.0.0 and later, NAPALM offers support for
+Python 3.8+ only.
+
 *Note*: Beginning with release 4.0.0 and later, NAPALM offers support for
 Python 3.7+ only.
 
 *Note*: Beginning with release 3.0.0 and later, NAPALM offers support for
 Python 3.6+ only.
```

### Comparing `napalm-4.1.0/napalm/__init__.py` & `napalm-5.0.0/napalm/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/__init__.py` & `napalm-5.0.0/napalm/base/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/base.py` & `napalm-5.0.0/napalm/base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __init__(
         self,
         hostname: str,
         username: str,
         password: str,
         timeout: int = 60,
-        optional_args: Dict = None,
+        optional_args: Optional[Dict] = None,
     ) -> None:
         """
         This is the base class you have to inherit from when writing your own Network Driver to
         manage any device. You will, in addition, have to override all the methods specified on
         this class. Make sure you follow the guidelines for every method and that you return the
         correct data.
 
@@ -738,15 +738,14 @@
             }
         """
         raise NotImplementedError
 
     def cli(
         self, commands: List[str], encoding: str = "text"
     ) -> Dict[str, Union[str, Dict[str, Any]]]:
-
         """
         Will execute a list of commands and return the output in a dictionary format.
 
         Example::
 
             {
                 u'show version and haiku':  u'''Hostname: re0.edge01.arn01
@@ -768,15 +767,14 @@
             }
         """
         raise NotImplementedError
 
     def get_bgp_neighbors_detail(
         self, neighbor_address: str = ""
     ) -> Dict[str, models.PeerDetailsDict]:
-
         """
         Returns a detailed view of the BGP neighbors as a dictionary of lists.
 
         :param neighbor_address: Retuns the statistics for a spcific BGP neighbor.
 
         Returns a dictionary of dictionaries. The keys for the first dictionary will be the vrf
         (global if no vrf).
@@ -863,15 +861,14 @@
                     ]
                 }
             }
         """
         raise NotImplementedError
 
     def get_arp_table(self, vrf: str = "") -> List[models.ARPTableDict]:
-
         """
         Returns a list of dictionaries having the following set of keys:
             * interface (string)
             * mac (string)
             * ip (string)
             * age (float)
 
@@ -898,15 +895,14 @@
                 }
             ]
 
         """
         raise NotImplementedError
 
     def get_ntp_peers(self) -> Dict[str, models.NTPPeerDict]:
-
         """
         Returns the NTP peers configuration as dictionary.
         The keys of the dictionary represent the IP Addresses of the peers.
         Inner dictionaries do not have yet any available keys.
 
         Example::
 
@@ -918,15 +914,14 @@
             }
 
         """
 
         raise NotImplementedError
 
     def get_ntp_servers(self) -> Dict[str, models.NTPServerDict]:
-
         """
         Returns the NTP servers configuration as dictionary.
         The keys of the dictionary represent the IP Addresses of the servers.
         Inner dictionaries do not have yet any available keys.
 
         Example::
 
@@ -938,15 +933,14 @@
             }
 
         """
 
         raise NotImplementedError
 
     def get_ntp_stats(self) -> List[models.NTPStats]:
-
         """
         Returns a list of NTP synchronization statistics.
 
             * remote (string)
             * referenceid (string)
             * synchronized (True/False)
             * stratum (int)
@@ -975,15 +969,14 @@
                     'jitter'        : 2.695
                 }
             ]
         """
         raise NotImplementedError
 
     def get_interfaces_ip(self) -> Dict[str, models.InterfacesIPDict]:
-
         """
         Returns all configured IP addresses on all interfaces as a dictionary of dictionaries.
         Keys of the main dictionary represent the name of the interface.
         Values of the main dictionary represent are dictionaries that may consist of two keys
         'ipv4' and 'ipv6' (one, both or none) which are themselves dictionaries with the IP
         addresses as keys.
         Each IP Address dictionary has the following keys:
@@ -1029,15 +1022,14 @@
                     }
                 }
             }
         """
         raise NotImplementedError
 
     def get_mac_address_table(self) -> List[models.MACAdressTable]:
-
         """
         Returns a lists of dictionaries. Each dictionary represents an entry in the MAC Address
         Table, having the following keys:
 
             * mac (string)
             * interface (string)
             * vlan (int)
@@ -1082,15 +1074,14 @@
             ]
         """
         raise NotImplementedError
 
     def get_route_to(
         self, destination: str = "", protocol: str = "", longer: bool = False
     ) -> Dict[str, models.RouteDict]:
-
         """
         Returns a dictionary of dictionaries containing details of all available routes to a
         destination.
 
         :param destination: The destination prefix to be used when filtering the routes.
         :param protocol: Retrieve the routes only for a specific protocol.
         :type protocol: optional
@@ -1157,15 +1148,14 @@
                     }
                 ]
             }
         """
         raise NotImplementedError
 
     def get_snmp_information(self) -> models.SNMPDict:
-
         """
         Returns a dict of dicts containing SNMP configuration.
         Each inner dictionary contains these fields
 
             * chassis_id (string)
             * community (dictionary)
             * contact (string)
@@ -1605,24 +1595,29 @@
                     }
                 }
             }
         """
         raise NotImplementedError
 
     def get_config(
-        self, retrieve: str = "all", full: bool = False, sanitized: bool = False
+        self,
+        retrieve: str = "all",
+        full: bool = False,
+        sanitized: bool = False,
+        format: str = "text",
     ) -> models.ConfigDict:
         """
         Return the configuration of a device.
 
         Args:
             retrieve(string): Which configuration type you want to populate, default is all of them.
                               The rest will be set to "".
             full(bool): Retrieve all the configuration. For instance, on ios, "sh run all".
             sanitized(bool): Remove secret data. Default: ``False``.
+            format(string): The configuration format style to be retrieved.
 
         Returns:
           The object returned is a dictionary with a key for each configuration store:
 
             - running(string) - Representation of the native running configuration
             - candidate(string) - Representation of the native candidate configuration. If the
               device doesnt differentiate between running and startup configuration this will an
```

### Comparing `napalm-4.1.0/napalm/base/clitools/cl_napalm.py` & `napalm-5.0.0/napalm/base/clitools/cl_napalm.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/clitools/cl_napalm_configure.py` & `napalm-5.0.0/napalm/base/clitools/cl_napalm_configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 logger = logging.getLogger("cl-napalm-config.py")
 
 
 def run(
     vendor, hostname, user, password, strategy, optional_args, config_file, dry_run
 ):
-
     logger.debug('Getting driver for OS "{driver}"'.format(driver=vendor))
     driver = get_network_driver(vendor)
 
     optional_args = parse_optional_args(optional_args)
     logger.debug(
         'Connecting to device "{}" with user "{}" and optional_args={}'.format(
             hostname, user, optional_args
```

### Comparing `napalm-4.1.0/napalm/base/clitools/cl_napalm_test.py` & `napalm-5.0.0/napalm/base/clitools/cl_napalm_test.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/clitools/cl_napalm_validate.py` & `napalm-5.0.0/napalm/base/clitools/cl_napalm_validate.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/clitools/helpers.py` & `napalm-5.0.0/napalm/base/clitools/helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/constants.py` & `napalm-5.0.0/napalm/base/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/exceptions.py` & `napalm-5.0.0/napalm/base/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     session or it is dropped by a firewall or
     the server.
     """
 
     pass
 
 
+class UnsupportedVersion(ConnectionException):
+    pass
+
+
 class ReplaceConfigException(NapalmException):
     pass
 
 
 class MergeConfigException(NapalmException):
     pass
```

### Comparing `napalm-4.1.0/napalm/base/helpers.py` & `napalm-5.0.0/napalm/base/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions for the NAPALM base."""
+
 import ipaddress
 import itertools
 import logging
 
 # std libs
 import os
 import re
```

### Comparing `napalm-4.1.0/napalm/base/mock.py` & `napalm-5.0.0/napalm/base/mock.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/models.py` & `napalm-5.0.0/napalm/base/models.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/netmiko_helpers.py` & `napalm-5.0.0/napalm/base/netmiko_helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/test/base.py` & `napalm-5.0.0/napalm/base/test/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,15 +525,14 @@
             result = result and self._test_model(
                 models.PingResultDictEntry, ping_result
             )
 
         self.assertTrue(result)
 
     def test_traceroute(self):
-
         destination = "8.8.8.8"
         try:
             get_traceroute = self.device.traceroute(destination)
         except NotImplementedError:
             raise SkipTest()
         result = isinstance(get_traceroute.get("success"), dict)
         traceroute_results = get_traceroute.get("success", {})
@@ -543,43 +542,40 @@
                 result = result and self._test_model(
                     models.TracerouteDict, probe_result
                 )
 
         self.assertTrue(result)
 
     def test_get_users(self):
-
         try:
             get_users = self.device.get_users()
         except NotImplementedError:
             raise SkipTest()
         result = len(get_users)
 
         for user, user_details in get_users.items():
             result = result and self._test_model(models.UsersDict, user_details)
             result = result and (0 <= user_details.get("level") <= 15)
 
         self.assertTrue(result)
 
     def test_get_optics(self):
-
         try:
             get_optics = self.device.get_optics()
         except NotImplementedError:
             raise SkipTest()
 
         assert isinstance(get_optics, dict)
 
         for iface, iface_data in get_optics.items():
             assert isinstance(iface, str)
             for channel in iface_data["physical_channels"]["channel"]:
                 assert len(channel) == 2
                 assert isinstance(channel["index"], int)
                 for field in ["input_power", "output_power", "laser_bias_current"]:
-
                     assert len(channel["state"][field]) == 4
                     assert isinstance(channel["state"][field]["instant"], float)
                     assert isinstance(channel["state"][field]["avg"], float)
                     assert isinstance(channel["state"][field]["min"], float)
                     assert isinstance(channel["state"][field]["max"], float)
 
     def test_get_config(self):
```

### Comparing `napalm-4.1.0/napalm/base/test/conftest.py` & `napalm-5.0.0/napalm/base/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test fixtures."""
+
 import ast
 import json
 import os
 
 NAPALM_TEST_MOCK = ast.literal_eval(os.getenv("NAPALM_TEST_MOCK", default="1"))
 NAPALM_HOSTNAME = os.getenv("NAPALM_HOSTNAME", default="127.0.0.1")
 NAPALM_USERNAME = os.getenv("NAPALM_USERNAME", default="vagrant")
```

### Comparing `napalm-4.1.0/napalm/base/test/double.py` & `napalm-5.0.0/napalm/base/test/double.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base class for Test doubles."""
+
 import json
 import re
 import os
 import sys
 
 
 class BaseTestDouble(object):
```

### Comparing `napalm-4.1.0/napalm/base/test/getters.py` & `napalm-5.0.0/napalm/base/test/getters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Testing framework."""
+
 import functools
 from itertools import zip_longest
 import inspect
 import json
 
 import pytest
 from napalm.base.test import helpers
@@ -108,15 +109,16 @@
 class BaseTestGetters(object):
     """Base class for testing drivers."""
 
     def test_method_signatures(self):
         """
         Test that all methods have the same signature.
 
-        The type hint annotations are ignored here because the import paths might differ."""
+        The type hint annotations are ignored here because the import paths might differ.
+        """
         errors = {}
         cls = self.driver
         # Create fictional driver instance (py3 needs bound methods)
         tmp_obj = cls(hostname="test", username="admin", password="pwd")
         attrs = [m for m, v in inspect.getmembers(tmp_obj)]
         for attr in attrs:
             func = getattr(tmp_obj, attr)
@@ -489,15 +491,14 @@
 
         for iface, iface_data in get_optics.items():
             assert isinstance(iface, str)
             for channel in iface_data["physical_channels"]["channel"]:
                 assert len(channel) == 2
                 assert isinstance(channel["index"], int)
                 for field in ["input_power", "output_power", "laser_bias_current"]:
-
                     assert len(channel["state"][field]) == 4
                     assert isinstance(channel["state"][field]["instant"], float)
                     assert isinstance(channel["state"][field]["avg"], float)
                     assert isinstance(channel["state"][field]["min"], float)
                     assert isinstance(channel["state"][field]["max"], float)
 
         return get_optics
```

### Comparing `napalm-4.1.0/napalm/base/test/helpers.py` & `napalm-5.0.0/napalm/base/test/helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/base/utils/jinja_filters.py` & `napalm-5.0.0/napalm/base/utils/jinja_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some common jinja filters."""
+
 from typing import Dict, Any
 
 
 class CustomJinjaFilters(object):
     """Utility filters for jinja2."""
 
     @classmethod
```

### Comparing `napalm-4.1.0/napalm/base/utils/string_parsers.py` & `napalm-5.0.0/napalm/base/utils/string_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Common methods to normalize a string """
+
 import re
 import struct
 from typing import Union, List, Iterable, Dict, Optional, Tuple
 
 
 def convert(text: str) -> Union[str, int]:
     """Convert text to integer, if it is a digit."""
```

### Comparing `napalm-4.1.0/napalm/base/validate.py` & `napalm-5.0.0/napalm/base/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Validation methods for the NAPALM base.
 
 See: https://napalm.readthedocs.io/en/latest/validate.html
 """
+
 import yaml
 import copy
 import re
+from math import isclose
 from typing import Dict, List, Union, TypeVar, Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from napalm.base import NetworkDriver
 from napalm.base.exceptions import ValidationException
 from napalm.base import models
 
 
 # We put it here to compile it only once
 numeric_compare_regex = re.compile(r"^(<|>|<=|>=|==|!=)(\d+(\.\d+){0,1})$")
+numeric_tolerance_regex = re.compile(r"^(\d+)%(\d+)$")
 
 
 def _get_validation_file(validation_file: str) -> Dict[str, Dict]:
     try:
         with open(validation_file, "r") as stream:
             try:
                 validation_source = yaml.safe_load(stream)
@@ -151,22 +154,25 @@
     elif isinstance(src, str):
         if src.startswith("<") or src.startswith(">"):
             cmp_result = _compare_numeric(src, dst)
             return cmp_result
         elif "<->" in src and len(src.split("<->")) == 2:
             cmp_result = _compare_range(src, dst)
             return cmp_result
+        elif re.search(r"^\d+%\d+$", src):
+            cmp_result = _compare_tolerance(src, dst)
+            return cmp_result
         else:
             m = re.search(src, str(dst))
             if m:
                 return bool(m)
             else:
                 return src == dst
 
-    elif type(src) == type(dst) == list:
+    elif isinstance(src, list) and isinstance(dst, list):
         pairs = zip(src, dst)
         diff_lists = [
             [(k, x[k], y[k]) for k in x if not re.search(x[k], y[k])]
             for x, y in pairs
             if x != y
         ]
         return empty_tree(diff_lists)
@@ -210,14 +216,30 @@
 
     if float(match[0]) <= dst_num <= float(match[1]):
         return True
     else:
         return False
 
 
+def _compare_tolerance(src_num: str, dst_num: str) -> bool:
+    """Compare against a tolerance percentage either side. You can use 't%%d'."""
+    dst_num = float(dst_num)
+
+    match = numeric_tolerance_regex.match(src_num)
+    if not match:
+        error = "Failed tolerance comparison. Collected: {}. Expected: {}".format(
+            dst_num, src_num
+        )
+        raise ValueError(error)
+
+    src_num = float(match.group(2))
+    max_diff = src_num * int(match.group(1)) / 100
+    return isclose(src_num, dst_num, abs_tol=max_diff)
+
+
 def empty_tree(input_list: List) -> bool:
     """Recursively iterate through values in nested lists."""
     for item in input_list:
         if not isinstance(item, list) or not empty_tree(item):
             return False
     return True
```

### Comparing `napalm-4.1.0/napalm/eos/__init__.py` & `napalm-5.0.0/napalm/eos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/eos.py` & `napalm-5.0.0/napalm/eos/eos.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,18 @@
 from napalm.base.exceptions import (
     CommitError,
     ConnectionException,
     MergeConfigException,
     ReplaceConfigException,
     SessionLockedException,
     CommandErrorException,
+    UnsupportedVersion,
 )
 from napalm.eos.constants import LLDP_CAPAB_TRANFORM_TABLE
-from napalm.eos.pyeapi_syntax_wrapper import Node
 from napalm.eos.utils.versions import EOSVersion
-from napalm.eos.utils.cli_syntax import cli_convert
 import napalm.base.constants as c
 
 # local modules
 # here add local imports
 # e.g. import napalm.eos.helpers etc.
 
 
@@ -119,23 +118,21 @@
         self.device = None
         self.hostname = hostname
         self.username = username
         self.password = password
         self.timeout = timeout
         self.config_session = None
         self.locked = False
-        self.cli_version = 1
 
         self.platform = "eos"
         self.profile = [self.platform]
         self.optional_args = optional_args or {}
 
         self.enablepwd = self.optional_args.pop("enable_password", "")
         self.eos_autoComplete = self.optional_args.pop("eos_autoComplete", None)
-        self.fn0039_config = self.optional_args.pop("eos_fn0039_config", False)
 
         # Define locking method
         self.lock_disable = self.optional_args.pop("lock_disable", False)
 
         self.force_cfg_session_invalid = self.optional_args.pop(
             "force_cfg_session_invalid", False
         )
@@ -197,45 +194,43 @@
     def open(self):
         """Implementation of NAPALM method open."""
         if self.transport == "ssh":
             self.device = self._netmiko_open(
                 device_type="arista_eos",
                 netmiko_optional_args=self.netmiko_optional_args,
             )
-            # let's try to determine if we need to use new EOS cli syntax
-            sh_ver = self._run_commands(["show version"])
-            if EOSVersion(sh_ver[0]["version"]) >= EOSVersion("4.23.0"):
-                self.cli_version = 2
         else:
             try:
                 connection = self.transport_class(
                     host=self.hostname,
                     username=self.username,
                     password=self.password,
                     timeout=self.timeout,
                     **self.eapi_kwargs,
                 )
 
                 if self.device is None:
-                    self.device = Node(connection, enablepwd=self.enablepwd)
+                    self.device = pyeapi.client.Node(
+                        connection, enablepwd=self.enablepwd
+                    )
                 # does not raise an Exception if unusable
 
-                # let's try to determine if we need to use new EOS cli syntax
-                sh_ver = self.device.run_commands(["show version"])
-                self.cli_version = (
-                    2 if EOSVersion(sh_ver[0]["version"]) >= EOSVersion("4.23.0") else 1
-                )
-
-                self.device.update_cli_version(self.cli_version)
             except ConnectionError as ce:
                 # and this is raised either if device not avaiable
                 # either if HTTP(S) agent is not enabled
                 # show management api http-commands
                 raise ConnectionException(str(ce))
 
+        # endif self.transport
+
+        sh_ver = self._run_commands(["show version"])
+        self._eos_version = EOSVersion(sh_ver[0]["version"])
+        if self._eos_version < EOSVersion("4.23.0"):
+            raise UnsupportedVersion(self._eos_version)
+
     def close(self):
         """Implementation of NAPALM method close."""
         self.discard_config()
         if self.transport == "ssh":
             self._netmiko_close()
         elif hasattr(self.device.connection, "close") and callable(
             self.device.connection.close
@@ -259,19 +254,14 @@
             self.device.connection.is_alive
         ):
             return self.device.connection.is_alive()
         return {"is_alive": True}  # always true as eAPI is HTTP-based
 
     def _run_commands(self, commands, **kwargs):
         if self.transport == "ssh":
-            if self.fn0039_config:
-                if isinstance(commands, str):
-                    commands = [cli_convert(commands, self.cli_version)]
-                else:
-                    commands = [cli_convert(cmd, self.cli_version) for cmd in commands]
             ret = []
             for command in commands:
                 if kwargs.get("encoding") == "text":
                     cmd_output = self._netmiko_device.send_command(command).replace(
                         "% Invalid input", ""
                     )
                     ret.append({"output": cmd_output})
@@ -459,18 +449,17 @@
         try:
             if not any(cmd == "end" for cmd in commands):
                 commands.append("end")  # exit config mode
             if self.eos_autoComplete is not None:
                 self._run_commands(
                     commands,
                     autoComplete=self.eos_autoComplete,
-                    fn0039_transform=self.fn0039_config,
                 )
             else:
-                self._run_commands(commands, fn0039_transform=self.fn0039_config)
+                self._run_commands(commands)
         except pyeapi.eapilib.CommandError as e:
             self.discard_config()
             msg = str(e)
             if replace:
                 raise ReplaceConfigException(msg)
             else:
                 raise MergeConfigException(msg)
@@ -687,21 +676,24 @@
         def get_re_group(res, key, default=None):
             """Small helper to retrieve data from re match groups"""
             try:
                 return res.group(key)
             except KeyError:
                 return default
 
-        NEIGHBOR_FILTER = "bgp neighbors vrf all | include IPv[46] (Unicast|6PE):.*[0-9]+ | grep -v ' IPv[46] Unicast:/.' | remote AS |^Local AS|Desc|BGP state |remote router ID"  # noqa
+        NEIGHBOR_FILTER = "vrf all | include IPv[46] (Unicast|6PE):.*[0-9]+ | grep -v ' IPv[46] Unicast:/.' | remote AS |^Local AS|Desc|BGP state |remote router ID"  # noqa
         output_summary_cmds = self._run_commands(
             ["show ipv6 bgp summary vrf all", "show ip bgp summary vrf all"],
             encoding="json",
         )
         output_neighbor_cmds = self._run_commands(
-            ["show ip " + NEIGHBOR_FILTER, "show ipv6 " + NEIGHBOR_FILTER],
+            [
+                "show ip bgp neighbors " + NEIGHBOR_FILTER,
+                "show ipv6 bgp peers " + NEIGHBOR_FILTER,
+            ],
             encoding="text",
         )
 
         bgp_counters = defaultdict(lambda: dict(peers={}))
         for summary in output_summary_cmds:
             """
             Json output looks as follows
@@ -827,18 +819,21 @@
                     "temperature": temp,
                     "is_alert": temp > s["overheatThreshold"],
                     "is_critical": temp > s["criticalThreshold"],
                 }
                 yield name, values
 
         sh_version_out = self._run_commands(["show version"])
-        is_veos = sh_version_out[0]["modelName"].lower() == "veos"
-        commands = ["show environment cooling", "show environment temperature"]
+        is_veos = sh_version_out[0]["modelName"].lower() in ["veos", "ceoslab"]
+        commands = [
+            "show system environment cooling",
+            "show system environment temperature",
+        ]
         if not is_veos:
-            commands.append("show environment power")
+            commands.append("show system environment power")
             fans_output, temp_output, power_output = self._run_commands(commands)
         else:
             fans_output, temp_output = self._run_commands(commands)
         environment_counters = {"fans": {}, "temperature": {}, "power": {}, "cpu": {}}
         cpu_output = self._run_commands(["show processes top once"], encoding="text")[
             0
         ]["output"]
@@ -903,15 +898,14 @@
 
         return environment_counters
 
     def _transform_lldp_capab(self, capabilities):
         return sorted([LLDP_CAPAB_TRANFORM_TABLE[c.lower()] for c in capabilities])
 
     def get_lldp_neighbors_detail(self, interface=""):
-
         lldp_neighbors_out = {}
 
         filters = []
         if interface:
             filters.append(interface)
 
         commands = [
@@ -1081,15 +1075,14 @@
                     for key in _GROUP_FIELD_MAP_.values()
                     if key in group_dict and key in _PEER_FIELD_MAP_.values()
                 }
             )  # copy in values from group dict if present
             return neighbor_dict
 
         def parse_options(options, default_value=False):
-
             if not options:
                 return {}
 
             config_property = options[0]
             field_name = _PROPERTY_FIELD_MAP_.get(config_property)
             field_type = _PROPERTY_TYPE_MAP_.get(config_property)
             field_value = _DATATYPE_DEFAULT_.get(field_type)  # to get the default value
@@ -1326,15 +1319,14 @@
                 )
             except Exception:
                 continue  # jump to next line
 
         return ntp_stats
 
     def get_interfaces_ip(self):
-
         interfaces_ip = {}
 
         interfaces_ipv4_out = self._run_commands(["show ip interface"])[0]["interfaces"]
         try:
             interfaces_ipv6_out = self._run_commands(["show ipv6 interface"])[0][
                 "interfaces"
             ]
@@ -1399,15 +1391,15 @@
                         napalm.base.helpers.ip,
                         interface_details.get("linkLocal", {}).get("address"),
                     ),
                     "masklen": int(
                         interface_details.get("linkLocal", {})
                         .get("subnet", "::/0")
                         .split("/")[-1]
-                    )
+                    ),
                     # when no link-local set, address will be None and maslken 0
                 }
             )
             for address in interface_details.get("addresses"):
                 ipv6_list.append(
                     {
                         "address": napalm.base.helpers.ip(address.get("address")),
@@ -1423,15 +1415,14 @@
                     interfaces_ip[interface_name]["ipv6"][ip.get("address")] = {
                         "prefix_length": ip.get("masklen")
                     }
 
         return interfaces_ip
 
     def get_mac_address_table(self):
-
         mac_table = []
 
         commands = ["show mac address-table"]
 
         mac_entries = (
             self._run_commands(commands)[0]
             .get("unicastTable", {})
@@ -1527,31 +1518,20 @@
                         if "vtepAddr" in next_hop:
                             next_hop["nexthopAddr"] = next_hop["vtepAddr"]
                             next_hop["interface"] = "vxlan1"
                         nexthop_ip = napalm.base.helpers.ip(next_hop.get("nexthopAddr"))
                         nexthop_interface_map[nexthop_ip] = next_hop.get("interface")
                     metric = route_details.get("metric")
                     if _vrf not in vrf_cache.keys():
-                        if self.cli_version == 1:
-                            command = "show ip{ipv} bgp {dest} {longer} detail vrf {_vrf}".format(
-                                ipv=ipv,
-                                dest=destination,
-                                longer="longer-prefixes" if longer else "",
-                                _vrf=_vrf,
-                            )
-                        else:
-                            # Newer EOS can't mix longer-prefix and detail
-                            command = (
-                                "show ip{ipv} bgp {dest} {longer} vrf {_vrf}".format(
-                                    ipv=ipv,
-                                    dest=destination,
-                                    longer="longer-prefixes" if longer else "",
-                                    _vrf=_vrf,
-                                )
-                            )
+                        command = "show ip{ipv} bgp {dest} {longer} vrf {_vrf}".format(
+                            ipv=ipv,
+                            dest=destination,
+                            longer="longer-prefixes" if longer else "",
+                            _vrf=_vrf,
+                        )
                         vrf_cache.update(
                             {
                                 _vrf: self._run_commands([command])[0]
                                 .get("vrfs", {})
                                 .get(_vrf, {})
                             }
                         )
@@ -1656,15 +1636,19 @@
 
     def get_snmp_information(self):
         """get_snmp_information() for EOS.  Re-written to not use TextFSM"""
 
         # Default values
         snmp_dict = {"chassis_id": "", "location": "", "contact": "", "community": {}}
 
-        commands = ["show snmp chassis", "show snmp location", "show snmp contact"]
+        commands = [
+            "show snmp v2-mib chassis",
+            "show snmp v2-mib location",
+            "show snmp v2-mib contact",
+        ]
         snmp_config = self._run_commands(commands, encoding="json")
         for line in snmp_config:
             for k, v in line.items():
                 if k == "chassisId":
                     snmp_dict["chassis_id"] = v
                 else:
                     # Some EOS versions add extra quotes
@@ -1691,15 +1675,15 @@
                 return "ssh_rsa", str(sshkey)
             elif sshkey.startswith("ssh-dss"):
                 return "ssh_dsa", str(sshkey)
             return "ssh_rsa", ""
 
         users = {}
 
-        commands = ["show user-account"]
+        commands = ["show users accounts"]
         user_items = self._run_commands(commands)[0].get("users", {})
 
         for user, user_details in user_items.items():
             user_details.pop("username", "")
             sshkey_value = user_details.pop("sshAuthorizedKey", "")
             sshkey_type, sshkey_value = _sshkey_type(sshkey_value)
             if sshkey_value != "":
@@ -1721,15 +1705,14 @@
         self,
         destination,
         source=c.TRACEROUTE_SOURCE,
         ttl=c.TRACEROUTE_TTL,
         timeout=c.TRACEROUTE_TIMEOUT,
         vrf=c.TRACEROUTE_VRF,
     ):
-
         _HOP_ENTRY_PROBE = [
             r"\s+",
             r"(",  # beginning of host_name (ip_address) RTT group
             r"(",  # beginning of host_name (ip_address) group only
             r"([a-zA-Z0-9\.:-]*)",  # hostname
             r"\s+",
             r"\(?([a-fA-F0-9\.:][^\)]*)\)?"  # IP Address between brackets
@@ -1878,15 +1861,14 @@
 
             # Using preset template to extract peer info
             peer_info = napalm.base.helpers.textfsm_extractor(
                 self, extractor_type, peer_output
             )
 
             for item in peer_info:
-
                 # Determining a few other fields in the final peer_info
                 item["up"] = True if item["up"] == "up" else False
                 item["local_address_configured"] = (
                     True if item["local_address"] else False
                 )
                 item["multihop"] = (
                     False if item["multihop"] == "0" or item["multihop"] == "" else True
@@ -1938,43 +1920,42 @@
                 item.pop("received_ipv6_prefix_count", None)
 
                 peer_details.append(item)
 
             return peer_details
 
         def _append(bgp_dict, peer_info):
-
             remote_as = peer_info["remote_as"]
             vrf_name = peer_info["routing_table"]
 
             if vrf_name not in bgp_dict.keys():
                 bgp_dict[vrf_name] = {}
             if remote_as not in bgp_dict[vrf_name].keys():
                 bgp_dict[vrf_name][remote_as] = []
 
             bgp_dict[vrf_name][remote_as].append(peer_info)
 
         commands = []
         summary_commands = []
         if not neighbor_address:
             commands.append("show ip bgp neighbors vrf all")
-            commands.append("show ipv6 bgp neighbors vrf all")
+            commands.append("show ipv6 bgp peers vrf all")
             summary_commands.append("show ip bgp summary vrf all")
             summary_commands.append("show ipv6 bgp summary vrf all")
         else:
             try:
                 peer_ver = ipaddress.ip_address(neighbor_address).version
             except Exception as e:
                 raise e
 
             if peer_ver == 4:
                 commands.append("show ip bgp neighbors %s vrf all" % neighbor_address)
                 summary_commands.append("show ip bgp summary vrf all")
             elif peer_ver == 6:
-                commands.append("show ipv6 bgp neighbors %s vrf all" % neighbor_address)
+                commands.append("show ipv6 bgp peers %s vrf all" % neighbor_address)
                 summary_commands.append("show ipv6 bgp summary vrf all")
 
         raw_output = self._run_commands(commands, encoding="text")
         bgp_summary = self._run_commands(summary_commands, encoding="json")
 
         bgp_detail_info = {}
 
@@ -1991,29 +1972,27 @@
 
         else:
             # Using preset template to extract peer info
             v4_peer_info = _parse_per_peer_bgp_detail(raw_output[0]["output"])
             v6_peer_info = _parse_per_peer_bgp_detail(raw_output[1]["output"])
 
         for peer_info in v4_peer_info:
-
             vrf_name = peer_info["routing_table"]
             peer_remote_addr = peer_info["remote_address"]
             peer_info["accepted_prefix_count"] = (
                 bgp_summary[0]["vrfs"][vrf_name]["peers"][peer_remote_addr][
                     "prefixAccepted"
                 ]
                 if peer_remote_addr in bgp_summary[0]["vrfs"][vrf_name]["peers"].keys()
                 else 0
             )
 
             _append(bgp_detail_info, peer_info)
 
         for peer_info in v6_peer_info:
-
             vrf_name = peer_info["routing_table"]
             peer_remote_addr = peer_info["remote_address"]
             peer_info["accepted_prefix_count"] = (
                 bgp_summary[1]["vrfs"][vrf_name]["peers"][peer_remote_addr][
                     "prefixAccepted"
                 ]
                 if peer_remote_addr in bgp_summary[1]["vrfs"][vrf_name]["peers"].keys()
@@ -2021,15 +2000,14 @@
             )
 
             _append(bgp_detail_info, peer_info)
 
         return bgp_detail_info
 
     def get_optics(self):
-
         command = ["show interfaces transceiver"]
 
         output = self._run_commands(command, encoding="json")[0]["interfaces"]
 
         # Formatting data into return data structure
         optics_detail = {}
 
@@ -2069,15 +2047,15 @@
             }
 
             port_detail["physical_channels"]["channel"].append(optic_states)
             optics_detail[port] = port_detail
 
         return optics_detail
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
+    def get_config(self, retrieve="all", full=False, sanitized=False, format="text"):
         """get_config implementation for EOS."""
         get_startup = retrieve == "all" or retrieve == "startup"
         get_running = retrieve == "all" or retrieve == "running"
         get_candidate = (
             retrieve == "all" or retrieve == "candidate"
         ) and self.config_session
 
@@ -2175,26 +2153,21 @@
                 vrf["interfaces"].extend([t.strip() for t in line[4].split(",") if t])
         if current_vrf:
             vrfs.append(vrf)
 
         return vrfs
 
     def _show_vrf(self):
-        if self.cli_version == 2:
-            return self._show_vrf_json()
-        else:
-            return self._show_vrf_text()
+        return self._show_vrf_json()
 
     def _get_vrfs(self):
         output = self._show_vrf()
 
         vrfs = [str(vrf["name"]) for vrf in output]
 
-        vrfs.append("default")
-
         return vrfs
 
     def get_network_instances(self, name=""):
         """get_network_instances implementation for EOS."""
 
         output = self._show_vrf()
         vrfs = {}
```

### Comparing `napalm-4.1.0/napalm/eos/templates/delete_snmp_config.j2` & `napalm-5.0.0/napalm/eos/templates/delete_snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/templates/snmp_config.j2` & `napalm-5.0.0/napalm/eos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl` & `napalm-5.0.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl` & `napalm-5.0.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/utils/textfsm_templates/vrf.tpl` & `napalm-5.0.0/napalm/eos/utils/textfsm_templates/vrf.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/eos/utils/versions.py` & `napalm-5.0.0/napalm/eos/utils/versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some functions to work with EOS version numbers"""
+
 import re
 
 
 class EOSVersion:
     """
     Class to represent EOS version
     """
```

### Comparing `napalm-4.1.0/napalm/ios/__init__.py` & `napalm-5.0.0/napalm/ios/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/ios/ios.py` & `napalm-5.0.0/napalm/ios/ios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """NAPALM Cisco IOS Handler."""
+
 # Copyright 2015 Spotify AB. All rights reserved.
 #
 # The contents of this file are licensed under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with the
 # License. You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
@@ -55,15 +56,15 @@
 WEEK_SECONDS = 7 * DAY_SECONDS
 YEAR_SECONDS = 365 * DAY_SECONDS
 
 # STD REGEX PATTERNS
 IP_ADDR_REGEX = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
 IPV4_ADDR_REGEX = IP_ADDR_REGEX
 IPV6_ADDR_REGEX_1 = r"::"
-IPV6_ADDR_REGEX_2 = r"[0-9a-fA-F:]{1,39}::[0-9a-fA-F:]{1,39}"
+IPV6_ADDR_REGEX_2 = r"[0-9a-fA-F:]{0,39}::[0-9a-fA-F:]{0,39}"
 IPV6_ADDR_REGEX_3 = (
     r"[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:"
     "[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}:[0-9a-fA-F]{1,4}"
 )
 # Should validate IPv6 address using an IP address library after matching with this regex
 IPV6_ADDR_REGEX = "(?:{}|{}|{})".format(
     IPV6_ADDR_REGEX_1, IPV6_ADDR_REGEX_2, IPV6_ADDR_REGEX_3
@@ -779,15 +780,14 @@
                 file_system=file_system,
             )
         use_scp = True
         if self.inline_transfer:
             use_scp = False
 
         with TransferClass(**kwargs) as transfer:
-
             # Check if file already exists and has correct MD5
             if transfer.check_file_exists() and transfer.compare_md5():
                 msg = "File already exists and has correct MD5: no SCP needed"
                 return (True, msg)
             if not transfer.verify_space_available():
                 msg = "Insufficient space available on remote device"
                 return (False, msg)
@@ -1216,15 +1216,14 @@
         output = self._send_command(command)
 
         interface = description = mac_address = speed = speedformat = ""
         is_enabled = is_up = None
 
         interface_dict = {}
         for line in output.splitlines():
-
             interface_regex_1 = r"^(\S+?)\s+is\s+(.+?),\s+line\s+protocol\s+is\s+(\S+)"
             interface_regex_2 = r"^(\S+)\s+is\s+(up|down)"
             interface_regex_3 = (
                 r"^(Control Plane Interface)"
                 r"\s+is\s+(.+?),\s+line\s+protocol\s+is\s+(\S+)"
             )
             for pattern in (interface_regex_1, interface_regex_2, interface_regex_3):
@@ -1955,20 +1954,25 @@
             afi = entry["afi"].lower()
             # check that we're looking at a supported afi
             if afi not in supported_afi:
                 continue
             # get neighbor_entry out of neighbor data
             neighbor_entry = None
             for neighbor in neighbor_data:
-                if (
-                    neighbor["afi"].lower() == afi
-                    and napalm.base.helpers.ip(neighbor["remote_addr"]) == remote_addr
-                ):
-                    neighbor_entry = neighbor
-                    break
+                current_neighbor = napalm.base.helpers.ip(neighbor["remote_addr"])
+                if neighbor["afi"].lower() == afi and current_neighbor == remote_addr:
+                    # Neighbor IPs in VRFs can overlap, so make sure
+                    # we haven't covered this VRF + IP already
+                    vrf = neighbor["vrf"] or "global"
+                    if (
+                        vrf == "global"
+                        or current_neighbor not in bgp_neighbor_data[vrf]["peers"]
+                    ):
+                        neighbor_entry = neighbor
+                        break
             # check for proper session data for the afi
             if neighbor_entry is None:
                 continue
             elif not isinstance(neighbor_entry, dict):
                 raise ValueError(
                     msg="Couldn't find neighbor data for %s in afi %s"
                     % (remote_addr, afi)
@@ -2093,71 +2097,83 @@
             bgp_neigh = napalm.base.helpers.textfsm_extractor(
                 self, "ip_bgp_neigh", raw_bgp_neigh
             )[0]
             details = {
                 "up": neigh["up"] != "never",
                 "local_as": napalm.base.helpers.as_number(neigh["local_as"]),
                 "remote_as": napalm.base.helpers.as_number(neigh["remote_as"]),
-                "router_id": napalm.base.helpers.ip(bgp_neigh["router_id"])
-                if bgp_neigh["router_id"]
-                else "",
-                "local_address": napalm.base.helpers.ip(bgp_neigh["local_address"])
-                if bgp_neigh["local_address"]
-                else "",
+                "router_id": (
+                    napalm.base.helpers.ip(bgp_neigh["router_id"])
+                    if bgp_neigh["router_id"]
+                    else ""
+                ),
+                "local_address": (
+                    napalm.base.helpers.ip(bgp_neigh["local_address"])
+                    if bgp_neigh["local_address"]
+                    else ""
+                ),
                 "local_address_configured": False,
-                "local_port": napalm.base.helpers.as_number(bgp_neigh["local_port"])
-                if bgp_neigh["local_port"]
-                else 0,
+                "local_port": (
+                    napalm.base.helpers.as_number(bgp_neigh["local_port"])
+                    if bgp_neigh["local_port"]
+                    else 0
+                ),
                 "routing_table": bgp_neigh["vrf"] if bgp_neigh["vrf"] else "global",
                 "remote_address": napalm.base.helpers.ip(bgp_neigh["neighbor"]),
-                "remote_port": napalm.base.helpers.as_number(bgp_neigh["remote_port"])
-                if bgp_neigh["remote_port"]
-                else 0,
+                "remote_port": (
+                    napalm.base.helpers.as_number(bgp_neigh["remote_port"])
+                    if bgp_neigh["remote_port"]
+                    else 0
+                ),
                 "multihop": False,
                 "multipath": False,
                 "remove_private_as": False,
                 "import_policy": "",
                 "export_policy": "",
-                "input_messages": napalm.base.helpers.as_number(
-                    bgp_neigh["msg_total_in"]
-                )
-                if bgp_neigh["msg_total_in"]
-                else 0,
-                "output_messages": napalm.base.helpers.as_number(
-                    bgp_neigh["msg_total_out"]
-                )
-                if bgp_neigh["msg_total_out"]
-                else 0,
-                "input_updates": napalm.base.helpers.as_number(
-                    bgp_neigh["msg_update_in"]
-                )
-                if bgp_neigh["msg_update_in"]
-                else 0,
-                "output_updates": napalm.base.helpers.as_number(
-                    bgp_neigh["msg_update_out"]
-                )
-                if bgp_neigh["msg_update_out"]
-                else 0,
+                "input_messages": (
+                    napalm.base.helpers.as_number(bgp_neigh["msg_total_in"])
+                    if bgp_neigh["msg_total_in"]
+                    else 0
+                ),
+                "output_messages": (
+                    napalm.base.helpers.as_number(bgp_neigh["msg_total_out"])
+                    if bgp_neigh["msg_total_out"]
+                    else 0
+                ),
+                "input_updates": (
+                    napalm.base.helpers.as_number(bgp_neigh["msg_update_in"])
+                    if bgp_neigh["msg_update_in"]
+                    else 0
+                ),
+                "output_updates": (
+                    napalm.base.helpers.as_number(bgp_neigh["msg_update_out"])
+                    if bgp_neigh["msg_update_out"]
+                    else 0
+                ),
                 "messages_queued_out": napalm.base.helpers.as_number(neigh["out_q"]),
                 "connection_state": bgp_neigh["bgp_state"],
                 "previous_connection_state": "",
                 "last_event": "",
                 "suppress_4byte_as": (
                     bgp_neigh["four_byte_as"] != "advertised and received"
                     if bgp_neigh["four_byte_as"]
                     else False
                 ),
                 "local_as_prepend": False,
-                "holdtime": napalm.base.helpers.as_number(bgp_neigh["holdtime"])
-                if bgp_neigh["holdtime"]
-                else 0,
+                "holdtime": (
+                    napalm.base.helpers.as_number(bgp_neigh["holdtime"])
+                    if bgp_neigh["holdtime"]
+                    else 0
+                ),
                 "configured_holdtime": 0,
-                "keepalive": napalm.base.helpers.as_number(bgp_neigh["keepalive"])
-                if bgp_neigh["keepalive"]
-                else 0,
+                "keepalive": (
+                    napalm.base.helpers.as_number(bgp_neigh["keepalive"])
+                    if bgp_neigh["keepalive"]
+                    else 0
+                ),
                 "configured_keepalive": 0,
                 "active_prefix_count": 0,
                 "received_prefix_count": 0,
                 "accepted_prefix_count": 0,
                 "suppressed_prefix_count": 0,
                 "advertised_prefix_count": 0,
                 "flap_count": 0,
@@ -3131,15 +3147,15 @@
                         "show ip route vrf {vrf} {prefix} {netmask}".format(
                             vrf=_vrf, prefix=prefix, netmask=netmask
                         )
                     )
             for cmditem in commands:
                 outvrf = self._send_command(cmditem)
                 output.append(outvrf)
-            for (outitem, _vrf) in zip(output, vrfs):  # for all VRFs
+            for outitem, _vrf in zip(output, vrfs):  # for all VRFs
                 route_proto_regex = RE_RP_FROM.search(outitem)
                 if route_proto_regex:
                     route_match = destination
                     if netmask == "":
                         # Get the matching route for a non-exact lookup
                         route_match_regex = RE_RP_ROUTE.search(outitem)
                         if route_match_regex:
@@ -3202,18 +3218,18 @@
                                 "preference": int(rmetric),
                             }
                             # process rt entry only if was created by routing protocol
                             # specified in 'protocol' parameter or if routing protocol
                             # was not specified
                             if protocol == "" or protocol == route_entry["protocol"]:
                                 if route_proto == "bgp":
-                                    route_entry[
-                                        "protocol_attributes"
-                                    ] = self._get_bgp_route_attr(
-                                        destination, _vrf, nh, ip_version
+                                    route_entry["protocol_attributes"] = (
+                                        self._get_bgp_route_attr(
+                                            destination, _vrf, nh, ip_version
+                                        )
                                     )
                                 nh_line_found = (
                                     False  # for next RT entry processing ...
                                 )
                                 routes[route_match].append(route_entry)
         return routes
 
@@ -3298,20 +3314,24 @@
         command = "show run | section username"
         output = self._send_command(command)
         if "Invalid input detected" in output:
             command = "show run | include username"
             output = self._send_command(command)
         for match in re.finditer(username_regex, output, re.M):
             users[match.groupdict()["username"]] = {
-                "level": int(match.groupdict()["priv_level"])
-                if match.groupdict()["priv_level"]
-                else 1,
-                "password": match.groupdict()["pwd_hash"]
-                if match.groupdict()["pwd_hash"]
-                else "",
+                "level": (
+                    int(match.groupdict()["priv_level"])
+                    if match.groupdict()["priv_level"]
+                    else 1
+                ),
+                "password": (
+                    match.groupdict()["pwd_hash"]
+                    if match.groupdict()["pwd_hash"]
+                    else ""
+                ),
                 "sshkeys": [],
             }
         for match in re.finditer(pub_keychain_regex, output, re.M):
             if match.groupdict()["username"] not in users:
                 continue
             users[match.groupdict()["username"]]["sshkeys"] = list(
                 map(
@@ -3546,15 +3566,14 @@
                     host_name = current_element
                     ip_address = current_element
 
         traceroute_dict["success"] = results
         return traceroute_dict
 
     def get_network_instances(self, name=""):
-
         instances = {}
         sh_vrf_detail = self._send_command("show vrf detail")
         show_ip_int_br = self._send_command("show ip interface brief")
 
         # retrieve all interfaces for the default VRF
         interface_dict = {}
         show_ip_int_br = show_ip_int_br.strip()
@@ -3579,15 +3598,14 @@
                 return instances
 
         if "Invalid input detected" in sh_vrf_detail:
             # No VRF support
             return instances
 
         for vrf in sh_vrf_detail.split("\n\n"):
-
             first_part = vrf.split("Address family")[0]
 
             # retrieve the name of the VRF and the Route Distinguisher
             vrf_name, RD = re.match(r"^VRF (\S+).*RD (.*);", first_part).groups()
             if RD == "<not set>":
                 RD = ""
 
@@ -3613,15 +3631,15 @@
                 "interfaces": {"interface": interfaces},
             }
         try:
             return instances if not name else instances[name]
         except AttributeError:
             raise ValueError("The vrf %s does not exist" % name)
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
+    def get_config(self, retrieve="all", full=False, sanitized=False, format="text"):
         """Implementation of get_config for IOS.
 
         Returns the startup or/and running configuration as dictionary.
         The keys of the dictionary represent the type of configuration
         (startup or running). The candidate is always empty string,
         since IOS does not support candidate configuration.
         """
@@ -3722,29 +3740,33 @@
         output = self._send_command(command)
         if output.find("Invalid input detected") >= 0:
             return self._get_vlan_from_id()
         else:
             return self._get_vlan_all_ports(output)
 
     def _get_vlan_all_ports(self, output):
-        find_regexp = re.compile(r"^(\d+)\s+(\S+)\s+\S+(\s+[A-Z][a-z].*)?$")
+        find_regexp = re.compile(
+            r"^(\d+)\s+"  # vlan id
+            r"(.*?(?=active|act\/[isl]{1}shut|act\/unsup))"  # vlan name
+            r"\w+(?:\/\w+)?\S+(\s+[A-Z][a-z].*)?$"  # ports
+        )
         continuation_regexp = re.compile(r"^\s+([A-Z][a-z].*)$")
         output = output.splitlines()
         vlans = {}
 
         was_vlan_or_cont = False
         vlan_id = None
         vlan_name = None
         interfaces = ""
         for line in output:
             vlan_m = find_regexp.match(line)
             if vlan_m:
                 was_vlan_or_cont = True
                 vlan_id = vlan_m.group(1)
-                vlan_name = vlan_m.group(2)
+                vlan_name = vlan_m.group(2).strip()
                 interfaces = vlan_m.group(3) or ""
                 vlans[vlan_id] = {"name": vlan_name, "interfaces": []}
 
             cont_m = None
             if was_vlan_or_cont:
                 cont_m = continuation_regexp.match(line)
                 if cont_m:
@@ -3763,15 +3785,15 @@
             )
 
         return vlans
 
     def _get_vlan_from_id(self):
         command = "show vlan brief"
         output = self._send_command(command)
-        vlan_regexp = r"^(\d+)\s+(\S+)\s+\S+.*$"
+        vlan_regexp = r"^(\d+)\W+(.*?(?=active|act\/[isl]{1}shut|act\/unsup))"
         find_vlan = re.findall(vlan_regexp, output, re.MULTILINE)
         vlans = {}
         for vlan_id, vlan_name in find_vlan:
             output = self._send_command("show vlan id {}".format(vlan_id))
             _vlans = self._get_vlan_all_ports(output)
             if len(_vlans) == 0:
                 vlans[vlan_id] = {"name": vlan_name, "interfaces": []}
```

### Comparing `napalm-4.1.0/napalm/ios/templates/snmp_config.j2` & `napalm-5.0.0/napalm/ios/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl` & `napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl` & `napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl` & `napalm-5.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl` & `napalm-5.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr/__init__.py` & `napalm-5.0.0/napalm/iosxr/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr/constants.py` & `napalm-5.0.0/napalm/iosxr/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr/iosxr.py` & `napalm-5.0.0/napalm/iosxr/iosxr.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         if not self.lock_on_connect:
             self.device.unlock()
 
     def rollback(self):
         self.device.rollback()
 
     def get_facts(self):
-
         facts = {
             "vendor": "Cisco",
             "os_version": "",
             "hostname": "",
             "uptime": -1.0,
             "serial_number": "",
             "fqdn": "",
@@ -252,15 +251,14 @@
                 "interface_list": interface_list,
             }
         )
 
         return facts
 
     def get_interfaces(self):
-
         interfaces = {}
 
         INTERFACE_DEFAULTS = {
             "is_enabled": False,
             "is_up": False,
             "mac_address": "",
             "description": "",
@@ -300,23 +298,33 @@
                     float, napalm.base.helpers.find_txt(interface_tree, "Bandwidth"), 0
                 )
                 * 1e-3,
             )
 
             mtu = int(napalm.base.helpers.find_txt(interface_tree, "MTU"))
             description = napalm.base.helpers.find_txt(interface_tree, "Description")
+            last_flapped = napalm.base.helpers.convert(
+                float,
+                napalm.base.helpers.find_txt(
+                    interface_tree, "LastStateTransitionTime", -1
+                ),
+                -1,
+            )
             interfaces[interface_name] = copy.deepcopy(INTERFACE_DEFAULTS)
             interfaces[interface_name].update(
                 {
                     "is_up": is_up,
                     "speed": speed,
                     "mtu": mtu,
                     "is_enabled": enabled,
                     "mac_address": mac_address,
                     "description": description,
+                    "last_flapped": (
+                        last_flapped / 1e9 if last_flapped != -1.0 else -1.0
+                    ),
                 }
             )
 
         return interfaces
 
     def get_interfaces_counters(self):
         rpc_command = "<Get><Operational><Interfaces><InterfaceTable></InterfaceTable>\
@@ -575,31 +583,31 @@
                     ) + napalm.base.helpers.convert(
                         int,
                         napalm.base.helpers.find_txt(
                             neighbor, "AFData/Entry/PrefixesDenied"
                         ),
                         0,
                     )
-                    this_neighbor["address_family"][this_afi][
-                        "accepted_prefixes"
-                    ] = napalm.base.helpers.convert(
-                        int,
-                        napalm.base.helpers.find_txt(
-                            neighbor, "AFData/Entry/PrefixesAccepted"
-                        ),
-                        0,
+                    this_neighbor["address_family"][this_afi]["accepted_prefixes"] = (
+                        napalm.base.helpers.convert(
+                            int,
+                            napalm.base.helpers.find_txt(
+                                neighbor, "AFData/Entry/PrefixesAccepted"
+                            ),
+                            0,
+                        )
                     )
-                    this_neighbor["address_family"][this_afi][
-                        "sent_prefixes"
-                    ] = napalm.base.helpers.convert(
-                        int,
-                        napalm.base.helpers.find_txt(
-                            neighbor, "AFData/Entry/PrefixesAdvertised"
-                        ),
-                        0,
+                    this_neighbor["address_family"][this_afi]["sent_prefixes"] = (
+                        napalm.base.helpers.convert(
+                            int,
+                            napalm.base.helpers.find_txt(
+                                neighbor, "AFData/Entry/PrefixesAdvertised"
+                            ),
+                            0,
+                        )
                     )
                 except AttributeError:
                     this_neighbor["address_family"][this_afi]["received_prefixes"] = -1
                     this_neighbor["address_family"][this_afi]["accepted_prefixes"] = -1
                     this_neighbor["address_family"][this_afi]["sent_prefixes"] = -1
 
                 neighbor_ip = napalm.base.helpers.ip(
@@ -840,15 +848,14 @@
                     )
                     this_reading["temperature"] = this_reading["temperature"] / 10
                     environment_status["temperature"][slot] = this_reading
 
         return environment_status
 
     def get_lldp_neighbors(self):
-
         # init result dict
         lldp = {}
         sh_lldp = self.device.show_lldp_neighbors().splitlines()[5:-3]
 
         for n in sh_lldp:
             local_interface = n.split()[1]
             if local_interface not in lldp.keys():
@@ -860,15 +867,14 @@
                     "port": napalm.base.helpers.convert(str, n.split()[4]),
                 }
             )
 
         return lldp
 
     def get_lldp_neighbors_detail(self, interface=""):
-
         lldp_neighbors = {}
 
         rpc_command = (
             "<Get><Operational>"
             "<LLDP><NodeTable></NodeTable></LLDP>"
             "</Operational></Get>"
         )
@@ -937,27 +943,26 @@
         if type(commands) is not list:
             raise TypeError("Please enter a valid list of commands!")
 
         for command in commands:
             try:
                 cli_output[str(command)] = str(self.device._execute_show(command))
             except TimeoutError:
-                cli_output[
-                    str(command)
-                ] = 'Execution of command \
+                cli_output[str(command)] = (
+                    'Execution of command \
                     "{command}" took too long! Please adjust your params!'.format(
-                    command=command
+                        command=command
+                    )
                 )
                 logger.error(str(cli_output))
                 raise CommandTimeoutException(str(cli_output))
 
         return cli_output
 
     def get_bgp_config(self, group="", neighbor=""):
-
         bgp_config = {}
 
         # a helper
         def build_prefix_limit(af_table, limit, prefix_percent, prefix_timeout):
             prefix_limit = {}
             inet = False
             inet6 = False
@@ -1198,15 +1203,14 @@
             "prefix_limit": {},
             "neighbors": bgp_group_neighbors.get("", {}),
         }
 
         return bgp_config
 
     def get_bgp_neighbors_detail(self, neighbor_address=""):
-
         bgp_neighbors_detail = {}
 
         active_vrfs = ["default"]
 
         active_vrfs_rpc_request = "<Get><Operational><BGP><ConfigInstanceTable><ConfigInstance>\
         <Naming><InstanceName>default</InstanceName></Naming><ConfigInstanceVRFTable/>\
         </ConfigInstance></ConfigInstanceTable></BGP></Operational></Get>"
@@ -1500,15 +1504,14 @@
                     "age": age,
                 }
             )
 
         return arp_table
 
     def get_ntp_peers(self):
-
         ntp_peers = {}
 
         rpc_command = "<Get><Configuration><NTP></NTP></Configuration></Get>"
 
         result_tree = ETREE.fromstring(self.device.make_rpc_call(rpc_command))
 
         for version in ["IPV4", "IPV6"]:
@@ -1525,15 +1528,14 @@
                 if not peer_address:
                     continue
                 ntp_peers[peer_address] = {}
 
         return ntp_peers
 
     def get_ntp_servers(self):
-
         ntp_servers = {}
 
         rpc_command = "<Get><Configuration><NTP></NTP></Configuration></Get>"
 
         result_tree = ETREE.fromstring(self.device.make_rpc_call(rpc_command))
 
         for version in ["IPV4", "IPV6"]:
@@ -1550,15 +1552,14 @@
                 if not server_address:
                     continue
                 ntp_servers[server_address] = {}
 
         return ntp_servers
 
     def get_ntp_stats(self):
-
         ntp_stats = []
 
         rpc_command = (
             "<Get><Operational><NTP><NodeTable></NodeTable></NTP></Operational></Get>"
         )
 
         result_tree = ETREE.fromstring(self.device.make_rpc_call(rpc_command))
@@ -1603,15 +1604,14 @@
                     "jitter": jitter,
                 }
             )
 
         return ntp_stats
 
     def get_interfaces_ip(self):
-
         interfaces_ip = {}
 
         rpc_command_ipv4_ipv6 = "<Get><Operational><IPV4Network></IPV4Network>\
         <IPV6Network></IPV6Network></Operational></Get>"
 
         # only one request
         ipv4_ipv6_tree = ETREE.fromstring(
@@ -1684,15 +1684,14 @@
                     interfaces_ip[interface_name]["ipv6"][address_ip] = {
                         "prefix_length": address_prefix
                     }
 
         return interfaces_ip
 
     def get_mac_address_table(self):
-
         mac_table = []
 
         rpc_command = (
             "<Get><Operational><L2VPNForwarding></L2VPNForwarding></Operational></Get>"
         )
 
         result_tree = ETREE.fromstring(self.device.make_rpc_call(rpc_command))
@@ -1721,15 +1720,14 @@
                     "last_move": 0.0,
                 }
             )
 
         return mac_table
 
     def get_route_to(self, destination="", protocol="", longer=False):
-
         routes = {}
         global IP_RIBRoute
 
         if not isinstance(destination, str):
             raise TypeError("Please specify a valid destination!")
 
         if longer:
@@ -1932,15 +1930,14 @@
                     )
                     routes[destination].append(single_route_details)
                     first_route = False
 
         return routes
 
     def get_snmp_information(self):
-
         snmp_information = {}
 
         snmp_rpc_command = "<Get><Configuration><SNMP></SNMP></Configuration></Get>"
 
         snmp_result_tree = ETREE.fromstring(self.device.make_rpc_call(snmp_rpc_command))
 
         _PRIVILEGE_MODE_MAP_ = {"ReadOnly": "ro", "ReadWrite": "rw"}
@@ -1962,15 +1959,14 @@
                 "mode": _PRIVILEGE_MODE_MAP_.get(privilege, ""),
                 "acl": acl,
             }
 
         return snmp_information
 
     def get_probes_config(self):
-
         sla_config = {}
 
         _PROBE_TYPE_XML_TAG_MAP_ = {
             "ICMPEcho": "icmp-ping",
             "UDPEcho": "udp-ping",
             "ICMPJitter": "icmp-ping-timestamp",
             "UDPJitter": "udp-ping-timestamp",
@@ -2010,15 +2006,14 @@
                 "probe_count": probe_count,
                 "test_interval": test_interval,
             }
 
         return sla_config
 
     def get_probes_results(self):
-
         sla_results = {}
 
         _PROBE_TYPE_XML_TAG_MAP_ = {
             "ICMPEcho": "icmp-ping",
             "UDPEcho": "udp-ping",
             "ICMPJitter": "icmp-ping-timestamp",
             "UDPJitter": "udp-ping-timestamp",
@@ -2194,15 +2189,14 @@
         self,
         destination,
         source=C.TRACEROUTE_SOURCE,
         ttl=C.TRACEROUTE_TTL,
         timeout=C.TRACEROUTE_TIMEOUT,
         vrf=C.TRACEROUTE_VRF,
     ):
-
         traceroute_result = {}
 
         ipv = 4
         try:
             ipv = ipaddress.ip_address(destination).version
         except ValueError:
             logger.error(
@@ -2290,26 +2284,25 @@
             if tag_name == "HopAddress":
                 last_probe_ip_address = tag_value
                 continue
             if tag_name == "HopHostName":
                 last_probe_host_name = tag_value
                 continue
             if tag_name == "DeltaTime":
-                last_hop_dict["probes"][last_probe_index][
-                    "rtt"
-                ] = napalm.base.helpers.convert(float, tag_value, 0.0)
+                last_hop_dict["probes"][last_probe_index]["rtt"] = (
+                    napalm.base.helpers.convert(float, tag_value, 0.0)
+                )
                 continue
 
         if last_hop_index:
             traceroute_result["success"][last_hop_index] = last_hop_dict
 
         return traceroute_result
 
     def get_users(self):
-
         users = {}
 
         _CISCO_GROUP_TO_CISCO_PRIVILEGE_MAP = {
             "root-system": 15,
             "operator": 5,
             "sysadmin": 1,
             "serviceadmin": 1,
@@ -2331,16 +2324,15 @@
             password = napalm.base.helpers.find_txt(user_entry, "Password/Password")
             user_details = _DEFAULT_USER_DETAILS.copy()
             user_details.update({"level": level, "password": str(password)})
             users[username] = user_details
 
         return users
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
-
+    def get_config(self, retrieve="all", full=False, sanitized=False, format="text"):
         config = {"startup": "", "running": "", "candidate": ""}  # default values
 
         # IOS-XR only supports "all" on "show run"
         run_full = " all" if full else ""
 
         filter_strings = [r"^Building configuration.*$", r"^!! IOS XR Configuration.*$"]
         filter_pattern = napalm.base.helpers.generate_regex_or(filter_strings)
```

### Comparing `napalm-4.1.0/napalm/iosxr/templates/delete_probes.j2` & `napalm-5.0.0/napalm/iosxr/templates/delete_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr/templates/set_probes.j2` & `napalm-5.0.0/napalm/iosxr/templates/set_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr/templates/snmp_config.j2` & `napalm-5.0.0/napalm/iosxr/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr_netconf/__init__.py` & `napalm-5.0.0/napalm/iosxr_netconf/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr_netconf/constants.py` & `napalm-5.0.0/napalm/iosxr_netconf/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/iosxr_netconf/iosxr_netconf.py` & `napalm-5.0.0/napalm/iosxr_netconf/iosxr_netconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,23 +447,22 @@
         interfaces_rpc_reply = self.device.get(
             filter=("subtree", C.INT_RPC_REQ_FILTER)
         ).xml
         # Converts string to etree
         interfaces_rpc_reply_etree = ETREE.fromstring(interfaces_rpc_reply)
 
         # Retrieves interfaces details
-        for (interface_tree, description_tree) in zip(
+        for interface_tree, description_tree in zip(
             interfaces_rpc_reply_etree.xpath(
                 ".//int:interfaces/int:interface-xr/int:interface", namespaces=C.NS
             ),
             interfaces_rpc_reply_etree.xpath(
                 ".//int:interfaces/int:interfaces/int:interface", namespaces=C.NS
             ),
         ):
-
             interface_name = self._find_txt(
                 interface_tree, "./int:interface-name", default="", namespaces=C.NS
             )
             if not interface_name:
                 continue
             is_up = (
                 self._find_txt(
@@ -676,15 +675,14 @@
         """Return BGP neighbors details."""
 
         def get_vrf_neighbors(rpc_reply_etree, xpath):
             """Return BGP neighbors details for a given VRF."""
             neighbors = {}
 
             for neighbor in rpc_reply_etree.xpath(xpath, namespaces=C.NS):
-
                 this_neighbor = {}
                 this_neighbor["local_as"] = napalm.base.helpers.convert(
                     int,
                     self._find_txt(
                         neighbor, "./bgp:local-as", default="", namespaces=C.NS
                     ),
                 )
@@ -799,38 +797,38 @@
                             neighbor,
                             "./bgp:af-data/bgp:prefixes-denied",
                             default="",
                             namespaces=C.NS,
                         ),
                         0,
                     )
-                    this_neighbor["address_family"][this_afi][
-                        "accepted_prefixes"
-                    ] = napalm.base.helpers.convert(
-                        int,
-                        self._find_txt(
-                            neighbor,
-                            "./bgp:af-data/bgp:prefixes-accepted",
-                            default="",
-                            namespaces=C.NS,
-                        ),
-                        0,
+                    this_neighbor["address_family"][this_afi]["accepted_prefixes"] = (
+                        napalm.base.helpers.convert(
+                            int,
+                            self._find_txt(
+                                neighbor,
+                                "./bgp:af-data/bgp:prefixes-accepted",
+                                default="",
+                                namespaces=C.NS,
+                            ),
+                            0,
+                        )
                     )
-                    this_neighbor["address_family"][this_afi][
-                        "sent_prefixes"
-                    ] = napalm.base.helpers.convert(
-                        int,
-                        self._find_txt(
-                            neighbor,
-                            "./bgp:af-data/\
+                    this_neighbor["address_family"][this_afi]["sent_prefixes"] = (
+                        napalm.base.helpers.convert(
+                            int,
+                            self._find_txt(
+                                neighbor,
+                                "./bgp:af-data/\
                             bgp:prefixes-advertised",
-                            default="",
-                            namespaces=C.NS,
-                        ),
-                        0,
+                                default="",
+                                namespaces=C.NS,
+                            ),
+                            0,
+                        )
                     )
                 except AttributeError:
                     this_neighbor["address_family"][this_afi]["received_prefixes"] = -1
                     this_neighbor["address_family"][this_afi]["accepted_prefixes"] = -1
                     this_neighbor["address_family"][this_afi]["sent_prefixes"] = -1
 
                 neighbor_ip = napalm.base.helpers.ip(
@@ -3109,15 +3107,15 @@
             )
             user_details = _DEFAULT_USER_DETAILS.copy()
             user_details.update({"level": level, "password": password})
             users[username] = user_details
 
         return users
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
+    def get_config(self, retrieve="all", full=False, sanitized=False, format="text"):
         """Return device configuration."""
 
         encoding = self.config_encoding
         # 'full' argument not supported; 'with-default' capability not supported.
         if full:
             raise NotImplementedError(
                 "'full' argument has not been implemented on the IOS-XR NETCONF driver"
```

### Comparing `napalm-4.1.0/napalm/junos/__init__.py` & `napalm-5.0.0/napalm/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/constants.py` & `napalm-5.0.0/napalm/junos/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/junos.py` & `napalm-5.0.0/napalm/junos/junos.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
         self.port = optional_args.get("port", 22)
         self.key_file = optional_args.get("key_file", None)
         self.keepalive = optional_args.get("keepalive", 30)
         self.ssh_config_file = optional_args.get("ssh_config_file", None)
         self.ignore_warning = optional_args.get("ignore_warning", False)
         self.auto_probe = optional_args.get("auto_probe", 0)
+        self.huge_tree = optional_args.get("huge_tree", False)
 
         # Define locking method
         self.lock_disable = optional_args.get("lock_disable", False)
         self.session_config_lock = optional_args.get("config_lock", False)
         self.config_private = optional_args.get("config_private", False)
 
         # Junos driver specific options
@@ -117,22 +118,24 @@
             self.device = Device(
                 hostname,
                 user=username,
                 password=password,
                 ssh_private_key_file=self.key_file,
                 ssh_config=self.ssh_config_file,
                 port=self.port,
+                huge_tree=self.huge_tree,
             )
         else:
             self.device = Device(
                 hostname,
                 user=username,
                 password=password,
                 port=self.port,
                 ssh_config=self.ssh_config_file,
+                huge_tree=self.huge_tree,
             )
 
         self.platform = "junos"
         self.profile = [self.platform]
 
     def open(self):
         """Open the connection with the device."""
@@ -1132,15 +1135,15 @@
                 if not command_safe_parts
                 else "{base} | {pipes}".format(
                     base=exploded_cmd[0], pipes=" | ".join(command_safe_parts)
                 )
             )
             raw_txt = self.device.cli(safe_command, warning=False, format=encoding)
             if isinstance(raw_txt, etree._Element):
-                raw_txt = etree.tostring(raw_txt.get_parent()).decode()
+                raw_txt = etree.tostring(raw_txt.getparent()).decode()
                 cli_output[str(command)] = raw_txt
             else:
                 cli_output[str(command)] = str(_process_pipe(command, raw_txt))
         return cli_output
 
     def get_bgp_config(self, group="", neighbor=""):
         """Return BGP configuration."""
@@ -1242,14 +1245,16 @@
             "apply_groups": list,
             "remove_private_as": bool,
             "multipath": bool,
             "multihop_ttl": int,
         }
         _GROUP_FIELDS_DATATYPE_MAP_.update(_COMMON_FIELDS_DATATYPE_)
 
+        _UNWANTED_GROUP_FIELDS = ["multihop", "cluster"]
+
         _DATATYPE_DEFAULT_ = {str: "", int: 0, bool: False, list: []}
 
         bgp_config = {}
 
         routing_options = junos_views.junos_routing_config_table(self.device)
         routing_options.get(options=self.junos_config_options)
 
@@ -1298,26 +1303,31 @@
         policy.get(options=self.junos_config_options)
         nhs_policies = dict()
         for policy_name, is_nhs_list in policy.items():
             # is_nhs_list is a list with one element. Ex: [('is_nhs', True)]
             is_nhs, boolean = is_nhs_list[0]
             nhs_policies[policy_name] = boolean if boolean is not None else False
 
+        unwanted_group_fields = dict()
+
         for bgp_group in bgp_items:
             bgp_group_name = bgp_group[0]
             bgp_group_details = bgp_group[1]
             bgp_config[bgp_group_name] = {
                 field: _DATATYPE_DEFAULT_.get(datatype)
                 for field, datatype in _GROUP_FIELDS_DATATYPE_MAP_.items()
                 if "_prefix_limit" not in field
             }
 
             # Always overwrite with the system local_as (this will either be
             # valid or will be zero i.e. the same as the default value).
             bgp_config[bgp_group_name]["local_as"] = system_bgp_asn
+            unwanted_group_fields[bgp_group_name] = dict(
+                {key: False for key in _UNWANTED_GROUP_FIELDS}
+            )
 
             for key, value in bgp_group_details:
                 if "_prefix_limit" in key or value is None:
                     continue
                 datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(key)
                 default = _DATATYPE_DEFAULT_.get(datatype)
 
@@ -1331,17 +1341,22 @@
                 if key == "apply_groups":
                     # Ensure apply_groups value is wrapped in a list
                     if isinstance(value, str):
                         value = [value]
                 if key == "neighbors":
                     bgp_group_peers = value
                     continue
-                bgp_config[bgp_group_name].update(
-                    {key: napalm.base.helpers.convert(datatype, value, default)}
-                )
+
+                if key in _UNWANTED_GROUP_FIELDS:
+                    unwanted_group_fields[bgp_group_name][key] = True
+                    continue
+                if datatype:
+                    bgp_config[bgp_group_name].update(
+                        {key: napalm.base.helpers.convert(datatype, value, default)}
+                    )
             prefix_limit_fields = {}
             for key, value in bgp_group_details:
                 if "_prefix_limit" in key and value is not None:
                     datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(key)
                     default = _DATATYPE_DEFAULT_.get(datatype)
                     prefix_limit_fields.update(
                         {
@@ -1349,17 +1364,15 @@
                                 "_prefix_limit", ""
                             ): napalm.base.helpers.convert(datatype, value, default)
                         }
                     )
             bgp_config[bgp_group_name]["prefix_limit"] = build_prefix_limit(
                 **prefix_limit_fields
             )
-            if "multihop" in bgp_config[bgp_group_name].keys():
-                # Delete 'multihop' key from the output
-                del bgp_config[bgp_group_name]["multihop"]
+            if unwanted_group_fields[bgp_group_name]["multihop"]:
                 if bgp_config[bgp_group_name]["multihop_ttl"] == 0:
                     # Set ttl to default value 64
                     bgp_config[bgp_group_name]["multihop_ttl"] = 64
 
             bgp_config[bgp_group_name]["neighbors"] = {}
             bgp_group_remote_as = bgp_config[bgp_group_name]["remote_as"]
             for bgp_group_neighbor in bgp_group_peers.items():
@@ -1406,15 +1419,15 @@
                         bgp_peer_details["remote_as"]
                     )
                     if key == "cluster":
                         bgp_peer_details["route_reflector_client"] = True
                         # we do not want cluster in the output
                         del bgp_peer_details["cluster"]
 
-                if "cluster" in bgp_config[bgp_group_name].keys():
+                if unwanted_group_fields[bgp_group_name]["cluster"]:
                     bgp_peer_details["route_reflector_client"] = True
                 prefix_limit_fields = {}
                 for key, value in bgp_group_details:
                     if "_prefix_limit" in key and value is not None:
                         datatype = _PEER_FIELDS_DATATYPE_MAP_.get(key)
                         default = _DATATYPE_DEFAULT_.get(datatype)
                         prefix_limit_fields.update(
@@ -1429,18 +1442,14 @@
                 )
                 bgp_config[bgp_group_name]["neighbors"][
                     bgp_peer_address
                 ] = bgp_peer_details
                 if neighbor and bgp_peer_address == neighbor_ip:
                     break  # found the desired neighbor
 
-            if "cluster" in bgp_config[bgp_group_name].keys():
-                # we do not want cluster in the output
-                del bgp_config[bgp_group_name]["cluster"]
-
         return bgp_config
 
     def get_bgp_neighbors_detail(self, neighbor_address=""):
         """Detailed view of the BGP neighbors operational data."""
         bgp_neighbors = {}
         default_neighbor_details = {
             "up": False,
@@ -1479,15 +1488,15 @@
             "advertised_prefix_count": -1,
             "flap_count": 0,
         }
         OPTION_KEY_MAP = {
             "RemovePrivateAS": "remove_private_as",
             "Multipath": "multipath",
             "Multihop": "multihop",
-            "AddressFamily": "local_address_configured"
+            "AddressFamily": "local_address_configured",
             # 'AuthKey'        : 'authentication_key_set'
             # but other vendors do not specify if auth key is set
             # other options:
             # Preference, HoldTime, Ttl, LogUpDown, Refresh
         }
 
         def _bgp_iter_core(neighbor_data, instance=None):
@@ -1634,15 +1643,19 @@
 
         ipv6_neighbors_table_raw = junos_views.junos_ipv6_neighbors_table(self.device)
         ipv6_neighbors_table_raw.get()
         ipv6_neighbors_table_items = ipv6_neighbors_table_raw.items()
 
         for ipv6_table_entry in ipv6_neighbors_table_items:
             ipv6_entry = {elem[0]: elem[1] for elem in ipv6_table_entry[1]}
-            ipv6_entry["mac"] = napalm.base.helpers.mac(ipv6_entry.get("mac"))
+            ipv6_entry["mac"] = (
+                ""
+                if ipv6_entry.get("mac") == "none"
+                else napalm.base.helpers.mac(ipv6_entry.get("mac"))
+            )
             ipv6_entry["ip"] = napalm.base.helpers.ip(ipv6_entry.get("ip"))
             ipv6_neighbors_table.append(ipv6_entry)
 
         return ipv6_neighbors_table
 
     def get_ntp_peers(self):
         """Return the NTP peers configured on the device."""
@@ -1719,15 +1732,15 @@
 
         interface_table = junos_views.junos_ip_interfaces_table(self.device)
         interface_table.get()
         interface_table_items = interface_table.items()
 
         _FAMILY_VMAP_ = {
             "inet": "ipv4",
-            "inet6": "ipv6"
+            "inet6": "ipv6",
             # can add more mappings
         }
         _FAMILY_MAX_PREFIXLEN = {"inet": 32, "inet6": 128}
 
         for interface_details in interface_table_items:
             ip_network = interface_details[0]
             ip_address = ip_network.split("/")[0]
@@ -2124,15 +2137,14 @@
         ttl=C.PING_TTL,
         timeout=C.PING_TIMEOUT,
         size=C.PING_SIZE,
         count=C.PING_COUNT,
         vrf=C.PING_VRF,
         source_interface=C.PING_SOURCE_INTERFACE,
     ):
-
         ping_dict = {}
 
         source_str = ""
         maxttl_str = ""
         timeout_str = ""
         size_str = ""
         count_str = ""
@@ -2432,18 +2444,19 @@
             }
             optics_detail[interface_name]["physical_channels"]["channel"].append(
                 intf_optics
             )
 
         return optics_detail
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
+    def get_config(self, retrieve="all", full=False, sanitized=False, format="text"):
         rv = {"startup": "", "running": "", "candidate": ""}
 
-        options = {"format": "text", "database": "candidate"}
+        self.format = format
+        options = {"format": self.format, "database": "candidate"}
         sanitize_strings = {
             r"^(\s+community\s+)\w+(;.*|\s+{.*)$": r"\1<removed>\2",
             r'^(.*)"\$\d\$\S+"(;.*)$': r"\1<removed>\2",
         }
         if retrieve in ("candidate", "all"):
             config = self.device.rpc.get_config(filter_xml=None, options=options)
             rv["candidate"] = str(config.text)
@@ -2454,15 +2467,14 @@
 
         if sanitized:
             return napalm.base.helpers.sanitize_configs(rv, sanitize_strings)
 
         return rv
 
     def get_network_instances(self, name=""):
-
         network_instances = {}
 
         ri_table = junos_views.junos_nw_instances_table(self.device)
         ri_table.get(options=self.junos_config_options)
         ri_entries = ri_table.items()
 
         vrf_interfaces = []
```

### Comparing `napalm-4.1.0/napalm/junos/templates/delete_snmp_config.j2` & `napalm-5.0.0/napalm/junos/templates/delete_snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/templates/delete_users.j2` & `napalm-5.0.0/napalm/junos/templates/delete_users.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/templates/set_probes.j2` & `napalm-5.0.0/napalm/junos/templates/set_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/templates/set_users.j2` & `napalm-5.0.0/napalm/junos/templates/set_users.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/templates/snmp_config.j2` & `napalm-5.0.0/napalm/junos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/junos/utils/junos_views.py` & `napalm-5.0.0/napalm/junos/utils/junos_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Load tables/views
 """
+
 import yaml
 import re
 from jnpr.junos.factory import FactoryLoader
 from os.path import splitext
 
 
 def _preprocess_yml(path):
```

### Comparing `napalm-4.1.0/napalm/junos/utils/junos_views.yml` & `napalm-5.0.0/napalm/junos/utils/junos_views.yml`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxapi_plumbing/__init__.py` & `napalm-5.0.0/napalm/nxapi_plumbing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Fork of pynxos library from network to code and mzbenami
 
 Re-implemented by ktbyers to support XML-RPC in addition to JSON-RPC
 """
+
 from napalm.nxapi_plumbing.device import Device
 from napalm.nxapi_plumbing.api_client import RPCClient, XMLClient
 from napalm.nxapi_plumbing.errors import (
     NXAPIError,
     NXAPICommandError,
     NXAPIConnectionError,
     NXAPIAuthError,
```

### Comparing `napalm-4.1.0/napalm/nxapi_plumbing/api_client.py` & `napalm-5.0.0/napalm/nxapi_plumbing/api_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Fork of pynxos library from network to code and mzbenami
 
 Reimplemented by ktbyers to support XML-RPC in addition to JSON-RPC
 """
+
 from __future__ import print_function, unicode_literals
 
 from builtins import super
 from typing import Optional, List, Dict, Any
 
 import requests
 from requests import Response
@@ -181,15 +182,14 @@
 
         # Add the 'command' that was executed to the response dictionary
         for i, response_dict in enumerate(response_list):
             response_dict["command"] = commands[i]
 
         new_response = []
         for response in response_list:
-
             # Detect errors
             self._error_check(response)
 
             # Some commands like "show run" can have a None result
             cmd_response = response.get("result")
             if cmd_response is None:
                 cmd_response = {}
```

### Comparing `napalm-4.1.0/napalm/nxapi_plumbing/device.py` & `napalm-5.0.0/napalm/nxapi_plumbing/device.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxapi_plumbing/errors.py` & `napalm-5.0.0/napalm/nxapi_plumbing/errors.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxos/__init__.py` & `napalm-5.0.0/napalm/nxos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxos/nxos.py` & `napalm-5.0.0/napalm/nxos/nxos.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,28 +116,26 @@
             optional_args = {}
         self.hostname = hostname
         self.username = username
         self.password = password
         self.timeout = timeout
         self.replace = True
         self.loaded = False
-        self.changed = False
         self.merge_candidate = ""
         self.candidate_cfg = "candidate_config.txt"
         self.rollback_cfg = "rollback_config.txt"
         self._dest_file_system = optional_args.pop("dest_file_system", "bootflash:")
         self.force_no_enable = optional_args.get("force_no_enable", False)
         self.netmiko_optional_args = netmiko_args(optional_args)
         self.device: Optional[NXOSDevice] = None
 
     @ensure_netmiko_conn
     def load_replace_candidate(
         self, filename: Optional[str] = None, config: Optional[str] = None
     ) -> None:
-
         if not filename and not config:
             raise ReplaceConfigException(
                 "filename or config parameter must be provided."
             )
 
         if not filename:
             assert isinstance(config, str)
@@ -154,19 +152,19 @@
                 dest_file=self.candidate_cfg,
                 file_system=self._dest_file_system,
                 direction="put",
                 overwrite_file=True,
             )
             if not transfer_result["file_exists"]:
                 raise ValueError()
-        except Exception:
+        except Exception as e:
             msg = (
                 "Could not transfer file. There was an error "
                 "during transfer. Please make sure remote "
-                "permissions are set."
+                f"permissions are set. Caught Error:\n{repr(str(e))}"
             )
             raise ReplaceConfigException(msg)
 
         self.replace = True
         self.loaded = True
         if config and os.path.isfile(tmp_file):
             os.remove(tmp_file)
@@ -188,27 +186,48 @@
         self.loaded = True
 
     def _send_command(
         self, command: str, raw_text: bool = False
     ) -> Dict[str, Union[str, Dict[str, Any]]]:
         raise NotImplementedError
 
+    def _check_file_exists(self, cfg_file: str) -> bool:
+        """
+        Check that the file exists on remote device using full path.
+
+        cfg_file can be a full path, e.g.: bootflash:rollback_config.txt
+        or just a filename, e.g.: rollback_config.txt
+
+        For example
+        # dir rollback_config.txt
+            71803    Sep 06 14:13:33 2023  rollback_config.txt
+
+        Usage for bootflash://sup-local
+        6211682304 bytes used
+        110314684416 bytes free
+        116526366720 bytes total
+        """
+        cmd = f"dir {cfg_file}"
+        output = self._send_command(command=cmd, raw_text=True)
+        if "No such file or directory" in output:
+            return False
+        else:
+            return True
+
     def _commit_merge(self) -> None:
         try:
             output = self._send_config(self.merge_candidate)
             if output and "Invalid command" in output:
                 raise MergeConfigException("Error while applying config!")
         except Exception as e:
-            self.changed = True
             self.rollback()
             err_header = "Configuration merge failed; automatic rollback attempted"
             merge_error = "{0}:\n{1}".format(err_header, repr(str(e)))
             raise MergeConfigException(merge_error)
 
-        self.changed = True
         # clear the merge buffer
         self.merge_candidate = ""
 
     def _get_merge_diff(self) -> str:
         """
         Uses netutils diff_network_config to create a partial configuration
         with the proper hierarchy.
@@ -440,15 +459,14 @@
         self,
         destination: str,
         source: str = c.TRACEROUTE_SOURCE,
         ttl: int = c.TRACEROUTE_TTL,
         timeout: int = c.TRACEROUTE_TIMEOUT,
         vrf: str = c.TRACEROUTE_VRF,
     ) -> models.TracerouteResultDict:
-
         _HOP_ENTRY_PROBE = [
             r"\s+",
             r"(",  # beginning of host_name (ip_address) RTT group
             r"(",  # beginning of host_name (ip_address) group only
             r"([a-zA-Z0-9\.:-]*)",  # hostname
             r"\s+",
             r"\(?([a-fA-F0-9\.:][^\)]*)\)?",  # IP Address between brackets
@@ -581,17 +599,20 @@
             fobj.write(config)
         return filename
 
     def _disable_confirmation(self) -> None:
         self._send_command_list(["terminal dont-ask"])
 
     def get_config(
-        self, retrieve: str = "all", full: bool = False, sanitized: bool = False
+        self,
+        retrieve: str = "all",
+        full: bool = False,
+        sanitized: bool = False,
+        format: str = "text",
     ) -> models.ConfigDict:
-
         # NX-OS adds some extra, unneeded lines that should be filtered.
         filter_strings = [
             r"!Command: show .*$",
             r"!Time:.*\d{4}\s*$",
             r"Startup config saved at:.*$",
         ]
         filter_pattern = generate_regex_or(filter_strings)
@@ -668,23 +689,23 @@
             # Convert any 'not advertised' to an empty string
             for field in lldp_entry:
                 if "not advertised" in lldp_entry[field]:
                     lldp_entry[field] = ""
             # Add field missing on IOS
             lldp_entry["parent_interface"] = ""
             # Translate the capability fields
-            lldp_entry[
-                "remote_system_capab"
-            ] = napalm.base.helpers.transform_lldp_capab(
-                lldp_entry["remote_system_capab"]
+            lldp_entry["remote_system_capab"] = (
+                napalm.base.helpers.transform_lldp_capab(
+                    lldp_entry["remote_system_capab"]
+                )
             )
-            lldp_entry[
-                "remote_system_enable_capab"
-            ] = napalm.base.helpers.transform_lldp_capab(
-                lldp_entry["remote_system_enable_capab"]
+            lldp_entry["remote_system_enable_capab"] = (
+                napalm.base.helpers.transform_lldp_capab(
+                    lldp_entry["remote_system_enable_capab"]
+                )
             )
             # Turn the interfaces into their long version
             local_intf = canonical_interface_name(local_intf)
             lldp.setdefault(local_intf, [])
             lldp[local_intf].append(lldp_entry)  # type: ignore
 
         return lldp
@@ -896,16 +917,14 @@
             "no terminal dont-ask",
         ]
         try:
             rollback_result = self._send_command_list(commands)
         except ConnectionError:
             # requests will raise an error with verbose warning output (don't fail on this).
             return
-        finally:
-            self.changed = True
 
         # For nx-api a list is returned so extract the result associated with the
         # 'rollback' command.
         rollback_result = rollback_result[1]
         assert isinstance(rollback_result, dict)
         msg = (
             rollback_result.get("msg")
@@ -917,18 +936,19 @@
         if "Rollback failed." in msg or error_msg:
             raise ReplaceConfigException(msg)
         elif rollback_result == []:
             raise ReplaceConfigException
 
     def rollback(self) -> None:
         assert isinstance(self.device, NXOSDevice)
-        if self.changed:
-            self.device.rollback(self.rollback_cfg)
-            self._copy_run_start()
-            self.changed = False
+        if not self._check_file_exists(cfg_file=self.rollback_cfg):
+            msg = f"Rollback file '{self.rollback_cfg}' does not exist on device."
+            raise ReplaceConfigException(msg)
+        self.device.rollback(self.rollback_cfg)
+        self._copy_run_start()
 
     def get_facts(self) -> models.FactsDict:
         facts: models.FactsDict = {}  # type: ignore
         facts["vendor"] = "Cisco"
 
         show_inventory_table = self._get_command_table(
             "show inventory", "TABLE_inv", "ROW_inv"
@@ -1045,14 +1065,15 @@
         bgp_state_dict = {
             "Idle": {"is_up": False, "is_enabled": True},
             "Active": {"is_up": False, "is_enabled": True},
             "Open": {"is_up": False, "is_enabled": True},
             "Established": {"is_up": True, "is_enabled": True},
             "Closing": {"is_up": True, "is_enabled": True},
             "Shutdown": {"is_up": False, "is_enabled": False},
+            "Admin (Shut)": {"is_up": False, "is_enabled": False},
         }
         """
         af_name_dict = {
             'af-id': {'safi': "af-name"},
             'af-id': {'safi': "af-name"},
             'af-id': {'safi': "af-name"}
         }
@@ -1561,17 +1582,27 @@
             # some nexus devices have keys postfixed with the shorthand device series name (ie n3k)
             # ex. on a 9k the key is ROW_psinfo, but on a 3k it is ROW_psinfo_n3k
             ps_info_row_key = [
                 i for i in ps_info_table.keys() if i.startswith("ROW_psinfo")
             ][0]
             for psinfo in ps_info_table[ps_info_row_key]:
                 normalized[psinfo["psnum"]]["status"] = (
-                    psinfo.get("ps_status", "ok") == "ok"
+                    psinfo.get("ps_status", "ok").lower() == "ok"
                 )
-                normalized[psinfo["psnum"]]["output"] = float(psinfo.get("watts", -1.0))
+                # typically the power output is key'd by watts
+                # other times it is keyed by "actual_out"
+                if "watts" in psinfo:
+                    normalized[psinfo["psnum"]]["output"] = float(
+                        psinfo.get("watts", -1.0)
+                    )
+                else:
+                    # When the power output is keyed by actual_out, it appears like "99 W"
+                    normalized[psinfo["psnum"]]["output"] = float(
+                        psinfo.get("actual_out", -1.0).split()[0]
+                    )
                 # Newer nxos versions provide the total capacity in the `tot_capa` key
                 if "tot_capa" in psinfo:
                     normalized[psinfo["psnum"]]["capacity"] = float(
                         psinfo["tot_capa"].split()[0]
                     )
                 # The capacity of the power supply can be determined by the model
                 # ie N2200-PAC-400W = 400 watts
```

### Comparing `napalm-4.1.0/napalm/nxos/templates/snmp_config.j2` & `napalm-5.0.0/napalm/nxos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl` & `napalm-5.0.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxos_ssh/__init__.py` & `napalm-5.0.0/napalm/nxos_ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/nxos_ssh/nxos_ssh.py` & `napalm-5.0.0/napalm/nxos_ssh/nxos_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 WEEK_SECONDS = 7 * DAY_SECONDS
 YEAR_SECONDS = 365 * DAY_SECONDS
 
 # STD REGEX PATTERNS
 IP_ADDR_REGEX = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
 IPV4_ADDR_REGEX = IP_ADDR_REGEX
 IPV6_ADDR_REGEX_1 = r"::"
-IPV6_ADDR_REGEX_2 = r"[0-9a-fA-F:]{1,39}::[0-9a-fA-F:]{1,39}"
+IPV6_ADDR_REGEX_2 = r"[0-9a-fA-F:]{0,39}::[0-9a-fA-F:]{0,39}"
 IPV6_ADDR_REGEX_3 = (
     r"[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}:"
     r"[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}:[0-9a-fA-F]{1,3}"
 )
 # Should validate IPv6 address using an IP address library after matching with this regex
 IPV6_ADDR_REGEX = r"(?:{}|{}|{})".format(
     IPV6_ADDR_REGEX_1, IPV6_ADDR_REGEX_2, IPV6_ADDR_REGEX_3
@@ -260,21 +260,30 @@
 def bgp_normalize_table_data(bgp_table):
     """The 'show bgp all summary vrf all' table can have entries that wrap multiple lines.
 
     2001:db8:4:701::2
                 4 65535  163664  163693      145    0    0     3w2d 3
     2001:db8:e0:dd::1
                 4    10  327491  327278      145    0    0     3w1d 4
+    2001:db8:e0:df::
+                4    12345678
+                         327465  327268      145    0    0     3w1d 4
 
     Normalize this so the line wrap doesn't exit.
     """
     bgp_table = bgp_table.strip()
-    bgp_multiline_pattern = r"({})\s*\n".format(IPV4_OR_IPV6_REGEX)
-    # Strip out the newline
-    return re.sub(bgp_multiline_pattern, r"\1", bgp_table)
+    # Remove newline after ipv6 address
+    bgp_ipv6_multiline_pattern = r"({})\s*\n".format(IPV4_OR_IPV6_REGEX)
+    bgp_table = re.sub(bgp_ipv6_multiline_pattern, r"\1", bgp_table)
+    # Remove newline after a long AS number
+    bgp_long_as_multiline_pattern = r"((?:{})\s*\d*\s*\d*)\s*\n".format(
+        IPV4_OR_IPV6_REGEX
+    )
+    bgp_table = re.sub(bgp_long_as_multiline_pattern, r"\1", bgp_table)
+    return bgp_table
 
 
 def bgp_table_parser(bgp_table):
     """Generator that parses a line of bgp summary table and returns a dict compatible with NAPALM
 
     Example line:
     10.2.1.14       4    10  472516  472238      361    0    0     3w1d 9
@@ -529,40 +538,39 @@
     def _load_cfg_from_checkpoint(self):
         commands = [
             "terminal dont-ask",
             "rollback running-config file {}".format(self.candidate_cfg),
             "no terminal dont-ask",
         ]
 
-        try:
-            rollback_result = self._send_command_list(
-                commands, expect_string=r"[#>]", read_timeout=90
-            )
-        finally:
-            self.changed = True
+        rollback_result = self._send_command_list(
+            commands, expect_string=r"[#>]", read_timeout=90
+        )
         msg = rollback_result
         if "Rollback failed." in msg:
             raise ReplaceConfigException(msg)
 
     def rollback(self):
-        if self.changed:
-            commands = [
-                "terminal dont-ask",
-                "rollback running-config file {}".format(self.rollback_cfg),
-                "no terminal dont-ask",
-            ]
-            result = self._send_command_list(
-                commands, expect_string=r"[#>]", read_timeout=90
-            )
-            if "completed" not in result.lower():
-                raise ReplaceConfigException(result)
-            # If hostname changes ensure Netmiko state is updated properly
-            self._netmiko_device.set_base_prompt()
-            self._copy_run_start()
-            self.changed = False
+        if not self._check_file_exists(self.rollback_cfg):
+            msg = f"Rollback file '{self.rollback_cfg}' does not exist on device."
+            raise ReplaceConfigException(msg)
+
+        commands = [
+            "terminal dont-ask",
+            "rollback running-config file {}".format(self.rollback_cfg),
+            "no terminal dont-ask",
+        ]
+        result = self._send_command_list(
+            commands, expect_string=r"[#>]", read_timeout=90
+        )
+        if "completed" not in result.lower():
+            raise ReplaceConfigException(result)
+        # If hostname changes ensure Netmiko state is updated properly
+        self._netmiko_device.set_base_prompt()
+        self._copy_run_start()
 
     def _apply_key_map(self, key_map, table):
         new_dict = {}
         for key, value in table.items():
             new_key = key_map.get(key)
             if new_key:
                 new_dict[new_key] = str(value)
@@ -1472,17 +1480,17 @@
                                 "last_active": nh_used,
                                 "next_hop": nh_ip,
                                 "selected_next_hop": nh_used,
                                 "inactive_reason": "",
                                 "preference": int(nh_metric),
                             }
                             if nh_source == "bgp":
-                                route_entry[
-                                    "protocol_attributes"
-                                ] = self._get_bgp_route_attr(cur_prefix, curvrf, nh_ip)
+                                route_entry["protocol_attributes"] = (
+                                    self._get_bgp_route_attr(cur_prefix, curvrf, nh_ip)
+                                )
                             else:
                                 route_entry["protocol_attributes"] = {}
                             nh_list.append(route_entry)
                 # process last next hop entries
                 if preffound:
                     if cur_prefix not in routes:
                         routes[cur_prefix] = []
```

### Comparing `napalm-4.1.0/napalm/nxos_ssh/templates/snmp_config.j2` & `napalm-5.0.0/napalm/nxos_ssh/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/pyIOSXR/__init__.py` & `napalm-5.0.0/napalm/pyIOSXR/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/napalm/pyIOSXR/exceptions.py` & `napalm-5.0.0/napalm/pyIOSXR/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 Contributors fooelisa, mirceaulinic, et all
 """
 
 
 class IOSXRException(Exception):
     def __init__(self, msg=None, dev=None):
-
         super(IOSXRException, self).__init__(msg)
         if dev:
             self._xr = dev
             # release the XML agent
             if self._xr._xml_agent_locker.locked():
                 self._xr._xml_agent_locker.release()
 
@@ -40,15 +39,14 @@
         super(ConnectError, self).__init__(msg=msg, dev=dev)
         if dev:
             self._xr = dev
             self._xr._xml_agent_alive = False
 
 
 class CommitError(IOSXRException):
-
     """Raised when unable to commit. Mostly due to ERROR 0x41866c00"""
 
     pass
 
 
 class LockError(IOSXRException):
     """Throw this exception when unable to lock the config DB."""
```

### Comparing `napalm-4.1.0/napalm/pyIOSXR/iosxr.py` & `napalm-5.0.0/napalm/pyIOSXR/iosxr.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         keyword params for show command:
           config=True/False :   set True to run show command in config mode
           eg: .show_configuration_merge(config=True)
 
         """
 
         def _getattr(*args, **kwargs):
-
             cmd = item.replace("_", " ")
             for arg in args:
                 cmd += " %s" % arg
 
             if kwargs.get("config"):
                 response = self._execute_config_show(cmd)
             else:
@@ -240,24 +239,22 @@
             command,
             read_timeout=self._XML_MODE_READ_TIMEOUT,
             strip_prompt=False,
             strip_command=False,
         )
 
     def _in_cli_mode(self):
-
         out = self._send_command_timing("\n")
         if not out:
             return False
         if self._cli_prompt in out:
             return True
         return False
 
     def _enter_xml_mode(self):
-
         self._unlock_xml_agent()
         # release - other commands should not have anyway access to the XML agent
         # when not in XML mode
         self._lock_xml_agent()  # make sure it won't collide with other parallel requests
 
         out = self._send_command_timing(self._XML_SHELL)  # send xml shell command
 
@@ -279,15 +276,14 @@
         delay_factor=None,  # noqa
         read_timeout=None,
         start=None,
         expect_string=None,
         read_output=None,
         receive=False,
     ):
-
         if not expect_string:
             expect_string = self._XML_MODE_PROMPT
 
         if read_output is None:
             read_output = ""
 
         if not read_timeout:
@@ -401,15 +397,14 @@
             raise XMLCLIError(output.strip(), self)
 
         self._unlock_xml_agent()
         return str(output.replace("XML>", "").strip())
 
     # previous module function __execute_rpc__
     def _execute_rpc(self, command_xml, delay_factor=0.1):
-
         xml_rpc_command = (
             '<?xml version="1.0" encoding="UTF-8"?><Request MajorVersion="1" MinorVersion="0">'
             + command_xml
             + "</Request>"
         )
 
         response = self._send_command(xml_rpc_command, delay_factor=delay_factor)
@@ -429,15 +424,14 @@
             raise IteratorIDError(self._ITERATOR_ID_ERROR_MSG, self)
 
         childs = [x.tag for x in list(root)]
 
         result_summary = root.find("ResultSummary")
 
         if result_summary is not None and int(result_summary.get("ErrorCount", 0)) > 0:
-
             if "CLI" in childs:
                 error_msg = root.find("CLI").get("ErrorMsg") or ""
             elif "Commit" in childs:
                 error_msg = root.find("Commit").get("ErrorMsg") or ""
                 error_code = root.find("Commit").get("ErrorCode") or ""
                 if error_code == "0x41866c00":
                     # yet another pointless IOS-XR error:
```

### Comparing `napalm-4.1.0/napalm.egg-info/PKG-INFO` & `napalm-5.0.0/napalm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 Metadata-Version: 2.1
 Name: napalm
-Version: 4.1.0
+Version: 5.0.0
 Summary: Network Automation and Programmability Abstraction Layer with Multivendor support
 Home-page: https://github.com/napalm-automation/napalm
 Author: David Barroso, Kirk Byers, Mircea Ulinic
 Author-email: dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=38.4.0
+Requires-Dist: cffi>=1.11.3
+Requires-Dist: paramiko>=2.6.0
+Requires-Dist: requests>=2.7.0
+Requires-Dist: textfsm
+Requires-Dist: jinja2
+Requires-Dist: netaddr
+Requires-Dist: pyYAML
+Requires-Dist: pyeapi>=1.0.2
+Requires-Dist: netmiko>=4.1.0
+Requires-Dist: junos-eznc>=2.7.0
+Requires-Dist: scp
+Requires-Dist: lxml>=4.3.0
+Requires-Dist: ncclient
+Requires-Dist: ttp
+Requires-Dist: ttp_templates
+Requires-Dist: netutils>=1.0.0
+Requires-Dist: typing-extensions>=4.3.0
 
 [![PyPI](https://img.shields.io/pypi/v/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/napalm.svg)](https://pypi.python.org/pypi/napalm)
 [![Actions Build](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml/badge.svg?branch=develop)](https://github.com/napalm-automation/napalm/actions/workflows/commit.yaml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
@@ -48,14 +67,17 @@
 Install
 =======
 
 ```
 pip install napalm
 ```
 
+*Note*: Beginning with release 5.0.0 and later, NAPALM offers support for
+Python 3.8+ only.
+
 *Note*: Beginning with release 4.0.0 and later, NAPALM offers support for
 Python 3.7+ only.
 
 *Note*: Beginning with release 3.0.0 and later, NAPALM offers support for
 Python 3.6+ only.
```

### Comparing `napalm-4.1.0/napalm.egg-info/SOURCES.txt` & `napalm-5.0.0/napalm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,23 +37,21 @@
 napalm/base/test/helpers.py
 napalm/base/utils/__init__.py
 napalm/base/utils/jinja_filters.py
 napalm/base/utils/string_parsers.py
 napalm/eos/__init__.py
 napalm/eos/constants.py
 napalm/eos/eos.py
-napalm/eos/pyeapi_syntax_wrapper.py
 napalm/eos/templates/delete_ntp_servers.j2
 napalm/eos/templates/delete_snmp_config.j2
 napalm/eos/templates/delete_users.j2
 napalm/eos/templates/set_ntp_servers.j2
 napalm/eos/templates/set_users.j2
 napalm/eos/templates/snmp_config.j2
 napalm/eos/utils/__init__.py
-napalm/eos/utils/cli_syntax.py
 napalm/eos/utils/versions.py
 napalm/eos/utils/textfsm_templates/bgp_detail.tpl
 napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl
 napalm/eos/utils/textfsm_templates/ntp_peers.tpl
 napalm/eos/utils/textfsm_templates/snmp_config.tpl
 napalm/eos/utils/textfsm_templates/vrf.tpl
 napalm/ios/__init__.py
```

### Comparing `napalm-4.1.0/setup.cfg` & `napalm-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `napalm-4.1.0/setup.py` & `napalm-5.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """setup.py file."""
+
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fs:
     reqs = [r for r in fs.read().splitlines() if (len(r) > 0 and not r.startswith("#"))]
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 
 __author__ = "David Barroso <dbarrosop@dravetech.com>"
 
 setup(
     name="napalm",
-    version="4.1.0",
+    version="5.0.0",
     packages=find_packages(exclude=("test*",)),
     test_suite="test_base",
     author="David Barroso, Kirk Byers, Mircea Ulinic",
     author_email="dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com",
     description="Network Automation and Programmability Abstraction Layer with Multivendor support",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
     ],
     url="https://github.com/napalm-automation/napalm",
     include_package_data=True,
     install_requires=reqs,
     entry_points={
```

