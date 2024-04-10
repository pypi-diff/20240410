# Comparing `tmp/m9s_account_deposit-7.0.2.2.tar.gz` & `tmp/m9s_account_deposit-7.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_account_deposit-7.0.2.2.tar", last modified: Mon Mar 25 10:24:41 2024, max compression
+gzip compressed data, was "m9s_account_deposit-7.0.2.3.tar", last modified: Wed Apr 10 12:01:35 2024, max compression
```

## Comparing `m9s_account_deposit-7.0.2.2.tar` & `m9s_account_deposit-7.0.2.3.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      211 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/.readthedocs.yaml
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/.woodpecker/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2027 2024-01-26 16:41:19.000000 m9s_account_deposit-7.0.2.2/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      764 2024-01-30 08:02:03.000000 m9s_account_deposit-7.0.2.2/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-14 16:04:29.000000 m9s_account_deposit-7.0.2.2/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/MANIFEST.in
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3432 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1034 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.2/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2009 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.2/account.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2495 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/account.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2507 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/configuration.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      460 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/configuration.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/contract.py
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/doc/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2797 2024-03-25 10:24:31.000000 m9s_account_deposit-7.0.2.2/doc/conf.py
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       36 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/doc/requirements-doc.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      304 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/exceptions.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8512 2024-03-25 09:57:50.000000 m9s_account_deposit-7.0.2.2/invoice.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/invoice.xml
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.707785 m9s_account_deposit-7.0.2.2/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1657 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/bg.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1869 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/ca.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1563 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/cs.po
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5126 2024-03-23 18:38:12.000000 m9s_account_deposit-7.0.2.2/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1895 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/es.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1700 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/es_419.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1833 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/et.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2003 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/fa.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1563 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/fi.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/fr.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1630 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/hu.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1697 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/id.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1896 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/it.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1869 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/lo.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1575 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/lt.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1884 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/nl.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1631 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/pl.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1707 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/pt.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1858 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/ro.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1655 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/ru.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1671 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/sl.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1627 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/tr.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1535 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/uk.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1593 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/locale/zh_CN.po
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3432 2024-03-25 10:24:40.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2702 2024-03-25 10:24:41.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-03-25 10:24:40.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-03-25 10:24:40.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-11 12:02:08.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      233 2024-03-25 10:24:40.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-03-25 10:24:40.000000 m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2081 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_bg.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1258 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_ca.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_de.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1256 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_en.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_es.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1256 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_fr.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_nl.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_pt.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_ru.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/minimal_chart_sl.xml
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     6650 2024-03-23 18:38:12.000000 m9s_account_deposit-7.0.2.2/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      695 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/party.xml
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4631 2024-01-26 16:40:10.000000 m9s_account_deposit-7.0.2.2/setup.py
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.707785 m9s_account_deposit-7.0.2.2/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      144 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/tests/__init__.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3022 2024-03-25 10:08:56.000000 m9s_account_deposit-7.0.2.2/tests/scenario_deposit.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3515 2024-02-24 20:39:55.000000 m9s_account_deposit-7.0.2.2/tests/scenario_deposit_second_currency.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      525 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.2/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.2/tests/test_scenario.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      648 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/tests/tools.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      568 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      499 2024-03-25 10:24:31.000000 m9s_account_deposit-7.0.2.2/tryton.cfg
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-25 10:24:41.711785 m9s_account_deposit-7.0.2.2/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      349 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/view/account_type_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      522 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/view/configuration_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.2/view/invoice_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      485 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/view/move_line_list_deposit.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      406 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/view/party_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      318 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.2/view/party_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      334 2023-12-14 16:04:29.000000 m9s_account_deposit-7.0.2.2/view/recall_deposit_form.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.134622 m9s_account_deposit-7.0.2.3/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/.woodpecker/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2027 2024-01-26 16:41:19.000000 m9s_account_deposit-7.0.2.3/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      764 2024-01-30 08:02:03.000000 m9s_account_deposit-7.0.2.3/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-14 16:04:29.000000 m9s_account_deposit-7.0.2.3/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3432 2024-04-10 12:01:35.134622 m9s_account_deposit-7.0.2.3/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1034 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.3/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2009 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.3/account.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2495 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/account.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2507 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/configuration.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      460 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/configuration.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/contract.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/doc/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     2775 2024-04-10 12:01:33.000000 m9s_account_deposit-7.0.2.3/doc/conf.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       36 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/doc/requirements-doc.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      304 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/exceptions.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8518 2024-04-10 12:00:52.000000 m9s_account_deposit-7.0.2.3/invoice.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/invoice.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1657 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/bg.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1869 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/ca.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1563 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/cs.po
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5126 2024-03-23 18:38:12.000000 m9s_account_deposit-7.0.2.3/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1895 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/es.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1700 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/es_419.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1833 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/et.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2003 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/fa.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1563 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/fi.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/fr.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1630 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/hu.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1697 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/id.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1896 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/it.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1869 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/lo.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1575 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/lt.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1884 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/nl.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1631 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/pl.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1707 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/pt.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1858 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/ro.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1655 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/ru.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1671 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/sl.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1627 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/tr.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1535 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/uk.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1593 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/locale/zh_CN.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.134622 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3432 2024-04-10 12:01:34.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2684 2024-04-10 12:01:35.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-10 12:01:34.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-04-10 12:01:34.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-11 12:02:08.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      233 2024-04-10 12:01:34.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-10 12:01:34.000000 m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2081 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_bg.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1258 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_ca.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_de.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1256 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_en.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_es.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1256 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_fr.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_nl.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1260 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_pt.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_ru.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/minimal_chart_sl.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     6593 2024-04-10 12:00:52.000000 m9s_account_deposit-7.0.2.3/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      695 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/party.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-10 12:01:35.134622 m9s_account_deposit-7.0.2.3/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4631 2024-01-26 16:40:10.000000 m9s_account_deposit-7.0.2.3/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      144 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3022 2024-03-25 10:08:56.000000 m9s_account_deposit-7.0.2.3/tests/scenario_deposit.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3515 2024-02-24 20:39:55.000000 m9s_account_deposit-7.0.2.3/tests/scenario_deposit_second_currency.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      525 2024-01-26 16:38:58.000000 m9s_account_deposit-7.0.2.3/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2023-12-15 08:53:22.000000 m9s_account_deposit-7.0.2.3/tests/test_scenario.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      648 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/tests/tools.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      568 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      499 2024-04-10 12:01:33.000000 m9s_account_deposit-7.0.2.3/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-10 12:01:35.130622 m9s_account_deposit-7.0.2.3/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      349 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/view/account_type_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      522 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/view/configuration_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2024-01-26 16:38:56.000000 m9s_account_deposit-7.0.2.3/view/invoice_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      485 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/view/move_line_list_deposit.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      406 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/view/party_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      318 2023-12-15 09:25:43.000000 m9s_account_deposit-7.0.2.3/view/party_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      334 2023-12-14 16:04:29.000000 m9s_account_deposit-7.0.2.3/view/recall_deposit_form.xml
```

### Comparing `m9s_account_deposit-7.0.2.2/.woodpecker/mail_curl.sh` & `m9s_account_deposit-7.0.2.3/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/.woodpecker/report.yml` & `m9s_account_deposit-7.0.2.3/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/.woodpecker/test.yml` & `m9s_account_deposit-7.0.2.3/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/CHANGELOG` & `m9s_account_deposit-7.0.2.3/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/COPYRIGHT` & `m9s_account_deposit-7.0.2.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/LICENSE` & `m9s_account_deposit-7.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/PKG-INFO` & `m9s_account_deposit-7.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_account_deposit
-Version: 7.0.2.2
+Version: 7.0.2.3
 Summary: Tryton Account Deposit Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_deposit.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_deposit-7.0.2.2/README.md` & `m9s_account_deposit-7.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/__init__.py` & `m9s_account_deposit-7.0.2.3/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/account.py` & `m9s_account_deposit-7.0.2.3/account.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/account.xml` & `m9s_account_deposit-7.0.2.3/account.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/configuration.py` & `m9s_account_deposit-7.0.2.3/configuration.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/doc/conf.py` & `m9s_account_deposit-7.0.2.3/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
```

### Comparing `m9s_account_deposit-7.0.2.2/invoice.py` & `m9s_account_deposit-7.0.2.3/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return True
 
     @fields.depends('party')
     def on_change_with_deposit(self, name=None):
         if self.party:
             return self.party.deposit
         else:
-            return None
+            return Decimal(0)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('posted')
     def post(cls, invoices):
         # Run validate_invoice before posting to set the invoice to a
         # different state than draft to not touch any more the deposit lines.
```

### Comparing `m9s_account_deposit-7.0.2.2/invoice.xml` & `m9s_account_deposit-7.0.2.3/invoice.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/bg.po` & `m9s_account_deposit-7.0.2.3/locale/bg.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/ca.po` & `m9s_account_deposit-7.0.2.3/locale/ca.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/cs.po` & `m9s_account_deposit-7.0.2.3/locale/cs.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/de.po` & `m9s_account_deposit-7.0.2.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/es.po` & `m9s_account_deposit-7.0.2.3/locale/es.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/es_419.po` & `m9s_account_deposit-7.0.2.3/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/et.po` & `m9s_account_deposit-7.0.2.3/locale/et.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/fa.po` & `m9s_account_deposit-7.0.2.3/locale/fa.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/fi.po` & `m9s_account_deposit-7.0.2.3/locale/fi.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/fr.po` & `m9s_account_deposit-7.0.2.3/locale/fr.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/hu.po` & `m9s_account_deposit-7.0.2.3/locale/hu.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/id.po` & `m9s_account_deposit-7.0.2.3/locale/id.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/it.po` & `m9s_account_deposit-7.0.2.3/locale/it.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/lo.po` & `m9s_account_deposit-7.0.2.3/locale/lo.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/lt.po` & `m9s_account_deposit-7.0.2.3/locale/lt.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/nl.po` & `m9s_account_deposit-7.0.2.3/locale/nl.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/pl.po` & `m9s_account_deposit-7.0.2.3/locale/pl.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/pt.po` & `m9s_account_deposit-7.0.2.3/locale/pt.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/ro.po` & `m9s_account_deposit-7.0.2.3/locale/ro.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/ru.po` & `m9s_account_deposit-7.0.2.3/locale/ru.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/sl.po` & `m9s_account_deposit-7.0.2.3/locale/sl.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/tr.po` & `m9s_account_deposit-7.0.2.3/locale/tr.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/uk.po` & `m9s_account_deposit-7.0.2.3/locale/uk.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/locale/zh_CN.po` & `m9s_account_deposit-7.0.2.3/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/PKG-INFO` & `m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-account-deposit
-Version: 7.0.2.2
+Version: 7.0.2.3
 Summary: Tryton Account Deposit Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_deposit.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_deposit-7.0.2.2/m9s_account_deposit.egg-info/SOURCES.txt` & `m9s_account_deposit-7.0.2.3/m9s_account_deposit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.md
 README.rst
 __init__.py
```

### Comparing `m9s_account_deposit-7.0.2.2/message.xml` & `m9s_account_deposit-7.0.2.3/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_bg.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_ca.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_de.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_en.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_es.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_fr.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_nl.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_pt.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_ru.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/minimal_chart_sl.xml` & `m9s_account_deposit-7.0.2.3/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/party.py` & `m9s_account_deposit-7.0.2.3/party.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,95 +22,98 @@
             "Deposit", currency='currency', digits='currency'),
         'get_deposit', searcher='search_deposit')
 
     @classmethod
     def get_deposit(cls, parties, name):
         '''
         Function to compute deposit for party ids.
-        Adapted from account/party/search_receivable_payable
+
+        Deviating from the upstream module we do not restrict to open fiscal
+        years (line_clause).
         '''
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         User = pool.get('res.user')
         cursor = Transaction().connection.cursor()
 
         line = MoveLine.__table__()
         account = Account.__table__()
         account_type = AccountType.__table__()
 
-        result = {p.id: Decimal(0) for p in parties}
+        values = {p.id: Decimal(0) for p in parties}
 
         user = User(Transaction().user)
         if not user.company:
-            return result
-        company_id = user.company.id
-        exp = Decimal(str(10.0 ** -user.company.currency.digits))
-
-        # Use credit - debit to display positive deposit amounts
-        amount = Sum(Coalesce(line.credit, 0) - Coalesce(line.debit, 0))
-        code = name
+            return values
+        currency = user.company.currency
+
+        # line_clause, _ = MoveLine.query_get(line)
+
         for sub_parties in grouped_slice(parties):
-            sub_ids = [p.id for p in sub_parties]
-            party_where = reduce_ids(line.party, sub_ids)
-            cursor.execute(*line.join(account,
-                    condition=account.id == line.account
-                    ).join(account_type,
-                    condition=account.type == account_type.id
-                    ).select(line.party, amount,
-                    where=(getattr(account_type, code)
-                        & (line.reconciliation == Null)
-                        & (account.company == company_id)
-                        & party_where),
+            party_clause = reduce_ids(line.party, [p.id for p in sub_parties])
+            cursor.execute(*line
+                .join(account, condition=account.id == line.account)
+                .join(account_type, condition=account.type == account_type.id)
+                .select(line.party,
+                    # Use credit - debit to positive deposit amount
+                    Sum(Coalesce(line.credit, 0) - Coalesce(line.debit, 0)),
+                    where=account_type.deposit
+                    & party_clause
+                    & (line.reconciliation == Null)
+                    & (account.company == user.company.id),
+                    # & line_clause,
                     group_by=line.party))
-            for party, value in cursor:
+            for party_id, value in cursor:
                 # SQLite uses float for SUM
                 if not isinstance(value, Decimal):
-                    value = Decimal(str(value))
-                result[party] = value.quantize(exp)
-        return result
+                    value = currency.round(Decimal(str(value)))
+                values[party_id] = value
+        return values
 
     @classmethod
     def search_deposit(cls, name, clause):
+        '''
+        Function to search deposit for party ids.
+
+        Deviating from the upstream module we do not restrict to open fiscal
+        years (line_clause).
+        '''
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         User = pool.get('res.user')
 
         line = MoveLine.__table__()
         account = Account.__table__()
         account_type = AccountType.__table__()
 
-        _, operator, value = clause
-
         user = User(Transaction().user)
         if not user.company:
             return []
-        company_id = user.company.id
-        code = 'deposit'
-        Operator = fields.SQL_OPERATORS[operator]
-
-        # Need to cast numeric for sqlite
-        cast_ = MoveLine.debit.sql_cast
-        amount = cast_(Sum(Coalesce(line.credit, 0) - Coalesce(line.debit, 0)))
-        if operator in {'in', 'not in'}:
-            value = [cast_(Literal(Decimal(v or 0))) for v in value]
-        else:
-            value = cast_(Literal(Decimal(value or 0)))
-        query = (line.join(account, condition=account.id == line.account
-                ).join(account_type, condition=account.type == account_type.id
-                ).select(line.party,
-                where=(getattr(account_type, code)
-                    & (line.party != Null)
-                    & (line.reconciliation == Null)
-                    & (account.company == company_id)),
+
+        # line_clause, _ = MoveLine.query_get(line)
+        Operator = fields.SQL_OPERATORS[clause[1]]
+
+        query = (line
+            .join(account, condition=account.id == line.account)
+            .join(account_type, condition=account.type == account_type.id)
+            .select(line.party,
+                where=account.active
+                & account_type.deposit
+                & (line.party != Null)
+                & (line.reconciliation == Null)
+                & (account.company == user.company.id),
+                # & line_clause,
                 group_by=line.party,
-                having=Operator(amount, value)))
+                having=Operator(
+                    Sum(Coalesce(line.debit, 0) - Coalesce(line.credit, 0)),
+                    Decimal(clause[2] or 0))))
         return [('id', 'in', query)]
 
     def get_deposit_balance(self, deposit_account, currency=None):
         'Return the deposit account balance (debit - credit) for the party'
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         transaction = Transaction()
```

### Comparing `m9s_account_deposit-7.0.2.2/party.xml` & `m9s_account_deposit-7.0.2.3/party.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/setup.py` & `m9s_account_deposit-7.0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/tests/scenario_deposit.rst` & `m9s_account_deposit-7.0.2.3/tests/scenario_deposit.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/tests/scenario_deposit_second_currency.rst` & `m9s_account_deposit-7.0.2.3/tests/scenario_deposit_second_currency.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/tests/test_module.py` & `m9s_account_deposit-7.0.2.3/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/tests/tools.py` & `m9s_account_deposit-7.0.2.3/tests/tools.py`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/tox.ini` & `m9s_account_deposit-7.0.2.3/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_account_deposit-7.0.2.2/view/configuration_form.xml` & `m9s_account_deposit-7.0.2.3/view/configuration_form.xml`

 * *Files identical despite different names*

