# Comparing `tmp/nmbrs-0.1.1.tar.gz` & `tmp/nmbrs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.1.1.tar", last modified: Sun Apr  7 12:16:52 2024, max compression
+gzip compressed data, was "nmbrs-0.1.2.tar", last modified: Wed Apr 10 07:45:11 2024, max compression
```

## Comparing `nmbrs-0.1.1.tar` & `nmbrs-0.1.2.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.212377 nmbrs-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-07 12:16:35.000000 nmbrs-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 12:16:35.000000 nmbrs-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-07 12:16:52.212377 nmbrs-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-07 12:16:35.000000 nmbrs-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-07 12:16:35.000000 nmbrs-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:16:52.212377 nmbrs-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-07 12:16:35.000000 nmbrs-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.196377 nmbrs-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.196377 nmbrs-0.1.1/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 12:16:50.000000 nmbrs-0.1.1/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.200377 nmbrs-0.1.1/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.200377 nmbrs-0.1.1/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.200377 nmbrs-0.1.1/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/exceptions/nmbrs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/exceptions/sso_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.200377 nmbrs-0.1.1/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.200377 nmbrs-0.1.1/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.204378 nmbrs-0.1.1/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.204378 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.212377 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.212377 nmbrs-0.1.1/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-07 12:16:35.000000 nmbrs-0.1.1/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:16:52.212377 nmbrs-0.1.1/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-07 12:16:52.000000 nmbrs-0.1.1/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-07 12:16:52.000000 nmbrs-0.1.1/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:16:52.000000 nmbrs-0.1.1/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 12:16:52.000000 nmbrs-0.1.1/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 12:16:52.000000 nmbrs-0.1.1/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-10 07:44:55.000000 nmbrs-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 07:44:55.000000 nmbrs-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 07:45:11.856049 nmbrs-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-10 07:44:55.000000 nmbrs-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 07:44:55.000000 nmbrs-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:45:11.856049 nmbrs-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-10 07:44:55.000000 nmbrs-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.840049 nmbrs-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.840049 nmbrs-0.1.2/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 07:45:10.000000 nmbrs-0.1.2/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.848049 nmbrs-0.1.2/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.848049 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.852049 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.1.1/LICENSE` & `nmbrs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/PKG-INFO` & `nmbrs-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
-Project-URL: Homepage, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
-Project-URL: Source, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
-Project-URL: Issues, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK/issues
+Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
+Project-URL: Source, https://github.com/LarsKluijtmans/nmbrs_api
+Project-URL: Issues, https://github.com/LarsKluijtmans/nmbrs_api/issues
 Keywords: nmbrs,soap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -155,22 +155,22 @@
 
 In case a user does not have access to the needed endpoints an AuthorizationError will be raised.
 
 To handle these Exceptions you can take inspiration from the following code.
 
 ```python
 from nmbrs import Nmbrs
-from nmbrs.exceptions import AuthorizationError
+from nmbrs.exceptions import AuthenticationException
 
 api = Nmbrs(username="__username__", token="__token__", auth_type="token")
 
 try:
     debtors = api.debtor.get_all()
-except AuthorizationError as e:
-    print(f"User does not have access to: {', '.join(e.resources)}'")
+except AuthenticationException as e:
+    print(f"User does not have access to: {e.resource}")
 ```
 
 ## Single Sign-on(SSO)
 
 When it comes to Nmbrs Single Sign-On service:
 
  - Username and Token
```

### Comparing `nmbrs-0.1.1/README.md` & `nmbrs-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -132,22 +132,22 @@
 
 In case a user does not have access to the needed endpoints an AuthorizationError will be raised.
 
 To handle these Exceptions you can take inspiration from the following code.
 
 ```python
 from nmbrs import Nmbrs
-from nmbrs.exceptions import AuthorizationError
+from nmbrs.exceptions import AuthenticationException
 
 api = Nmbrs(username="__username__", token="__token__", auth_type="token")
 
 try:
     debtors = api.debtor.get_all()
-except AuthorizationError as e:
-    print(f"User does not have access to: {', '.join(e.resources)}'")
+except AuthenticationException as e:
+    print(f"User does not have access to: {e.resource}")
 ```
 
 ## Single Sign-on(SSO)
 
 When it comes to Nmbrs Single Sign-On service:
 
  - Username and Token
```

### Comparing `nmbrs-0.1.1/src/nmbrs/api.py` & `nmbrs-0.1.2/src/nmbrs/api.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/data_classes/company.py` & `nmbrs-0.1.2/src/nmbrs/data_classes/company.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/data_classes/data_class.py` & `nmbrs-0.1.2/src/nmbrs/data_classes/data_class.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/data_classes/debtor.py` & `nmbrs-0.1.2/src/nmbrs/data_classes/debtor.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-0.1.2/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/service/company_service.py` & `nmbrs-0.1.2/src/nmbrs/service/company_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.svw.set_auth_header(auth_header)
         self.wage_component.set_auth_header(auth_header)
         self.wage_cost.set_auth_header(auth_header)
         self.wage_model.set_auth_header(auth_header)
         self.wage_tax.set_auth_header(auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:List_GetAll"])
+    @nmbrs_exception_handler(resource="CompanyService:List_GetAll")
     def get_all(self) -> list[Company]:
         """
         Retrieve all companies.
 
         For more information, refer to the official documentation:
             [Soap call List_GetAll](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=List_GetAll)
 
@@ -104,15 +104,15 @@
             list[Company]: A list of Company objects.
         """
         companies = self.client.service.List_GetAll(_soapheaders=self.auth_header)
         companies = [Company(company) for company in serialize_object(companies)]
         return companies
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:List_GetByDebtor"])
+    @nmbrs_exception_handler(resource="CompanyService:List_GetByDebtor")
     def get_by_debtor(self, debtor_id: int) -> list[Company]:
         """
         Get all the companies belonging to a debtor.
 
         For more information, refer to the official documentation:
             [Soap call List_GetByDebtor](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=List_GetByDebtor)
 
@@ -122,15 +122,15 @@
         Returns:
             list[Company]: A list of Company objects.
         """
         companies = self.client.service.List_GetByDebtor(DebtorId=debtor_id, _soapheaders=self.auth_header)
         companies = [Company(company) for company in serialize_object(companies)]
         return companies
 
-    @nmbrs_exception_handler(resources=["CompanyService:Company_GetCurrentByEmployeeId"])
+    @nmbrs_exception_handler(resource="CompanyService:Company_GetCurrentByEmployeeId")
     def get_by_employee(self, employee_id: int) -> Company | None:
         """
         Get company by employee id.
 
         For more information, refer to the official documentation:
             [Company_GetCurrentByEmployeeId](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Company_GetCurrentByEmployeeId)
 
@@ -141,15 +141,15 @@
             Company: A list of Company objects.
         """
         company = self.client.service.Company_GetCurrentByEmployeeId(EmployeeId=employee_id, _soapheaders=self.auth_header)
         if company is None:
             return None
         return Company(serialize_object(company))
 
-    @nmbrs_exception_handler(resources=["CompanyService:Company_GetCurrentPeriod"])
+    @nmbrs_exception_handler(resource="CompanyService:Company_GetCurrentPeriod")
     def get_current_period(self, company_id: int) -> Period | None:
         """
         Get the current period of the company.
 
         For more information, refer to the official documentation:
             [Soap call Company_GetCurrentPeriod](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Company_GetCurrentPeriod)
 
@@ -160,15 +160,15 @@
             Period: year, period and period type and the company.
         """
         period = self.client.service.Company_GetCurrentPeriod(CompanyId=company_id, _soapheaders=self.auth_header)
         if period is None:
             return None
         return Period(company_id=company_id, data=serialize_object(period))
 
-    @nmbrs_exception_handler(resources=["CompanyService:Company_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:Company_Insert")
     def insert(
         self, debtor_id: int, name: str, period_type: int, default_id: int, labour_agreement_group_id: str, pay_in_advance: bool
     ) -> int:
         """
         Insert a new company.
 
         This method inserts a new debtor with the provided details into the Nmbrs system.
@@ -194,15 +194,15 @@
             DefaultCompanyId=default_id,
             LabourAgreementSettingsGroupGuid=labour_agreement_group_id,
             PayInAdvance=pay_in_advance,
             _soapheaders=self.auth_header,
         )
         return inserted
 
-    @nmbrs_exception_handler(resources=["CompanyService:ContactPerson_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:ContactPerson_Get")
     def get_contact_person(self, company_id: int) -> ContactPerson:
         """
         Get contact person by company ID.
 
         For more information, refer to the official documentation:
             [ContactPerson_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=ContactPerson_Get)
 
@@ -211,15 +211,15 @@
 
         Returns:
             ContactPerson: The contact person details.
         """
         contact_person = self.client.service.ContactPerson_Get(CompanyId=company_id, _soapheaders=self.auth_header)
         return ContactPerson(company_id=company_id, data=serialize_object(contact_person))
 
-    @nmbrs_exception_handler(resources=["CompanyService:Converter_GetByCompany_IntToGuid"])
+    @nmbrs_exception_handler(resource="CompanyService:Converter_GetByCompany_IntToGuid")
     def get_converter_mappings(self, company_id: int, entity: str) -> GuidConvertor:
         """
         Get converter mappings for the given entity and company ID.
 
         For more information, refer to the official documentation:
             [Converter_GetByCompany_IntToGuid](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Converter_GetByCompany_IntToGuid)
 
@@ -230,15 +230,15 @@
         Returns:
             GuidConvertor: The converter mappings response.
         """
         guids = self.client.service.Converter_GetByCompany_IntToGuid(Entity=entity, CompanyId=company_id, _soapheaders=self.auth_header)
         return GuidConvertor(company_id=company_id, data=serialize_object(guids))
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:DefaultEmployeeTemplates_GetByCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:DefaultEmployeeTemplates_GetByCompany")
     def get_default_employee_templates(self, company_id: int) -> list[DefaultEmployeeTemplate]:
         """
         Get available default employee templates by company.
 
         For more information, refer to the official documentation:
             [Converter_GetByCompany_IntToGuid](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=DefaultEmployeeTemplates_GetByCompany)
 
@@ -251,15 +251,15 @@
         employee_templates = self.client.service.DefaultEmployeeTemplates_GetByCompany(CompanyId=company_id, _soapheaders=self.auth_header)
         employee_templates = [
             DefaultEmployeeTemplate(company_id=company_id, data=employee_template)
             for employee_template in serialize_object(employee_templates)
         ]
         return employee_templates
 
-    @nmbrs_exception_handler(resources=["CompanyService:FileExplorer_UploadFile"])
+    @nmbrs_exception_handler(resource="CompanyService:FileExplorer_UploadFile")
     def upload_file(self, company_id: int, document_name: str, document_sub_folder: str, data: bytes) -> None:
         """
         Upload a document for a company.
 
         For further details, see the official documentation:
             [FileExplorer_UploadFile](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=FileExplorer_UploadFile)
 
@@ -278,15 +278,15 @@
                 "StrDocumentName": document_name,
                 "StrDocumentSubFolder": document_sub_folder,
                 "Body": data,
             },
             _soapheaders=self.auth_header,
         )
 
-    @nmbrs_exception_handler(resources=["CompanyService:Schedule_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:Schedule_GetCurrent")
     def get_current_schedule(self, company_id: int) -> FulltimeSchedules:
         """
         Retrieve the current schedules for a company.
 
         For further details, see the official documentation:
             [Schedule_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Schedule_GetCurrent)
 
@@ -296,15 +296,15 @@
         Returns:
             FulltimeSchedules: A FulltimeSchedules object.
         """
         response = self.client.service.Schedule_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         return FulltimeSchedules(company_id=company_id, data=serialize_object(response))
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:PayrollWorkflow_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:PayrollWorkflow_Get")
     def get_payroll_workflow(self, company_id: int, year: int, period: int) -> list[PayrollWorkflowTrack]:
         """
         Get the company's payroll workflow tracks and actions.
 
         For further details, see the official documentation:
             [PayrollWorkflow_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=PayrollWorkflow_Get)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/debtor_service.py` & `nmbrs-0.1.2/src/nmbrs/service/debtor_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         # Micro services
         self.department.set_auth_header(auth_header)
         self.function.set_auth_header(auth_header)
         self.webhook.set_auth_header(auth_header)
         self.title.set_auth_header(auth_header)
 
-    @nmbrs_exception_handler(resources=["DebtorService:Environment_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:Environment_Get")
     def get_domain(self, username: str, token: str) -> Domain:
         """
         Generate authentication header for standard token-based authentication.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Environment_Get)
 
@@ -74,15 +74,15 @@
         Returns:
             Domain: The domain object associated with the token.
         """
         env = self.debtor_service.service.Environment_Get(_soapheaders={"AuthHeader": {"Username": username, "Token": token}})
         return Domain(data=serialize_object(env))
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:List_GetAll"])
+    @nmbrs_exception_handler(resource="DebtorService:List_GetAll")
     def get_all(self) -> list[Debtor]:
         """
         Retrieve all debtors.
 
         For more information, refer to the official documentation:
             [Soap call List_GetAll](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=List_GetAll)
 
@@ -90,15 +90,15 @@
             list[Debtor]: A list of Debtor objects representing all debtors.
         """
         debtors = self.debtor_service.service.List_GetAll(_soapheaders=self.auth_header)
         debtors = [Debtor(debtor) for debtor in serialize_object(debtors)]
         return debtors
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:List_GetByNumber"])
+    @nmbrs_exception_handler(resource="DebtorService:List_GetByNumber")
     def get_all_by_number(self, number: str) -> list[Debtor]:
         """
         Retrieve all debtors by number.
 
         For more information, refer to the official documentation:
             [Soap call List_GetByNumber](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=List_GetByNumber)
 
@@ -108,15 +108,15 @@
         Returns:
             list[Debtor]: A list of Debtor objects representing all debtors.
         """
         debtors = self.debtor_service.service.List_GetByNumber(Number=number, _soapheaders=self.auth_header)
         debtors = [Debtor(debtor) for debtor in serialize_object(debtors)]
         return debtors
 
-    @nmbrs_exception_handler(resources=["DebtorService:Debtor_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:Debtor_Get")
     def get(self, debtor_id: int) -> Debtor | None:
         """
         Retrieve a debtor by ID.
 
         For more information, refer to the official documentation:
             [Soap call Debtor_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_Get)
 
@@ -127,15 +127,15 @@
             Debtor | None: A Debtor object representing the debtor if found, otherwise None.
         """
         debtor = self.debtor_service.service.Debtor_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if debtor is None:
             return None
         return Debtor(serialize_object(debtor))
 
-    @nmbrs_exception_handler(resources=["DebtorService:Debtor_Insert"])
+    @nmbrs_exception_handler(resource="DebtorService:Debtor_Insert")
     def insert(self, debtor_id: int, number: str, name: str) -> int:
         """
         Insert a new debtor.
 
         For more information, refer to the official documentation:
             [Soap call Debtor_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_Insert)
 
@@ -147,15 +147,15 @@
         Returns:
             int: The ID of the inserted debtor if successful.
         """
         data = {"Debtor": {"Id": debtor_id, "Number": number, "Name": name}}
         inserted = self.debtor_service.service.Debtor_Insert(**data, _soapheaders=self.auth_header)
         return inserted
 
-    @nmbrs_exception_handler(resources=["DebtorService:Debtor_Update"])
+    @nmbrs_exception_handler(resource="DebtorService:Debtor_Update")
     def update(self, debtor_id: int, number: str, name: str) -> None:
         """
         Update an existing debtor.
 
         For more information, refer to the official documentation:
             [Soap call Debtor_Update](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_Update)
 
@@ -164,15 +164,15 @@
             number (str): The new number of the debtor.
             name (str): The new name of the debtor.
         """
         data = {"Debtor": {"Id": debtor_id, "Number": number, "Name": name}}
         self.debtor_service.service.Debtor_Update(**data, _soapheaders=self.auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:AbsenceXML_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:AbsenceXML_Get")
     def get_absence_xml(self, debtor_id: int, start_date: datetime, end_date: datetime) -> list[AbsenceVerzuim]:
         """
         Retrieve absence data for a debtor within a specified date range.
 
         For more information, refer to the official documentation:
             [Soap call AbsenceXML_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=AbsenceXML_Get)
 
@@ -186,15 +186,15 @@
         """
         data = {"DebtorId": debtor_id, "from": start_date, "to": end_date}
         absences = self.debtor_service.service.AbsenceXML_Get(**data, _soapheaders=self.auth_header)
         absences = [AbsenceVerzuim(absence) for absence in serialize_object(absences)]
         return absences
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:AccountantContact_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:AccountantContact_GetList")
     def get_all_accountant_contact_info(self, debtor_id: int) -> list[ContactInfo]:
         """
         Retrieve all accountant contact information.
 
         For more information, refer to the official documentation:
             [Soap call AccountantContact_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=AccountantContact_GetList)
 
@@ -204,15 +204,15 @@
         Returns:
             list[ContactInfo]: A list of ContactInfo objects representing the accountant contact information.
         """
         accountants = self.debtor_service.service.AccountantContact_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
         accountants = [ContactInfo(debtor_id=debtor_id, data=accountant) for accountant in serialize_object(accountants)]
         return accountants
 
-    @nmbrs_exception_handler(resources=["DebtorService:Address_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:Address_Get")
     def get_address(self, debtor_id: int) -> Address | None:
         """
         Retrieve address information for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Address_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Address_Get)
 
@@ -223,15 +223,15 @@
             Address | None: An Address object representing the address if found, otherwise None.
         """
         address = self.debtor_service.service.Address_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if address is None:
             return None
         return Address(debtor_id=debtor_id, data=serialize_object(address))
 
-    @nmbrs_exception_handler(resources=["DebtorService:BankAccount_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:BankAccount_Get")
     def get_bank_account(self, debtor_id: int) -> BankAccount | None:
         """
         Retrieve bank account information for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call BankAccount_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=BankAccount_Get)
 
@@ -242,15 +242,15 @@
             BankAccount | None: A BankAccount object representing the bank account if found, otherwise None.
         """
         bank_account = self.debtor_service.service.BankAccount_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if bank_account is None:
             return None
         return BankAccount(debtor_id=debtor_id, data=serialize_object(bank_account))
 
-    @nmbrs_exception_handler(resources=["DebtorService:ContactPerson_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:ContactPerson_Get")
     def get_contact_person(self, debtor_id: int) -> ContactInfo | None:
         """
         Retrieve contact person information for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call ContactPerson_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=ContactPerson_Get)
 
@@ -261,30 +261,30 @@
             ContactInfo | None: A ContactInfo object representing the contact person if found, otherwise None.
         """
         contact_person = self.debtor_service.service.ContactPerson_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if contact_person is None:
             return None
         return ContactInfo(debtor_id=debtor_id, data=serialize_object(contact_person))
 
-    @nmbrs_exception_handler(resources=["DebtorService:Debtor_IsOwner"])
+    @nmbrs_exception_handler(resource="DebtorService:Debtor_IsOwner")
     def is_owner(self) -> bool:
         """
         Check if the current user is the owner of the debtor.
 
         For more information, refer to the official documentation:
             [Soap call Debtor_IsOwner](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_IsOwner)
 
         Returns:
             bool: True if the current user is the owner of the debtor, otherwise False.
         """
         is_owner = self.debtor_service.service.Debtor_IsOwner(_soapheaders=self.auth_header)
         return is_owner
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:LabourAgreementSettings_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:LabourAgreementSettings_GetList")
     def get_all_labour_agreements(self, debtor_id: int, year: int, period: int) -> list[LabourAgreementSettings]:
         """
         Retrieve all labour agreement settings for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call LabourAgreementSettings_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=LabourAgreementSettings_GetList)
 
@@ -302,15 +302,15 @@
         )
         labour_agreements = [
             LabourAgreementSettings(debtor_id=debtor_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:Manager_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:Manager_GetList")
     def get_all_managers(self, debtor_id: int) -> list[Manager]:
         """
         Retrieve all managers for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Manager_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Manager_GetList)
 
@@ -320,15 +320,15 @@
         Returns:
             list[Manager]: A list of Manager objects representing all managers for the debtor.
         """
         managers = self.debtor_service.service.Manager_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
         managers = [Manager(debtor_id=debtor_id, data=manager) for manager in serialize_object(managers)]
         return managers
 
-    @nmbrs_exception_handler(resources=["DebtorService:ServiceLevel_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:ServiceLevel_Get")
     def get_service_level(self, debtor_id: int) -> ServiceLevel | None:
         """
         Retrieve service level information for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call ServiceLevel_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=ServiceLevel_Get)
 
@@ -341,15 +341,15 @@
         """
         service_level = self.debtor_service.service.ServiceLevel_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         if service_level is None:
             return None
         return ServiceLevel(debtor_id=debtor_id, data=serialize_object(service_level))
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:Tags_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:Tags_Get")
     def get_tags(self, debtor_id: int) -> list[Tag]:
         """
         Retrieve all tags for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Tags_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Tags_Get)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/employee_service.py` & `nmbrs-0.1.2/src/nmbrs/service/employee_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,16 @@
         self.hour_component = EmployeeHourComponentFixedService(self.client)  # TO BE implemented
         self.labour_agreement = EmployeeLabourAgreementService(self.client)  # TO BE implemented
         self.lease_car = EmployeeLeaseCarService(self.client)  # TO BE implemented
         self.leave = EmployeeLeaveService(self.client)  # TO BE implemented
         self.levensloop = EmployeeLevensLoopService(self.client)  # TO BE implemented
         self.manager = EmployeeManagerService(self.client)  # TO BE implemented
         self.partner = EmployeePartnerService(self.client)  # TO BE implemented
-        self.personal_info = EmployeePersonalInfoService(self.client)  # TO BE implemented
+        self.personal_info = EmployeePersonalInfoService(self.client)
+
         self.salary = EmployeeSalaryService(self.client)  # TO BE implemented
         self.schedule = EmployeeScheduleService(self.client)  # TO BE implemented
         self.service = EmployeeServiceService(self.client)  # TO BE implemented
         self.spaarloon = EmployeeSpaarloonService(self.client)  # TO BE implemented
         self.svw = EmployeeSvwService(self.client)  # TO BE implemented
         self.time_registration = EmployeeTimeRegistrationService(self.client)  # TO BE implemented
         self.time_schedule = EmployeeTimeScheduleService(self.client)  # TO BE implemented
@@ -116,30 +117,30 @@
         self.svw.set_auth_header(auth_header)
         self.time_registration.set_auth_header(auth_header)
         self.time_schedule.set_auth_header(auth_header)
         self.wage_component.set_auth_header(auth_header)
         self.wage_tax.set_auth_header(auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["EmployeeService:EmployeeType_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:EmployeeType_GetList")
     def get_types(self) -> list[EmployeeTypes]:
         """
         Get the list of all employee types available.
 
         For more information, refer to the official documentation:
             [EmployeeType_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EmployeeType_GetList)
 
         Returns:
             list[EmployeeTypes]: A list of employee type objects.
         """
         employee_types = self.client.service.EmployeeType_GetList(_soapheaders=self.auth_header)
         employee_types = [EmployeeTypes(employee_type) for employee_type in serialize_object(employee_types)]
         return employee_types
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employee_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employee_GetCurrent")
     def get_current_period(self, employee_id: int) -> Period | None:
         """
         Get the employees current period, Format = yyyy-pp-type, example: 2010-5-M or 2010-4-4W.
 
         For more information, refer to the official documentation:
             [Employee_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_GetCurrent)
 
@@ -151,15 +152,15 @@
         """
         period = self.client.service.Employee_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
         if period is None:
             return None
         return Period(employee_id=employee_id, data=serialize_object(period))
 
     @return_list
-    @nmbrs_exception_handler(resources=["EmployeeService:List_GetByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:List_GetByCompany")
     def get_by_company(self, company_id: int, employee_type: int) -> list[Employee]:
         """
         Get all employees that belong to a company and to a specific employee type.
 
         For more information, refer to the official documentation:
             [List_GetByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=List_GetByCompany)
 
@@ -171,15 +172,15 @@
             list[Employee]: A list of employee objects.
         """
         employees = self.client.service.List_GetByCompany(CompanyId=company_id, EmployeeType=employee_type, _soapheaders=self.auth_header)
         employees = [Employee(employee) for employee in serialize_object(employees)]
         return employees
 
     @return_list
-    @nmbrs_exception_handler(resources=["EmployeeService:List_GetByDebtor"])
+    @nmbrs_exception_handler(resource="EmployeeService:List_GetByDebtor")
     def get_by_debtor(self, debtor_id: int, employee_type: int) -> list[Employee]:
         """
         Get all employees that belong to a debtor and to a specific employee type.
 
         For more information, refer to the official documentation:
             [List_GetByDebtor](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=List_GetByDebtor)
 
@@ -190,128 +191,128 @@
         Returns:
             list[Employee]: A list of employee objects.
         """
         employees = self.client.service.List_GetByDebtor(DebtorId=debtor_id, EmployeeType=employee_type, _soapheaders=self.auth_header)
         employees = [Employee(employee) for employee in serialize_object(employees)]
         return employees
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employee_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employee_Insert")
     def insert(self):
         """
         Create a new Employee, returns the id of this Employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employee_InsertBasedOnDefault"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employee_InsertBasedOnDefault")
     def insert_based_on_default(self):
         """
         Insert new employee based on default employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_InsertBasedOnDefault](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_InsertBasedOnDefault)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employee_InsertByEmployeeType"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employee_InsertByEmployeeType")
     def insert_with_type(self):
         """
         Create a new employee based on the employee type and returns the Id of this employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_InsertByEmployeeType](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_InsertByEmployeeType)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employee_Transition"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employee_Transition")
     def transition(self):
         """
         Transition employee to a different employee type. For example, from applicant to new hire. Or from new hire to payroll.
 
         For more information, refer to the official documentation:
             [Employee_Transition](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_Transition)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:EndServiceReason_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:EndServiceReason_GetList")
     def get_all_end_service_reasons(self):
         """
         Get all End Service Reasons.
 
         For more information, refer to the official documentation:
             [EndServiceReason_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EndServiceReason_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:EndServiceReason_GetListByYear"])
+    @nmbrs_exception_handler(resource="EmployeeService:EndServiceReason_GetListByYear")
     def get_all_end_service_reasons_by_year(self):
         """
         Get all End Service Reasons of given year.
 
         For more information, refer to the official documentation:
             [EndServiceReason_GetListByYear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EndServiceReason_GetListByYear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:ExtraFieldsWithStartDate_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:ExtraFieldsWithStartDate_GetList")
     def get_extra_fields_with_start_date(self):
         """
         Get employee extra fields list, including the ones of type Text+Date.
 
         For more information, refer to the official documentation:
             [ExtraFieldsWithStartDate_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=ExtraFieldsWithStartDate_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:ExtraFields_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:ExtraFields_GetList")
     def get_extra_fields(self):
         """
         Get employee extra fields list.
 
         For more information, refer to the official documentation:
             [ExtraFields_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=ExtraFields_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:PerformanceReview_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:PerformanceReview_Get")
     def get_performance(self):
         """
         Get the HR Performance Review for the given Employee ID.
 
         For more information, refer to the official documentation:
             [PerformanceReview_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:PerformanceReview_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:PerformanceReview_GetAll_AllEmployeesByCompany")
     def get_all_performance_by_company(self):
         """
         Get the HR Performance Reviews for all the employees in the given Company ID.
 
         For more information, refer to the official documentation:
             [PerformanceReview_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Reports_GetJournalsReportByEmployee"])
+    @nmbrs_exception_handler(resource="EmployeeService:Reports_GetJournalsReportByEmployee")
     def get_journal(self):
         """
         Returns the Journal Report for Employee.
 
         For more information, refer to the official documentation:
             [Reports_GetJournalsReportByEmployee](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Reports_GetJournalsReportByEmployee)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Reservations_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Reservations_GetList")
     def get_reservations(self):
         """
         Get the reservation items for the given employee.
 
         For more information, refer to the official documentation:
             [Reservations_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Reservations_GetList)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/address.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/address.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:Address_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:Address_GetCurrent")
     def get(self, company_id: int) -> Address | None:
         """
         Get the current address of the company.
 
         For more information, refer to the official documentation:
             [Address_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Address_GetCurrent)
 
@@ -32,15 +32,15 @@
             Address | None: An Address object if found, otherwise None.
         """
         address = self.client.service.Address_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         if address is None:
             return None
         return Address(company_id=company_id, data=serialize_object(address))
 
-    @nmbrs_exception_handler(resources=["CompanyService:Address_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:Address_Insert")
     def insert(
         self,
         company_id: int,
         address_id: int,
         default: bool,
         street: str,
         house_number: str,
@@ -84,15 +84,15 @@
                 "StateProvince": state_province,
                 "CountryISOCode": country_iso_code,
             },
         }
         response = self.client.service.Address_Insert(**data, _soapheaders=self.auth_header)
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:Address_Update"])
+    @nmbrs_exception_handler(resource="CompanyService:Address_Update")
     def update(
         self,
         company_id: int,
         address_id: int,
         default: bool,
         street: str,
         house_number: str,
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:BankAccount_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:BankAccount_GetCurrent")
     def get_current(self, company_id: int) -> BankAccount | None:
         """
         Get the company's current bank account.
 
         For more information, refer to the official documentation:
             [BankAccount_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=BankAccount_GetCurrent)
 
@@ -32,15 +32,15 @@
             BankAccount: An BankAccount object.
         """
         bank_account = self.client.service.BankAccount_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         if bank_account is None:
             return None
         return BankAccount(company_id=company_id, data=serialize_object(bank_account))
 
-    @nmbrs_exception_handler(resources=["CompanyService:BankAccount_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:BankAccount_Insert")
     def insert(
         self,
         company_id: int,
         account_id: int,
         account_number: str,
         description: str,
         iban: str,
@@ -79,15 +79,15 @@
             "City": city,
             "Name": name,
             "Type": account_type,
         }
         response = self.client.service.BankAccount_Insert(CompanyId=company_id, BankAccount=bank_account, _soapheaders=self.auth_header)
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:BankAccount_Update"])
+    @nmbrs_exception_handler(resource="CompanyService:BankAccount_Update")
     def update(
         self,
         company_id: int,
         account_id: int,
         account_number: str,
         description: str,
         iban: str,
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:CostCenter_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:CostCenter_GetList")
     def get(self, company_id: int) -> list[CostCenter]:
         """
         Retrieve cost centers associated with a company.
 
         For further details, see the official documentation:
             [CostCenter_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostCenter_GetList)
 
@@ -32,15 +32,15 @@
 
         Returns:
             list[CostCenter]: A list of cost center objects.
         """
         cost_centers = self.client.service.CostCenter_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
         return [CostCenter(company_id=company_id, data=cost_center) for cost_center in serialize_object(cost_centers)]
 
-    @nmbrs_exception_handler(resources=["CompanyService:CostCenter_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:CostCenter_Insert")
     def insert(self, company_id: int, cost_center_id: int, code: str, description: str) -> int:
         """
         Insert or update a cost center within a company.
 
         For further details, see the official documentation:
             [CostCenter_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostCenter_Insert)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:CostUnit_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:CostUnit_GetList")
     def get(self, company_id: int) -> list[CostUnit]:
         """
         Get cost units that belong to a company
 
         For more information, refer to the official documentation:
             [CostUnit_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostUnit_GetList)
 
@@ -32,15 +32,15 @@
 
         Returns:
             list[CostUnit]: A list of cost unit objects.
         """
         cost_units = self.client.service.CostUnit_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
         return [CostUnit(company_id=company_id, data=cost_unit) for cost_unit in serialize_object(cost_units)]
 
-    @nmbrs_exception_handler(resources=["CompanyService:CostUnit_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:CostUnit_Insert")
     def insert(self, company_id: int, cost_unit_id: int, code: str, description: str) -> int:
         """
         Update or insert a Cost Unit into a company.
 
         For more information, refer to the official documentation:
             [CostUnit_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostUnit_Insert)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:HourModel_GetHourCodes"])
+    @nmbrs_exception_handler(resource="CompanyService:HourModel_GetHourCodes")
     def get(self, company_id: int) -> list[HourCode]:
         """
         Get hour codes that belong to a company's hour model.
 
         For more information, refer to the official documentation:
             [HourModel_GetHourCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HourModel_GetHourCodes)
 
@@ -33,15 +33,15 @@
         Returns:
             list[HourCode]: A list of hour code objects.
         """
         hour_codes = self.client.service.HourModel_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_header)
         return [HourCode(company_id=company_id, data=hour_code) for hour_code in serialize_object(hour_codes)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:HourModel2_GetHourCodes"])
+    @nmbrs_exception_handler(resource="CompanyService:HourModel2_GetHourCodes")
     def get_2(self, company_id: int) -> list[HourCode]:
         """
         Get hour codes that belong to a company's hour model 2.
 
         For more information, refer to the official documentation:
             [HourModel2_GetHourCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HourModel2_GetHourCodes)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/journal.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,105 +11,105 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCompany")
     def get_run_by_company(self):
         """
         Returns the Journal XML, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCompany](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCompany_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCompany_v2")
     def get_run_by_company_2(self):
         """
         Returns the Journal XML.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCompany_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCompany_v2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCostCenter"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCostCenter")
     def get_run_by_cost_center(self):
         """
         Returns the Journal XML, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCostCenter](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCostCenter)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCostCenter_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCostCenter_v2")
     def get_run_by_cost_center_2(self):
         """
         Returns the Journal XML.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCostCenter_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCostCenter_v2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCostCenterCostUnit"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCostCenterCostUnit")
     def get_run_by_cost_center_nad_cost_unit(self):
         """
         Returns the Journal XML with Cost Center/Cost Unit information, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCostCenterCostUnit](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCostCenterCostUnit)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunCostCenterCostUnitPerYear"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCostCenterCostUnitPerYear")
     def get_run_by_cost_center_nad_cost_unit_per_year(self):
         """
         Returns the Journal XML with Cost Center/Cost Unit information of the given year.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunCostCenterCostUnitPerYear](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunCostCenterCostUnitPerYear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunDepartment"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunDepartment")
     def get_run_by_department(self):
         """
         Returns the Journal XML, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunDepartment](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunDepartment)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunDepartment_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunDepartment_v2")
     def get_run_by_department_2(self):
         """
         Returns the Journal XML.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunDepartment_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunDepartment_v2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunEmployee"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunEmployee")
     def get_run_by_employee(self):
         """
         Returns the Journal XML, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunEmployee](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunEmployee)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:Journals_GetByRunEmployee_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunEmployee_v2")
     def get_run_by_employee_2(self):
         """
         Returns the Journal XML.
 
         For more information, refer to the official documentation:
             [Journals_GetByRunEmployee_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Journals_GetByRunEmployee_v2)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:LabourAgreements_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:LabourAgreements_Get")
     def get(self, company_id: int, period: int, year: int):
         """
         Get a list of all the labour agreements that are assigned to a company.
 
         For more information, refer to the official documentation:
             [LabourAgreements_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=LabourAgreements_Get)
 
@@ -45,15 +45,15 @@
         )
         labour_agreements = [
             LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:LabourAgreements_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:LabourAgreements_GetCurrent")
     def get_current(self, company_id: int):
         """
         Get a list of current labour agreements assigned to a company.
 
         For more information, refer to the official documentation:
             [LabourAgreements_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=LabourAgreements_GetCurrent)
 
@@ -66,15 +66,15 @@
         labour_agreements = self.client.service.LabourAgreements_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         labour_agreements = [
             LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:CompanyLeaveTypeGroups_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:CompanyLeaveTypeGroups_Get")
     def get_leave_type_groups(
         self, company_id: int, labour_agreement_settings_group_id: int, year: int, period: int
     ) -> list[LeaveTypeGroup]:
         """
         Get the company's leave type groups.
 
         For further details, see the official documentation:
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/pension.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:PensionExport_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetList")
     def get(self, company_id: int) -> list[Pension]:
         """
         Returns pension exports that belong to a company for a certain year.
 
         For more information, refer to the official documentation:
             [PensionExport_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=PensionExport_GetList)
 
@@ -32,15 +32,15 @@
 
         Returns:
             list[Pension]: A list of pension objects.
         """
         pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
         return [Pension(company_id=company_id, data=pension) for pension in serialize_object(pensions)]
 
-    @nmbrs_exception_handler(resources=["CompanyService:PensionExport_GetXML"])
+    @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetXML")
     def get_xml(self, company_id: int, pension_export_id: int) -> PensionXML:
         """
         Returns one XML pension export by ID that belong to a company.
 
         For more information, refer to the official documentation:
             [PensionExport_GetXML](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=PensionExport_GetXML)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/run.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:RunRequest_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:RunRequest_GetList")
     def get_requests(self, company_id: int, year: int) -> list[RunRequest]:
         """
         Returns a list of requested runs with status for given company and year.
 
         For more information, refer to the official documentation:
             [RunRequest_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=RunRequest_GetList)
 
@@ -34,29 +34,29 @@
 
         Returns:
             list[RunRequest]: A list of run requests objects.
         """
         run_requests = self.client.service.RunRequest_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
         return [RunRequest(company_id=company_id, data=run_request) for run_request in serialize_object(run_requests)]
 
-    @nmbrs_exception_handler(resources=["CompanyService:RunRequest_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:RunRequest_Insert")
     def insert_request(self, company_id: int):
         """
         Requests a run for given company.
 
         For more information, refer to the official documentation:
             [RunRequest_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=RunRequest_Insert)
 
         Args:
             company_id (int): The ID of the company.
         """
         self.client.service.RunRequest_Insert(CompanyId=company_id, _soapheaders=self.auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:Run_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:Run_GetList")
     def get(self, company_id: int, year: int) -> list[RunInfo]:
         """
         Get the company's run list for a specified year.
 
         For more information, refer to the official documentation:
             [Run_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Run_GetList)
 
@@ -67,15 +67,15 @@
         Returns:
             list[RunInfo]: A list of run info objects.
         """
         runs = self.client.service.Run_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
         return [RunInfo(company_id=company_id, data=run) for run in serialize_object(runs)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:Run_GetEmployeesByRunCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:Run_GetEmployeesByRunCompany")
     def get_all_employees_by_run(self, company_id: int, year: int, run_id: int) -> list[Employee]:
         """
         Get the employee's list for a specified company id, run id and year
 
         For more information, refer to the official documentation:
             [Run_GetEmployeesByRunCompany](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Run_GetEmployeesByRunCompany)
 
@@ -91,15 +91,15 @@
             CompanyId=company_id, Year=year, RunId=run_id, _soapheaders=self.auth_header
         )
         return [
             Employee({"Id": employee.get("EmployeeId"), "Number": employee.get("EmployeeNumber")})
             for employee in serialize_object(employees)
         ]
 
-    @nmbrs_exception_handler(resources=["CompanyService:HrDocuments_EmployerCostPerHour_Year"])
+    @nmbrs_exception_handler(resource="CompanyService:HrDocuments_EmployerCostPerHour_Year")
     def get_hr_documents_cost_per_hour_year(self, company_id: int, run_id: int, year: int, period: int) -> bytes:
         """
         Get HR Document: Employer Cost per Hour per company per period.
 
         For further details, see the official documentation:
             [HrDocuments_EmployerCostPerHour_Year](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HrDocuments_EmployerCostPerHour_Year)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,225 +11,225 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_AnualStatement"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_AnualStatement")
     def get_annual_statement(self):
         """
         Get Annual Statement in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_AnualStatement](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_AnualStatement)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_CompanyWageComponentsCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_CompanyWageComponentsCumulative")
     def get_annual_wage_components(self):
         """
         Get Annual Company Wage Components Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_CompanyWageComponentsCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_CompanyWageComponentsCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesCompanyrCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesCompanyrCumulative")
     def get_annual_journal_entries_company(self):
         """
         Get Annual Journal Entries company Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_JournalEntriesCompanyrCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_JournalEntriesCompanyrCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesCostCenterCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesCostCenterCumulative")
     def get_annual_journal_entries_cost_center(self):
         """
         Get Annual Journal Entries Cost Center Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_JournalEntriesCostCenterCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_JournalEntriesCostCenterCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesDepartmentCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesDepartmentCumulative")
     def get_annual_journal_entries_department(self):
         """
         Get Annual Journal Entries Department Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_JournalEntriesDepartmentCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_JournalEntriesDepartmentCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesEmployeeCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_JournalEntriesEmployeeCumulative")
     def get_annual_journal_entries_employee(self):
         """
         Get Annual Journal Entries Employee Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_JournalEntriesEmployeeCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_JournalEntriesEmployeeCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_LeaveSaldos"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_LeaveSaldos")
     def get_annual_leave_saldo(self):
         """
         Get Annual Leave Saldos in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_LeaveSaldos](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_LeaveSaldos)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_PaymentListCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_PaymentListCumulative")
     def get_annual_payment_list(self):
         """
         Get Annual Payment List Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_PaymentListCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_PaymentListCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_PayrollRegister"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_PayrollRegister")
     def get_annual_payroll(self):
         """
         Get Annual Journal Entries Department Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_PayrollRegister](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_PayrollRegister)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_PayrollRegisterAllEmployees"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_PayrollRegisterAllEmployees")
     def get_annual_payroll_employees(self):
         """
         Get Annual PayrollRegister All Employee in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_PayrollRegisterAllEmployees](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_PayrollRegisterAllEmployees)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_PayrollRegisterSummaryCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_PayrollRegisterSummaryCumulative")
     def get_annual_payroll_summary(self):
         """
         Get Annual Payroll Register Summary Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_PayrollRegisterSummaryCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_PayrollRegisterSummaryCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_ReservationSaldos"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_ReservationSaldos")
     def get_annual_reservation_saldo(self):
         """
         Get Annual Reservation Saldo in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_ReservationSaldos](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_ReservationSaldos)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_SentWageTaxDeclarations"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_SentWageTaxDeclarations")
     def get_annual_wage_tax_declaration(self):
         """
         Get Annual Document Sent Wage Tax Declarations in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_SentWageTaxDeclarations](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_SentWageTaxDeclarations)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewByPeriod"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewByPeriod")
     def get_annual_wage_tax_declaration_by_period(self):
         """
         Get Annual Document WageTax Declaration Overview Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewByPeriod](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewByPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewCumulative"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewCumulative")
     def get_annual_wage_tax_declaration_cumulative(self):
         """
         Get Annual Document WageTax Declaration Overview Cumulative in PDF.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewCumulative](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_AnnualDocument_WageTaxDeclarationOverviewCumulative)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetAllPayslipsPDFByRunCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetAllPayslipsPDFByRunCompany")
     def get_annual_all_payslips(self):
         """
         Get all payslip PDF's of a company for a specific run period, takes year from active year of the company.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetAllPayslipsPDFByRunCompany](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetAllPayslipsPDFByRunCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetAllPayslipsPDFByRunCompany_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetAllPayslipsPDFByRunCompany_v2")
     def get_annual_all_payslips_2(self):
         """
         Get all payslip PDF's of a company for a specific run period.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetAllPayslipsPDFByRunCompany_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetAllPayslipsPDFByRunCompany_v2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetEmployeePayslipsInOnePDFByRunCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetEmployeePayslipsInOnePDFByRunCompany")
     def get_annual_all_payslips_as_one(self):
         """
         Get all employees payslips in one PDF by run company for a specific run period.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetEmployeePayslipsInOnePDFByRunCompany](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetEmployeePayslipsInOnePDFByRunCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetEmployeePayslipsPDFByRunCompany"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetEmployeePayslipsPDFByRunCompany")
     def get_annual_all_payslips_by_employee(self):
         """
         Get employee payslips in PDF by run company for a specific run period, takes year from active year of the company
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetEmployeePayslipsPDFByRunCompany](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetEmployeePayslipsPDFByRunCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetEmployeePayslipsPDFByRunCompany_v2"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetEmployeePayslipsPDFByRunCompany_v2")
     def get_annual_all_payslips_by_employee_2(self):
         """
         Get employee payslips in PDF by run company for a specific run period.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetEmployeePayslipsPDFByRunCompany_v2](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetEmployeePayslipsPDFByRunCompany_v2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetSEPA"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetSEPA")
     def get_SEPA(self):
         """
         Get SEPA file.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetSEPA](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetSEPA)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryDocuments_GetSEPA_Tax"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_GetSEPA_Tax")
     def get_SEPA_tax(self):
         """
         Get SEPA Tax file.
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetSEPA_Tax](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryDocuments_GetSEPA_Tax)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable_Get")
     def get(self, company_id: int, period: int, year: int) -> list[SalaryTable]:
         """
         Returns a list of available tables for the company.
 
         For more information, refer to the official documentation:
             [SalaryTable_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable_Get)
 
@@ -35,15 +35,15 @@
         Returns:
             list[SalaryTable]: A list of salary table objects.
         """
         salary_tables = self.client.service.SalaryTable_Get(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
         return [SalaryTable(company_id=company_id, data=salary_table) for salary_table in serialize_object(salary_tables)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_Get")
     def get_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available tables for the company with unique identifiers.
 
         For more information, refer to the official documentation:
             [SalaryTable2_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable2_Get)
 
@@ -55,15 +55,15 @@
         Returns:
             list[str]: A list of salary table guids.
         """
         salary_tables = self.client.service.SalaryTable2_Get(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
         return [salary_table.get("GuidSalaryTable") for salary_table in serialize_object(salary_tables)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable_GetScales"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable_GetScales")
     def get_scale(self, company_id: int, period: int, year: int) -> list[SalaryTableScale]:
         """
         Returns a list of available scales for the company salary table.
 
         For more information, refer to the official documentation:
             [SalaryTable_GetScales](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable_GetScales)
 
@@ -75,15 +75,15 @@
         Returns:
             list[SalaryTableScale]: A list of salary table scale objects.
         """
         scales = self.client.service.SalaryTable_GetScales(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
         return [SalaryTableScale(company_id=company_id, data=scale) for scale in serialize_object(scales)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_GetScales"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_GetScales")
     def get_scale_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available scales for the company salary table with unique identifiers.
 
         For more information, refer to the official documentation:
             [SalaryTable2_GetScales](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable2_GetScales)
 
@@ -97,15 +97,15 @@
         """
         salary_tables = self.client.service.SalaryTable2_GetScales(
             CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
         )
         return [salary_table.get("GuidSalaryTableScale") for salary_table in serialize_object(salary_tables)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable_GetSteps"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable_GetSteps")
     def get_step(self, company_id: int, period: int, year: int, scale: SalaryTableScale) -> list[SalaryTableStep]:
         """
         Returns a list of available steps for the company salary table and selected scale.
 
         For more information, refer to the official documentation:
             [SalaryTable_GetSteps](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable_GetSteps)
 
@@ -127,15 +127,15 @@
         }
         steps = self.client.service.SalaryTable_GetSteps(
             CompanyId=company_id, Period=period, Year=year, Scale=_scale, _soapheaders=self.auth_header
         )
         return [SalaryTableStep(company_id=company_id, data=step) for step in serialize_object(steps)]
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:SalaryTable2_GetSteps"])
+    @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_GetSteps")
     def get_step_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available steps for the company salary table and selected scale with unique identifiers.
 
         For more information, refer to the official documentation:
             [SalaryTable2_GetSteps](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SalaryTable2_GetSteps)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/svw.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["CompanyService:SVW_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:SVW_GetCurrent")
     def get_current(self, company_id: int) -> SVW:
         """
         Get the current SVW settings.
 
         For more information, refer to the official documentation:
             [SVW_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SVW_GetCurrent)
 
@@ -30,15 +30,15 @@
 
         Returns:
             SVW: object representing svw settings
         """
         svw = self.client.service.SVW_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         return SVW(company_id=company_id, data=serialize_object(svw))
 
-    @nmbrs_exception_handler(resources=["CompanyService:SVW_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:SVW_UpdateCurrent")
     def insert_current(self, company_id: int, svw: SVW) -> None:
         """
         Update the current SVW settings.
 
         For more information, refer to the official documentation:
             [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SVW_UpdateCurrent)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Get")
     def fixed_get(self, company_id: int, year: int, period: int) -> list[WageComponent]:
         """
         Retrieve all fixed wage components for a specified company, year, and period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Get)
 
@@ -41,15 +41,15 @@
         wage_components = [
             WageComponent(company_id=company_id, component_type="fixed", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_GetCurrent")
     def fixed_get_current(self, company_id: int):
         """
         Retrieve all fixed wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_GetCurrent)
 
@@ -62,15 +62,15 @@
         wage_components = self.client.service.WageComponentFixed_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         wage_components = [
             WageComponent(company_id=company_id, component_type="fixed", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Insert")
     def fixed_insert(
         self,
         wage_component: WageComponent,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> int:
@@ -96,15 +96,15 @@
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
             _soapheaders=self.auth_header,
         )
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_InsertCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_InsertCurrent")
     def fixed_insert_current(self, wage_component: WageComponent) -> int:
         """
         Insert a fixed wage component for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_InsertCurrent)
 
@@ -117,15 +117,15 @@
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentFixed_InsertCurrent(
             CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_header
         )
         return response
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Insert_Batch"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Insert_Batch")
     def fixed_insert_batch(
         self,
         wage_components: list[WageComponent],
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
@@ -155,15 +155,15 @@
                 }
             )
         response = self.client.service.WageComponentFixed_Insert_Batch(
             WageComponents=new_wage_components, Period=period, Year=year, UnprotectedMode=protected_mode, _soapheaders=self.auth_header
         )
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentFixed_Stop"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Stop")
     def fixed_stop(
         self,
         company_id: int,
         component_id: int,
         period: int,
         year: int,
         protected_mode: bool,
@@ -190,15 +190,15 @@
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
             _soapheaders=self.auth_header,
         )
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Get"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Get")
     def variable_get(self, company_id: int, year: int, period: int) -> list[WageComponent]:
         """
         Retrieve all variable wage components for a specified company, year, and period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Get)
 
@@ -216,15 +216,15 @@
         wage_components = [
             WageComponent(company_id=company_id, component_type="variable", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_GetCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_GetCurrent")
     def variable_get_current(self, company_id: int) -> list[WageComponent]:
         """
         Retrieve all variable wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_GetCurrent)
 
@@ -237,15 +237,15 @@
         wage_components = self.client.service.WageComponentVar_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
         wage_components = [
             WageComponent(company_id=company_id, component_type="variable", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Insert")
     def variable_insert(
         self,
         wage_component: WageComponent,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> int:
@@ -271,15 +271,15 @@
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
             _soapheaders=self.auth_header,
         )
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_InsertCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_InsertCurrent")
     def variable_insert_current(self, wage_component: WageComponent) -> int:
         """
         Insert a variable wage component for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_InsertCurrent)
 
@@ -292,15 +292,15 @@
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentVar_InsertCurrent(
             CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_header
         )
         return response
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Insert_Batch"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Insert_Batch")
     def variable_insert_batch(
         self,
         wage_components: list[WageComponent],
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
@@ -330,15 +330,15 @@
                 }
             )
         response = self.client.service.WageComponentVar_Insert_Batch(
             WageComponents=new_wage_components, Period=period, Year=year, UnprotectedMode=protected_mode, _soapheaders=self.auth_header
         )
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_Clear"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Clear")
     def variable_clear(
         self,
         company_id: int,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
@@ -362,15 +362,15 @@
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
             _soapheaders=self.auth_header,
         )
         return response
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageComponentVar_ClearCurrent"])
+    @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_ClearCurrent")
     def variable_clear_current(self, company_id: int) -> list[int]:
         """
         Clear all variable wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_ClearCurrent)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WorkCost_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:WorkCost_GetList")
     def get(self, company_id: int, year: int) -> list[WageCost]:
         """
         Retrieve the list of work cost values for a given company and year.
 
         For more information, refer to the official documentation:
             [WorkCost_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WorkCost_GetList)
 
@@ -34,15 +34,15 @@
         Returns:
             list[WageCost]: A list of work cost values.
         """
         wage_costs = self.client.service.WorkCost_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
         wage_costs = [WageCost(company_id=company_id, data=wage_cost) for wage_cost in serialize_object(wage_costs)]
         return wage_costs
 
-    @nmbrs_exception_handler(resources=["CompanyService:WorkCost_Insert"])
+    @nmbrs_exception_handler(resource="CompanyService:WorkCost_Insert")
     def insert(self, company_id: int, value: float, period: int, year: int):
         """
         Insert a work cost value from the financial administration for a specific period.
 
         For more information, refer to the official documentation:
             [WorkCost_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WorkCost_Insert)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageModel_GetWageCodes"])
+    @nmbrs_exception_handler(resource="CompanyService:WageModel_GetWageCodes")
     def get(self, company_id: int) -> list[WageModel]:
         """
         Retrieve the list of wage codes belonging to a company's wage model.
 
         For more information, refer to the official documentation:
             [WageModel_GetWageCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageModel_GetWageCodes)
 
@@ -34,15 +34,15 @@
             list[WageModel]: A list of wage codes belonging to the company's wage model.
         """
         wage_models = self.client.service.WageModel_GetWageCodes(CompanyId=company_id, _soapheaders=self.auth_header)
         wage_models = [WageModel(company_id=company_id, data=wage_model) for wage_model in serialize_object(wage_models)]
         return wage_models
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageModel2_GetWageCodes"])
+    @nmbrs_exception_handler(resource="CompanyService:WageModel2_GetWageCodes")
     def get_2(self, company_id: int) -> list[WageModel]:
         """
         Retrieve the list of wage codes belonging to a company's wage model.
 
         For more information, refer to the official documentation:
             [WageModel2_GetWageCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageModel2_GetWageCodes)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["CompanyService:WageTax_GetList"])
+    @nmbrs_exception_handler(resource="CompanyService:WageTax_GetList")
     def get_all_wagetax(self, company_id: int, year: int) -> list[WageTax]:
         """
         Retrieve all wage taxes for a specific company and year.
 
         For more information, refer to the official documentation:
             [WageTax_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetList)
 
@@ -34,15 +34,15 @@
         Returns:
             list[WageTax]: A list of WageTax objects for the specified company and year.
         """
         wage_taxes = self.client.service.WageTax_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_header)
         wage_taxes = [WageTax(company_id=company_id, data=wage_tax) for wage_tax in serialize_object(wage_taxes)]
         return wage_taxes
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageTax_GetXML"])
+    @nmbrs_exception_handler(resource="CompanyService:WageTax_GetXML")
     def get_wagetax_details(self, company_id: int, loonaangifte_id: int) -> WageTaxXML:
         """
         Retrieve wage tax details for a specific company and loonaangifte ID.
 
         For more information, refer to the official documentation:
             [WageTax_GetXML](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_GetXML)
 
@@ -57,15 +57,15 @@
             CompanyId=company_id,
             LoonaangifteID=loonaangifte_id,
             _soapheaders=self.auth_header,
         )
         wage_tax_details = WageTaxXML(wage_tax_details)
         return wage_tax_details
 
-    @nmbrs_exception_handler(resources=["CompanyService:WageTax_SetSentExternal"])
+    @nmbrs_exception_handler(resource="CompanyService:WageTax_SetSentExternal")
     def set_send_as_external(self, company_id: int, loonaangifte_id: int) -> bool:
         """
         Set the wage tax status to Sent as External.
 
         For more information, refer to the official documentation:
             [WageTax_SetSentExternal](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageTax_SetSentExternal)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/department.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["DebtorService:Department_Delete"])
+    @nmbrs_exception_handler(resource="DebtorService:Department_Delete")
     def delete(self, debtor_id: int, department_id: int) -> None:
         """
         Delete a department of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_Delete](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_Delete)
 
         Args:
             debtor_id (int): The ID of the debtor.
             department_id (int): The ID of the department to delete.
         """
         self.client.service.Department_Delete(DebtorId=debtor_id, id=department_id, _soapheaders=self.auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:Department_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:Department_GetList")
     def get_all(self, debtor_id: int) -> list[Department]:
         """
         Retrieve all departments of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_GetList)
 
@@ -47,15 +47,15 @@
         Returns:
             list[Department]: A list of Department objects representing all departments of the debtor.
         """
         departments = self.client.service.Department_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
         departments = [Department(debtor_id=debtor_id, data=department) for department in serialize_object(departments)]
         return departments
 
-    @nmbrs_exception_handler(resources=["DebtorService:Department_Insert"])
+    @nmbrs_exception_handler(resource="DebtorService:Department_Insert")
     def insert(self, debtor_id: int, department_id: int, code: int, description: str) -> int:
         """
         Insert a new department for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_Insert)
 
@@ -75,15 +75,15 @@
                 "Code": code,
                 "Description": description,
             },
         }
         inserted = self.client.service.Department_Insert(**data, _soapheaders=self.auth_header)
         return inserted
 
-    @nmbrs_exception_handler(resources=["DebtorService:Department_Update"])
+    @nmbrs_exception_handler(resource="DebtorService:Department_Update")
     def update(self, debtor_id: int, department_id: int, code: int, description: str) -> None:
         """
         Update an existing department of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_Update](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_Update)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/function.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["DebtorService:Function_Delete"])
+    @nmbrs_exception_handler(resource="DebtorService:Function_Delete")
     def delete(self, debtor_id: int, function_id: int) -> None:
         """
         Delete a function of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_Delete](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_Delete)
 
         Args:
             debtor_id (int): The ID of the debtor.
             function_id (int): The ID of the function to be deleted.
         """
         self.client.service.Function_Delete(DebtorId=debtor_id, id=function_id, _soapheaders=self.auth_header)
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:Function_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:Function_GetList")
     def get_all(self, debtor_id: int) -> list[Function]:
         """
         Retrieve all functions of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_GetList)
 
@@ -48,15 +48,15 @@
         Returns:
             list[Function]: A list of Function objects representing all functions of the debtor.
         """
         functions = self.client.service.Function_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
         functions = [Function(debtor_id=debtor_id, data=function) for function in serialize_object(functions)]
         return functions
 
-    @nmbrs_exception_handler(resources=["DebtorService:Function_Insert"])
+    @nmbrs_exception_handler(resource="DebtorService:Function_Insert")
     def insert(self, debtor_id: int, function_id: int, code: int, description: str) -> int:
         """
         Insert a new function for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_Insert)
 
@@ -72,15 +72,15 @@
         data = {
             "DebtorId": debtor_id,
             "function": {"Id": function_id, "Code": code, "Description": description},
         }
         inserted = self.client.service.Function_Insert(**data, _soapheaders=self.auth_header)
         return inserted
 
-    @nmbrs_exception_handler(resources=["DebtorService:Function_Update"])
+    @nmbrs_exception_handler(resource="DebtorService:Function_Update")
     def update(self, debtor_id: int, function_id: int, code: int, description: str) -> None:
         """
         Update a function for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_Update](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_Update)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/title.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:Title_GetList"])
+    @nmbrs_exception_handler(resource="DebtorService:Title_GetList")
     def get_all(self, debtor_id: int) -> list[str]:
         """
         Retrieve all titles for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Title_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Title_GetList)
 
@@ -32,15 +32,15 @@
         Returns:
             list[str]: A list of strings representing all titles associated with the debtor.
         """
         titles = self.client.service.Title_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
         titles = [title["TitleName"] for title in serialize_object(titles)]
         return titles
 
-    @nmbrs_exception_handler(resources=["DebtorService:Title_Insert"])
+    @nmbrs_exception_handler(resource="DebtorService:Title_Insert")
     def insert(self, debtor_id: int, title: str) -> None:
         """
         Insert a title for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Title_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Title_Insert)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["DebtorService:WebhookSettings_Delete"])
+    @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Delete")
     def delete(self, debtor_id: int, webhook_id: int) -> bool:
         """
         Delete a webhook for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Delete](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=WebhookSettings_Delete)
 
@@ -37,15 +37,15 @@
             DebtorId=debtor_id,
             WebhookSettingId=webhook_id,
             _soapheaders=self.auth_header,
         )
         return deleted
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:WebhookSettings_Get"])
+    @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Get")
     def get_all(self, debtor_id: int) -> list[WebhookSetting]:
         """
         Retrieve all webhooks for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Get](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=WebhookSettings_Get)
 
@@ -56,30 +56,30 @@
             list[WebhookSetting]: A list of WebhookSetting objects representing all webhooks associated with the debtor.
         """
         webhooks = self.client.service.WebhookSettings_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
         webhooks = [WebhookSetting(debtor_id=debtor_id, data=webhook) for webhook in serialize_object(webhooks)]
         return webhooks
 
     @return_list
-    @nmbrs_exception_handler(resources=["DebtorService:WebhookSettings_GetEvents"])
+    @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_GetEvents")
     def get_all_events(self) -> list[Event]:
         """
         Retrieve all webhook events.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_GetEvents](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=WebhookSettings_GetEvents)
 
         Returns:
             list[Event]: A list of Event objects representing all webhook events.
         """
         events = self.client.service.WebhookSettings_GetEvents(_soapheaders=self.auth_header)
         events = [Event(event) for event in serialize_object(events)]
         return events
 
-    @nmbrs_exception_handler(resources=["DebtorService:WebhookSettings_Insert"])
+    @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Insert")
     def insert(self, debtor_id: int, insert_webhook_settings: WebhookSetting) -> int:
         """
         Insert a webhook for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=WebhookSettings_Insert)
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-# pylint: disable=line-too-long
-"""Microservice responsible for absence related actions on the employee level."""
+"""Microservice responsible for lease car related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeAbsenceService(MicroService):
-    """Microservice responsible for absence related actions on the employee level."""
+class EmployeeLeaseCarService(MicroService):
+    """Microservice responsible for lease car related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Get")
     def get(self):
         """
-        Get a list of all absences.
+        Get the active lease car contract for given period.
 
         For more information, refer to the official documentation:
-            [Absence_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_GetList)
+            [LeaseCar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence2_GetList"])
-    def get_2(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_GetCurrent")
+    def get_current(self):
         """
-        Get a list of all absences with their respective cause.
+        Get currently active lease car contract.
 
         For more information, refer to the official documentation:
-            [Absence2_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_GetList)
+            [LeaseCar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_GetList")
+    def get_all(self):
+        """
+        Get lease car contract list, until given period.
+
+        For more information, refer to the official documentation:
+            [LeaseCar_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetList)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_GetAll_EmployeesByCompany")
     def get_all_by_company(self):
         """
-        Get a list of all absence of all company employees.
+        Get lease car contract list for all employee in company, until given period.
 
         For more information, refer to the official documentation:
-            [Absence_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_GetAll_AllEmployeesByCompany)
+            [LeaseCar_GetAll_EmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetAll_EmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence_Insert"])
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar2_GetAll_EmployeesByCompany")
+    def get_all_by_company_2(self):
         """
-        Insert an absence, this item will start from the given date in the object.
+        Get lease car contract list for all employee in company, until given period.
 
         For more information, refer to the official documentation:
-            [Absence_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_Insert)
+            [LeaseCar2_GetAll_EmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar2_GetAll_EmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence2_Insert"])
-    def insert_2(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Insert")
+    def insert(self):
         """
-        Insert an absence with cause, this item will start from the given date in the object.
+        Insert a new lease car contract, this contract will start from given date within the object.
 
         For more information, refer to the official documentation:
-            [Absence2_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_Insert)
+            [LeaseCar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence_PartialRecoveryInsert"])
-    def insert_partial_recovery(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_InsertCurrent")
+    def insert_current(self):
         """
-        Insert an absence partial recovery message.
+        Insert a new lease car contract, this contract will start from given date within the object.
 
         For more information, refer to the official documentation:
-            [Absence_PartialRecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_PartialRecoveryInsert)
+            [LeaseCar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Absence_RecoveryInsert"])
-    def insert_recovery(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Delete")
+    def delete(self):
         """
-        Insert an absence recovery message.
+        Delete a lease car contract. This action can not be undone.
 
         For more information, refer to the official documentation:
-            [Absence_RecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_RecoveryInsert)
+            [LeaseCar_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:AbsenceNotification_Insert"])
-    def insert_notification(self):
+    @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Stop")
+    def stop(self):
         """
-        Insert a new absence date, this item will start from the given date in the object to the requested absence dossier.
+        Stop the currently active lease car contract.
 
         For more information, refer to the official documentation:
-            [AbsenceNotification_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=AbsenceNotification_Insert)
+            [LeaseCar_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/address.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_GetList")
     def get(self):
         """
         Get all addresses which are active in given period.
 
         For more information, refer to the official documentation:
             [Address_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_GetListCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_GetListCurrent")
     def get_current(self):
         """
         Get all currently active addresses.
 
         For more information, refer to the official documentation:
             [Address_GetListCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetListCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get all addresses of all employees.
 
         For more information, refer to the official documentation:
             [Address_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_Delete")
     def delete(self):
         """
         Get all active bank accounts for given period.
 
         For more information, refer to the official documentation:
             [Address_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_Update")
     def update(self):
         """
         Delete Employee Address.
 
         For more information, refer to the official documentation:
             [Address_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_Insert")
     def insert(self):
         """
         Insert given address to the specified period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Address_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Address_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Address_InsertCurrent")
     def insert_current(self):
         """
         Insert given address to the current period.
 
         For more information, refer to the official documentation:
             [Address_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_InsertCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,55 +11,55 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:BankAccount_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetList")
     def get(self):
         """
         Get all active bank accounts for given period.
 
         For more information, refer to the official documentation:
             [BankAccount_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:BankAccount_GetListCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetListCurrent")
     def get_current(self):
         """
         Get all active bank accounts for the current period.
 
         For more information, refer to the official documentation:
             [BankAccount_GetListCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_GetListCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:BankAccount_DeleteCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_DeleteCurrent")
     def delete(self):
         """
         Delete given bank account.
 
         For more information, refer to the official documentation:
             [BankAccount_DeleteCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_DeleteCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:BankAccount_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_Insert")
     def insert(self):
         """
         Insert given bank account to the given period. Unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [BankAccount_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:BankAccount_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_InsertCurrent")
     def insert_current(self):
         """
         Insert given bank account to the current period.
 
         For more information, refer to the official documentation:
             [BankAccount_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_InsertCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/child.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,65 +11,65 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Children_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Children_Get")
     def get(self):
         """
         Get employee childs.
 
         For more information, refer to the official documentation:
             [Children_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Children_GetAll_Employeesbycompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Children_GetAll_Employeesbycompany")
     def get_all_by_company(self):
         """
         Get employee childs.
 
         For more information, refer to the official documentation:
             [Children_GetAll_Employeesbycompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_GetAll_Employeesbycompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Child_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Child_Delete")
     def delete(self):
         """
         Delete's child.
 
         For more information, refer to the official documentation:
             [Child_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Child_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Children_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Children_Insert")
     def insert(self):
         """
         Insert an employee child.
 
         For more information, refer to the official documentation:
             [Children_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Children_InsertBatch"])
+    @nmbrs_exception_handler(resource="EmployeeService:Children_InsertBatch")
     def insert_batch(self):
         """
         Insert employee children.
 
         For more information, refer to the official documentation:
             [Children_InsertBatch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_InsertBatch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Children_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Children_Update")
     def update(self):
         """
         Update employee child.
 
         For more information, refer to the official documentation:
             [Children_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_Update)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/contract.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetAll"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_GetAll")
     def get_all(self):
         """
         Get all contracts for the specified employee.
 
         For more information, refer to the official documentation:
             [Contract_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetAll)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetCurrentPeriod"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_GetCurrentPeriod")
     def get_current(self):
         """
         Get a list of all active contracts for specified employee in current period.
 
         For more information, refer to the official documentation:
             [Contract_GetCurrentPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetCurrentPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @return_list
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[Contract]:
         """
         Get all contracts of all employees.
 
         For more information, refer to the official documentation:
             [Contract_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetAll_AllEmployeesByCompany)
 
@@ -58,45 +58,45 @@
         contracts = serialize_object(contracts)
         _contracts = []
         for employee in contracts:
             for contract in employee["EmployeeContracts"]["EmployeeContract"]:
                 _contracts.append(Contract(employee_id=employee["EmployeeId"], data=contract))
         return _contracts
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_Delete")
     def delete(self):
         """
         Delete a contract from the system. This action can not be undone.
 
         For more information, refer to the official documentation:
             [Contract_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_Update")
     def update(self):
         """
         Update the specified contract for specified employee. Contract start date can’t be updated, this field will be ignored.
 
         For more information, refer to the official documentation:
             [Contract_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_Insert")
     def insert(self):
         """
         Insert Contract. If the start date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Contract_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Contract_InsertCurrentPeriod"])
+    @nmbrs_exception_handler(resource="EmployeeService:Contract_InsertCurrentPeriod")
     def insert_current(self):
         """
         Insert Contract in current period for specified employee.
 
         For more information, refer to the official documentation:
             [Contract_InsertCurrentPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_InsertCurrentPeriod)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,55 +11,55 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:CostCenter_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:CostCenter_Get")
     def get(self):
         """
         Get all cost center per employee.
 
         For more information, refer to the official documentation:
             [CostCenter_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:CostCenter_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:CostCenter_GetCurrent")
     def get_current(self):
         """
         Get all active cost centers of a specific employee on the current period.
 
         For more information, refer to the official documentation:
             [CostCenter_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:CostCenter_GetAllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:CostCenter_GetAllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get all cost centers of all employees per company.
 
         For more information, refer to the official documentation:
             [CostCenter_GetAllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_GetAllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:CostCenter_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:CostCenter_Update")
     def update(self):
         """
         Update cost center.
 
         For more information, refer to the official documentation:
             [CostCenter_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:CostCenter_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:CostCenter_UpdateCurrent")
     def update_current(self):
         """
         Update cost centers starting from the current period.
 
         For more information, refer to the official documentation:
             [CostCenter_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/days.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,125 +12,125 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Get")
     def fixed_get(self):
         """
         Get fixed days worked for given period.
 
         For more information, refer to the official documentation:
             [DaysFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_GetCurrent")
     def fixed_get_current(self):
         """
         Get fixed days worked for the current period.
 
         For more information, refer to the official documentation:
             [DaysFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_Set"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Set")
     def fixed_set(self):
         """
         Set fixed days for given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Set](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Set)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_SetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_SetCurrent")
     def fixed_set_current(self):
         """
         Set fixed days worked for the current period.
 
         For more information, refer to the official documentation:
             [DaysFixed_SetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_SetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_Set_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Set_Batch")
     def fixed_set_batch(self):
         """
         Set fixed days for given period for a batch of Employees. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Set_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Set_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysFixed_Stop"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Stop")
     def fixed_stop(self):
         """
         Stop fixed days, the given period is the last for these days. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVar_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVar_Get")
     def variable_get(self):
         """
         Get variable days worked for given period.
 
         For more information, refer to the official documentation:
             [DaysVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVar_Set_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVar_Set_Batch")
     def variable_set_batch(self):
         """
         Set variable days for given period for a batch of Employees. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysVar_Set_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVar_Set_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVarWorked_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_Get")
     def days_worked_get(self):
         """
         Get days worked and +/- days for wage components per day filled in for given period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVarWorked_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_GetCurrent")
     def days_worked_get_current(self):
         """
         Get days worked and +/- days for wage components per day for the current period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVarWorked_Set"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_Set")
     def days_worked_set(self):
         """
         Get days worked and +/- days for wage components per day for the current period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_Set](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_Set)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:DaysVarWorked_SetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_SetCurrent")
     def days_worked_set_current(self):
         """
         Set days worked and +/- days for wage components per day for the given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_SetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_SetCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/department.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Department_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Department_GetCurrent")
     def get_current(self):
         """
         Get the currently active department.
 
         For more information, refer to the official documentation:
             [Department_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Department_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Department_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get all department history of all employees.
 
         For more information, refer to the official documentation:
             [Department_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Department_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Department_UpdateCurrent")
     def update_current(self):
         """
         Update the department starting the current period.
 
         For more information, refer to the official documentation:
             [Department_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:EmployeeDocument_UploadDocument"])
+    @nmbrs_exception_handler(resource="EmployeeService:EmployeeDocument_UploadDocument")
     def upload(self):
         """
         Uploads document for employee.
 
         For more information, refer to the official documentation:
             [EmployeeDocument_UploadDocument](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EmployeeDocument_UploadDocument)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:EmployeeDocument_UploadDocumentFull"])
+    @nmbrs_exception_handler(resource="EmployeeService:EmployeeDocument_UploadDocumentFull")
     def upload_full(self):
         """
         Uploads document for employee with all the fields.
 
         For more information, refer to the official documentation:
             [EmployeeDocument_UploadDocumentFull](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EmployeeDocument_UploadDocumentFull)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/employment.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employment_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employment_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get all (historical) employment records for all employees that belong to the company.
 
         For more information, refer to the official documentation:
             [Employment_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employment_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Employment_UpdateEmploymentInitialStartDate"])
+    @nmbrs_exception_handler(resource="EmployeeService:Employment_UpdateEmploymentInitialStartDate")
     def update_start_date(self):
         """
         Update employee service initial start date.
 
         For more information, refer to the official documentation:
             [Employment_UpdateEmploymentInitialStartDate](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employment_UpdateEmploymentInitialStartDate)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Function_GetFunction"])
+    @nmbrs_exception_handler(resource="EmployeeService:Function_GetFunction")
     def get_by_id(self):
         """
         Get Function by functionID.
 
         For more information, refer to the official documentation:
             [Function_GetFunction](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetFunction)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Function_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Function_GetCurrent")
     def get_current(self):
         """
         Get the currently active function.
 
         For more information, refer to the official documentation:
             [Function_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Function_GetAll_AllEmployeesByCompany_V2"])
+    @nmbrs_exception_handler(resource="EmployeeService:Function_GetAll_AllEmployeesByCompany_V2")
     def get_all_by_company(self):
         """
         Get all Function history of all employees.
 
         For more information, refer to the official documentation:
             [Function_GetAll_AllEmployeesByCompany_V2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetAll_AllEmployeesByCompany_V2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Function_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Function_Update")
     def update(self):
         """
         Update the function starting from the given period.
 
         For more information, refer to the official documentation:
             [Function_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Function_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Function_UpdateCurrent")
     def update_current(self):
         """
         Update the function starting from current period.
 
         For more information, refer to the official documentation:
             [Function_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,165 +12,165 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Get")
     def fixed_get(self):
         """
         Get all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_GetCurrent")
     def fixed_get_current(self):
         """
         Get all extra hour components for the current period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert")
     def fixed_insert(self):
         """
         Insert an extra hour component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_InsertCurrent")
     def fixed_insert_current(self):
         """
         Insert an extra hour component to the current period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_Insert_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert_Batch")
     def fixed_insert_batch(self):
         """
         Insert a batch of extra hour components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_Insert_With_End"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert_With_End")
     def fixed_insert_with_end(self):
         """
         Insert an extra hour component with end to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentFixed_Stop"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Stop")
     def fixed_stop(self):
         """
         Stop an hour component. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Get")
     def variable_get(self):
         """
         Get all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_GetCurrent")
     def variable_get_current(self):
         """
         Get all extra hour components for the current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Insert")
     def variable_insert(self):
         """
         Insert an extra hour component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_InsertCurrent")
     def variable_insert_current(self):
         """
         Insert an extra hour component to the current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_Insert_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Insert_Batch")
     def variable_insert_batch(self):
         """
         Insert a batch of extra hour components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_Clear"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Clear")
     def variable_clear(self):
         """
         Clear all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponentVar_ClearCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_ClearCurrent")
     def variable_clear_current(self):
         """
         Clear all extra hour components for current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_ClearCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponent_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponent_Delete")
     def delete(self):
         """
         Delete an hour component linked to an employee by HourComponentID.
 
         For more information, refer to the official documentation:
             [HourComponent_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponent_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:HourComponent_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:HourComponent_Update")
     def update(self):
         """
         Update any Hour Component Variable or Fixed.
         In case of being a Fixed Hour Component the parameters EndYear and EndPeriod inside the method can be specified.
         If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LabourAgreements_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:LabourAgreements_Get")
     def get(self):
         """
         Get the labour agreement settings to an employee.
 
         For more information, refer to the official documentation:
             [LabourAgreements_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LabourAgreements_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LabourAgreements_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:LabourAgreements_GetCurrent")
     def get_current(self):
         """
         Get labour agreement settings to an employee for the current period.
 
         For more information, refer to the official documentation:
             [LabourAgreements_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LabourAgreements_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LabourAgreements_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:LabourAgreements_Update")
     def update(self):
         """
         Update the labour agreement that is assigned to an employee. Unprotected mode flag activated.
 
         For more information, refer to the official documentation:
             [LabourAgreements_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LabourAgreements_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LabourAgreements_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:LabourAgreements_UpdateCurrent")
     def update_current(self):
         """
         Update the labour agreement that is assigned to an employee for the current period.
 
         For more information, refer to the official documentation:
             [LabourAgreements_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LabourAgreements_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,78 @@
-"""Microservice responsible for lease car related actions on the employee level."""
+# pylint: disable=line-too-long
+"""Microservice responsible for service related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeLeaseCarService(MicroService):
-    """Microservice responsible for lease car related actions on the employee level."""
+class EmployeeServiceService(MicroService):
+    """Microservice responsible for service related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_Get"])
-    def get(self):
-        """
-        Get the active lease car contract for given period.
-
-        For more information, refer to the official documentation:
-            [LeaseCar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Get)
-        """
-        raise NotImplementedError()  # pragma: no cover
-
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_GetCurrent"])
-    def get_current(self):
-        """
-        Get currently active lease car contract.
-
-        For more information, refer to the official documentation:
-            [LeaseCar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetCurrent)
-        """
-        raise NotImplementedError()  # pragma: no cover
-
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Service_GetList")
     def get_all(self):
         """
-        Get lease car contract list, until given period.
+        Get all service intervals.
 
         For more information, refer to the official documentation:
-            [LeaseCar_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetList)
+            [Service_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_GetAll_EmployeesByCompany"])
-    def get_all_by_company(self):
-        """
-        Get lease car contract list for all employee in company, until given period.
-
-        For more information, refer to the official documentation:
-            [LeaseCar_GetAll_EmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_GetAll_EmployeesByCompany)
-        """
-        raise NotImplementedError()  # pragma: no cover
-
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar2_GetAll_EmployeesByCompany"])
-    def get_all_by_company_2(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Service_Insert")
+    def insert(self):
         """
-        Get lease car contract list for all employee in company, until given period.
+        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [LeaseCar2_GetAll_EmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar2_GetAll_EmployeesByCompany)
+            [Service_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_Insert"])
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Service_Insert2")
+    def insert_2(self):
         """
-        Insert a new lease car contract, this contract will start from given date within the object.
+        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
-            [LeaseCar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Insert)
+            [Service_Insert2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_InsertCurrent"])
-    def insert_current(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Service_Delete")
+    def delete(self):
         """
-        Insert a new lease car contract, this contract will start from given date within the object.
+        Delete a service interval.
 
         For more information, refer to the official documentation:
-            [LeaseCar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_InsertCurrent)
+            [Service_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_Delete"])
-    def delete(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Service_StopCurrent")
+    def stop_current(self):
         """
-        Delete a lease car contract. This action can not be undone.
+        Stop the current service interval. If the date is before the company's current period, unprotected mode flag is required.
+        If the employee income type requires and the employee is an applicant the EndServiceReasonId is mandatory, otherwise this field is ignored whatever the value is passed.
 
         For more information, refer to the official documentation:
-            [LeaseCar_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Delete)
+            [Service_StopCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_StopCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaseCar_Stop"])
-    def stop(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Service_RemoveOutService")
+    def remove_out_service(self):
         """
-        Stop the currently active lease car contract.
+        Remove out of service date.
 
         For more information, refer to the official documentation:
-            [LeaseCar_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Stop)
+            [Service_RemoveOutService](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_RemoveOutService)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/leave.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,75 +11,75 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaveBalance_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:LeaveBalance_Get")
     def get(self):
         """
         Get the Leave Balance for the given employee.
 
         For more information, refer to the official documentation:
             [LeaveBalance_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaveBalance_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Leave_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Leave_GetList")
     def get_all(self):
         """
         Get a list of leave for the given year, type and usage type.
 
         For more information, refer to the official documentation:
             [Leave_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Leave_GetList_V2"])
+    @nmbrs_exception_handler(resource="EmployeeService:Leave_GetList_V2")
     def get_all_2(self):
         """
         Get a list of leave for the given year, type and usage type.
 
         For more information, refer to the official documentation:
             [Leave_GetList_V2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_GetList_V2)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:LeaveBalance_GetPerType"])
+    @nmbrs_exception_handler(resource="EmployeeService:LeaveBalance_GetPerType")
     def get_by_type(self):
         """
         Get the leave balance for the given employee and type.
 
         For more information, refer to the official documentation:
             [LeaveBalance_GetPerType](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaveBalance_GetPerType)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Leave_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Leave_Insert")
     def insert(self):
         """
         Insert a new leave, starting from a specific date.
 
         For more information, refer to the official documentation:
             [Leave_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Leave_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Leave_Update")
     def update(self):
         """
         Insert a new leave, starting from a specific date.
 
         For more information, refer to the official documentation:
             [Leave_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Leave_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Leave_Delete")
     def delete(self):
         """
         Delete a leave entry.
 
         For more information, refer to the official documentation:
             [Leave_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_Delete)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Levensloop_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Get")
     def get(self):
         """
         Get the active levensloop for given period.
 
         For more information, refer to the official documentation:
             [Levensloop_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Levensloop_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Insert")
     def insert(self):
         """
         Start levensloop for given date and amount.
 
         For more information, refer to the official documentation:
             [Levensloop_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Levensloop_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Delete")
     def delete(self):
         """
         Delete the given levensloop. This action can not be undone.
 
         For more information, refer to the official documentation:
             [Levensloop_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Levensloop_Stop"])
+    @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Stop")
     def stop(self):
         """
         Stop the active levensloop for given date.
 
         For more information, refer to the official documentation:
             [Levensloop_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Stop)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Manager_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Manager_Get")
     def get(self):
         """
         Get the manager of an employee to the specified period.
 
         For more information, refer to the official documentation:
             [Manager_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Manager_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Manager_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Manager_GetCurrent")
     def get_current(self):
         """
         Get the manager of an employee.
 
         For more information, refer to the official documentation:
             [Manager_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Manager_GetCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/partner.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Partner_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Partner_Get")
     def get(self):
         """
         Get employee partner.
 
         For more information, refer to the official documentation:
             [Partner_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Partner_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Partner_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Partner_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get employee partner.
 
         For more information, refer to the official documentation:
             [Partner_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Partner_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Partner_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Partner_Update")
     def update(self):
         """
         Update the employee partner info.
 
         For more information, refer to the official documentation:
             [Partner_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Partner_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Partner_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Partner_Delete")
     def delete(self):
         """
         Delete employee's partner.
 
         For more information, refer to the official documentation:
             [Partner_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Partner_Delete)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/salary.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,105 +12,105 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_Get")
     def get(self):
         """
         Get the active salary for the given period.
 
         For more information, refer to the official documentation:
             [Salary_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_GetCurrent")
     def get_current(self):
         """
         Get the active salary for the given period.
 
         For more information, refer to the official documentation:
             [Salary_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_GetList")
     def get_all(self):
         """
         Get all salary, within given period.
 
         For more information, refer to the official documentation:
             [Salary_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self):
         """
         Get all salary, until current period.
 
         For more information, refer to the official documentation:
             [Salary_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SalaryDocuments_GetAnnualStatementPDF"])
+    @nmbrs_exception_handler(resource="EmployeeService:SalaryDocuments_GetAnnualStatementPDF")
     def get_annual_pdf(self):
         """
         Get employee annual statement in PDF
 
         For more information, refer to the official documentation:
             [SalaryDocuments_GetAnnualStatementPDF](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SalaryDocuments_GetAnnualStatementPDF)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_GetEstimatedCostPerHour"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_GetEstimatedCostPerHour")
     def get_hourly_cost(self):
         """
         Get estimated cost per hour for a given employee and period.
 
         For more information, refer to the official documentation:
             [Salary_GetEstimatedCostPerHour](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_GetEstimatedCostPerHour)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SalaryTable_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:SalaryTable_Insert")
     def insert(self):
         """
         Insert salary table to salary.
 
         For more information, refer to the official documentation:
             [SalaryTable_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SalaryTable_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SalaryTable_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:SalaryTable_InsertCurrent")
     def insert_current(self):
         """
         Insert salary table to salary of current salary.
 
         For more information, refer to the official documentation:
             [SalaryTable_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SalaryTable_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_Update")
     def update(self):
         """
         Update salary. This salary will start from the date given.
 
         For more information, refer to the official documentation:
             [Salary_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Salary_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Salary_UpdateCurrent")
     def update_current(self):
         """
         Update salary. This salary will start from the first date of the current period.
 
         For more information, refer to the official documentation:
             [Salary_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetList")
     def get_all(self):
         """
         Get all schedules, until given period.
 
         For more information, refer to the official documentation:
             [Schedule_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_Get")
     def get(self):
         """
         Get schedule the active schedule for given period.
 
         For more information, refer to the official documentation:
             [Schedule_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetCurrent")
     def get_current(self):
         """
         Get currently active schedule.
 
         For more information, refer to the official documentation:
             [Schedule_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_GetAll_AllEmployeesByCompany"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[Schedule]:
         """
         Get all schedules of all employees from company.
 
         For more information, refer to the official documentation:
             [Schedule_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetAll_AllEmployeesByCompany)
 
@@ -66,35 +66,35 @@
         schedules = serialize_object(schedules)
         _schedules = []
         for employee in schedules:
             for schedule in employee["EmployeeSchedules"]["Schedule_V2"]:
                 _schedules.append(Schedule(employee_id=employee["EmployeeId"], data=schedule))
         return _schedules
 
-    @nmbrs_exception_handler(resources=["EmployeeService:ScheduleCalendar_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:ScheduleCalendar_Get")
     def get_calender(self):
         """
         Get the employee's schedule calendar for given period.
 
         For more information, refer to the official documentation:
             [ScheduleCalendar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=ScheduleCalendar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_Update")
     def update(self):
         """
         Update schedule starting from the given date. The company default rooster number can be specified.
 
         For more information, refer to the official documentation:
             [Schedule_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Schedule_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_UpdateCurrent")
     def update_current(self):
         """
         Update schedule starting from the current period. The company default rooster number can be specified.
 
         For more information, refer to the official documentation:
             [Schedule_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_UpdateCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/svw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-# pylint: disable=line-too-long
-"""Microservice responsible for service related actions on the employee level."""
+"""Microservice responsible for svw related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeServiceService(MicroService):
-    """Microservice responsible for service related actions on the employee level."""
+class EmployeeSvwService(MicroService):
+    """Microservice responsible for svw related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_GetList"])
-    def get_all(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_Get")
+    def get(self):
         """
-        Get all service intervals.
+        Get the active SVW settings for given period.
 
         For more information, refer to the official documentation:
-            [Service_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_GetList)
+            [SVW_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert"])
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_GetCurrent")
+    def get_current(self):
         """
-        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
+        Get the currently active SVW settings.
 
         For more information, refer to the official documentation:
-            [Service_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert)
+            [SVW_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Insert2"])
-    def insert_2(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_GetList")
+    def get_all(self):
         """
-        Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
+        Get a list of all SVW settings.
 
         For more information, refer to the official documentation:
-            [Service_Insert2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert2)
+            [SVW_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_Delete"])
-    def delete(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_GetAll_AllEmployeesByCompany")
+    def get_all_by_company(self):
         """
-        Delete a service interval.
+        Get all (historical) svw setting records for all employees that belong to the company.
 
         For more information, refer to the official documentation:
-            [Service_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Delete)
+            [SVW_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_StopCurrent"])
-    def stop_current(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_Update")
+    def update(self):
         """
-        Stop the current service interval. If the date is before the company's current period, unprotected mode flag is required.
-        If the employee income type requires and the employee is an applicant the EndServiceReasonId is mandatory, otherwise this field is ignored whatever the value is passed.
+        Update SVW settings starting from given period.
 
         For more information, refer to the official documentation:
-            [Service_StopCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_StopCurrent)
+            [SVW_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Service_RemoveOutService"])
-    def remove_out_service(self):
+    @nmbrs_exception_handler(resource="EmployeeService:SVW_UpdateCurrent")
+    def update_current(self):
         """
-        Remove out of service date.
+        Update SVW settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [Service_RemoveOutService](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_RemoveOutService)
+            [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_UpdateCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Spaarloon_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Get")
     def get(self):
         """
         Get the active spaarloon for given period.
 
         For more information, refer to the official documentation:
             [Spaarloon_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Spaarloon_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_GetList")
     def get_all(self):
         """
         Get a list of spaarloonvalues.
 
         For more information, refer to the official documentation:
             [Spaarloon_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Spaarloon_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Insert")
     def insert(self):
         """
         Start spaarloon for given date and amount. If the startdate is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Spaarloon_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Spaarloon_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Delete")
     def delete(self):
         """
         Delete the given spaarloon from the system. This action can not be undone.
 
         For more information, refer to the official documentation:
             [Spaarloon_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:Spaarloon_Stop"])
+    @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Stop")
     def stop(self):
         """
         Stop the active spaarloon for given date.
 
         For more information, refer to the official documentation:
             [Spaarloon_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_Stop)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-"""Microservice responsible for svw related actions on the employee level."""
+"""Microservice responsible for wage tax related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeSvwService(MicroService):
-    """Microservice responsible for svw related actions on the employee level."""
+class EmployeeWageTaxService(MicroService):
+    """Microservice responsible for wage tax related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get")
     def get(self):
         """
-        Get the active SVW settings for given period.
+        Get the active loonheffing settings for given period.
 
         For more information, refer to the official documentation:
-            [SVW_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Get)
+            [WageTax_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetCurrent")
     def get_current(self):
         """
-        Get the currently active SVW settings.
+        Get the currently active loonheffing settings.
 
         For more information, refer to the official documentation:
-            [SVW_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetCurrent)
+            [WageTax_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetList")
     def get_all(self):
         """
-        Get a list of all SVW settings.
+        Get a list of all loonheffing settings.
 
         For more information, refer to the official documentation:
-            [SVW_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetList)
+            [WageTax_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_GetAll_AllEmployeesByCompany"])
-    def get_all_by_company(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get_SE")
+    def get_settings(self):
         """
-        Get all (historical) svw setting records for all employees that belong to the company.
+        Get active wage tax settings for a specific period.
 
         For more information, refer to the official documentation:
-            [SVW_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_GetAll_AllEmployeesByCompany)
+            [WageTax_Get_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get_SE)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update")
     def update(self):
         """
-        Update SVW settings starting from given period.
+        Update loonheffing settings starting from given period
 
         For more information, refer to the official documentation:
-            [SVW_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_Update)
+            [WageTax_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:SVW_UpdateCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_UpdateCurrent")
     def update_current(self):
         """
-        Update SVW settings starting from the current period.
+        Update loonheffing settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SVW_UpdateCurrent)
+            [WageTax_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_UpdateCurrent)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update_SE")
+    def update_settings(self):
+        """
+        Update loonheffing settings starting from given period.
+
+        For more information, refer to the official documentation:
+            [WageTax_Update_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update_SE)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_GetList"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_GetList")
     def get_all(self):
         """
         Get Time Registration items filtered by time.
 
         For more information, refer to the official documentation:
             [TimeRegistration_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert")
     def insert(self):
         """
         Register item into the calendar of an employee.
 
         For more information, refer to the official documentation:
             [TimeRegistration_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_Insert_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert_Batch")
     def insert_batch(self):
         """
         Register items into the calendars.
 
         For more information, refer to the official documentation:
             [TimeRegistration_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_GetAll_AllTimeRegistrationCodes"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_GetAll_AllTimeRegistrationCodes")
     def get_codes(self):
         """
         Get available TimeRegistrationCodes.
 
         For more information, refer to the official documentation:
             [TimeRegistration_GetAll_AllTimeRegistrationCodes](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_GetAll_AllTimeRegistrationCodes)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Delete")
     def delete(self):
         """
         Delete Time Registration Item By ID.
 
         For more information, refer to the official documentation:
             [TimeRegistration_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_Clear"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Clear")
     def clear(self):
         """
         Delete Time Registration Item By EmployeeId and given dates.
 
         For more information, refer to the official documentation:
             [TimeRegistration_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeRegistration_ClearCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_ClearCurrent")
     def clear_current(self):
         """
         Delete Time Registration Item By EmployeeId.
 
         For more information, refer to the official documentation:
             [TimeRegistration_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_ClearCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeSchedule_AllEmployee_GetListByPeriod"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_AllEmployee_GetListByPeriod")
     def get_all_by_company(self):
         """
         Get Time Schedules from employee and period.
 
         For more information, refer to the official documentation:
             [TimeSchedule_AllEmployee_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_AllEmployee_GetListByPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeSchedule_GetAll"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetAll")
     def get_all(self):
         """
         Get all Time Schedules from employee.
 
         For more information, refer to the official documentation:
             [TimeSchedule_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetAll)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeSchedule_GetListByPeriod"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetListByPeriod")
     def get(self):
         """
         Get Time Schedules from employee and period.
 
         For more information, refer to the official documentation:
             [TimeSchedule_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetListByPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeSchedule_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_Insert")
     def insert(self):
         """
         Add a new TimeSchedule.
 
         For more information, refer to the official documentation:
             [TimeSchedule_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:TimeSchedule_DeleteByID"])
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_DeleteByID")
     def delete(self):
         """
         Delete employee time schedule.
 
         For more information, refer to the official documentation:
             [TimeSchedule_DeleteByID](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_DeleteByID)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,187 +12,187 @@
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponent_Delete"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponent_Delete")
     def delete(self):
         """
         Delete a wage component by ID.
 
         For more information, refer to the official documentation:
             [WageComponent_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponent_Delete)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponent_Update"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponent_Update")
     def update(self):
         """
         Update any wage Component Variable or Fixed.
         In case of being a Fixed Wage Component the parameters EndYear and EndPeriod inside the method can be specified.
         If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponent_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponent_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Get")
     def fixed_get(self):
         """
         Get all fixed wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_GetCurrent")
     def fixed_get_current(self):
         """
         Get all fixed wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_GetCurrent")
     def fixed_insert(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_With_End"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_With_End")
     def fixed_insert_with_end(self):
         """
         Insert a wage component to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_InsertCurrent")
     def fixed_insert_current(self):
         """
         Insert a wage component to the current period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_InsertCurrent_With_End"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_InsertCurrent_With_End")
     def fixed_insert_current_with_end(self):
         """
         Insert a wage component to the current period with end period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_Batch")
     def fixed_insert_batch(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Insert_Batch_With_End"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_Batch_With_End")
     def fixed_insert_batch_with_end(self):
         """
         Insert a batch of wage components to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_Batch_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentFixed_Stop"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Stop")
     def fixed_stop(self):
         """
         Stop a wage component ending after given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Get"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Get")
     def variable_get(self):
         """
         Get all variable wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_GetCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_GetCurrent")
     def variable_get_current(self):
         """
         Get all variable wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Insert"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Insert")
     def variable_insert(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_InsertCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_InsertCurrent")
     def variable_insert_current(self):
         """
         Insert a wage components to the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Insert_Batch"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Insert_Batch")
     def variable_insert_batch(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_Clear"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Clear")
     def variable_clear(self):
         """
         Clear all variable wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resources=["EmployeeService:WageComponentVar_ClearCurrent"])
+    @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_ClearCurrent")
     def variable_clear_current(self):
         """
         Clear all variable wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_ClearCurrent)
         """
```

### Comparing `nmbrs-0.1.1/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-0.1.2/src/nmbrs/service/microservices/micro_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/service/service.py` & `nmbrs-0.1.2/src/nmbrs/service/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/service/sso_service.py` & `nmbrs-0.1.2/src/nmbrs/service/sso_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,48 +38,48 @@
             str: The generated Single Sign-On URL.
         """
         if self.sso_url not in nmbrs_env:
             nmbrs_env = f"{nmbrs_env}{self.sso_url}"
 
         return f"https://{nmbrs_env}/applications/common/externalactions.aspx?login={target}&ID={token}"
 
-    @nmbrs_exception_handler(resources=["SingleSignOn:GetToken"])
-    @nmbrs_sso_exception_handler(resources=["SingleSignOn:GetToken"])
+    @nmbrs_exception_handler(resource="SingleSignOn:GetToken")
+    @nmbrs_sso_exception_handler(resource="SingleSignOn:GetToken")
     def sso_auth_with_password(self, username: str, password: str) -> str:
         """
         Perform Single Sign-On authentication using username and password.
 
         Args:
             username (str): A string representing the username for authentication.
             password (str): A string representing the password for authentication.
 
         Returns:
             str: Single sign-on token, valid for 30 seconds
         """
         token = self.sso_service.service.GetToken(Username=username, Password=password)
         return token
 
-    @nmbrs_exception_handler(resources=["SingleSignOn:GetToken2"])
-    @nmbrs_sso_exception_handler(resources=["SingleSignOn:GetToken2"])
+    @nmbrs_exception_handler(resource="SingleSignOn:GetToken2")
+    @nmbrs_sso_exception_handler(resource="SingleSignOn:GetToken2")
     def sso_auth_with_token(self, username: str, token: str) -> str:
         """
         Perform Single Sign-On authentication using username and token.
 
         Args:
             username (str): A string representing the username for authentication.
             token (str): A string representing the token for authentication.
 
         Returns:
             str: Single sign-on token, valid for 30 seconds
         """
         token = self.sso_service.service.GetToken2(Username=username, Token=token)
         return token
 
-    @nmbrs_exception_handler(resources=["SingleSignOn:GetTokenWithDomain"])
-    @nmbrs_sso_exception_handler(resources=["SingleSignOn:GetTokenWithDomain"])
+    @nmbrs_exception_handler(resource="SingleSignOn:GetTokenWithDomain")
+    @nmbrs_sso_exception_handler(resource="SingleSignOn:GetTokenWithDomain")
     def sso_auth_with_domain(self, username: str, password: str, domain: str) -> str:
         """
         Perform Single Sign-On authentication using username, password, and domain.
 
         Args:
             username (str): A string representing the username for authentication.
             password (str): A string representing the password for authentication.
```

### Comparing `nmbrs-0.1.1/src/nmbrs/utils/find_empty_params.py` & `nmbrs-0.1.2/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs/utils/return_list.py` & `nmbrs-0.1.2/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.1/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-0.1.2/src/nmbrs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
-Project-URL: Homepage, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
-Project-URL: Source, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK
-Project-URL: Issues, https://github.com/LarsKluijtmans/Visma-NMBRS-SOAP-API-SDK/issues
+Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
+Project-URL: Source, https://github.com/LarsKluijtmans/nmbrs_api
+Project-URL: Issues, https://github.com/LarsKluijtmans/nmbrs_api/issues
 Keywords: nmbrs,soap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -155,22 +155,22 @@
 
 In case a user does not have access to the needed endpoints an AuthorizationError will be raised.
 
 To handle these Exceptions you can take inspiration from the following code.
 
 ```python
 from nmbrs import Nmbrs
-from nmbrs.exceptions import AuthorizationError
+from nmbrs.exceptions import AuthenticationException
 
 api = Nmbrs(username="__username__", token="__token__", auth_type="token")
 
 try:
     debtors = api.debtor.get_all()
-except AuthorizationError as e:
-    print(f"User does not have access to: {', '.join(e.resources)}'")
+except AuthenticationException as e:
+    print(f"User does not have access to: {e.resource}")
 ```
 
 ## Single Sign-on(SSO)
 
 When it comes to Nmbrs Single Sign-On service:
 
  - Username and Token
```

### Comparing `nmbrs-0.1.1/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-0.1.2/src/nmbrs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 src/nmbrs/data_classes/debtor.py
 src/nmbrs/data_classes/employee.py
 src/nmbrs/data_classes/general.py
 src/nmbrs/data_classes/utils/__init__.py
 src/nmbrs/data_classes/utils/xml.py
 src/nmbrs/exceptions/__init__.py
 src/nmbrs/exceptions/exceptions.py
-src/nmbrs/exceptions/nmbrs_exceptions.py
-src/nmbrs/exceptions/sso_exceptions.py
+src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
 src/nmbrs/service/__init__.py
 src/nmbrs/service/company_service.py
 src/nmbrs/service/debtor_service.py
 src/nmbrs/service/employee_service.py
 src/nmbrs/service/service.py
 src/nmbrs/service/sso_service.py
 src/nmbrs/service/microservices/__init__.py
```

