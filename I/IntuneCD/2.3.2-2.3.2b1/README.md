# Comparing `tmp/IntuneCD-2.3.2.tar.gz` & `tmp/IntuneCD-2.3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-2.3.2.tar", last modified: Wed Apr 10 10:22:09 2024, max compression
+gzip compressed data, was "IntuneCD-2.3.2b1.tar", last modified: Tue Apr  9 07:03:24 2024, max compression
```

## Comparing `IntuneCD-2.3.2.tar` & `IntuneCD-2.3.2b1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.086821 IntuneCD-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.090821 IntuneCD-2.3.2/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.090821 IntuneCD-2.3.2/src/IntuneCD/backup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.094821 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthenticationMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/ExternalIdentities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.098821 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/APNs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Activationlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AutopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/CompliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagementPartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/NotificationTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/PowershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/backup_intune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/document_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/document_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.102821 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseBackupModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    36404 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseGraphModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseUpdateModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/IntuneCDBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/process_audit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/intunecdlib/process_scope_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/run_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.102821 IntuneCD-2.3.2/src/IntuneCD/update/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.106822 IntuneCD-2.3.2/src/IntuneCD/update/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/src/IntuneCD/update/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/NotificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/PowerShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/src/IntuneCD/update_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 10:22:09.000000 IntuneCD-2.3.2/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:22:09.110822 IntuneCD-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-10 10:22:03.000000 IntuneCD-2.3.2/tests/test_get_authparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.761375 IntuneCD-2.3.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.765375 IntuneCD-2.3.2b1/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.765375 IntuneCD-2.3.2b1/src/IntuneCD/backup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.769374 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthenticationMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/ExternalIdentities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.777374 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/APNs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Activationlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AutopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/CompliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/NotificationTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/PowershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/backup_intune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/document_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/document_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.777374 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseBackupModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36404 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseGraphModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseUpdateModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/IntuneCDBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/process_audit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/process_scope_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/run_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.777374 IntuneCD-2.3.2b1/src/IntuneCD/update/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.781374 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/NotificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/PowerShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/src/IntuneCD/update_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 07:03:24.000000 IntuneCD-2.3.2b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:03:24.785374 IntuneCD-2.3.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-09 07:03:19.000000 IntuneCD-2.3.2b1/tests/test_get_authparams.py
```

### Comparing `IntuneCD-2.3.2/LICENSE` & `IntuneCD-2.3.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/PKG-INFO` & `IntuneCD-2.3.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.2
+Version: 2.3.2b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-2.3.2/README.md` & `IntuneCD-2.3.2b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/setup.cfg` & `IntuneCD-2.3.2b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 2.3.2
+version = 2.3.2.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/Applications.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/Applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthenticationFlows.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthenticationMethods.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthenticationMethods.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/B2B.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/DeviceRegistration.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/Domains.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/ExternalIdentities.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/ExternalIdentities.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/GroupSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/RoamingSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/SSPR.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Entra/SecurityDefaults.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/APNs.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/APNs.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Activationlock.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Activationlock.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppConfiguration.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppProtection.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Applications.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/AutopilotDevices.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/AutopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Compliance.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/CompliancePartner.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/CompliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ComplianceScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ConditionalAccess.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/CustomAttributes.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceCategories.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceCompliance.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceCompliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Filters.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagementIntents.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ManagementPartner.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ManagementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/NotificationTemplates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/NotificationTemplates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/PowershellScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/PowershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ProactiveRemediation.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ReusableSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/Roles.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ScopeTags.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/SettingsCatalog.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/ShellScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup_entra.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/backup_intune.py` & `IntuneCD-2.3.2b1/src/IntuneCD/backup_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/document_entra.py` & `IntuneCD-2.3.2b1/src/IntuneCD/document_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/document_intune.py` & `IntuneCD-2.3.2b1/src/IntuneCD/document_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseBackupModule.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseBackupModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseGraphModule.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseGraphModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/BaseUpdateModule.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/BaseUpdateModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/IntuneCDBase.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/IntuneCDBase.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/archive.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/assignment_report.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/documentation_functions.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/get_accesstoken.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/get_authparams.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/process_audit_data.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/process_audit_data.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/intunecdlib/process_scope_tags.py` & `IntuneCD-2.3.2b1/src/IntuneCD/intunecdlib/process_scope_tags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/run_backup.py` & `IntuneCD-2.3.2b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/run_documentation.py` & `IntuneCD-2.3.2b1/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/run_update.py` & `IntuneCD-2.3.2b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationFlows.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/AuthorizationPolicy.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/B2B.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/DeviceRegistration.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/Domains.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/GroupSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/RoamingSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/SSPR.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Entra/SecurityDefaults.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppConfiguration.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppProtection.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/Compliance.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ComplianceScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ConditionalAccess.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/CustomAttributes.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceCategories.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceCompliance.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceCompliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/DeviceManagementSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/Filters.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ManagementIntents.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/NotificationTemplate.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/NotificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/PowerShellScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/PowerShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ProactiveRemediation.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ReusableSettings.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/Roles.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ScopeTags.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/SettingsCatalog.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/ShellScripts.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update_entra.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD/update_intune.py` & `IntuneCD-2.3.2b1/src/IntuneCD/update_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-2.3.2b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.2
+Version: 2.3.2b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-2.3.2/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-2.3.2b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/tests/test_archive.py` & `IntuneCD-2.3.2b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/tests/test_documentation_functions.py` & `IntuneCD-2.3.2b1/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.2/tests/test_get_authparams.py` & `IntuneCD-2.3.2b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

