# Comparing `tmp/illumio_pylo-0.3.3.tar.gz` & `tmp/illumio_pylo-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illumio_pylo-0.3.3.tar", last modified: Wed Apr 10 10:37:29 2024, max compression
+gzip compressed data, was "illumio_pylo-0.3.4.tar", last modified: Wed Apr 10 12:13:52 2024, max compression
```

## Comparing `illumio_pylo-0.3.3.tar` & `illumio_pylo-0.3.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.440639 illumio_pylo-0.3.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.436639 illumio_pylo-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.440639 illumio_pylo-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.github/workflows/doxygen-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.github/workflows/make-binaries.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.444639 illumio_pylo-0.3.3/dev_playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/check_unique_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/check_unique_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/delete_all_workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/delete_unused_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/explorer_report_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/export_rules_to_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/generate-random-workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/healthcheck_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/import-labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/import_workloads_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/iplists_stats_duplicates_unused_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/recalculate_explorer_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/recalculate_explorer_logs_multithreaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/rules_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/rules_exporter_special.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/test_change_workload_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/test_query2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/test_securityprincipals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/ven_idle_to_illumination.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/dev_playground/ven_reassign_pce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.444639 illumio_pylo-0.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/examples/explorer_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/examples/extend_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.448639 illumio_pylo-0.3.3/illumio_pylo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.448639 illumio_pylo-0.3.3/illumio_pylo/API/
--rw-r--r--   0 runner    (1001) docker     (127)    60494 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/APIConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/AuditLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/ClusterHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/CredentialsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/Explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/JsonPayloadTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/RuleSearchQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/AgentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.452639 illumio_pylo-0.3.3/illumio_pylo/Helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21890 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Helpers/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/IPList.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/IPMap.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/LabelCommon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/LabelGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/LabelStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/LabeledObject.py
--rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/ReferenceTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/RulesetStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/SecurityPrincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/SoftwareVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/VirtualService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/VirtualServiceStore.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/Workload.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/WorkloadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/WorkloadStoreSubClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.452639 illumio_pylo-0.3.3/illumio_pylo/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/NativeParsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.452639 illumio_pylo-0.3.3/illumio_pylo/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/iplist_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/iplist_import_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/ruleset_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/update_pce_objects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.452639 illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/LabelCreation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_compatibility_report_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_duplicate_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_idle_to_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_reset_names_to_null.py
--rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.452639 illumio_pylo-0.3.3/illumio_pylo/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/docs/Doxygen
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/illumio_pylo/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/credentials.example.json
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/health_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/iplists-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/iplists-import-example.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/workloads-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/illumio_pylo/utilities/resources/workloads-import-example.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/illumio_pylo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 10:37:29.000000 illumio_pylo-0.3.3/illumio_pylo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-10 10:37:29.000000 illumio_pylo-0.3.3/illumio_pylo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:37:29.000000 illumio_pylo-0.3.3/illumio_pylo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 10:37:29.000000 illumio_pylo-0.3.3/illumio_pylo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 10:37:29.000000 illumio_pylo-0.3.3/illumio_pylo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:37:29.456639 illumio_pylo-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 10:37:22.000000 illumio_pylo-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.957493 illumio_pylo-0.3.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.953493 illumio_pylo-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.957493 illumio_pylo-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/doxygen-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/make-binaries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.961493 illumio_pylo-0.3.4/dev_playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/check_unique_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/check_unique_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/delete_all_workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/delete_unused_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/explorer_report_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/export_rules_to_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/generate-random-workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/healthcheck_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/import-labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/import_workloads_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/iplists_stats_duplicates_unused_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs_multithreaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/rules_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/rules_exporter_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_change_workload_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_query2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_securityprincipals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/ven_idle_to_illumination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/ven_reassign_pce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.961493 illumio_pylo-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/examples/explorer_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/examples/extend_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/API/
+-rw-r--r--   0 runner    (1001) docker     (127)    60500 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/APIConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/AuditLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/ClusterHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/CredentialsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/Explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/JsonPayloadTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/RuleSearchQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/AgentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21890 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/IPList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/IPMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelCommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabeledObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/ReferenceTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/RulesetStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/SecurityPrincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/SoftwareVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/VirtualService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/VirtualServiceStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/WorkloadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/WorkloadStoreSubClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/NativeParsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_import_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ruleset_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/update_pce_objects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/LabelCreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_compatibility_report_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_duplicate_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_idle_to_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_reset_names_to_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/docs/Doxygen
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/credentials.example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/health_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/setup.py
```

### Comparing `illumio_pylo-0.3.3/.devcontainer/devcontainer.json` & `illumio_pylo-0.3.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/.github/workflows/doxygen-publish.yml` & `illumio_pylo-0.3.4/.github/workflows/doxygen-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/.github/workflows/make-binaries.yml` & `illumio_pylo-0.3.4/.github/workflows/make-binaries.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/.github/workflows/python-publish.yml` & `illumio_pylo-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/LICENSE` & `illumio_pylo-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/PKG-INFO` & `illumio_pylo-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.3/README.md` & `illumio_pylo-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/check_unique_hostnames.py` & `illumio_pylo-0.3.4/dev_playground/check_unique_hostnames.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/check_unique_services.py` & `illumio_pylo-0.3.4/dev_playground/check_unique_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/delete_all_workloads.py` & `illumio_pylo-0.3.4/dev_playground/delete_all_workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/delete_unused_services.py` & `illumio_pylo-0.3.4/dev_playground/delete_unused_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/explorer_report_exporter.py` & `illumio_pylo-0.3.4/dev_playground/explorer_report_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/export_rules_to_firewall.py` & `illumio_pylo-0.3.4/dev_playground/export_rules_to_firewall.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/generate-random-workloads.py` & `illumio_pylo-0.3.4/dev_playground/generate-random-workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/healthcheck_log.py` & `illumio_pylo-0.3.4/dev_playground/healthcheck_log.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/import-labels.py` & `illumio_pylo-0.3.4/dev_playground/import-labels.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/import_workloads_placeholders.py` & `illumio_pylo-0.3.4/dev_playground/import_workloads_placeholders.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/iplists_stats_duplicates_unused_finder.py` & `illumio_pylo-0.3.4/dev_playground/iplists_stats_duplicates_unused_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/recalculate_explorer_logs.py` & `illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/recalculate_explorer_logs_multithreaded.py` & `illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs_multithreaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,17 @@
 resolution_cache = {}
 
 
 def do_log_resolution(q: Queue, thread_num: int):
     global skip_count
     global resolution_cache
 
-    local_connector = pylo.APIConnector(connector.hostname, connector.port, connector.api_user, connector.api_key, connector.skipSSLCertCheck, connector.orgID)
+    local_connector = pylo.APIConnector(fqdn=connector.fqdn, port=connector.port,
+                                        api_user=connector.api_user, api_key=connector.api_key,
+                                        skip_ssl_cert_check= connector.skipSSLCertCheck, org_id=connector.org_id)
 
     while True:
 
         log, local_log_number = q.get()
 
         output_text = ''
```

### Comparing `illumio_pylo-0.3.3/dev_playground/rules_exporter.py` & `illumio_pylo-0.3.4/dev_playground/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/rules_exporter_special.py` & `illumio_pylo-0.3.4/dev_playground/rules_exporter_special.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/test.py` & `illumio_pylo-0.3.4/dev_playground/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from illumio_pylo import log
 import logging
 
 
 log.setLevel(logging.DEBUG)
 
 
-con = pylo.APIConnector(fqdn="192.168.253.10", port=8443, skip_ssl_cert_check=True, apiuser='api_185c2399e24b631c2',
-                        apikey='2dbaf8fe5bb9278e26388e5d35229a6797ff5c622154b6289edfc03e7c0f9782')
+con = pylo.APIConnector(fqdn="192.168.253.10", port=8443, skip_ssl_cert_check=True, api_user='api_185c2399e24b631c2',
+                        api_key='2dbaf8fe5bb9278e26388e5d35229a6797ff5c622154b6289edfc03e7c0f9782')
 
 con.collect_pce_infos()
 
 print('*** Successful connection to PCE ' + con.hostname + ' running ASP version ' + con.get_software_version_string())
 
 print("\n")
 print("** Now loading Organization from API...")
```

### Comparing `illumio_pylo-0.3.3/dev_playground/test_change_workload_desc.py` & `illumio_pylo-0.3.4/dev_playground/test_change_workload_desc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/test_query.py` & `illumio_pylo-0.3.4/dev_playground/test_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/test_query2.py` & `illumio_pylo-0.3.4/dev_playground/test_query2.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/test_securityprincipals.py` & `illumio_pylo-0.3.4/dev_playground/test_securityprincipals.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/ven_idle_to_illumination.py` & `illumio_pylo-0.3.4/dev_playground/ven_idle_to_illumination.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/dev_playground/ven_reassign_pce.py` & `illumio_pylo-0.3.4/dev_playground/ven_reassign_pce.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/examples/explorer_query.py` & `illumio_pylo-0.3.4/examples/explorer_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/examples/extend_cli.py` & `illumio_pylo-0.3.4/examples/extend_cli.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/APIConnector.py` & `illumio_pylo-0.3.4/illumio_pylo/API/APIConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,24 +58,24 @@
         'label_dimensions': 'label_dimensions'
     }
 
 
 class APIConnector:
     """docstring for APIConnector."""
 
-    def __init__(self, fqdn: str, port, apiuser: str, apikey: str, skip_ssl_cert_check=False, org_id=1, name='unnamed'):
+    def __init__(self, fqdn: str, port, api_user: str, api_key: str, skip_ssl_cert_check=False, org_id=1, name='unnamed'):
         self.name = name
         self.fqdn: str = fqdn
         if type(port) is int:
             port = str(port)
         self.port: int = port
-        self._api_key: str = apikey
+        self._api_key: str = api_key
         self._decrypted_api_key: str = None
-        self.api_user: str = apiuser
-        self.orgID: int = org_id
+        self.api_user: str = api_user
+        self.org_id: int = org_id
         self.skipSSLCertCheck: bool = skip_ssl_cert_check
         self.version: Optional['pylo.SoftwareVersion'] = None
         self.version_string: str = "Not Defined"
         self._cached_session = requests.session()
 
     @property
     def api_key(self):
@@ -144,15 +144,15 @@
             path = path[1:]
         url = "https://{0}:{1}/{2}".format(self.fqdn, self.port, path)
         return url
 
     def _make_api_url(self, path: str = '', include_org_id=False) -> str:
         url = self._make_base_url('/api/v2')
         if include_org_id:
-            url += '/orgs/' + str(self.orgID)
+            url += '/orgs/' + str(self.org_id)
         url += path
 
         return url
 
     def do_get_call(self, path, json_arguments=None, include_org_id=True, json_output_expected=True, async_call=False, params=None, skip_product_version_check=False,
                     retry_count_if_api_call_limit_reached=default_retry_count_if_api_call_limit_reached,
                     retry_wait_time_if_api_call_limit_reached=default_retry_wait_time_if_api_call_limit_reached,
```

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/AuditLog.py` & `illumio_pylo-0.3.4/illumio_pylo/API/AuditLog.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/ClusterHealth.py` & `illumio_pylo-0.3.4/illumio_pylo/API/ClusterHealth.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/CredentialsManager.py` & `illumio_pylo-0.3.4/illumio_pylo/API/CredentialsManager.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/Explorer.py` & `illumio_pylo-0.3.4/illumio_pylo/API/Explorer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/JsonPayloadTypes.py` & `illumio_pylo-0.3.4/illumio_pylo/API/JsonPayloadTypes.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/API/RuleSearchQuery.py` & `illumio_pylo-0.3.4/illumio_pylo/API/RuleSearchQuery.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/AgentStore.py` & `illumio_pylo-0.3.4/illumio_pylo/AgentStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Exception.py` & `illumio_pylo-0.3.4/illumio_pylo/Exception.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Helpers/exports.py` & `illumio_pylo-0.3.4/illumio_pylo/Helpers/exports.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Helpers/functions.py` & `illumio_pylo-0.3.4/illumio_pylo/Helpers/functions.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/IPList.py` & `illumio_pylo-0.3.4/illumio_pylo/IPList.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/IPMap.py` & `illumio_pylo-0.3.4/illumio_pylo/IPMap.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Label.py` & `illumio_pylo-0.3.4/illumio_pylo/Label.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/LabelCommon.py` & `illumio_pylo-0.3.4/illumio_pylo/LabelCommon.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/LabelGroup.py` & `illumio_pylo-0.3.4/illumio_pylo/LabelGroup.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/LabelStore.py` & `illumio_pylo-0.3.4/illumio_pylo/LabelStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/LabeledObject.py` & `illumio_pylo-0.3.4/illumio_pylo/LabeledObject.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Organization.py` & `illumio_pylo-0.3.4/illumio_pylo/Organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :param include_deleted_workloads:
         :param callback_api_objects_downloaded: callback function that will be called after each API has finished downloading all objects
         :return:
         """
         credentials = get_credentials_from_file(fqdn_or_profile_name, credential_file)
 
         connector = pylo.APIConnector(fqdn=credentials.fqdn, port=credentials.port,
-                                      apiuser=credentials.api_user, apikey=credentials.api_key,
+                                      api_user=credentials.api_user, api_key=credentials.api_key,
                                       org_id=credentials.org_id,
                                       skip_ssl_cert_check=not credentials.verify_ssl, name=fqdn_or_profile_name)
 
         objects = connector.get_pce_objects(list_of_objects_to_load=list_of_objects_to_load,
                                             include_deleted_workloads=include_deleted_workloads)
 
         if callback_api_objects_downloaded is not None:
```

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Query.py` & `illumio_pylo-0.3.4/illumio_pylo/Query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/ReferenceTracker.py` & `illumio_pylo-0.3.4/illumio_pylo/ReferenceTracker.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Rule.py` & `illumio_pylo-0.3.4/illumio_pylo/Rule.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Ruleset.py` & `illumio_pylo-0.3.4/illumio_pylo/Ruleset.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/RulesetStore.py` & `illumio_pylo-0.3.4/illumio_pylo/RulesetStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/SecurityPrincipal.py` & `illumio_pylo-0.3.4/illumio_pylo/SecurityPrincipal.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Service.py` & `illumio_pylo-0.3.4/illumio_pylo/Service.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/SoftwareVersion.py` & `illumio_pylo-0.3.4/illumio_pylo/SoftwareVersion.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/VirtualService.py` & `illumio_pylo-0.3.4/illumio_pylo/VirtualService.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/VirtualServiceStore.py` & `illumio_pylo-0.3.4/illumio_pylo/VirtualServiceStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/Workload.py` & `illumio_pylo-0.3.4/illumio_pylo/Workload.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/WorkloadStore.py` & `illumio_pylo-0.3.4/illumio_pylo/WorkloadStore.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/WorkloadStoreSubClasses.py` & `illumio_pylo-0.3.4/illumio_pylo/WorkloadStoreSubClasses.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/__init__.py` & `illumio_pylo-0.3.4/illumio_pylo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 import os
 import sys
 from typing import Callable
 
 from .tmp import *
 from .Helpers import *
@@ -39,15 +39,15 @@
 def get_organization(fqdn: str, port: int, api_user: str, api_key: str,
                      organization_id: int, verify_ssl: bool = True,
                      list_of_objects_to_load: Optional[List['pylo.ObjectTypes']] = None,
                      include_deleted_workloads: bool = False) -> Organization:
     """
     Load an organization from the API with parameters provided as arguments.
     """
-    api = APIConnector(fqdn=fqdn, port=port, apiuser=api_user, apikey=api_key, org_id=organization_id,
+    api = APIConnector(fqdn=fqdn, port=port, api_user=api_user, api_key=api_key, org_id=organization_id,
                        skip_ssl_cert_check=not verify_ssl)
     org = Organization(1)
     org.load_from_api(api, include_deleted_workloads=include_deleted_workloads,
                       list_of_objects_to_load=list_of_objects_to_load)
 
     return org
```

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/NativeParsers.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/NativeParsers.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/__init__.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/__init__.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/credential_manager.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/credential_manager.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/iplist_analyzer.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_analyzer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/iplist_import_from_file.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_import_from_file.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/ruleset_export.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ruleset_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/update_pce_objects_cache.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/update_pce_objects_cache.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/LabelCreation.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/LabelCreation.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/utils/misc.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/misc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_compatibility_report_export.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_compatibility_report_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_duplicate_remover.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_duplicate_remover.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_idle_to_visibility.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_idle_to_visibility.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/ven_upgrader.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_upgrader.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_export.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_import.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_import.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_reset_names_to_null.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_reset_names_to_null.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_update.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_update.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/cli/commands/workload_used_in_rule_finder.py` & `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_used_in_rule_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/docs/Doxygen` & `illumio_pylo-0.3.4/illumio_pylo/docs/Doxygen`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/tmp.py` & `illumio_pylo-0.3.4/illumio_pylo/tmp.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/utilities/health_monitoring.py` & `illumio_pylo-0.3.4/illumio_pylo/utilities/health_monitoring.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/utilities/resources/iplists-import-example.xlsx` & `illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo/utilities/resources/workloads-import-example.xlsx` & `illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/illumio_pylo.egg-info/PKG-INFO` & `illumio_pylo-0.3.4/illumio_pylo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.3/illumio_pylo.egg-info/SOURCES.txt` & `illumio_pylo-0.3.4/illumio_pylo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/pyproject.toml` & `illumio_pylo-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.3/setup.py` & `illumio_pylo-0.3.4/setup.py`

 * *Files identical despite different names*

