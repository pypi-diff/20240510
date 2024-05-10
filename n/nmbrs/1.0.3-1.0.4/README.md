# Comparing `tmp/nmbrs-1.0.3.tar.gz` & `tmp/nmbrs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-1.0.3.tar", last modified: Wed May  1 12:48:37 2024, max compression
+gzip compressed data, was "nmbrs-1.0.4.tar", last modified: Fri May 10 21:24:59 2024, max compression
```

## Comparing `nmbrs-1.0.3.tar` & `nmbrs-1.0.4.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.333263 nmbrs-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-01 12:48:21.000000 nmbrs-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 12:48:21.000000 nmbrs-1.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-01 12:48:37.329263 nmbrs-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-05-01 12:48:21.000000 nmbrs-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 12:48:21.000000 nmbrs-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:48:37.333263 nmbrs-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-01 12:48:21.000000 nmbrs-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.313262 nmbrs-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.317263 nmbrs-1.0.3/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/__logging__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-01 12:48:35.000000 nmbrs-1.0.3/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.317263 nmbrs-1.0.3/src/nmbrs/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/auth/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.317263 nmbrs-1.0.3/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.317263 nmbrs-1.0.3/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.317263 nmbrs-1.0.3/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.321262 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/background_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
--rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.321262 nmbrs-1.0.3/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.321262 nmbrs-1.0.3/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.325263 nmbrs-1.0.3/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.325263 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.329263 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/report_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.329263 nmbrs-1.0.3/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/utils/get_module_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 12:48:21.000000 nmbrs-1.0.3/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:37.329263 nmbrs-1.0.3/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-01 12:48:37.000000 nmbrs-1.0.3/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-01 12:48:37.000000 nmbrs-1.0.3/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:48:37.000000 nmbrs-1.0.3/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 12:48:37.000000 nmbrs-1.0.3/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:48:37.000000 nmbrs-1.0.3/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.819023 nmbrs-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-10 21:24:44.000000 nmbrs-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 21:24:44.000000 nmbrs-1.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-10 21:24:59.819023 nmbrs-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-05-10 21:24:44.000000 nmbrs-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-10 21:24:44.000000 nmbrs-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:24:59.819023 nmbrs-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 21:24:44.000000 nmbrs-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.799023 nmbrs-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.803023 nmbrs-1.0.4/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/__logging__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-10 21:24:57.000000 nmbrs-1.0.4/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.803023 nmbrs-1.0.4/src/nmbrs/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/auth/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.807023 nmbrs-1.0.4/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.807023 nmbrs-1.0.4/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.807023 nmbrs-1.0.4/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.807023 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.807023 nmbrs-1.0.4/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20350 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.811023 nmbrs-1.0.4/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.811023 nmbrs-1.0.4/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.815023 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.819023 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/report_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.819023 nmbrs-1.0.4/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/utils/get_module_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-10 21:24:44.000000 nmbrs-1.0.4/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:24:59.819023 nmbrs-1.0.4/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-10 21:24:59.000000 nmbrs-1.0.4/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-10 21:24:59.000000 nmbrs-1.0.4/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:24:59.000000 nmbrs-1.0.4/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 21:24:59.000000 nmbrs-1.0.4/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 21:24:59.000000 nmbrs-1.0.4/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-1.0.3/LICENSE` & `nmbrs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/PKG-INFO` & `nmbrs-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-1.0.3/README.md` & `nmbrs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/setup.py` & `nmbrs-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/__logging__.py` & `nmbrs-1.0.4/src/nmbrs/__logging__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/__version__.py` & `nmbrs-1.0.4/src/nmbrs/__version__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Versioning details."""
 
 __title__ = "nmbrs"
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 __author__ = "Lars Kluijtmans"
 __author_email__ = "info@lk-software.com"
 __maintainer__ = "Lars Kluijtmans"
 __maintainer_email__ = "info@lk-software.com"
 __description__ = "Python SDK for the Visma Nmbrs SOAP API."
 __license__ = "Lars Kluijtmans"
```

### Comparing `nmbrs-1.0.3/src/nmbrs/auth/token_manager.py` & `nmbrs-1.0.4/src/nmbrs/auth/token_manager.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/company.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/company.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/data_class.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/data_class.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/debtor.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/debtor.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/employee.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/employee.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/serialize.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/serialize.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-1.0.4/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/background_task.py` & `nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/background_task.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py` & `nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py` & `nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py` & `nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py` & `nmbrs-1.0.4/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/company_service.py` & `nmbrs-1.0.4/src/nmbrs/service/company_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,33 +46,177 @@
     def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
         super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs client
         self.client = Client(f"{self.base_uri}{self.company_uri}")
 
         # Micro services
-        self.address = CompanyAddressService(self.auth_manager, self.client)
-        self.bank_account = CompanyBankAccountService(self.auth_manager, self.client)
-        self.cost_center = CompanyCostCenterService(self.auth_manager, self.client)
-        self.cost_unit = CompanyCostUnitService(self.auth_manager, self.client)
-        self.hour_model = CompanyHourModelService(self.auth_manager, self.client)
-        self.journal = CompanyJournalService(self.auth_manager, self.client)  # TO BE implemented
-        self.labour_agreement = CompanyLabourAgreementService(self.auth_manager, self.client)
-        self.pension = CompanyPensionService(self.auth_manager, self.client)
-        self.run = CompanyRunService(self.auth_manager, self.client)
-        self.salary_documents = CompanySalaryDocumentService(self.auth_manager, self.client)  # TO BE implemented
-        self.salary_table = CompanySalaryTableService(self.auth_manager, self.client)
-        self.svw = CompanySvwService(self.auth_manager, self.client)
-        self.wage_component = CompanyWageComponentService(self.auth_manager, self.client)
-        self.wage_cost = CompanyWageCostService(self.auth_manager, self.client)
-        self.wage_model = CompanyWageModelService(self.auth_manager, self.client)
-        self.wage_tax = CompanyWageTaxService(self.auth_manager, self.client)
+        self._address = None
+        self._bank_account = None
+        self._cost_center = None
+        self._cost_unit = None
+        self._hour_model = None
+        self._journal = None
+        self._labour_agreement = None
+        self._pension = None
+        self._run = None
+        self._salary_documents = None
+        self._salary_table = None
+        self._svw = None
+        self._wage_component = None
+        self._wage_cost = None
+        self._wage_model = None
+        self._wage_tax = None
 
         logger.info("CompanyService initialized.")
 
+    @property
+    def address(self):
+        """
+        Lazily initializes and returns the CompanyAddressService instance.
+        """
+        if self._address is None:
+            self._address = CompanyAddressService(self.auth_manager, self.client)
+        return self._address
+
+    @property
+    def bank_account(self):
+        """
+        Lazily initializes and returns the CompanyBankAccountService instance.
+        """
+        if self._bank_account is None:
+            self._bank_account = CompanyBankAccountService(self.auth_manager, self.client)
+        return self._bank_account
+
+    @property
+    def cost_center(self):
+        """
+        Lazily initializes and returns the CompanyCostCenterService instance.
+        """
+        if self._cost_center is None:
+            self._cost_center = CompanyCostCenterService(self.auth_manager, self.client)
+        return self._cost_center
+
+    @property
+    def cost_unit(self):
+        """
+        Lazily initializes and returns the CompanyCostUnitService instance.
+        """
+        if self._cost_unit is None:
+            self._cost_unit = CompanyCostUnitService(self.auth_manager, self.client)
+        return self._cost_unit
+
+    @property
+    def hour_model(self):
+        """
+        Lazily initializes and returns the CompanyHourModelService instance.
+        """
+        if self._hour_model is None:
+            self._hour_model = CompanyHourModelService(self.auth_manager, self.client)
+        return self._hour_model
+
+    @property
+    def journal(self):
+        """
+        Lazily initializes and returns the CompanyJournalService instance.
+        """
+        if self._journal is None:
+            self._journal = CompanyJournalService(self.auth_manager, self.client)
+        return self._journal
+
+    @property
+    def labour_agreement(self):
+        """
+        Lazily initializes and returns the CompanyLabourAgreementService instance.
+        """
+        if self._labour_agreement is None:
+            self._labour_agreement = CompanyLabourAgreementService(self.auth_manager, self.client)
+        return self._labour_agreement
+
+    @property
+    def pension(self):
+        """
+        Lazily initializes and returns the CompanyPensionService instance.
+        """
+        if self._pension is None:
+            self._pension = CompanyPensionService(self.auth_manager, self.client)
+        return self._pension
+
+    @property
+    def run(self):
+        """
+        Lazily initializes and returns the CompanyRunService instance.
+        """
+        if self._run is None:
+            self._run = CompanyRunService(self.auth_manager, self.client)
+        return self._run
+
+    @property
+    def salary_documents(self):
+        """
+        Lazily initializes and returns the CompanySalaryDocumentService instance.
+        """
+        if self._salary_documents is None:
+            self._salary_documents = CompanySalaryDocumentService(self.auth_manager, self.client)
+        return self._salary_documents
+
+    @property
+    def salary_table(self):
+        """
+        Lazily initializes and returns the CompanySalaryTableService instance.
+        """
+        if self._salary_table is None:
+            self._salary_table = CompanySalaryTableService(self.auth_manager, self.client)
+        return self._salary_table
+
+    @property
+    def svw(self):
+        """
+        Lazily initializes and returns the CompanySvwService instance.
+        """
+        if self._svw is None:
+            self._svw = CompanySvwService(self.auth_manager, self.client)
+        return self._svw
+
+    @property
+    def wage_component(self):
+        """
+        Lazily initializes and returns the CompanyWageComponentService instance.
+        """
+        if self._wage_component is None:
+            self._wage_component = CompanyWageComponentService(self.auth_manager, self.client)
+        return self._wage_component
+
+    @property
+    def wage_cost(self):
+        """
+        Lazily initializes and returns the CompanyWageCostService instance.
+        """
+        if self._wage_cost is None:
+            self._wage_cost = CompanyWageCostService(self.auth_manager, self.client)
+        return self._wage_cost
+
+    @property
+    def wage_model(self):
+        """
+        Lazily initializes and returns the CompanyWageModelService instance.
+        """
+        if self._wage_model is None:
+            self._wage_model = CompanyWageModelService(self.auth_manager, self.client)
+        return self._wage_model
+
+    @property
+    def wage_tax(self):
+        """
+        Lazily initializes and returns the CompanyWageTaxService instance.
+        """
+        if self._wage_tax is None:
+            self._wage_tax = CompanyWageTaxService(self.auth_manager, self.client)
+        return self._wage_tax
+
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:List_GetAll")
     def get_all(self) -> list[Company]:
         """
         Retrieve all companies.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-1.0.3/src/nmbrs/service/debtor_service.py` & `nmbrs-1.0.4/src/nmbrs/service/debtor_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,21 +40,57 @@
     def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
         super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs services
         self.client = Client(f"{self.base_uri}{self.debtor_uri}")
 
         # Micro services
-        self.department = DebtorDepartmentService(self.auth_manager, self.client)
-        self.function = DebtorFunctionService(self.auth_manager, self.client)
-        self.webhook = DebtorWebHooksService(self.auth_manager, self.client)
-        self.title = DebtorTitleService(self.auth_manager, self.client)
+        self._department = None
+        self._function = None
+        self._webhook = None
+        self._title = None
 
         logger.info("DebtorService initialized.")
 
+    @property
+    def department(self):
+        """
+        Lazily initializes and returns the DebtorDepartmentService instance.
+        """
+        if self._department is None:
+            self._department = DebtorDepartmentService(self.auth_manager, self.client)
+        return self._department
+
+    @property
+    def function(self):
+        """
+        Lazily initializes and returns the DebtorFunctionService instance.
+        """
+        if self._function is None:
+            self._function = DebtorFunctionService(self.auth_manager, self.client)
+        return self._function
+
+    @property
+    def webhook(self):
+        """
+        Lazily initializes and returns the DebtorWebHooksService instance.
+        """
+        if self._webhook is None:
+            self._webhook = DebtorWebHooksService(self.auth_manager, self.client)
+        return self._webhook
+
+    @property
+    def title(self):
+        """
+        Lazily initializes and returns the DebtorTitleService instance.
+        """
+        if self._title is None:
+            self._title = DebtorTitleService(self.auth_manager, self.client)
+        return self._title
+
     @nmbrs_exception_handler(resource="DebtorService:Environment_Get")
     def get_domain(self, username: str, token: str) -> Domain:
         """
         Generate authentication header for standard token-based authentication.
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Environment_Get)
```

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/address.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/journal.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/pension.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/run.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/run.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/title.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/absence.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/child.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/contract.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/days.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/employment.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/leave.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/manager.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/partner.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/salary.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/employee/wage_tax.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-1.0.4/src/nmbrs/service/microservices/micro_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/report_service.py` & `nmbrs-1.0.4/src/nmbrs/service/report_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/service.py` & `nmbrs-1.0.4/src/nmbrs/service/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/service/sso_service.py` & `nmbrs-1.0.4/src/nmbrs/service/sso_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/utils/find_empty_params.py` & `nmbrs-1.0.4/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/utils/get_module_path.py` & `nmbrs-1.0.4/src/nmbrs/utils/get_module_path.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs/utils/nmbrs_exception_handler.py` & `nmbrs-1.0.4/src/nmbrs/utils/nmbrs_exception_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Exception Handling Decorators for Nmbrs SOAP API"""
 
 import logging
+import time
 
 import zeep.exceptions
 
 from .get_module_path import get_module_path
 from ..exceptions import (
     AuthenticationException,
     AuthorizationException,
@@ -63,16 +64,20 @@
     Args:
         resource (str): Resources being called.
     """
 
     def decorator(func):
         def wrapper(*args, **kwargs):
             try:
+                start_time = time.time()
                 response = func(*args, **kwargs)
+                end_time = time.time()
+
                 logger.name = get_module_path(func)
+                logger.debug("%s execution time: %s seconds", resource, end_time - start_time)
 
                 if response is None:
                     logger.debug("Used resource: %s, was not able to retrieve anything.", resource)
                 elif isinstance(response, list):
                     logger.debug("Used resource: %s, retrieved %s entries.", resource, len(response))
                 else:
                     logger.debug("Used resource: %s, retrieved %s entries.", resource, 1)
```

### Comparing `nmbrs-1.0.3/src/nmbrs/utils/return_list.py` & `nmbrs-1.0.4/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-1.0.3/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-1.0.4/src/nmbrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-1.0.3/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-1.0.4/src/nmbrs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 src/nmbrs/data_classes/utils/xml.py
 src/nmbrs/exceptions/__init__.py
 src/nmbrs/exceptions/exceptions.py
 src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
 src/nmbrs/exceptions/nmbrs_exceptions/background_task.py
 src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
 src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
-src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
 src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
 src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
 src/nmbrs/service/__init__.py
 src/nmbrs/service/company_service.py
 src/nmbrs/service/debtor_service.py
 src/nmbrs/service/employee_service.py
 src/nmbrs/service/report_service.py
```

