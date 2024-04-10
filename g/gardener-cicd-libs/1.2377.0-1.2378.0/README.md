# Comparing `tmp/gardener-cicd-libs-1.2377.0.tar.gz` & `tmp/gardener-cicd-libs-1.2378.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2377.0.tar", last modified: Wed Apr 10 11:55:26 2024, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2378.0.tar", last modified: Wed Apr 10 13:21:09 2024, max compression
```

## Comparing `gardener-cicd-libs-1.2377.0.tar` & `gardener-cicd-libs-1.2378.0.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1878 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.378494 gardener-cicd-libs-1.2377.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     5885 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10129 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     4925 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     6641 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.382494 gardener-cicd-libs-1.2377.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5055 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     4552 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6160 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     9392 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7649 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)    12929 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)    11021 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)    10471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    14273 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6390 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)    13503 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9039 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.386494 gardener-cicd-libs-1.2377.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     5797 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     6269 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)    26917 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)     6363 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/upload.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.386494 gardener-cicd-libs-1.2377.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.386494 gardener-cicd-libs-1.2377.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14167 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    14992 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     5950 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12014 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    19848 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.386494 gardener-cicd-libs-1.2377.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7034 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)     9849 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)      549 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    11777 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    16915 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.390494 gardener-cicd-libs-1.2377.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1980 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17414 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     4610 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     2179 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4205 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    12471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5053 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     5923 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1341 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    20426 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     3793 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    14289 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2098 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)     9246 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4710 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.394494 gardener-cicd-libs-1.2377.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 11:55:21.000000 gardener-cicd-libs-1.2377.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4380 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.398494 gardener-cicd-libs-1.2377.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)      811 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10346 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     2730 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    12322 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     4985 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     2260 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     4630 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)      890 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)    10331 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8764 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     4003 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     7200 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     4374 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)    12160 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    13851 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     8448 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4649 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6674 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    22903 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     5265 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.398494 gardener-cicd-libs-1.2377.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23388 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5013 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.398494 gardener-cicd-libs-1.2377.0/container/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12483 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.398494 gardener-cicd-libs-1.2377.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1538 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.402495 gardener-cicd-libs-1.2377.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/cosign_util.py
--rw-r--r--   0 root         (0) root         (0)     2085 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/oci_platform.py
--rw-r--r--   0 root         (0) root         (0)    27381 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6717 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/rbsc_bom.py
--rw-r--r--   0 root         (0) root         (0)     2779 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/replicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.402495 gardener-cicd-libs-1.2377.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     6370 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2744 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.402495 gardener-cicd-libs-1.2377.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16656 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     2335 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.402495 gardener-cicd-libs-1.2377.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10817 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     7356 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1878 2024-04-10 11:55:26.000000 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5787 2024-04-10 11:55:26.000000 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:55:26.000000 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      848 2024-04-10 11:55:26.000000 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-10 11:55:26.000000 gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.406494 gardener-cicd-libs-1.2377.0/gci/
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gci/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10005 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gci/component-descriptor-v2-schema.yaml
--rw-r--r--   0 root         (0) root         (0)    19933 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gci/componentmodel.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gci/oci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.406494 gardener-cicd-libs-1.2377.0/github/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7904 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.406494 gardener-cicd-libs-1.2377.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14491 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)     3603 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)    11393 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    30739 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/compliance/report.py
--rw-r--r--   0 root         (0) root         (0)     1189 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    33477 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    16120 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6460 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.406494 gardener-cicd-libs-1.2377.0/mail/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9161 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)      286 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/makoutil.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.406494 gardener-cicd-libs-1.2377.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15299 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     7062 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/release_notes/markdown.py
--rw-r--r--   0 root         (0) root         (0)    11426 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     9661 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/reutil.py
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4736 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/test/
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1541 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1858 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.410495 gardener-cicd-libs-1.2377.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)      851 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2189 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1082 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/test/container/
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/test/github/
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5495 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/github/github_util_test.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/gitutil_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5470 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:55:26.414495 gardener-cicd-libs-1.2377.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3765 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    17898 2024-04-10 11:54:39.000000 gardener-cicd-libs-1.2377.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.085673 gardener-cicd-libs-1.2378.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-10 13:21:09.085673 gardener-cicd-libs-1.2378.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.049672 gardener-cicd-libs-1.2378.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10129 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     6641 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.053672 gardener-cicd-libs-1.2378.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     9392 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7649 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    12929 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)    11021 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    14273 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6390 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)    13503 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9039 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.053672 gardener-cicd-libs-1.2378.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     8130 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     6269 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)    26917 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/upload.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.057672 gardener-cicd-libs-1.2378.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.057672 gardener-cicd-libs-1.2378.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14167 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    14992 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     5950 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12014 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    19848 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.057672 gardener-cicd-libs-1.2378.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)     9849 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    11777 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    16915 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.061673 gardener-cicd-libs-1.2378.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17414 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    12471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5053 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    20426 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    14289 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)     9246 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4710 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.061673 gardener-cicd-libs-1.2378.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 13:21:04.000000 gardener-cicd-libs-1.2378.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4380 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.069673 gardener-cicd-libs-1.2378.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)      811 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10346 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    12322 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     4630 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)      890 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)    10331 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8764 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     7254 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     4374 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)    12160 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    13851 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     8448 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6674 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    22903 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.069673 gardener-cicd-libs-1.2378.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23388 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5013 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.069673 gardener-cicd-libs-1.2378.0/container/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12483 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.069673 gardener-cicd-libs-1.2378.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.069673 gardener-cicd-libs-1.2378.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/cosign_util.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/oci_platform.py
+-rw-r--r--   0 root         (0) root         (0)    29148 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6717 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/rbsc_bom.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/replicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.073673 gardener-cicd-libs-1.2378.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     6373 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.073673 gardener-cicd-libs-1.2378.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16656 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.073673 gardener-cicd-libs-1.2378.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10817 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     7356 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.085673 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-10 13:21:08.000000 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5787 2024-04-10 13:21:09.000000 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:21:08.000000 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-10 13:21:08.000000 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-10 13:21:08.000000 gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.073673 gardener-cicd-libs-1.2378.0/gci/
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10005 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gci/component-descriptor-v2-schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    19933 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gci/componentmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gci/oci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/github/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7904 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14491 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)    11393 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    30739 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/compliance/report.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    33477 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    16120 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6460 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9161 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)      286 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/makoutil.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15299 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)    11426 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     9661 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/reutil.py
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-10 13:21:09.085673 gardener-cicd-libs-1.2378.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.077673 gardener-cicd-libs-1.2378.0/test/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)      517 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/github/github_util_test.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/gitutil_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.081673 gardener-cicd-libs-1.2378.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5470 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:21:09.085673 gardener-cicd-libs-1.2378.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3765 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    17898 2024-04-10 13:20:09.000000 gardener-cicd-libs-1.2378.0/version.py
```

### Comparing `gardener-cicd-libs-1.2377.0/LICENSE` & `gardener-cicd-libs-1.2378.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/PKG-INFO` & `gardener-cicd-libs-1.2378.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gardener-cicd-libs
-Version: 1.2377.0
+Version: 1.2378.0
 Summary: Gardener CI/CD Libraries
 Requires-Python: >=3.10
 License-File: LICENSE
-Requires-Dist: gardener-cicd-base>=1.2377.0
-Requires-Dist: gardener-oci>=1.2377.0
+Requires-Dist: gardener-cicd-base>=1.2378.0
+Requires-Dist: gardener-oci>=1.2378.0
 Requires-Dist: GitPython
 Requires-Dist: Mako<2.0.0
 Requires-Dist: Sphinx
 Requires-Dist: aliyun-python-sdk-core==2.15.0
 Requires-Dist: aliyun-python-sdk-ecs==4.24.71
 Requires-Dist: aliyun-python-sdk-ram==3.3.0
 Requires-Dist: awesomeversion
```

### Comparing `gardener-cicd-libs-1.2377.0/README.md` & `gardener-cicd-libs-1.2378.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2378.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/aws.py` & `gardener-cicd-libs-1.2378.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/clamav.py` & `gardener-cicd-libs-1.2378.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/concourse.py` & `gardener-cicd-libs-1.2378.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/delivery.py` & `gardener-cicd-libs-1.2378.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2378.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/gcp.py` & `gardener-cicd-libs-1.2378.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/github.py` & `gardener-cicd-libs-1.2378.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2378.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/oci.py` & `gardener-cicd-libs-1.2378.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/protecode.py` & `gardener-cicd-libs-1.2378.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2378.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2378.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cli.py` & `gardener-cicd-libs-1.2378.0/cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/access.py` & `gardener-cicd-libs-1.2378.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/purge.py` & `gardener-cicd-libs-1.2378.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2378.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/upload.py` & `gardener-cicd-libs-1.2378.0/cnudie/upload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/util.py` & `gardener-cicd-libs-1.2378.0/cnudie/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cnudie/validate.py` & `gardener-cicd-libs-1.2378.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/client/api.py` & `gardener-cicd-libs-1.2378.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/client/model.py` & `gardener-cicd-libs-1.2378.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2378.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/client/util.py` & `gardener-cicd-libs-1.2378.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2378.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/factory.py` & `gardener-cicd-libs-1.2378.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/base.py` & `gardener-cicd-libs-1.2378.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/job.py` & `gardener-cicd-libs-1.2378.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2378.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2378.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/step.py` & `gardener-cicd-libs-1.2378.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/draft_release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/update_component_deps.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2378.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/replicator.py` & `gardener-cicd-libs-1.2378.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2378.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2378.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2378.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2378.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2378.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/component_descriptor_util.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/component_descriptor_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/draft_release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/os_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             if not isinstance(scan_result.data, dm.OsID):
                 logger.warning('unexpected scan-result-type: {scan_result=}')
             else:
                 scan_result.data: dm.OsID
 
                 return gcm.OsIdScanResult(
                     scanned_element=cnudie.iter.ResourceNode(
-                        path=(component,),
+                        path=(cnudie.iter.NodePathEntry(component),),
                         resource=resource,
                     ),
                     os_id=scan_result.data.os_info,
                     skip_upload_to_deliverydb=True, # no need to re-upload (got it from there)
                 )
 
     # there was no scanresult, so we have to scan
@@ -121,15 +121,15 @@
         # if we could not determine os-info, upload a dummy os-info (with all entries set to None)
         # to keep track of the failed scan attempt
         last_os_info = um.OperatingSystemId()
 
     # pylint: disable=E1123
     return gcm.OsIdScanResult(
         scanned_element=cnudie.iter.ResourceNode(
-            path=(component,),
+            path=(cnudie.iter.NodePathEntry(component),),
             resource=resource,
         ),
         os_id=last_os_info,
     )
 
 
 def scan_result_group_collection_for_outdated_os_ids(
```

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/update_component_deps.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/update_component_deps.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2378.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2378.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2378.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/util.py` & `gardener-cicd-libs-1.2378.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/concourse/validator.py` & `gardener-cicd-libs-1.2378.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/container/util.py` & `gardener-cicd-libs-1.2378.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/cosign/payload.py` & `gardener-cicd-libs-1.2378.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/cosign_util.py` & `gardener-cicd-libs-1.2378.0/ctt/cosign_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/filters.py` & `gardener-cicd-libs-1.2378.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/oci_platform.py` & `gardener-cicd-libs-1.2378.0/ctt/oci_platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2378.0/ctt/process_dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # SPDX-FileCopyrightText: 2021 SAP SE or an SAP affiliate company and Gardener contributors
 #
 # SPDX-License-Identifier: Apache-2.0
 
+import collections.abc
 import concurrent.futures
 import dataclasses
 import enum
 import hashlib
 import itertools
 import json
 import jsonschema
 import logging
 import os
-import typing
 import threading
 
 import ccc.oci
 import ci.util
 import ctt.replicate
 import cnudie.iter
 import cnudie.retrieve
 import cnudie.upload
 import container.util
 import cosign.payload as cp
+import dso.labels
 import gci.componentmodel as cm
 import oci
 import oci.client
 import oci.model as om
 
 import ctt.cosign_util as cosign
 import ctt.filters as filters
@@ -75,16 +76,15 @@
             )
         )
 
     def process(
         self,
         component: cm.Component,
         resource: cm.Resource,
-        processing_mode: ProcessingMode,
-        inject_ocm_coordinates_into_oci_manifests: bool = False,
+        inject_ocm_coordinates_into_oci_manifests: bool=False,
     ) -> processing_model.ProcessingJob:
         if not self.matches(component, resource):
             return None
 
         logging.info(f'{inject_ocm_coordinates_into_oci_manifests=}')
         logging.info(
             f'{self._name} will process: '
@@ -98,15 +98,15 @@
                 source_ref=None,
                 target_ref=None,  # must be set by a later step
                 remove_files=None,  # _may_ be set by a later step
             ),
             inject_ocm_coordinates_into_oci_manifest=inject_ocm_coordinates_into_oci_manifests,
         )
 
-        job = self._processor.process(processing_job=job)
+        job: processing_model.ProcessingJob = self._processor.process(processing_job=job)
 
         first = True
         for uploader in self._uploaders:
             job = uploader.process(job, target_as_source=not first)
             first = False
 
         lssd_label = create_lssd_label(
@@ -122,32 +122,32 @@
             processed_resource=patched_resource,
         )
 
         return job
 
 
 def create_lssd_label(
-    processing_rules: typing.List[str],
+    processing_rules: list[str],
 ) -> cm.Label:
     lssd_label_name = 'cloud.gardener.cnudie/sdo/lssd'
     label = cm.Label(
         name=lssd_label_name,
         value={
             'processingRules': processing_rules,
         },
     )
 
     return label
 
 
-def parse_processing_cfg(path):
+def parse_processing_cfg(path: str):
     raw_cfg = ci.util.parse_yaml_file(path)
 
     processing_cfg_dir = os.path.abspath(os.path.dirname(path))
-    for name, cfg in raw_cfg.get('processors', {}).items():
+    for _, cfg in raw_cfg.get('processors', {}).items():
         cfg['kwargs']['base_dir'] = processing_cfg_dir
 
     return raw_cfg
 
 
 def _filter(filter_cfg: dict):
     filter_ctor = getattr(filters, filter_cfg['type'])
@@ -172,16 +172,16 @@
         ci.util.fail(f'no such uploader: {upload_type}')
     uploader = upload_ctor(**uploader_cfg.get('kwargs', {}))
     return uploader
 
 
 def processing_pipeline(
     processing_cfg: dict,
-    shared_processors: dict = {},
-    shared_uploaders: dict = {},
+    shared_processors: dict={},
+    shared_uploaders: dict={},
 ) -> ProcessingPipeline:
     name = processing_cfg.get('name', '<no name>')
 
     filter_cfgs = processing_cfg['filter']
     if isinstance(filter_cfgs, dict):
         filter_cfgs = [filter_cfgs]
     filters = [_filter(filter_cfg=filter_cfg) for filter_cfg in filter_cfgs]
@@ -227,32 +227,35 @@
         cfg_entries,
         itertools.repeat(shared_processors, len(cfg_entries)),
         itertools.repeat(shared_uploaders, len(cfg_entries)),
     )
 
 
 def create_jobs(
-    processing_cfg_path,
+    processing_cfg_path: str,
     component_descriptor_v2: cm.ComponentDescriptor,
-    processing_mode,
-    inject_ocm_coordinates_into_oci_manifests,
+    inject_ocm_coordinates_into_oci_manifests: bool,
     component_descriptor_lookup: cnudie.retrieve.ComponentDescriptorLookupById,
+    component_filter: collections.abc.Callable[[cm.Component], bool]=None,
+    reftype_filter: collections.abc.Callable[[cnudie.iter.NodeReferenceType], bool]=None,
 ):
     processing_cfg = parse_processing_cfg(processing_cfg_path)
 
     shared_processors = {
         name: _processor(cfg) for name, cfg in processing_cfg.get('processors', {}).items()
     }
     shared_uploaders = {
         name: _uploader(cfg) for name, cfg in processing_cfg.get('uploaders', {}).items()
     }
 
     for component, resource in cnudie.iter.iter_resources(
         component=component_descriptor_v2,
         lookup=component_descriptor_lookup,
+        component_filter=component_filter,
+        reftype_filter=reftype_filter,
     ):
         resource: cm.Resource
         # XXX only support OCI-resources for now
         if not resource.type is cm.ArtefactType.OCI_IMAGE:
             continue
 
         oci_resource = resource
@@ -260,15 +263,14 @@
             parse_processing_cfg(processing_cfg_path),
             shared_processors,
             shared_uploaders,
         ):
             job = pipeline.process(
                 component=component,
                 resource=oci_resource,
-                processing_mode=processing_mode,
                 inject_ocm_coordinates_into_oci_manifests=inject_ocm_coordinates_into_oci_manifests,
             )
 
             if not job:
                 continue  # pipeline did not want to process
 
             yield job
@@ -283,17 +285,17 @@
 uploaded_image_refs_to_ready_events = {}  # <ref>:<event> (set if digest is available)
 upload_image_lock = threading.Lock()
 
 
 # uploads a single OCI artifact and returns the content digest
 def process_upload_request(
     processing_job: processing_model.ProcessingJob,
-    replication_mode=oci.ReplicationMode.PREFER_MULTIARCH,
-    platform_filter: typing.Callable[[om.OciPlatform], bool] = None,
-    oci_client: oci.client.Client = None,
+    replication_mode: oci.ReplicationMode=oci.ReplicationMode.PREFER_MULTIARCH,
+    platform_filter: collections.abc.Callable[[om.OciPlatform], bool]=None,
+    oci_client: oci.client.Client=None,
 ) -> str:
     global uploaded_image_refs_to_digests
     global uploaded_image_refs_to_ready_events
     global upload_image_lock
 
     if not oci_client:
         oci_client = ccc.oci.oci_client()
@@ -315,15 +317,15 @@
         upload_done_event.wait()
 
     if tgt_ref in uploaded_image_refs_to_digests:  # digest already present
         logger.info(f'{tgt_ref=} - was already uploaded by another rule - skipping')
         return uploaded_image_refs_to_digests[tgt_ref]
 
     # most common case: tgt has not yet been processed - process and afterwards signal
-    # other threads waiting for upload result that result is ready be setting the event
+    # other threads waiting for upload result that result is ready by setting the event
 
     accept = replication_mode.accept_header()
     manifest_blob_ref = oci_client.head_manifest(
         image_reference=tgt_ref,
         absent_ok=True,
         accept=accept,
     )
@@ -377,34 +379,44 @@
     else:
         src_name, _ = image_reference.rsplit(':', 1)
 
     return f'{src_name}@{docker_content_digest}'
 
 
 def process_images(
-    processing_cfg_path,
-    component_descriptor_v2,
+    processing_cfg_path: str,
+    component_descriptor_v2: cm.ComponentDescriptor,
     tgt_ctx_base_url: str,
     component_descriptor_lookup: cnudie.retrieve.ComponentDescriptorLookupById,
-    processing_mode=ProcessingMode.REGULAR,
+    processing_mode: ProcessingMode=ProcessingMode.REGULAR,
     upload_mode=None,
     upload_mode_cd=None,
     upload_mode_images=None,
-    replication_mode=oci.ReplicationMode.PREFER_MULTIARCH,
-    inject_ocm_coordinates_into_oci_manifests=False,
-    skip_cd_validation=False,
-    generate_cosign_signatures=False,
+    replication_mode: oci.ReplicationMode=oci.ReplicationMode.PREFER_MULTIARCH,
+    inject_ocm_coordinates_into_oci_manifests: bool=False,
+    skip_cd_validation: bool=False,
+    generate_cosign_signatures: bool=False,
     cosign_repository=None,
-    signing_server_url=None,
-    root_ca_cert_path=None,
-    platform_filter: typing.Callable[[om.OciPlatform], bool] = None,
-    bom_resources: typing.Sequence[BOMEntry] = [],
-    skip_component_upload: typing.Callable[[cm.Component], bool] = None,
-    oci_client: oci.client.Client = None,
+    signing_server_url: str=None,
+    root_ca_cert_path: str=None,
+    platform_filter: collections.abc.Callable[[om.OciPlatform], bool]=None,
+    bom_resources: collections.abc.Sequence[BOMEntry]=[],
+    skip_component_upload: collections.abc.Callable[[cm.Component], bool]=None,
+    oci_client: oci.client.Client=None,
+    component_filter: collections.abc.Callable[[cm.Component], bool]=None,
+    skip_labels: collections.abc.Callable[[str], bool]=None,
 ):
+    '''
+    note: Passing a filter to prevent component descriptors from being replicated using the
+    `skip_component_upload` parameter will still replicate all its resources (i.e. oci images)
+    as well as referenced components. In contrast to that, passing a filter using the
+    `component_filter` parameter will also exclude its resources as well as all transitive component
+    references from the replication. In both cases, `True` means the respective component is
+    _excluded_.
+    '''
     if not oci_client:
         oci_client = ccc.oci.oci_client()
 
     if processing_mode is ProcessingMode.DRY_RUN:
         ci.util.warning('dry-run: not downloading or uploading any images')
 
     if upload_mode_images:
@@ -416,20 +428,28 @@
     src_ctx_base_url = component_descriptor_v2.component.current_repository_ctx().baseUrl
 
     if src_ctx_base_url == tgt_ctx_base_url:
         raise RuntimeError('current repo context and target repo context must be different!')
 
     executor = concurrent.futures.ThreadPoolExecutor(max_workers=16)
 
+    reftype_filter = None
+    if skip_labels and skip_labels(dso.labels.ExtraComponentReferencesLabel.name):
+        def filter_extra_component_refs(reftype: cnudie.iter.NodeReferenceType) -> bool:
+            return reftype is cnudie.iter.NodeReferenceType.EXTRA_COMPONENT_REFS_LABEL
+
+        reftype_filter = filter_extra_component_refs
+
     jobs = create_jobs(
-        processing_cfg_path,
+        processing_cfg_path=processing_cfg_path,
         component_descriptor_v2=component_descriptor_v2,
-        processing_mode=processing_mode,
         inject_ocm_coordinates_into_oci_manifests=inject_ocm_coordinates_into_oci_manifests,
         component_descriptor_lookup=component_descriptor_lookup,
+        component_filter=component_filter,
+        reftype_filter=reftype_filter,
     )
 
     def process_job(processing_job: processing_model.ProcessingJob):
         if processing_mode is ProcessingMode.DRY_RUN:
             return processing_job
         elif processing_mode is ProcessingMode.REGULAR:
             pass
@@ -551,53 +571,48 @@
             processing_job.upload_request = dataclasses.replace(
                 processing_job.upload_request,
                 target_ref=target_ref,
             )
         else:
             target_ref = processing_job.upload_request.target_ref
 
-        bom_resources.append(
-            BOMEntry(
-                target_ref,
-                BOMEntryType.Docker,
-                f'{processing_job.component.name}/{processing_job.resource.name}',
-            )
-        )
+        bom_resources.append(BOMEntry(
+            url=target_ref,
+            type=BOMEntryType.Docker,
+            comp=f'{processing_job.component.name}/{processing_job.resource.name}',
+        ))
 
         return processing_job
 
     jobs = executor.map(process_job, jobs)
 
     # group jobs by component-version (TODO: either make Component immutable, or implement
     # __eq__ / __hash__
-    def cname_version(component):
+    def cname_version(component: cm.Component):
         return (component.name, component.version)
 
     def job_cname_version(job: processing_model.ProcessingJob):
         return cname_version(job.component)
 
-    def append_ctx_repo(ctx_base_url, component):
+    def append_ctx_repo(ctx_base_url: str | cm.OciOcmRepository, component: cm.Component):
         if isinstance(ctx_base_url, str):
             ocm_repo = cm.OciOcmRepository(baseUrl=ctx_base_url)
         elif isinstance(ctx_base_url, cm.OciOcmRepository):
             ocm_repo = ctx_base_url
         else:
             raise TypeError(ctx_base_url)
 
         if component.current_repository_ctx().baseUrl != ocm_repo.baseUrl:
-            component.repositoryContexts.append(
-                ocm_repo,
-            )
+            component.repositoryContexts.append(ocm_repo)
 
-    components = []
+    components: list[cm.Component] = []
     for _, job_group in itertools.groupby(
         sorted(jobs, key=job_cname_version),
         job_cname_version,
     ):
-
         patched_resources = {}
 
         # patch-in overwrites (caveat: must be done sequentially, as lists are not threadsafe)
         for job in job_group:
             component = job.component
             patched_resource = job.processed_resource or job.resource
             patched_resources[job.resource.identity(component.resources)] = patched_resource
@@ -618,14 +633,16 @@
     processed_component_versions = {cname_version(c) for c in components}
 
     # hack: add all components w/o resources (those would otherwise be ignored)
     for component_node in cnudie.iter.iter(
         component=component_descriptor_v2,
         lookup=component_descriptor_lookup,
         node_filter=cnudie.iter.Filter.components,
+        component_filter=component_filter,
+        reftype_filter=reftype_filter,
     ):
         component = component_node.component
         if not cname_version(component) in processed_component_versions:
             components.append(component)
             processed_component_versions.add(cname_version(component))
 
     root = component_descriptor_v2.component
@@ -640,21 +657,22 @@
         src_ocm_repo = src_component.current_repository_ctx()
         append_ctx_repo(src_ocm_repo, component)
         append_ctx_repo(tgt_ctx_base_url, component)
 
         ocm_repository = component.current_repository_ctx()
         oci_ref = ocm_repository.component_version_oci_ref(component)
 
-        bom_resources.append(
-            BOMEntry(
-                oci_ref,
-                BOMEntryType.Docker,
-                component.name,
-            )
-        )
+        if skip_labels:
+            component.labels = [label for label in component.labels if not skip_labels(label.name)]
+
+        bom_resources.append(BOMEntry(
+            url=oci_ref,
+            type=BOMEntryType.Docker,
+            comp=component.name,
+        ))
 
     source_comp = component_descriptor_v2.component
 
     # publish the (patched) component-descriptors
     def reupload_component(component: cm.Component):
         if skip_component_upload and skip_component_upload(component):
             return
@@ -753,15 +771,19 @@
     # find the original component (yes, this is hacky / cumbersome)
     original_comp = [
         c for c in components
         if c.name == source_comp.name and c.version == source_comp.version
     ]
     if not (leng := len(original_comp)) == 1:
         if leng < 1:
-            raise RuntimeError(f'did not find {source_comp.name=} - this is a bug!')
+            logger.warning(
+                f'did not find {source_comp.name=} - probably the component filter filtered it out '
+                'or this is a bug. Will continue with the unchanged root component descriptor'
+            )
+            return component_descriptor_v2
         if leng > 1:
             raise RuntimeError(f'found more than one version of {source_comp.name=} - pbly a bug!')
 
     return dataclasses.replace(
         component_descriptor_v2,
-        component=original_comp[0],  # safe, because we check for leng above
+        component=original_comp[0], # safe, because we check for leng above
     )
```

### Comparing `gardener-cicd-libs-1.2377.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2378.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/processors.py` & `gardener-cicd-libs-1.2378.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2378.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/replicate.py` & `gardener-cicd-libs-1.2378.0/ctt/replicate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 logger = logging.getLogger(__name__)
 
 
 def replicate_oci_artifact_with_patched_component_descriptor(
     src_name: str,
     src_version: str,
-    patched_component_descriptor: gci.componentmodel.ComponentDescriptor,
+    patched_component_descriptor: cm.ComponentDescriptor,
     src_ctx_repo: cm.OciOcmRepository,
 ):
     if isinstance(src_ctx_repo, str):
-        src_ctx_repo = cm.OciRepositoryContext(baseUrl=src_ctx_repo)
+        src_ctx_repo = cm.OciOcmRepository(baseUrl=src_ctx_repo)
 
     if not isinstance(src_ctx_repo, cm.OciOcmRepository):
         raise NotImplementedError(src_ctx_repo)
 
     client = ccc.oci.oci_client()
 
     component = patched_component_descriptor.component
@@ -42,15 +42,15 @@
 
     src_ref = src_ctx_repo.component_version_oci_ref(
         name=src_name,
         version=src_version,
     )
 
     src_manifest = client.manifest(
-        image_reference=src_ref
+        image_reference=src_ref,
     )
 
     raw_fobj = gci.oci.component_descriptor_to_tarfileobj(patched_component_descriptor)
 
     cd_digest = hashlib.sha256()
     while (chunk := raw_fobj.read(4096)):
         cd_digest.update(chunk)
```

### Comparing `gardener-cicd-libs-1.2377.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2378.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2378.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2378.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2378.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2378.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2378.0/ctt/uploaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,31 +134,34 @@
         self,
         suffix,
         separator='-',
     ):
         self._suffix = suffix
         self._separator = separator
 
-    def process(self, processing_job, target_as_source=False):
-        if processing_job.resource.type is not cm.ResourceType.OCI_IMAGE:
+    def process(
+        self,
+        processing_job: pm.ProcessingJob,
+        target_as_source: bool=False,
+    ):
+        if processing_job.resource.type is not cm.ArtefactType.OCI_IMAGE:
             raise NotImplementedError
 
         if not target_as_source:
             src_ref = processing_job.resource.access.imageReference
         else:
             src_ref = processing_job.upload_request.target_ref
 
-        src_prefix, src_name, src_tag = oci.client._split_image_reference(src_ref)
+        src_ref = om.OciImageReference.to_image_ref(src_ref)
 
-        if ':' in src_tag:
+        if src_ref.has_digest_tag:
             raise RuntimeError('Cannot append tag suffix to resource that is accessed via digest')
 
-        src_name = ci.util.urljoin(src_prefix, src_name)
-        tgt_tag = self._separator.join((src_tag, self._suffix))
-        tgt_ref = ':'.join((src_name, tgt_tag))
+        tgt_tag = self._separator.join((src_ref.tag, self._suffix))
+        tgt_ref = ':'.join((src_ref.ref_without_tag, tgt_tag))
 
         upload_request = dataclasses.replace(
             processing_job.upload_request,
             source_ref=processing_job.resource.access.imageReference,
             target_ref=tgt_ref,
         )
```

### Comparing `gardener-cicd-libs-1.2377.0/ctt/util.py` & `gardener-cicd-libs-1.2378.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/delivery/client.py` & `gardener-cicd-libs-1.2378.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/delivery/model.py` & `gardener-cicd-libs-1.2378.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/delivery/util.py` & `gardener-cicd-libs-1.2378.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/dockerutil.py` & `gardener-cicd-libs-1.2378.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/dso/cvss.py` & `gardener-cicd-libs-1.2378.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/dso/labels.py` & `gardener-cicd-libs-1.2378.0/dso/labels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import dataclasses
 import enum
 import functools
 import inspect
-import typing
 import sys
 
 import dacite
 
 import gci.componentmodel as cm
 import dso.cvss
 
 
 @dataclasses.dataclass(frozen=True)
 class PathRegexes:
-    include_paths: typing.List[str] = dataclasses.field(default_factory=list)
-    exclude_paths: typing.List[str] = dataclasses.field(default_factory=list)
+    include_paths: list[str] = dataclasses.field(default_factory=list)
+    exclude_paths: list[str] = dataclasses.field(default_factory=list)
 
 
 class ScanPolicy(enum.Enum):
     SCAN = 'scan'
     SKIP = 'skip'
 
 
@@ -32,16 +31,16 @@
     name: str
     value: LabelValue
 
 
 @dataclasses.dataclass(frozen=True)
 class ScanningHint(LabelValue):
     policy: ScanPolicy
-    path_config: typing.Optional[PathRegexes]
-    comment: typing.Optional[str]
+    path_config: PathRegexes | None
+    comment: str | None
 
 
 @dataclasses.dataclass(frozen=True)
 class BinaryIdScanLabel(Label):
     name = 'cloud.gardener.cnudie/dso/scanning-hints/binary_id/v1'
     _alt_name = 'cloud.gardener.cnudie/dso/scanning-hints/binary/v1' # deprecated
     value: ScanningHint
@@ -88,14 +87,26 @@
 
 @dataclasses.dataclass(frozen=True)
 class CveCategorisationLabel(Label):
     name = 'gardener.cloud/cve-categorisation'
     value: dso.cvss.CveCategorisation
 
 
+@dataclasses.dataclass(frozen=True)
+class ExtraComponentReference:
+    component_reference: cm.ComponentIdentity
+    purpose: tuple[str] | None
+
+
+@dataclasses.dataclass(frozen=True)
+class ExtraComponentReferencesLabel(Label):
+    name = 'ocm.software/ocm-gear/extra-component-references'
+    value: tuple[ExtraComponentReference, ...]
+
+
 @functools.cache
 def _label_to_type() -> dict[str, Label]:
     own_module = sys.modules[__name__]
     types = tuple(t for entry
         in inspect.getmembers(own_module, inspect.isclass)
         if (t := entry[1]) != Label and issubclass(t, Label)
     )
@@ -121,10 +132,10 @@
             'value': label.value,
         }
 
     return dacite.from_dict(
         data_class=t,
         data=label,
         config=dacite.Config(
-            cast=(tuple, enum.Enum)
+            cast=[tuple, enum.Enum],
         ),
     )
```

### Comparing `gardener-cicd-libs-1.2377.0/dso/model.py` & `gardener-cicd-libs-1.2378.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/PKG-INFO` & `gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gardener-cicd-libs
-Version: 1.2377.0
+Version: 1.2378.0
 Summary: Gardener CI/CD Libraries
 Requires-Python: >=3.10
 License-File: LICENSE
-Requires-Dist: gardener-cicd-base>=1.2377.0
-Requires-Dist: gardener-oci>=1.2377.0
+Requires-Dist: gardener-cicd-base>=1.2378.0
+Requires-Dist: gardener-oci>=1.2378.0
 Requires-Dist: GitPython
 Requires-Dist: Mako<2.0.0
 Requires-Dist: Sphinx
 Requires-Dist: aliyun-python-sdk-core==2.15.0
 Requires-Dist: aliyun-python-sdk-ecs==4.24.71
 Requires-Dist: aliyun-python-sdk-ram==3.3.0
 Requires-Dist: awesomeversion
```

### Comparing `gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2378.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gardener-cicd-base>=1.2377.0
-gardener-oci>=1.2377.0
+gardener-cicd-base>=1.2378.0
+gardener-oci>=1.2378.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.15.0
 aliyun-python-sdk-ecs==4.24.71
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
```

### Comparing `gardener-cicd-libs-1.2377.0/gci/component-descriptor-v2-schema.yaml` & `gardener-cicd-libs-1.2378.0/gci/component-descriptor-v2-schema.yaml`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gci/componentmodel.py` & `gardener-cicd-libs-1.2378.0/gci/componentmodel.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gci/oci.py` & `gardener-cicd-libs-1.2378.0/gci/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/codeowners.py` & `gardener-cicd-libs-1.2378.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2378.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2378.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/compliance/model.py` & `gardener-cicd-libs-1.2378.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/compliance/report.py` & `gardener-cicd-libs-1.2378.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/retry.py` & `gardener-cicd-libs-1.2378.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/user.py` & `gardener-cicd-libs-1.2378.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/util.py` & `gardener-cicd-libs-1.2378.0/github/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/github/webhook.py` & `gardener-cicd-libs-1.2378.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gitutil.py` & `gardener-cicd-libs-1.2378.0/gitutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/gziputil.py` & `gardener-cicd-libs-1.2378.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/http_requests.py` & `gardener-cicd-libs-1.2378.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2378.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/mailutil.py` & `gardener-cicd-libs-1.2378.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2378.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2378.0/release_notes/fetch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/release_notes/markdown.py` & `gardener-cicd-libs-1.2378.0/release_notes/markdown.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/release_notes/model.py` & `gardener-cicd-libs-1.2378.0/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/release_notes/utils.py` & `gardener-cicd-libs-1.2378.0/release_notes/utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/reutil.py` & `gardener-cicd-libs-1.2378.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/setup.py` & `gardener-cicd-libs-1.2378.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/slackclient/util.py` & `gardener-cicd-libs-1.2378.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/tarutil.py` & `gardener-cicd-libs-1.2378.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/__init__.py` & `gardener-cicd-libs-1.2378.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/_test_utils.py` & `gardener-cicd-libs-1.2378.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/traits/filter_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 import gci.componentmodel as cm
 
 import concourse.model.traits.filter as examinee
 import cnudie.iter
 
 
-def component(name='TestComponent', version='1.2.3', resources=()):
-    return cm.Component(
-        name=name,
-        version=version,
-        repositoryContexts=(),
-        provider=None,
-        sources=resources,
-        resources=(),
-        componentReferences=(),
+def node_path_entry(name='TestComponent', version='1.2.3', resources=()):
+    return cnudie.iter.NodePathEntry(
+        component=cm.Component(
+            name=name,
+            version=version,
+            repositoryContexts=(),
+            provider=None,
+            sources=resources,
+            resources=(),
+            componentReferences=(),
+        ),
     )
 
 
 def resource(name='resourceName', version='1.2.3'):
     return cm.Resource(
         name=name,
         version=version,
@@ -56,21 +58,21 @@
             )
         ]
     )
     test_filter = examinee.filter_for_matching_config(test_config)
 
     assert test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(),
+            node_path_entry(),
         ))
     )
 
     assert not test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='unknown-component'),
+            node_path_entry(name='unknown-component'),
         )
     ))
 
 
 def test_component_attr_excluded():
     test_config = examinee.MatchingConfig(
         name='Some Config Name',
@@ -82,21 +84,21 @@
             )
         ]
     )
     test_filter = examinee.filter_for_matching_config(test_config)
 
     assert test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='excluded-component'),
+            node_path_entry(name='excluded-component'),
         )
     ))
 
     assert not test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='TestComponent'),
+            node_path_entry(name='TestComponent'),
         )
     ))
 
 
 def test_resource_attr_included():
     test_config = examinee.MatchingConfig(
         name='Some Config Name',
@@ -166,27 +168,27 @@
             )
         ]
     )
     test_filter = examinee.filter_for_matching_config(test_config)
 
     assert not test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='AName'),
+            node_path_entry(name='AName'),
         )
     ))
 
     assert not test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='AnotherName'),
+            node_path_entry(name='AnotherName'),
         )
     ))
 
     assert not test_filter(
         cnudie.iter.ComponentNode(path=(
-            component(name='YetAnotherName'),
+            node_path_entry(name='YetAnotherName'),
         )
     ))
 
 
 def test_multiple_resource_rules():
     test_config = examinee.MatchingConfig(
         name='Some Config Name',
@@ -249,27 +251,27 @@
         ),
     ]
     test_filter = examinee.filter_for_matching_configs(test_configs)
 
     assert test_filter(
         cnudie.iter.ResourceNode(
             path=(
-                component(name='ComponentName'),
+                node_path_entry(name='ComponentName'),
             ),
             resource=resource(name='YetAnotherName'),
     ))
 
     assert test_filter(
         cnudie.iter.ResourceNode(
             path=(
-                component(name='ComponentName'),
+                node_path_entry(name='ComponentName'),
             ),
             resource=resource(name='AnotherResource'),
     ))
 
     assert test_filter(
         cnudie.iter.ResourceNode(
             path=(
-                component(name='another-component'),
+                node_path_entry(name='another-component'),
             ),
             resource=resource(name='ResourceName'),
     ))
```

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2378.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/release_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2378.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2378.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/gitutil_test.py` & `gardener-cicd-libs-1.2378.0/test/gitutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/reutil_test.py` & `gardener-cicd-libs-1.2378.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/test/version_test.py` & `gardener-cicd-libs-1.2378.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/unixutil/model.py` & `gardener-cicd-libs-1.2378.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/unixutil/scan.py` & `gardener-cicd-libs-1.2378.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2377.0/version.py` & `gardener-cicd-libs-1.2378.0/version.py`

 * *Files identical despite different names*

