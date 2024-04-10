# Comparing `tmp/nmbrs-0.1.2.tar.gz` & `tmp/nmbrs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.1.2.tar", last modified: Wed Apr 10 07:45:11 2024, max compression
+gzip compressed data, was "nmbrs-0.1.3.tar", last modified: Wed Apr 10 10:31:42 2024, max compression
```

## Comparing `nmbrs-0.1.2.tar` & `nmbrs-0.1.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-10 07:44:55.000000 nmbrs-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 07:44:55.000000 nmbrs-0.1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 07:45:11.856049 nmbrs-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-10 07:44:55.000000 nmbrs-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 07:44:55.000000 nmbrs-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:45:11.856049 nmbrs-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-10 07:44:55.000000 nmbrs-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.840049 nmbrs-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.840049 nmbrs-0.1.2/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 07:45:10.000000 nmbrs-0.1.2/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.844049 nmbrs-0.1.2/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.848049 nmbrs-0.1.2/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.848049 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.852049 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 07:44:55.000000 nmbrs-0.1.2/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:45:11.856049 nmbrs-0.1.2/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 07:45:11.000000 nmbrs-0.1.2/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.209637 nmbrs-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-10 10:31:27.000000 nmbrs-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 10:31:27.000000 nmbrs-0.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 10:31:42.209637 nmbrs-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-10 10:31:27.000000 nmbrs-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 10:31:27.000000 nmbrs-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:31:42.209637 nmbrs-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-10 10:31:27.000000 nmbrs-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.193637 nmbrs-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.193637 nmbrs-0.1.3/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 10:31:40.000000 nmbrs-0.1.3/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.197637 nmbrs-0.1.3/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17711 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.197637 nmbrs-0.1.3/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.197637 nmbrs-0.1.3/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.197637 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.201637 nmbrs-0.1.3/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.201637 nmbrs-0.1.3/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.201637 nmbrs-0.1.3/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.205637 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.209637 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.209637 nmbrs-0.1.3/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 10:31:27.000000 nmbrs-0.1.3/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:31:42.209637 nmbrs-0.1.3/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 10:31:42.000000 nmbrs-0.1.3/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 10:31:42.000000 nmbrs-0.1.3/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:31:42.000000 nmbrs-0.1.3/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 10:31:42.000000 nmbrs-0.1.3/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 10:31:42.000000 nmbrs-0.1.3/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.1.2/LICENSE` & `nmbrs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/PKG-INFO` & `nmbrs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-0.1.2/README.md` & `nmbrs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/setup.py` & `nmbrs-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/__version__.py` & `nmbrs-0.1.3/src/nmbrs/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Versioning details."""
 
 __title__ = "nmbrs"
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 __author__ = "Lars Kluijtmans"
 __author_email__ = "info@lk-software.com"
 __maintainer__ = "Lars Kluijtmans"
 __maintainer_email__ = "info@lk-software.com"
 __description__ = "Python SDK for the Visma Nmbrs SOAP API."
 __license__ = "Lars Kluijtmans"
```

### Comparing `nmbrs-0.1.2/src/nmbrs/api.py` & `nmbrs-0.1.3/src/nmbrs/api.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/data_classes/company.py` & `nmbrs-0.1.3/src/nmbrs/data_classes/company.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 from .utils.xml import parse_xml_to_dict
 
 
 class Company(DataClass):
     """A class representing a company."""
 
     def __init__(self, data: dict) -> None:
-        self.id: int = data.get("ID", None)
-        self.number: int = data.get("Number", None)
-        self.name: str = data.get("Name", None)
-        self.phone_number: str = data.get("PhoneNumber", None)
-        self.fax_number: str = data.get("FaxNumber", None)
-        self.email: str = data.get("Email", None)
-        self.website: str = data.get("Website", None)
-        self.loonaangifte_tijdvak: str = data.get("LoonaangifteTijdvak", None)
-        self.kvk_number: str = data.get("KvkNr", None)
+        self.id: int = data.get("ID")
+        self.number: int = data.get("Number")
+        self.name: str = data.get("Name")
+        self.phone_number: str = data.get("PhoneNumber")
+        self.fax_number: str = data.get("FaxNumber")
+        self.email: str = data.get("Email")
+        self.website: str = data.get("Website")
+        self.loonaangifte_tijdvak: str = data.get("LoonaangifteTijdvak")
+        self.kvk_number: str = data.get("KvkNr")
 
 
 class BankAccount(DataClass):
     """A class representing a bank account."""
 
     def __init__(self, company_id: int, data: dict) -> None:
         self.company_id = company_id
-        self.id: int = data.get("Id", None)
-        self.number: str = data.get("Number", None)
-        self.description: str = data.get("Description", None)
-        self.iban: str = data.get("IBAN", None)
-        self.bic: str = data.get("BIC", None)
-        self.city: str = data.get("City", None)
-        self.name: str = data.get("Name", None)
-        self.type: str = data.get("Type", None)
+        self.id: int = data.get("Id")
+        self.number: str = data.get("Number")
+        self.description: str = data.get("Description")
+        self.iban: str = data.get("IBAN")
+        self.bic: str = data.get("BIC")
+        self.city: str = data.get("City")
+        self.name: str = data.get("Name")
+        self.type: str = data.get("Type")
 
 
 class Address(DataClass):
     """A class representing an address."""
 
     def __init__(self, company_id: int, data: dict) -> None:
         self.company_id = company_id
-        self.id: int = data.get("Id", None)
-        self.default: bool = data.get("Default", None)
-        self.street: str = data.get("Street", None)
-        self.house_number: str = data.get("HouseNumber", None)
-        self.house_number_addition: str = data.get("HouseNumberAddition", None)
-        self.postal_code: str = data.get("PostalCode", None)
-        self.city: str = data.get("City", None)
-        self.state_province: str = data.get("StateProvince", None)
-        self.country_iso_code: str = data.get("CountryISOCode", None)
+        self.id: int = data.get("Id")
+        self.default: bool = data.get("Default")
+        self.street: str = data.get("Street")
+        self.house_number: str = data.get("HouseNumber")
+        self.house_number_addition: str = data.get("HouseNumberAddition")
+        self.postal_code: str = data.get("PostalCode")
+        self.city: str = data.get("City")
+        self.state_province: str = data.get("StateProvince")
+        self.country_iso_code: str = data.get("CountryISOCode")
 
 
 class LabourAgreement(DataClass):
     """A class representing a labour agreement."""
 
     def __init__(self, company_id: int, data: dict) -> None:
         self.company_id = company_id
@@ -91,26 +91,26 @@
 
 
 class WageTax(DataClass):
     """A class representing a wage tax."""
 
     def __init__(self, company_id: int, data: dict) -> None:
         self.company_id = company_id
-        self.loonaangifte_id: int = data.get("LoonaangifteID", None)
-        self.serial_number: int = data.get("SerialNumber", None)
-        self.payment_reference: str = data.get("PaymentReference", None)
-        self.total_general: int = data.get("TotalGeneral", None)
-        self.period: int = data.get("Period", None)
-        self.year: int = data.get("Year", None)
-        self.status: str = data.get("Status", None)
-        self.sent_at: datetime = data.get("SentAt", None)
-        self.tijdvak_start: datetime = data.get("TijdvakStart", None)
-        self.tijdvak_end: datetime = data.get("TijdvakEnd", None)
-        self.correction_tijdvak_start: datetime = data.get("CorrectionTijdvakStart", None)
-        self.correction_tijdvak_end: datetime = data.get("CorrectionTijdvakEnd", None)
+        self.loonaangifte_id: int = data.get("LoonaangifteID")
+        self.serial_number: int = data.get("SerialNumber")
+        self.payment_reference: str = data.get("PaymentReference")
+        self.total_general: int = data.get("TotalGeneral")
+        self.period: int = data.get("Period")
+        self.year: int = data.get("Year")
+        self.status: str = data.get("Status")
+        self.sent_at: datetime = data.get("SentAt")
+        self.tijdvak_start: datetime = data.get("TijdvakStart")
+        self.tijdvak_end: datetime = data.get("TijdvakEnd")
+        self.correction_tijdvak_start: datetime = data.get("CorrectionTijdvakStart")
+        self.correction_tijdvak_end: datetime = data.get("CorrectionTijdvakEnd")
 
 
 class WageTaxXML(DataClass):
     """A class representing wage tax XML."""
 
     def __init__(self, xml: str) -> None:
         self.xml: str = xml
```

### Comparing `nmbrs-0.1.2/src/nmbrs/data_classes/data_class.py` & `nmbrs-0.1.3/src/nmbrs/data_classes/data_class.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/data_classes/debtor.py` & `nmbrs-0.1.3/src/nmbrs/data_classes/debtor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from .utils.xml import parse_xml_to_dict
 
 
 class Domain(DataClass):
     """A class representing domain."""
 
     def __init__(self, data: dict) -> None:
-        self.domain: int = data.get("Domain", None)
-        self.sub_domain: int = data.get("SubDomain", None)
+        self.domain: int = data.get("Domain")
+        self.sub_domain: int = data.get("SubDomain")
 
 
 class AbsenceVerzuim(DataClass):
     """A class representing absence data."""
 
     def __init__(self, data: dict) -> None:
-        self.debtor_id: int = data.get("DebtorID", None)
-        self.company_id: int = data.get("CompanyID", None)
-        self.employee_id: int = data.get("EmployeeID", None)
-        self.xml: str = data.get("XML", None)
+        self.debtor_id: int = data.get("DebtorID")
+        self.company_id: int = data.get("CompanyID")
+        self.employee_id: int = data.get("EmployeeID")
+        self.xml: str = data.get("XML")
 
     def to_dict(self) -> dict:
         """
         Convert the instance to a dictionary.
 
         :return: A dictionary representation of the instance.
         """
@@ -38,135 +38,135 @@
 
 
 class Address(DataClass):
     """A class representing an address."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.id: int = data.get("Id", None)
-        self.default: bool = data.get("Default", None)
-        self.street: str = data.get("Street", None)
-        self.house_number: str = data.get("HouseNumber", None)
-        self.house_number_addition: str = data.get("HouseNumberAddition", None)
-        self.postal_code: str = data.get("PostalCode", None)
-        self.city: str = data.get("City", None)
-        self.state_province: str = data.get("StateProvince", None)
-        self.country_iso_code: str = data.get("CountryISOCode", None)
+        self.id: int = data.get("Id")
+        self.default: bool = data.get("Default")
+        self.street: str = data.get("Street")
+        self.house_number: str = data.get("HouseNumber")
+        self.house_number_addition: str = data.get("HouseNumberAddition")
+        self.postal_code: str = data.get("PostalCode")
+        self.city: str = data.get("City")
+        self.state_province: str = data.get("StateProvince")
+        self.country_iso_code: str = data.get("CountryISOCode")
 
 
 class BankAccount(DataClass):
     """A class representing a bank account."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.id: int = data.get("Id", None)
-        self.number: str = data.get("Number", None)
-        self.description: str = data.get("Description", None)
-        self.iban: str = data.get("IBAN", None)
-        self.bic: str = data.get("BIC", None)
-        self.city: str = data.get("City", None)
-        self.name: str = data.get("Name", None)
-        self.type: str = data.get("Type", None)
+        self.id: int = data.get("Id")
+        self.number: str = data.get("Number")
+        self.description: str = data.get("Description")
+        self.iban: str = data.get("IBAN")
+        self.bic: str = data.get("BIC")
+        self.city: str = data.get("City")
+        self.name: str = data.get("Name")
+        self.type: str = data.get("Type")
 
 
 class ContactInfo(DataClass):
     """A class representing a contact info."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.email: str = data.get("Email", None)
-        self.name: str = data.get("Name", None)
-        self.phone: str = data.get("Phone", None)
+        self.email: str = data.get("Email")
+        self.name: str = data.get("Name")
+        self.phone: str = data.get("Phone")
 
 
 class Debtor(DataClass):
     """A class representing a debtor."""
 
     def __init__(self, data: dict) -> None:
-        self.id: int = data.get("Id", None)
-        self.number: str = data.get("Number", None)
-        self.name: str = data.get("Name", None)
+        self.id: int = data.get("Id")
+        self.number: str = data.get("Number")
+        self.name: str = data.get("Name")
 
 
 class Department(DataClass):
     """A class representing a department."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.id: int = data.get("Id", None)
-        self.code: int = data.get("Code", None)
-        self.description: str = data.get("Description", None)
+        self.id: int = data.get("Id")
+        self.code: int = data.get("Code")
+        self.description: str = data.get("Description")
 
 
 class Function(DataClass):
     """A class representing a function."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.id: int = data.get("Id", None)
-        self.code: int = data.get("Code", None)
-        self.description: str = data.get("Description", None)
+        self.id: int = data.get("Id")
+        self.code: int = data.get("Code")
+        self.description: str = data.get("Description")
 
 
 class LabourAgreementSettings(DataClass):
     """A class representing labour agreement settings."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.id: int = data.get("Id", None)
-        self.guid: str = data.get("Guid", None)
-        self.int_number: int = data.get("IntNumber", None)
-        self.str_name: str = data.get("StrName", None)
-        self.debtor_id: int = data.get("IntDebiteurID", None)
+        self.id: int = data.get("Id")
+        self.guid: str = data.get("Guid")
+        self.int_number: int = data.get("IntNumber")
+        self.str_name: str = data.get("StrName")
+        self.debtor_id: int = data.get("IntDebiteurID")
 
 
 class Manager(DataClass):
     """A class representing manager information."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.number: int = data.get("Number", None)
-        self.first_name: str = data.get("FirstName", None)
-        self.name: str = data.get("Name", None)
-        self.department: str = data.get("Department", None)
-        self.function: str = data.get("Function", None)
-        self.phone_number: str = data.get("PhoneNumber", None)
-        self.mobile: str = data.get("Mobile", None)
-        self.fax: str = data.get("Fax", None)
-        self.email: str = data.get("Email", None)
+        self.number: int = data.get("Number")
+        self.first_name: str = data.get("FirstName")
+        self.name: str = data.get("Name")
+        self.department: str = data.get("Department")
+        self.function: str = data.get("Function")
+        self.phone_number: str = data.get("PhoneNumber")
+        self.mobile: str = data.get("Mobile")
+        self.fax: str = data.get("Fax")
+        self.email: str = data.get("Email")
 
 
 class ServiceLevel(DataClass):
     """A class representing service level information."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.start_period: int = data.get("StartPeriod", None)
-        self.start_year: int = data.get("StartYear", None)
-        self.service_level: str = data.get("ServiceLevel", None)
-        self.start_contract: datetime = data.get("StartContract", None)
+        self.start_period: int = data.get("StartPeriod")
+        self.start_year: int = data.get("StartYear")
+        self.service_level: str = data.get("ServiceLevel")
+        self.start_contract: datetime = data.get("StartContract")
 
 
 class Tag(DataClass):
     """A class representing debtor tag information."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.number: int = data.get("Number", None)
-        self.hex_color: str = data.get("HexColor", None)
-        self.tag: str = data.get("Tag", None)
+        self.number: int = data.get("Number")
+        self.hex_color: str = data.get("HexColor")
+        self.tag: str = data.get("Tag")
 
 
 class Event(DataClass):
     """A class representing an event."""
 
     def __init__(self, data: dict) -> None:
-        self.event_id: int = data.get("EventId", None)
-        self.event_name: str = data.get("EventName", None)
-        self.active: bool = data.get("Active", None)
+        self.event_id: int = data.get("EventId")
+        self.event_name: str = data.get("EventName")
+        self.active: bool = data.get("Active")
 
     def to_insert_dict(self) -> dict:
         """
         Convert the instance to a dictionary representing the XML insert format.
 
         :return: A dictionary representation of the event instance.
         """
@@ -177,18 +177,18 @@
 
 
 class WebhookSetting(DataClass):
     """A class representing a webhook setting."""
 
     def __init__(self, debtor_id: int, data: dict) -> None:
         self.debtor_id = debtor_id
-        self.webhook_setting_id: int = data.get("WebhookSettingId", None)
-        self.name: str = data.get("Name", None)
-        self.endpoint: str = data.get("Endpoint", None)
-        self.active: bool = data.get("Active", None)
+        self.webhook_setting_id: int = data.get("WebhookSettingId")
+        self.name: str = data.get("Name")
+        self.endpoint: str = data.get("Endpoint")
+        self.active: bool = data.get("Active")
         events_data = data.get("Event", [])
         if not isinstance(events_data, list):
             events_data = [events_data]
         self.events: list[Event] = [Event(event_data) for event_data in events_data]
 
     def to_insert_dict(self) -> dict:
         """
```

### Comparing `nmbrs-0.1.2/src/nmbrs/data_classes/employee.py` & `nmbrs-0.1.3/src/nmbrs/data_classes/employee.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from .data_class import DataClass
 
 
 class Employee(DataClass):
     """A class representing an employee."""
 
     def __init__(self, data: dict):
-        self.id: int = data.get("Id", None)
-        self.number: int = data.get("Number", None)
-        self.name: str = data.get("DisplayName", None)
+        self.id: int = data.get("Id")
+        self.number: int = data.get("Number")
+        self.name: str = data.get("DisplayName")
 
 
 class EmployeeTypes(DataClass):
     """A class representing an employee type."""
 
     def __init__(self, data: dict):
-        self.id: int = data.get("Id", None)
-        self.description: str = data.get("Description", None)
+        self.id: int = data.get("Id")
+        self.description: str = data.get("Description")
 
 
 class Period(DataClass):
     """A class representing a period of a company."""
 
     def __init__(self, employee_id: int, data: str):
         parts = data.split("-")
@@ -35,25 +35,25 @@
 
 
 class Contract(DataClass):
     """A class representing a contract."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
-        self.contract_id: int = data.get("ContractID", None)
-        self.creation_date: datetime = data.get("CreationDate", None)
-        self.start_date: datetime = data.get("StartDate", None)
-        self.trial_period: datetime = data.get("TrialPeriod", None)
-        self.end_date: datetime = data.get("EndDate", None)
-        self.employment_type: int = data.get("EmployementType", None)
-        self.employment_sequence_tax_id: int = data.get("EmploymentSequenceTaxId", None)
-        self.indefinite: bool = data.get("Indefinite", None)
-        self.phase_classification: int = data.get("PhaseClassification", None)
-        self.written_contract: bool = data.get("WrittenContract", None)
-        self.hours_per_week: Decimal = data.get("HoursPerWeek", None)
+        self.contract_id: int = data.get("ContractID")
+        self.creation_date: datetime = data.get("CreationDate")
+        self.start_date: datetime = data.get("StartDate")
+        self.trial_period: datetime = data.get("TrialPeriod")
+        self.end_date: datetime = data.get("EndDate")
+        self.employment_type: int = data.get("EmployementType")
+        self.employment_sequence_tax_id: int = data.get("EmploymentSequenceTaxId")
+        self.indefinite: bool = data.get("Indefinite")
+        self.phase_classification: int = data.get("PhaseClassification")
+        self.written_contract: bool = data.get("WrittenContract")
+        self.hours_per_week: Decimal = data.get("HoursPerWeek")
 
 
 class Schedule(DataClass):
     """A class representing a schedule."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
@@ -137,7 +137,66 @@
         self.salary_value: Decimal = data.get("SalaryValue")
         self.street: str = data.get("Street")
         self.house_number: str = data.get("HouseNumber")
         self.house_number_addition: str = data.get("HouseNumberAddition")
         self.post_code: str = data.get("PostCode")
         self.hourly_wage: Decimal = data.get("HourlyWage")
         self.contract_hours: Decimal = data.get("ContractHours")
+
+
+class Absence(DataClass):
+    """A class representing absence"""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id: int = employee_id
+        self.id: int = data.get("AbsenceId")
+        self.comment: str = data.get("Comment")
+        self.percentage: int = data.get("Percentage")
+        self.start: datetime = data.get("Start")
+        self.registration_start_date: datetime = data.get("RegistrationStartDate")
+        self.end: datetime = data.get("End")
+        self.registration_end_date: datetime = data.get("RegistrationEndDate")
+        self.dossier: str = data.get("Dossier")
+        self.dossier_number: int = data.get("Dossiernr")
+        self.cause: AbsenceCause = AbsenceCause(data.get("AbsenceCause"))
+
+
+class AbsenceCause(DataClass):
+    """A class representing the cause of an absence"""
+
+    def __init__(self, data: dict | None):
+        if data is None:
+            return
+        self.id: int = data.get("CauseId")
+        self.cause: str = data.get("Cause")
+
+
+class Address(DataClass):
+    """A class representing an address"""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id: int = employee_id
+        self.id: int = data.get("Id")
+        self.default: bool = data.get("Default")
+        self.street: str = data.get("Street")
+        self.house_number: str = data.get("HouseNumber")
+        self.house_number_addition: str = data.get("HouseNumberAddition")
+        self.postcode: str = data.get("PostalCode")
+        self.city: str = data.get("City")
+        self.state_province: str = data.get("StateProvince")
+        self.country_iso_code: str = data.get("CountryISOCode")
+        self.type: str = data.get("Type")
+
+
+class BankAccount(DataClass):
+    """A class representing a bank account."""
+
+    def __init__(self, employee_id: int, data: dict) -> None:
+        self.employee_id = employee_id
+        self.id: int = data.get("Id")
+        self.number: str = data.get("Number")
+        self.description: str = data.get("Description")
+        self.iban: str = data.get("IBAN")
+        self.bic: str = data.get("BIC")
+        self.city: str = data.get("City")
+        self.name: str = data.get("Name")
+        self.type: str = data.get("Type")
```

### Comparing `nmbrs-0.1.2/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-0.1.3/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py` & `nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py` & `nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py` & `nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py` & `nmbrs-0.1.3/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/company_service.py` & `nmbrs-0.1.3/src/nmbrs/service/company_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/debtor_service.py` & `nmbrs-0.1.3/src/nmbrs/service/debtor_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/employee_service.py` & `nmbrs-0.1.3/src/nmbrs/service/employee_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     def __init__(self, sandbox: bool = True) -> None:
         super().__init__(sandbox)
 
         # Initialize nmbrs services
         self.client = Client(f"{self.base_uri}{self.employee_uri}")
 
         # Micro services
-        self.absence = EmployeeAbsenceService(self.client)  # TO BE implemented
-        self.address = EmployeeAddressService(self.client)  # TO BE implemented
+        self.absence = EmployeeAbsenceService(self.client)
+        self.address = EmployeeAddressService(self.client)
         self.bank_account = EmployeeBankAccountService(self.client)  # TO BE implemented
         self.child = EmployeeChildService(self.client)  # TO BE implemented
         self.contract = EmployeeContractService(self.client)  # TO BE implemented
         self.cost_center = EmployeeCostCenterService(self.client)  # TO BE implemented
         self.days = EmployeeDaysService(self.client)  # TO BE implemented
         self.department = EmployeeDepartmentsService(self.client)  # TO BE implemented
         self.document = EmployeeDocumentService(self.client)  # TO BE implemented
@@ -66,15 +66,14 @@
         self.labour_agreement = EmployeeLabourAgreementService(self.client)  # TO BE implemented
         self.lease_car = EmployeeLeaseCarService(self.client)  # TO BE implemented
         self.leave = EmployeeLeaveService(self.client)  # TO BE implemented
         self.levensloop = EmployeeLevensLoopService(self.client)  # TO BE implemented
         self.manager = EmployeeManagerService(self.client)  # TO BE implemented
         self.partner = EmployeePartnerService(self.client)  # TO BE implemented
         self.personal_info = EmployeePersonalInfoService(self.client)
-
         self.salary = EmployeeSalaryService(self.client)  # TO BE implemented
         self.schedule = EmployeeScheduleService(self.client)  # TO BE implemented
         self.service = EmployeeServiceService(self.client)  # TO BE implemented
         self.spaarloon = EmployeeSpaarloonService(self.client)  # TO BE implemented
         self.svw = EmployeeSvwService(self.client)  # TO BE implemented
         self.time_registration = EmployeeTimeRegistrationService(self.client)  # TO BE implemented
         self.time_schedule = EmployeeTimeScheduleService(self.client)  # TO BE implemented
```

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/address.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/journal.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/pension.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/run.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/run.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/title.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,101 @@
 # pylint: disable=line-too-long
-"""Microservice responsible for absence related actions on the employee level."""
+"""Microservice responsible for schedule related actions on the employee level."""
 
 from zeep import Client
+from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....data_classes.employee import Schedule
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeAbsenceService(MicroService):
-    """Microservice responsible for absence related actions on the employee level."""
+class EmployeeScheduleService(MicroService):
+    """Microservice responsible for schedule related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence_GetList")
-    def get(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetList")
+    def get_all(self):
         """
-        Get a list of all absences.
+        Get all schedules, until given period.
 
         For more information, refer to the official documentation:
-            [Absence_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_GetList)
+            [Schedule_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence2_GetList")
-    def get_2(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_Get")
+    def get(self):
         """
-        Get a list of all absences with their respective cause.
+        Get schedule the active schedule for given period.
 
         For more information, refer to the official documentation:
-            [Absence2_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_GetList)
+            [Schedule_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence_GetAll_AllEmployeesByCompany")
-    def get_all_by_company(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetCurrent")
+    def get_current(self):
         """
-        Get a list of all absence of all company employees.
+        Get currently active schedule.
 
         For more information, refer to the official documentation:
-            [Absence_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_GetAll_AllEmployeesByCompany)
+            [Schedule_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence_Insert")
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetAll_AllEmployeesByCompany")
+    def get_all_by_company(self, company_id: int) -> list[Schedule]:
         """
-        Insert an absence, this item will start from the given date in the object.
+        Get all schedules of all employees from company.
 
         For more information, refer to the official documentation:
-            [Absence_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_Insert)
-        """
-        raise NotImplementedError()  # pragma: no cover
+            [Schedule_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_GetAll_AllEmployeesByCompany)
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence2_Insert")
-    def insert_2(self):
-        """
-        Insert an absence with cause, this item will start from the given date in the object.
+        Args:
+            company_id (int): The ID of the company.
 
-        For more information, refer to the official documentation:
-            [Absence2_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_Insert)
+        Returns:
+            list[Contract]: a list of contract objects
         """
-        raise NotImplementedError()  # pragma: no cover
+        schedules = self.client.service.Schedule_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        schedules = serialize_object(schedules)
+        _schedules = []
+        for employee in schedules:
+            for schedule in employee["EmployeeSchedules"]["Schedule_V2"]:
+                _schedules.append(Schedule(employee_id=employee["EmployeeId"], data=schedule))
+        return _schedules
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence_PartialRecoveryInsert")
-    def insert_partial_recovery(self):
+    @nmbrs_exception_handler(resource="EmployeeService:ScheduleCalendar_Get")
+    def get_calender(self):
         """
-        Insert an absence partial recovery message.
+        Get the employee's schedule calendar for given period.
 
         For more information, refer to the official documentation:
-            [Absence_PartialRecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_PartialRecoveryInsert)
+            [ScheduleCalendar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=ScheduleCalendar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Absence_RecoveryInsert")
-    def insert_recovery(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_Update")
+    def update(self):
         """
-        Insert an absence recovery message.
+        Update schedule starting from the given date. The company default rooster number can be specified.
 
         For more information, refer to the official documentation:
-            [Absence_RecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_RecoveryInsert)
+            [Schedule_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:AbsenceNotification_Insert")
-    def insert_notification(self):
+    @nmbrs_exception_handler(resource="EmployeeService:Schedule_UpdateCurrent")
+    def update_current(self):
         """
-        Insert a new absence date, this item will start from the given date in the object to the requested absence dossier.
+        Update schedule starting from the current period. The company default rooster number can be specified.
 
         For more information, refer to the official documentation:
-            [AbsenceNotification_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=AbsenceNotification_Insert)
+            [Schedule_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Schedule_UpdateCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,86 @@
-# pylint: disable=line-too-long
-"""Microservice responsible for address related actions on the employee level."""
+"""Microservice responsible for wage tax related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeAddressService(MicroService):
-    """Microservice responsible for address related actions on the employee level."""
+class EmployeeWageTaxService(MicroService):
+    """Microservice responsible for wage tax related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_GetList")
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get")
     def get(self):
         """
-        Get all addresses which are active in given period.
+        Get the active loonheffing settings for given period.
 
         For more information, refer to the official documentation:
-            [Address_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetList)
+            [WageTax_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_GetListCurrent")
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetCurrent")
     def get_current(self):
         """
-        Get all currently active addresses.
+        Get the currently active loonheffing settings.
 
         For more information, refer to the official documentation:
-            [Address_GetListCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetListCurrent)
+            [WageTax_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_GetAll_AllEmployeesByCompany")
-    def get_all_by_company(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetList")
+    def get_all(self):
         """
-        Get all addresses of all employees.
+        Get a list of all loonheffing settings.
 
         For more information, refer to the official documentation:
-            [Address_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_GetAll_AllEmployeesByCompany)
+            [WageTax_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_Delete")
-    def delete(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get_SE")
+    def get_settings(self):
         """
-        Get all active bank accounts for given period.
+        Get active wage tax settings for a specific period.
 
         For more information, refer to the official documentation:
-            [Address_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Delete)
+            [WageTax_Get_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get_SE)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_Update")
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update")
     def update(self):
         """
-        Delete Employee Address.
+        Update loonheffing settings starting from given period
 
         For more information, refer to the official documentation:
-            [Address_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Update)
+            [WageTax_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_Insert")
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_UpdateCurrent")
+    def update_current(self):
         """
-        Insert given address to the specified period. If the period is before the company's current period, unprotected mode flag is required.
+        Update loonheffing settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [Address_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Insert)
+            [WageTax_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_UpdateCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:Address_InsertCurrent")
-    def insert_current(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update_SE")
+    def update_settings(self):
         """
-        Insert given address to the current period.
+        Update loonheffing settings starting from given period.
 
         For more information, refer to the official documentation:
-            [Address_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_InsertCurrent)
+            [WageTax_Update_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update_SE)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-"""Microservice responsible for bank account related actions on the employee level."""
+# pylint: disable=line-too-long
+"""Microservice responsible for time schedule related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeBankAccountService(MicroService):
-    """Microservice responsible for bank account related actions on the employee level."""
+class EmployeeTimeScheduleService(MicroService):
+    """Microservice responsible for time schedule related actions on the employee level."""
 
     def __init__(self, client: Client) -> None:
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
-    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetList")
-    def get(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_AllEmployee_GetListByPeriod")
+    def get_all_by_company(self):
         """
-        Get all active bank accounts for given period.
+        Get Time Schedules from employee and period.
 
         For more information, refer to the official documentation:
-            [BankAccount_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_GetList)
+            [TimeSchedule_AllEmployee_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_AllEmployee_GetListByPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetListCurrent")
-    def get_current(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetAll")
+    def get_all(self):
         """
-        Get all active bank accounts for the current period.
+        Get all Time Schedules from employee.
 
         For more information, refer to the official documentation:
-            [BankAccount_GetListCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_GetListCurrent)
+            [TimeSchedule_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetAll)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_DeleteCurrent")
-    def delete(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetListByPeriod")
+    def get(self):
         """
-        Delete given bank account.
+        Get Time Schedules from employee and period.
 
         For more information, refer to the official documentation:
-            [BankAccount_DeleteCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_DeleteCurrent)
+            [TimeSchedule_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetListByPeriod)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_Insert")
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_Insert")
     def insert(self):
         """
-        Insert given bank account to the given period. Unprotected mode flag is required.
+        Add a new TimeSchedule.
 
         For more information, refer to the official documentation:
-            [BankAccount_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_Insert)
+            [TimeSchedule_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:BankAccount_InsertCurrent")
-    def insert_current(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_DeleteByID")
+    def delete(self):
         """
-        Insert given bank account to the current period.
+        Delete employee time schedule.
 
         For more information, refer to the official documentation:
-            [BankAccount_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_InsertCurrent)
+            [TimeSchedule_DeleteByID](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_DeleteByID)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/child.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/contract.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/days.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/employment.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/leave.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/manager.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/partner.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/salary.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-0.1.3/src/nmbrs/service/microservices/micro_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/service.py` & `nmbrs-0.1.3/src/nmbrs/service/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/service/sso_service.py` & `nmbrs-0.1.3/src/nmbrs/service/sso_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/utils/find_empty_params.py` & `nmbrs-0.1.3/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/utils/nmbrs_exception_handler.py` & `nmbrs-0.1.3/src/nmbrs/utils/nmbrs_exception_handler.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs/utils/return_list.py` & `nmbrs-0.1.3/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.2/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-0.1.3/src/nmbrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-0.1.2/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-0.1.3/src/nmbrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

