# Comparing `tmp/sirmordred-0.9.3rc1.tar.gz` & `tmp/sirmordred-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirmordred-0.9.3rc1.tar", max compression
+gzip compressed data, was "sirmordred-1.0.0rc1.tar", max compression
```

## Comparing `sirmordred-0.9.3rc1.tar` & `sirmordred-1.0.0rc1.tar`

### file list

```diff
@@ -1,96 +1,98 @@
--rw-r--r--   0        0        0    35147 2023-08-06 17:52:49.136124 sirmordred-0.9.3rc1/LICENSE
--rw-r--r--   0        0        0    40852 2023-08-06 17:52:49.140124 sirmordred-0.9.3rc1/README.md
--rw-r--r--   0        0        0     8246 2023-08-06 17:52:49.140124 sirmordred-0.9.3rc1/menu.yaml
--rw-r--r--   0        0        0     2171 2023-08-06 17:52:49.140124 sirmordred-0.9.3rc1/pyproject.toml
--rw-r--r--   0        0        0      835 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/__init__.py
--rw-r--r--   0        0        0       91 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/_version.py
--rwxr-xr-x   0        0        0     4924 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/bin/sirmordred.py
--rw-r--r--   0        0        0    33508 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/config.py
--rw-r--r--   0        0        0     1836 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/error.py
--rw-r--r--   0        0        0     2306 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/github.py
--rwxr-xr-x   0        0        0    12672 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/sirmordred.py
--rw-r--r--   0        0        0     9833 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task.py
--rw-r--r--   0        0        0     6487 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_collection.py
--rw-r--r--   0        0        0    20942 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_enrich.py
--rw-r--r--   0        0        0     3396 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_identities.py
--rw-r--r--   0        0        0     4424 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_manager.py
--rw-r--r--   0        0        0    29060 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_panels.py
--rw-r--r--   0        0        0     6484 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/task_projects.py
--rw-r--r--   0        0        0     1981 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/find_affiliation_conflicts.py
--rw-r--r--   0        0        0      766 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/grimoirelab_valid.yml
--rwxr-xr-x   0        0        0     4709 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/healthcheck.py
--rw-r--r--   0        0        0        0 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/logs/all.log
--rw-r--r--   0        0        0     7846 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/micro.py
--rw-r--r--   0        0        0     2858 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/panels_config.py
--rw-r--r--   0        0        0      864 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/projects.json
--rw-r--r--   0        0        0     3141 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/projects_json2yml.py
--rw-r--r--   0        0        0     3634 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/sirmordred/utils/setup.cfg
--rw-r--r--   0        0        0     4398 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/tests/aliases.json
--rw-r--r--   0        0        0   497664 2023-08-06 17:52:49.148124 sirmordred-0.9.3rc1/tests/archives/askbot.archive
--rw-r--r--   0        0        0   150528 2023-08-06 17:52:49.148124 sirmordred-0.9.3rc1/tests/archives/bugzilla.archive
--rw-r--r--   0        0        0    52224 2023-08-06 17:52:49.148124 sirmordred-0.9.3rc1/tests/archives/bugzillarest.archive
--rw-r--r--   0        0        0    73728 2023-08-06 17:52:49.148124 sirmordred-0.9.3rc1/tests/archives/confluence.archive
--rw-r--r--   0        0        0  7141376 2023-08-06 17:52:49.172124 sirmordred-0.9.3rc1/tests/archives/crates.archive
--rw-r--r--   0        0        0   291840 2023-08-06 17:52:49.176124 sirmordred-0.9.3rc1/tests/archives/discourse.archive
--rw-r--r--   0        0        0    16384 2023-08-06 17:52:49.176124 sirmordred-0.9.3rc1/tests/archives/dockerhub.archive
--rw-r--r--   0        0        0  1713152 2023-08-06 17:52:49.180124 sirmordred-0.9.3rc1/tests/archives/functest.archive
--rw-r--r--   0        0        0    49152 2023-08-06 17:52:49.184125 sirmordred-0.9.3rc1/tests/archives/gerrit.archive
--rw-r--r--   0        0        0  9424896 2023-08-06 17:52:49.260125 sirmordred-0.9.3rc1/tests/archives/github-issue.archive
--rw-r--r--   0        0        0 23023616 2023-08-06 17:52:49.296126 sirmordred-0.9.3rc1/tests/archives/github-pull.archive
--rw-r--r--   0        0        0   208896 2023-08-06 17:52:49.296126 sirmordred-0.9.3rc1/tests/archives/gitlab-issue.archive
--rw-r--r--   0        0        0   937984 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/gitlab-merge.archive
--rw-r--r--   0        0        0    65536 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/googlehits.archive
--rw-r--r--   0        0        0   228352 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/jenkins.archive
--rw-r--r--   0        0        0    86016 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/jira.archive
--rw-r--r--   0        0        0    69632 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/launchpad.archive
--rw-r--r--   0        0        0    31744 2023-08-06 17:52:49.300126 sirmordred-0.9.3rc1/tests/archives/mediawiki-1.23.archive
--rw-r--r--   0        0        0   245760 2023-08-06 17:52:49.304126 sirmordred-0.9.3rc1/tests/archives/mediawiki-1.28.archive
--rw-r--r--   0        0        0   136192 2023-08-06 17:52:49.304126 sirmordred-0.9.3rc1/tests/archives/meetup.archive
--rw-r--r--   0        0        0  2310144 2023-08-06 17:52:49.308126 sirmordred-0.9.3rc1/tests/archives/mozillaclub.archive
--rw-r--r--   0        0        0    35840 2023-08-06 17:52:49.308126 sirmordred-0.9.3rc1/tests/archives/nntp.archive
--rw-r--r--   0        0        0    88064 2023-08-06 17:52:49.308126 sirmordred-0.9.3rc1/tests/archives/phabricator.archive
--rw-r--r--   0        0        0    61440 2023-08-06 17:52:49.308126 sirmordred-0.9.3rc1/tests/archives/redmine.archive
--rw-r--r--   0        0        0   182272 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/remo.archive
--rw-r--r--   0        0        0    25600 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/rss.archive
--rw-r--r--   0        0        0    86016 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/slack.archive
--rw-r--r--   0        0        0    17408 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/stackexchange.archive
--rw-r--r--   0        0        0    15360 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/telegram.archive
--rw-r--r--   0        0        0   385024 2023-08-06 17:52:49.312126 sirmordred-0.9.3rc1/tests/archives/twitter.archive
--rw-r--r--   0        0        0     1769 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/tests/archives-test-projects.json
--rw-r--r--   0        0        0     5845 2023-08-06 17:52:49.144124 sirmordred-0.9.3rc1/tests/archives-test.cfg
--rw-r--r--   0        0        0 15031534 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/eclipse-projects.json
--rw-r--r--   0        0        0       55 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/healthcheck_cache_invalid.json
--rw-r--r--   0        0        0       56 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/healthcheck_cache_valid.json
--rw-r--r--   0        0        0       56 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/healthcheck_cache_wrong_key.json
--rw-r--r--   0        0        0     2932 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/mordred.log
--rw-r--r--   0        0        0     3244 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/orgs_sortinghat.json
--rw-r--r--   0        0        0     3587 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/perceval_identities_sortinghat.json
--rw-r--r--   0        0        0     3607 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/remote_identities_sortinghat.json
--rw-r--r--   0        0        0     2032 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/task-identities-data.json
--rw-r--r--   0        0        0     4487 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/task-params-expected
--rw-r--r--   0        0        0     1716 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/task-params-test-projects.json
--rw-r--r--   0        0        0     4392 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/task-params-test.cfg
--rw-r--r--   0        0        0     2484 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/data/url-projects.json
--rwxr-xr-x   0        0        0     1166 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/run_tests.py
--rw-r--r--   0        0        0     6562 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/sortinghat_settings.py
--rw-r--r--   0        0        0     1451 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/test-no-collection.cfg
--rw-r--r--   0        0        0     4655 2023-08-06 17:52:49.364127 sirmordred-0.9.3rc1/tests/test-no-sh.cfg
--rw-r--r--   0        0        0      178 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test-projects-no-collection.json
--rw-r--r--   0        0        0     2484 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test-projects.json
--rw-r--r--   0        0        0      721 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test-repos-projects.json
--rw-r--r--   0        0        0     1798 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test-repos.cfg
--rw-r--r--   0        0        0     4936 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test.cfg
--rw-r--r--   0        0        0    14731 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_config.py
--rw-r--r--   0        0        0     1849 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_github.py
--rw-r--r--   0        0        0     3235 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_healthcheck.py
--rw-r--r--   0        0        0     2706 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_sirmordred.py
--rw-r--r--   0        0        0     7303 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_studies.cfg
--rw-r--r--   0        0        0     5392 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task.py
--rw-r--r--   0        0        0     5956 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_collection.py
--rw-r--r--   0        0        0    11770 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_enrich.py
--rw-r--r--   0        0        0     5817 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_identities.py
--rw-r--r--   0        0        0    10141 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_manager.py
--rw-r--r--   0        0        0     6380 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_panels.py
--rw-r--r--   0        0        0    13869 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_task_projects.py
--rw-r--r--   0        0        0     1499 2023-08-06 17:52:49.368127 sirmordred-0.9.3rc1/tests/test_wrong.cfg
--rw-r--r--   0        0        0    42445 1970-01-01 00:00:00.000000 sirmordred-0.9.3rc1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-04-10 08:05:13.394938 sirmordred-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    40852 2024-04-10 08:05:13.394938 sirmordred-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     8246 2024-04-10 08:05:13.394938 sirmordred-1.0.0rc1/menu.yaml
+-rw-r--r--   0        0        0     2182 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      835 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/_version.py
+-rwxr-xr-x   0        0        0     5022 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/bin/sirmordred.py
+-rw-r--r--   0        0        0    33508 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/config.py
+-rw-r--r--   0        0        0     1836 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/error.py
+-rw-r--r--   0        0        0     2306 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/github.py
+-rwxr-xr-x   0        0        0    12432 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/sirmordred.py
+-rw-r--r--   0        0        0    10093 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task.py
+-rw-r--r--   0        0        0     7762 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_autorefresh.py
+-rw-r--r--   0        0        0     6487 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_collection.py
+-rw-r--r--   0        0        0    21143 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_enrich.py
+-rw-r--r--   0        0        0     3396 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_identities.py
+-rw-r--r--   0        0        0     4424 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_manager.py
+-rw-r--r--   0        0        0    29060 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_panels.py
+-rw-r--r--   0        0        0     6484 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/task_projects.py
+-rw-r--r--   0        0        0     1981 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/find_affiliation_conflicts.py
+-rw-r--r--   0        0        0      766 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/grimoirelab_valid.yml
+-rwxr-xr-x   0        0        0     4709 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/healthcheck.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/logs/all.log
+-rw-r--r--   0        0        0     7849 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/micro.py
+-rw-r--r--   0        0        0     2858 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/panels_config.py
+-rw-r--r--   0        0        0      864 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/projects.json
+-rw-r--r--   0        0        0     3141 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/projects_json2yml.py
+-rw-r--r--   0        0        0     3634 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/sirmordred/utils/setup.cfg
+-rw-r--r--   0        0        0     4398 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/tests/aliases.json
+-rw-r--r--   0        0        0   497664 2024-04-10 08:05:13.402938 sirmordred-1.0.0rc1/tests/archives/askbot.archive
+-rw-r--r--   0        0        0   150528 2024-04-10 08:05:13.402938 sirmordred-1.0.0rc1/tests/archives/bugzilla.archive
+-rw-r--r--   0        0        0    52224 2024-04-10 08:05:13.402938 sirmordred-1.0.0rc1/tests/archives/bugzillarest.archive
+-rw-r--r--   0        0        0    73728 2024-04-10 08:05:13.402938 sirmordred-1.0.0rc1/tests/archives/confluence.archive
+-rw-r--r--   0        0        0  7141376 2024-04-10 08:05:13.422938 sirmordred-1.0.0rc1/tests/archives/crates.archive
+-rw-r--r--   0        0        0   291840 2024-04-10 08:05:13.422938 sirmordred-1.0.0rc1/tests/archives/discourse.archive
+-rw-r--r--   0        0        0    16384 2024-04-10 08:05:13.422938 sirmordred-1.0.0rc1/tests/archives/dockerhub.archive
+-rw-r--r--   0        0        0  1713152 2024-04-10 08:05:13.426938 sirmordred-1.0.0rc1/tests/archives/functest.archive
+-rw-r--r--   0        0        0    49152 2024-04-10 08:05:13.426938 sirmordred-1.0.0rc1/tests/archives/gerrit.archive
+-rw-r--r--   0        0        0  9424896 2024-04-10 08:05:13.482938 sirmordred-1.0.0rc1/tests/archives/github-issue.archive
+-rw-r--r--   0        0        0 23023616 2024-04-10 08:05:13.510938 sirmordred-1.0.0rc1/tests/archives/github-pull.archive
+-rw-r--r--   0        0        0   208896 2024-04-10 08:05:13.510938 sirmordred-1.0.0rc1/tests/archives/gitlab-issue.archive
+-rw-r--r--   0        0        0   937984 2024-04-10 08:05:13.510938 sirmordred-1.0.0rc1/tests/archives/gitlab-merge.archive
+-rw-r--r--   0        0        0    65536 2024-04-10 08:05:13.510938 sirmordred-1.0.0rc1/tests/archives/googlehits.archive
+-rw-r--r--   0        0        0   228352 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/jenkins.archive
+-rw-r--r--   0        0        0    86016 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/jira.archive
+-rw-r--r--   0        0        0    69632 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/launchpad.archive
+-rw-r--r--   0        0        0    31744 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/mediawiki-1.23.archive
+-rw-r--r--   0        0        0   245760 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/mediawiki-1.28.archive
+-rw-r--r--   0        0        0   136192 2024-04-10 08:05:13.514938 sirmordred-1.0.0rc1/tests/archives/meetup.archive
+-rw-r--r--   0        0        0  2310144 2024-04-10 08:05:13.518938 sirmordred-1.0.0rc1/tests/archives/mozillaclub.archive
+-rw-r--r--   0        0        0    35840 2024-04-10 08:05:13.518938 sirmordred-1.0.0rc1/tests/archives/nntp.archive
+-rw-r--r--   0        0        0    88064 2024-04-10 08:05:13.518938 sirmordred-1.0.0rc1/tests/archives/phabricator.archive
+-rw-r--r--   0        0        0    61440 2024-04-10 08:05:13.518938 sirmordred-1.0.0rc1/tests/archives/redmine.archive
+-rw-r--r--   0        0        0   182272 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/remo.archive
+-rw-r--r--   0        0        0    25600 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/rss.archive
+-rw-r--r--   0        0        0    86016 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/slack.archive
+-rw-r--r--   0        0        0    17408 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/stackexchange.archive
+-rw-r--r--   0        0        0    15360 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/telegram.archive
+-rw-r--r--   0        0        0   385024 2024-04-10 08:05:13.522938 sirmordred-1.0.0rc1/tests/archives/twitter.archive
+-rw-r--r--   0        0        0     1769 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/tests/archives-test-projects.json
+-rw-r--r--   0        0        0     5845 2024-04-10 08:05:13.398938 sirmordred-1.0.0rc1/tests/archives-test.cfg
+-rw-r--r--   0        0        0 15031534 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/eclipse-projects.json
+-rw-r--r--   0        0        0       55 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/healthcheck_cache_invalid.json
+-rw-r--r--   0        0        0       56 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/healthcheck_cache_valid.json
+-rw-r--r--   0        0        0       56 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/healthcheck_cache_wrong_key.json
+-rw-r--r--   0        0        0     2932 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/mordred.log
+-rw-r--r--   0        0        0     3244 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/orgs_sortinghat.json
+-rw-r--r--   0        0        0     3587 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/perceval_identities_sortinghat.json
+-rw-r--r--   0        0        0     3607 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/remote_identities_sortinghat.json
+-rw-r--r--   0        0        0     2032 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0     4487 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/task-params-expected
+-rw-r--r--   0        0        0     1716 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/task-params-test-projects.json
+-rw-r--r--   0        0        0     4392 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/task-params-test.cfg
+-rw-r--r--   0        0        0     2484 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/data/url-projects.json
+-rwxr-xr-x   0        0        0     1166 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     6585 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/sortinghat_settings.py
+-rw-r--r--   0        0        0     1451 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-no-collection.cfg
+-rw-r--r--   0        0        0     4655 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-no-sh.cfg
+-rw-r--r--   0        0        0      178 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-projects-no-collection.json
+-rw-r--r--   0        0        0     2484 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-projects.json
+-rw-r--r--   0        0        0      721 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-repos-projects.json
+-rw-r--r--   0        0        0     1798 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test-repos.cfg
+-rw-r--r--   0        0        0     4936 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test.cfg
+-rw-r--r--   0        0        0    14731 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_config.py
+-rw-r--r--   0        0        0     1849 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_github.py
+-rw-r--r--   0        0        0     3235 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_healthcheck.py
+-rw-r--r--   0        0        0     2706 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_sirmordred.py
+-rw-r--r--   0        0        0     7303 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_studies.cfg
+-rw-r--r--   0        0        0     5392 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_task.py
+-rw-r--r--   0        0        0     6715 2024-04-10 08:05:13.562938 sirmordred-1.0.0rc1/tests/test_task_autorefresh.py
+-rw-r--r--   0        0        0     5956 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_collection.py
+-rw-r--r--   0        0        0    11770 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_enrich.py
+-rw-r--r--   0        0        0     5817 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_identities.py
+-rw-r--r--   0        0        0    10141 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_manager.py
+-rw-r--r--   0        0        0     6380 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_panels.py
+-rw-r--r--   0        0        0    13869 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_task_projects.py
+-rw-r--r--   0        0        0     1499 2024-04-10 08:05:13.566938 sirmordred-1.0.0rc1/tests/test_wrong.cfg
+-rw-r--r--   0        0        0    42454 1970-01-01 00:00:00.000000 sirmordred-1.0.0rc1/PKG-INFO
```

### Comparing `sirmordred-0.9.3rc1/LICENSE` & `sirmordred-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/README.md` & `sirmordred-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/menu.yaml` & `sirmordred-1.0.0rc1/menu.yaml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/pyproject.toml` & `sirmordred-1.0.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sirmordred"
-version = "0.9.3-rc.1"
+version = "1.0.0-rc.1"
 description = "Drive GrimoireLab tools to produce a dashboard"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -19,15 +19,15 @@
 
 packages = [
     { include = "sirmordred" },
     { include = "tests", format = "sdist" },
 ]
 
 classifiers = [
-   "Development Status :: 4 - Beta",
+   "Development Status :: 5 - Production/Stable",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Topic :: Software Development",
    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
    "Programming Language :: Python :: 3"
 ]
 
@@ -37,15 +37,15 @@
 [tool.poetry.scripts]
 'sirmordred' = 'sirmordred.bin.sirmordred:main'
 'healthcheck.py' = 'sirmordred.utils.healthcheck:main'
 'micro.py' = 'sirmordred.utils.micro:main'
 'panels_config.py' = 'sirmordred.utils.panels_config:main'
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = "^3.8"
 
 colorlog = "4.1.0"
 elasticsearch = "6.3.1"
 elasticsearch-dsl = "6.3.1"
 file-read-backwards = "2.0.0"
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 sortinghat = { version = ">=0.7.20", allow-prereleases = true}
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/__init__.py` & `sirmordred-1.0.0rc1/sirmordred/__init__.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/bin/sirmordred.py` & `sirmordred-1.0.0rc1/sirmordred/bin/sirmordred.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         return 1
 
     try:
         config = Config(args.config_files[0], args.config_files[1:])
         config_dict = config.get_conf()
         logs_dir = config_dict['general'].get('logs_dir', None)
         debug_mode = config_dict['general']['debug']
-        logger = setup_logs(logs_dir, debug_mode)
+        short_name = config_dict['general']['short_name']
+        logger = setup_logs(logs_dir, debug_mode, short_name)
     except RuntimeError as error:
         print("Error while consuming configuration: {}".format(error))
         return 1
 
     if args.phases:
         logger.info("Executing sirmordred for phases: {}".format(args.phases))
         # HACK: the internal dict of Config is modified directly
@@ -74,26 +75,26 @@
         config_dict['general']['update'] = False
         for phase in config_dict['phases']:
             config_dict['phases'][phase] = True if phase in args.phases else False
 
     SirMordred(config).start()
 
 
-def setup_logs(logs_dir, debug_mode):
+def setup_logs(logs_dir, debug_mode, short_name):
 
     if debug_mode:
         logging_mode = logging.DEBUG
     else:
         logging_mode = logging.INFO
 
     logger = logging.getLogger()
     logger.setLevel(logging_mode)
 
     # create formatter and add it to the handlers
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    formatter = logging.Formatter(f'%(asctime)s - {short_name} - %(name)s - %(levelname)s - %(message)s')
 
     # create file handler
     if logs_dir:
         fh_filepath = os.path.join(logs_dir, 'all.log')
         fh = logging.FileHandler(fh_filepath)
         fh.setLevel(logging_mode)
         # Set format
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/config.py` & `sirmordred-1.0.0rc1/sirmordred/config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/error.py` & `sirmordred-1.0.0rc1/sirmordred/error.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/github.py` & `sirmordred-1.0.0rc1/sirmordred/github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/sirmordred.py` & `sirmordred-1.0.0rc1/sirmordred/sirmordred.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 warnings.filterwarnings("ignore", message="numpy.ufunc size changed")
 
 from grimoire_elk.enriched.utils import grimoire_con
 
 from sirmordred.config import Config
 from sirmordred.error import DataCollectionError
 from sirmordred.error import DataEnrichmentError
+from sirmordred.task_autorefresh import TaskAutorefresh
 from sirmordred.task_collection import TaskRawDataCollection
 from sirmordred.task_enrich import TaskEnrich
 from sirmordred.task_identities import TaskIdentitiesMerge
 from sirmordred.task_manager import TasksManager
 from sirmordred.task_panels import TaskPanels, TaskPanelsMenu
 from sirmordred.task_projects import TaskProjects
 
@@ -293,22 +294,18 @@
 
         # Tasks to be executed during updating process
         all_tasks_cls = []
         all_tasks_cls.append(TaskProjects)  # projects update is always needed
         if self.conf['phases']['collection']:
             all_tasks_cls.append(TaskRawDataCollection)
         if self.conf['phases']['identities']:
-            # load identities and orgs periodically for updates
-            # all_tasks_cls.append(TaskIdentitiesLoad) Not supported on the new sortinghat graphQL
             all_tasks_cls.append(TaskIdentitiesMerge)
-            # This is done in enrichement before doing the enrich
-            # if self.conf['phases']['collection']:
-            #     all_tasks_cls.append(TaskIdentitiesCollection)
         if self.conf['phases']['enrichment']:
             all_tasks_cls.append(TaskEnrich)
+            all_tasks_cls.append(TaskAutorefresh)
 
         # this is the main loop, where the execution should spend
         # most of its time
 
         while True:
 
             if not all_tasks_cls:
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/task.py` & `sirmordred-1.0.0rc1/sirmordred/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,16 +183,18 @@
         json_projects_map = None
         clean = False
         connector = get_connector_from_name(self.get_backend(self.backend_section))
 
         if 'projects_file' in self.conf['projects']:
             json_projects_map = self.conf['projects']['projects_file']
 
-        enrich_backend = connector[2](self.db_sh, json_projects_map,
-                                      self.db_user, self.db_password, self.db_host)
+        enrich_backend = connector[2](db_sortinghat=self.db_sh, json_projects_map=json_projects_map,
+                                      db_user=self.db_user, db_password=self.db_password, db_host=self.db_host,
+                                      db_port=self.db_port, db_path=self.db_path, db_ssl=self.db_ssl,
+                                      db_verify_ssl=self.db_verify_ssl, db_tenant=self.db_tenant)
         elastic_enrich = get_elastic(self.conf['es_enrichment']['url'],
                                      self.conf[self.backend_section]['enriched_index'],
                                      clean, enrich_backend)
         enrich_backend.set_elastic(elastic_enrich)
         if 'pair-programming' in self.conf[self.backend_section]:
             enrich_backend.pair_programming = self.conf[self.backend_section]['pair-programming']
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_collection.py` & `sirmordred-1.0.0rc1/sirmordred/task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_enrich.py` & `sirmordred-1.0.0rc1/sirmordred/task_enrich.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,16 +298,18 @@
         if not es.indices.exists(index=aoc_index):
             logger.debug("Not doing autorefresh, index doesn't exist for Areas of Code study")
             return
 
         logger.debug("Doing autorefresh for Areas of Code study")
 
         # Create a GitEnrich backend tweaked to work with AOC index
-        aoc_backend = GitEnrich(self.db_sh, cfg['projects']['projects_file'],
-                                self.db_user, self.db_password, self.db_host)
+        aoc_backend = GitEnrich(db_sortinghat=self.db_sh, json_projects_map=cfg['projects']['projects_file'],
+                                db_user=self.db_user, db_password=self.db_password, db_host=self.db_host,
+                                db_port=self.db_port, db_path=self.db_path, db_ssl=self.db_ssl,
+                                db_verify_ssl=self.db_verify_ssl, db_tenant=self.db_tenant)
         aoc_backend.mapping = None
         aoc_backend.roles = ['author']
         elastic_enrich = get_elastic(self.conf['es_enrichment']['url'],
                                      aoc_index, clean=False, backend=aoc_backend)
         aoc_backend.set_elastic(elastic_enrich)
 
         self.__autorefresh(aoc_backend, studies=True)
@@ -436,15 +438,14 @@
                 self.retain_identities(retention_time)
                 logger.info('[%s] identities retention end', self.backend_section)
 
             autorefresh = cfg['es_enrichment']['autorefresh']
 
             if autorefresh and self.db:
                 logger.info('[%s] autorefresh start', self.backend_section)
-                a = self._get_enrich_backend()
                 self.__autorefresh(self._get_enrich_backend())
                 logger.info('[%s] autorefresh end', self.backend_section)
             else:
                 logger.info('[%s] autorefresh not active', self.backend_section)
 
             self.__studies(retention_time)
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_identities.py` & `sirmordred-1.0.0rc1/sirmordred/task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_manager.py` & `sirmordred-1.0.0rc1/sirmordred/task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_panels.py` & `sirmordred-1.0.0rc1/sirmordred/task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/task_projects.py` & `sirmordred-1.0.0rc1/sirmordred/task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/find_affiliation_conflicts.py` & `sirmordred-1.0.0rc1/sirmordred/utils/find_affiliation_conflicts.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/grimoirelab_valid.yml` & `sirmordred-1.0.0rc1/sirmordred/utils/grimoirelab_valid.yml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/healthcheck.py` & `sirmordred-1.0.0rc1/sirmordred/utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/micro.py` & `sirmordred-1.0.0rc1/sirmordred/utils/micro.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,44 +30,42 @@
 from sirmordred.config import Config
 from sirmordred.task_collection import TaskRawDataCollection
 from sirmordred.task_identities import TaskIdentitiesMerge
 from sirmordred.task_enrich import TaskEnrich
 from sirmordred.task_panels import TaskPanels, TaskPanelsMenu
 from sirmordred.task_projects import TaskProjects
 
-DEBUG_LOG_FORMAT = "[%(asctime)s - %(name)s - %(levelname)s] - %(message)s"
-INFO_LOG_FORMAT = "%(asctime)s %(message)s"
 COLOR_LOG_FORMAT_SUFFIX = "\033[1m %(log_color)s "
 LOG_COLORS = {'DEBUG': 'white', 'INFO': 'cyan', 'WARNING': 'yellow', 'ERROR': 'red', 'CRITICAL': 'red,bg_white'}
 
 
 def main():
     args = get_params()
-    config_logging(args.debug, args.logs_dir)
-    micro_mordred(args.cfg_path, args.backend_sections,
+    config = Config(args.cfg_path)
+    short_name = config['general']['short_name']
+    config_logging(args.debug, args.logs_dir, short_name)
+    micro_mordred(config, args.backend_sections,
                   args.repos_to_check, args.raw,
                   args.identities_merge,
                   args.enrich,
                   args.panels)
 
 
-def micro_mordred(cfg_path, backend_sections, repos_to_check, raw, identities_merge, enrich, panels):
-    """Execute the Mordred tasks using the configuration file (`cfg_path`).
+def micro_mordred(config, backend_sections, repos_to_check, raw, identities_merge, enrich, panels):
+    """Execute the Mordred tasks using the configuration file.
 
-    :param cfg_path: the path of a Mordred configuration file
+    :param config: Mordred configuration file
     :param backend_sections: the backend sections where the raw/enrich/identities phases will be executed
     :param repos_to_check: process a repository only if it is in this list, or `None` for all repos
     :param raw: if true, it activates the collection of raw data
     :param identities_merge: if true, it activates the identities merging process
     :param enrich: if true, it activates the enrichment of the raw data
     :param panels: if true, it activates the upload of all panels declared in the configuration file
     """
 
-    config = Config(cfg_path)
-
     if raw:
         for backend in backend_sections:
             get_raw(config, backend, repos_to_check)
 
     if identities_merge:
         get_identities_merge(config)
 
@@ -141,22 +139,22 @@
 
     task = TaskPanelsMenu(config)
     task.execute()
 
     logging.info("Panels creation finished!")
 
 
-def config_logging(debug, logs_dir):
+def config_logging(debug, logs_dir, short_name):
     """Config logging level output output"""
 
     if debug:
-        fmt = DEBUG_LOG_FORMAT
+        fmt = f"[%(asctime)s - {short_name} - %(name)s - %(levelname)s] - %(message)s"
         logging_mode = logging.DEBUG
     else:
-        fmt = INFO_LOG_FORMAT
+        fmt = f"%(asctime)s - {short_name} - %(message)s"
         logging_mode = logging.INFO
 
     # Setting the color scheme and level into the root logger
     logging.basicConfig(level=logging_mode)
     stream = logging.root.handlers[0]
     formatter = colorlog.ColoredFormatter(fmt=COLOR_LOG_FORMAT_SUFFIX + fmt,
                                           log_colors=LOG_COLORS)
```

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/panels_config.py` & `sirmordred-1.0.0rc1/sirmordred/utils/panels_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/projects.json` & `sirmordred-1.0.0rc1/sirmordred/utils/projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/projects_json2yml.py` & `sirmordred-1.0.0rc1/sirmordred/utils/projects_json2yml.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/sirmordred/utils/setup.cfg` & `sirmordred-1.0.0rc1/sirmordred/utils/setup.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/aliases.json` & `sirmordred-1.0.0rc1/tests/aliases.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/askbot.archive` & `sirmordred-1.0.0rc1/tests/archives/askbot.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/bugzilla.archive` & `sirmordred-1.0.0rc1/tests/archives/bugzilla.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/bugzillarest.archive` & `sirmordred-1.0.0rc1/tests/archives/bugzillarest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/confluence.archive` & `sirmordred-1.0.0rc1/tests/archives/confluence.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/crates.archive` & `sirmordred-1.0.0rc1/tests/archives/crates.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/discourse.archive` & `sirmordred-1.0.0rc1/tests/archives/discourse.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/dockerhub.archive` & `sirmordred-1.0.0rc1/tests/archives/dockerhub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/functest.archive` & `sirmordred-1.0.0rc1/tests/archives/functest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/gerrit.archive` & `sirmordred-1.0.0rc1/tests/archives/gerrit.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/github-issue.archive` & `sirmordred-1.0.0rc1/tests/archives/github-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/github-pull.archive` & `sirmordred-1.0.0rc1/tests/archives/github-pull.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/gitlab-issue.archive` & `sirmordred-1.0.0rc1/tests/archives/gitlab-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/gitlab-merge.archive` & `sirmordred-1.0.0rc1/tests/archives/gitlab-merge.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/googlehits.archive` & `sirmordred-1.0.0rc1/tests/archives/googlehits.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/jenkins.archive` & `sirmordred-1.0.0rc1/tests/archives/jenkins.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/jira.archive` & `sirmordred-1.0.0rc1/tests/archives/jira.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/launchpad.archive` & `sirmordred-1.0.0rc1/tests/archives/launchpad.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/mediawiki-1.23.archive` & `sirmordred-1.0.0rc1/tests/archives/mediawiki-1.23.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/mediawiki-1.28.archive` & `sirmordred-1.0.0rc1/tests/archives/mediawiki-1.28.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/meetup.archive` & `sirmordred-1.0.0rc1/tests/archives/meetup.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/mozillaclub.archive` & `sirmordred-1.0.0rc1/tests/archives/mozillaclub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/nntp.archive` & `sirmordred-1.0.0rc1/tests/archives/nntp.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/phabricator.archive` & `sirmordred-1.0.0rc1/tests/archives/phabricator.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/redmine.archive` & `sirmordred-1.0.0rc1/tests/archives/redmine.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/remo.archive` & `sirmordred-1.0.0rc1/tests/archives/remo.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/rss.archive` & `sirmordred-1.0.0rc1/tests/archives/rss.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/slack.archive` & `sirmordred-1.0.0rc1/tests/archives/slack.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/stackexchange.archive` & `sirmordred-1.0.0rc1/tests/archives/stackexchange.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/telegram.archive` & `sirmordred-1.0.0rc1/tests/archives/telegram.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives/twitter.archive` & `sirmordred-1.0.0rc1/tests/archives/twitter.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives-test-projects.json` & `sirmordred-1.0.0rc1/tests/archives-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/archives-test.cfg` & `sirmordred-1.0.0rc1/tests/archives-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/eclipse-projects.json` & `sirmordred-1.0.0rc1/tests/data/eclipse-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/mordred.log` & `sirmordred-1.0.0rc1/tests/data/mordred.log`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/orgs_sortinghat.json` & `sirmordred-1.0.0rc1/tests/data/orgs_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/perceval_identities_sortinghat.json` & `sirmordred-1.0.0rc1/tests/data/perceval_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/remote_identities_sortinghat.json` & `sirmordred-1.0.0rc1/tests/data/remote_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/task-identities-data.json` & `sirmordred-1.0.0rc1/tests/data/task-identities-data.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/task-params-expected` & `sirmordred-1.0.0rc1/tests/data/task-params-expected`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/task-params-test-projects.json` & `sirmordred-1.0.0rc1/tests/data/task-params-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/task-params-test.cfg` & `sirmordred-1.0.0rc1/tests/data/task-params-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/data/url-projects.json` & `sirmordred-1.0.0rc1/tests/data/url-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/run_tests.py` & `sirmordred-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/sortinghat_settings.py` & `sirmordred-1.0.0rc1/tests/sortinghat_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,7 +290,10 @@
 SORTINGHAT_API_PAGE_SIZE = 10
 
 #
 # genderize.io token, used only for gender recommendations
 #
 
 SORTINGHAT_GENDERIZE_API_KEY = None
+
+
+MULTI_TENANT = False
```

### Comparing `sirmordred-0.9.3rc1/tests/test-no-collection.cfg` & `sirmordred-1.0.0rc1/tests/test-no-collection.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test-no-sh.cfg` & `sirmordred-1.0.0rc1/tests/test-no-sh.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test-projects.json` & `sirmordred-1.0.0rc1/tests/test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test-repos-projects.json` & `sirmordred-1.0.0rc1/tests/test-repos-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test-repos.cfg` & `sirmordred-1.0.0rc1/tests/test-repos.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test.cfg` & `sirmordred-1.0.0rc1/tests/test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_config.py` & `sirmordred-1.0.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_github.py` & `sirmordred-1.0.0rc1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_healthcheck.py` & `sirmordred-1.0.0rc1/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_sirmordred.py` & `sirmordred-1.0.0rc1/tests/test_sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_studies.cfg` & `sirmordred-1.0.0rc1/tests/test_studies.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task.py` & `sirmordred-1.0.0rc1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_collection.py` & `sirmordred-1.0.0rc1/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_enrich.py` & `sirmordred-1.0.0rc1/tests/test_task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_identities.py` & `sirmordred-1.0.0rc1/tests/test_task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_manager.py` & `sirmordred-1.0.0rc1/tests/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_panels.py` & `sirmordred-1.0.0rc1/tests/test_task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_task_projects.py` & `sirmordred-1.0.0rc1/tests/test_task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/tests/test_wrong.cfg` & `sirmordred-1.0.0rc1/tests/test_wrong.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.3rc1/PKG-INFO` & `sirmordred-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sirmordred
-Version: 0.9.3rc1
+Version: 1.0.0rc1
 Summary: Drive GrimoireLab tools to produce a dashboard
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
-Requires-Python: >=3.7.1,<4.0.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

