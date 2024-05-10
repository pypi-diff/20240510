# Comparing `tmp/affixapi-1.1.72.tar.gz` & `tmp/affixapi-1.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.72.tar", last modified: Thu May  9 14:31:25 2024, max compression
+gzip compressed data, was "affixapi-1.1.74.tar", last modified: Fri May 10 12:46:44 2024, max compression
```

## Comparing `affixapi-1.1.72.tar` & `affixapi-1.1.74.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.388737 affixapi-1.1.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 14:31:20.000000 affixapi-1.1.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 14:31:25.388737 affixapi-1.1.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21795 2024-05-09 14:31:20.000000 affixapi-1.1.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.388737 affixapi-1.1.72/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 14:31:25.000000 affixapi-1.1.72/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-09 14:31:25.000000 affixapi-1.1.72/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:31:25.000000 affixapi-1.1.72/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 14:31:25.000000 affixapi-1.1.72/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 14:31:25.000000 affixapi-1.1.72/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.360737 affixapi-1.1.72/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.364737 affixapi-1.1.72/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.364737 affixapi-1.1.72/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.376737 affixapi-1.1.72/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24681 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16515 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/currency_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.376737 affixapi-1.1.72/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-09 14:31:20.000000 affixapi-1.1.72/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 14:31:25.388737 affixapi-1.1.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 14:31:20.000000 affixapi-1.1.72/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:31:25.388737 affixapi-1.1.72/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_currency_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-09 14:31:20.000000 affixapi-1.1.72/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 12:46:36.000000 affixapi-1.1.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 12:46:44.441792 affixapi-1.1.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-10 12:46:36.000000 affixapi-1.1.74/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 12:46:44.000000 affixapi-1.1.74/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.417791 affixapi-1.1.74/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.421792 affixapi-1.1.74/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.421792 affixapi-1.1.74/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.429792 affixapi-1.1.74/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17888 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24681 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.429792 affixapi-1.1.74/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-10 12:46:36.000000 affixapi-1.1.74/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 12:46:44.441792 affixapi-1.1.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 12:46:36.000000 affixapi-1.1.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:44.441792 affixapi-1.1.74/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-10 12:46:36.000000 affixapi-1.1.74/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.72/LICENSE` & `affixapi-1.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/PKG-INFO` & `affixapi-1.1.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.72
+Version: 1.1.74
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -360,15 +360,15 @@
  - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyRequest](docs/CurrencyRequest.md)
+ - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
```

### Comparing `affixapi-1.1.72/README.md` & `affixapi-1.1.74/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
  - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyRequest](docs/CurrencyRequest.md)
+ - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
```

### Comparing `affixapi-1.1.72/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.74/affixapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.72
+Version: 1.1.74
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -360,15 +360,15 @@
  - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyRequest](docs/CurrencyRequest.md)
+ - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
```

### Comparing `affixapi-1.1.72/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.74/affixapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 openapi_client/model/compensation_history_no_non_null_request.py
 openapi_client/model/compensation_history_response.py
 openapi_client/model/create_employee_request.py
 openapi_client/model/create_employee_request_bank_account.py
 openapi_client/model/create_employee_request_dependents.py
 openapi_client/model/create_employee_request_emergency_contacts.py
 openapi_client/model/create_employee_request_manager.py
-openapi_client/model/currency_request.py
+openapi_client/model/currency_not_null_request.py
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
 openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
 openapi_client/model/employment_history_no_non_null_request.py
 openapi_client/model/employment_history_response.py
@@ -95,15 +95,15 @@
 test/test_compensation_history_response.py
 test/test_core_api.py
 test/test_create_employee_request.py
 test/test_create_employee_request_bank_account.py
 test/test_create_employee_request_dependents.py
 test/test_create_employee_request_emergency_contacts.py
 test/test_create_employee_request_manager.py
-test/test_currency_request.py
+test/test_currency_not_null_request.py
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
 test/test_employee_response_manager.py
 test/test_employees20230301_response.py
 test/test_employment_history_no_non_null_request.py
 test/test_employment_history_response.py
```

### Comparing `affixapi-1.1.72/openapi_client/__init__.py` & `affixapi-1.1.74/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.74/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/api/core_api.py` & `affixapi-1.1.74/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/api/management_api.py` & `affixapi-1.1.74/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.74/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/api_client.py` & `affixapi-1.1.74/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/apis/__init__.py` & `affixapi-1.1.74/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/configuration.py` & `affixapi-1.1.74/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/exceptions.py` & `affixapi-1.1.74/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.74/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/address_response.py` & `affixapi-1.1.74/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/client_request.py` & `affixapi-1.1.74/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/client_response.py` & `affixapi-1.1.74/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.74/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/company_response.py` & `affixapi-1.1.74/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/compensation_history_no_non_null_request.py` & `affixapi-1.1.74/openapi_client/model/compensation_history_no_non_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
-    from openapi_client.model.currency_request import CurrencyRequest
-    globals()['CurrencyRequest'] = CurrencyRequest
+    from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
+    globals()['CurrencyNotNullRequest'] = CurrencyNotNullRequest
 
 
 class CompensationHistoryNoNonNullRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -54,14 +54,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('pay_frequency',): {
+            'YEAR': "year",
             'WEEKLY': "weekly",
             'BIWEEKLY': "biweekly",
             'SEMIMONTHLY': "semimonthly",
             'MONTHLY': "monthly",
             'OTHER': "other",
         },
         ('employment_type',): {
@@ -91,15 +92,15 @@
         """
         lazy_import()
         return {
             'pay_rate': (float,),  # noqa: E501
             'pay_period': (str,),  # noqa: E501
             'pay_frequency': (str,),  # noqa: E501
             'employment_type': (str,),  # noqa: E501
-            'currency': (CurrencyRequest,),  # noqa: E501
+            'currency': (CurrencyNotNullRequest,),  # noqa: E501
             'effective_date': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -129,15 +130,15 @@
         """CompensationHistoryNoNonNullRequest - a model defined in OpenAPI
 
         Args:
             pay_rate (float):
             pay_period (str):
             pay_frequency (str):
             employment_type (str):
-            currency (CurrencyRequest):
+            currency (CurrencyNotNullRequest):
             effective_date (date):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `affixapi-1.1.72/openapi_client/model/compensation_history_response.py` & `affixapi-1.1.74/openapi_client/model/compensation_history_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('pay_frequency',): {
             'None': None,
+            'YEAR': "year",
             'WEEKLY': "weekly",
             'BIWEEKLY': "biweekly",
             'SEMIMONTHLY': "semimonthly",
             'MONTHLY': "monthly",
             'OTHER': "other",
             'NULL': "null",
         },
```

### Comparing `affixapi-1.1.72/openapi_client/model/create_employee_request.py` & `affixapi-1.1.74/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.74/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.74/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.74/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.74/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/currency_request.py` & `affixapi-1.1.74/openapi_client/model/currency_not_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class CurrencyRequest(ModelSimple):
+class CurrencyNotNullRequest(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -47,15 +47,14 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'None': None,
-            'NULL': "null",
             'USD': "usd",
             'GBP': "gbp",
             'EUR': "eur",
         },
     }
 
     validations = {
@@ -95,23 +94,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CurrencyRequest - a model defined in OpenAPI
+        """CurrencyNotNullRequest - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["null", "usd", "gbp", "eur", ]  # noqa: E501
+            args[0] (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["null", "usd", "gbp", "eur", ]  # noqa: E501
+            value (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.72/openapi_client/model/currency_response.py` & `affixapi-1.1.74/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/disconnect_response.py` & `affixapi-1.1.74/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employee_response.py` & `affixapi-1.1.74/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.74/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.74/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employment_history_no_non_null_request.py` & `affixapi-1.1.74/openapi_client/model/employment_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employment_history_response.py` & `affixapi-1.1.74/openapi_client/model/employment_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employment_status_not_null_not_nullable.py` & `affixapi-1.1.74/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.74/openapi_client/model/employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/employment_status_response.py` & `affixapi-1.1.74/openapi_client/model/employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.74/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/group_response.py` & `affixapi-1.1.74/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.74/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.74/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.74/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/identity_response.py` & `affixapi-1.1.74/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/inline_response400.py` & `affixapi-1.1.74/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/inline_response401.py` & `affixapi-1.1.74/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/inline_response409.py` & `affixapi-1.1.74/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/introspect_response.py` & `affixapi-1.1.74/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.74/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/location_response.py` & `affixapi-1.1.74/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/message_response.py` & `affixapi-1.1.74/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/mode_request.py` & `affixapi-1.1.74/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/mode_response.py` & `affixapi-1.1.74/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payrun_response.py` & `affixapi-1.1.74/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.74/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslip_response.py` & `affixapi-1.1.74/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.74/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.74/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.74/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.74/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.74/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/policy_type_response.py` & `affixapi-1.1.74/openapi_client/model/policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/provider_request.py` & `affixapi-1.1.74/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/provider_response.py` & `affixapi-1.1.74/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/providers_response.py` & `affixapi-1.1.74/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/scopes_request.py` & `affixapi-1.1.74/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/scopes_response.py` & `affixapi-1.1.74/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.74/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.74/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.74/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.74/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/timesheet_response.py` & `affixapi-1.1.74/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.74/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/token_request.py` & `affixapi-1.1.74/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/token_response.py` & `affixapi-1.1.74/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/tokens_response.py` & `affixapi-1.1.74/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.74/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/model_utils.py` & `affixapi-1.1.74/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/openapi_client/models/__init__.py` & `affixapi-1.1.74/openapi_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
 from openapi_client.model.compensation_history_response import CompensationHistoryResponse
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
 from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
-from openapi_client.model.currency_request import CurrencyRequest
+from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.employment_history_no_non_null_request import EmploymentHistoryNoNonNullRequest
 from openapi_client.model.employment_history_response import EmploymentHistoryResponse
```

### Comparing `affixapi-1.1.72/openapi_client/rest.py` & `affixapi-1.1.74/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/setup.py` & `affixapi-1.1.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.72"
+VERSION = "1.1.74"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.72/test/test_2023_03_01_api.py` & `affixapi-1.1.74/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_address_no_non_null_request.py` & `affixapi-1.1.74/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_address_response.py` & `affixapi-1.1.74/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_client_request.py` & `affixapi-1.1.74/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_client_response.py` & `affixapi-1.1.74/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_companies20230301_response.py` & `affixapi-1.1.74/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_company_response.py` & `affixapi-1.1.74/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_compensation_history_no_non_null_request.py` & `affixapi-1.1.74/test/test_compensation_history_no_non_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.currency_request import CurrencyRequest
-globals()['CurrencyRequest'] = CurrencyRequest
+from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
+globals()['CurrencyNotNullRequest'] = CurrencyNotNullRequest
 from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
 
 
 class TestCompensationHistoryNoNonNullRequest(unittest.TestCase):
     """CompensationHistoryNoNonNullRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `affixapi-1.1.72/test/test_compensation_history_response.py` & `affixapi-1.1.74/test/test_compensation_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_core_api.py` & `affixapi-1.1.74/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_create_employee_request.py` & `affixapi-1.1.74/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.74/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_create_employee_request_dependents.py` & `affixapi-1.1.74/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.74/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_create_employee_request_manager.py` & `affixapi-1.1.74/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_currency_request.py` & `affixapi-1.1.74/test/test_currency_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.currency_request import CurrencyRequest
+from openapi_client.model.currency_response import CurrencyResponse
 
 
-class TestCurrencyRequest(unittest.TestCase):
-    """CurrencyRequest unit test stubs"""
+class TestCurrencyResponse(unittest.TestCase):
+    """CurrencyResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrencyRequest(self):
-        """Test CurrencyRequest"""
+    def testCurrencyResponse(self):
+        """Test CurrencyResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CurrencyRequest()  # noqa: E501
+        # model = CurrencyResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.72/test/test_currency_response.py` & `affixapi-1.1.74/test/test_currency_not_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.currency_response import CurrencyResponse
+from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
 
 
-class TestCurrencyResponse(unittest.TestCase):
-    """CurrencyResponse unit test stubs"""
+class TestCurrencyNotNullRequest(unittest.TestCase):
+    """CurrencyNotNullRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrencyResponse(self):
-        """Test CurrencyResponse"""
+    def testCurrencyNotNullRequest(self):
+        """Test CurrencyNotNullRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CurrencyResponse()  # noqa: E501
+        # model = CurrencyNotNullRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.72/test/test_disconnect_response.py` & `affixapi-1.1.74/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employee_response.py` & `affixapi-1.1.74/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employee_response_manager.py` & `affixapi-1.1.74/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employees20230301_response.py` & `affixapi-1.1.74/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employment_history_no_non_null_request.py` & `affixapi-1.1.74/test/test_employment_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employment_history_response.py` & `affixapi-1.1.74/test/test_employment_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employment_status_not_null_not_nullable.py` & `affixapi-1.1.74/test/test_employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employment_status_not_null_request.py` & `affixapi-1.1.74/test/test_employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_employment_status_response.py` & `affixapi-1.1.74/test/test_employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_group_no_null_enum_request.py` & `affixapi-1.1.74/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_group_response.py` & `affixapi-1.1.74/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_groups20230301_response.py` & `affixapi-1.1.74/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.74/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_id_and_message_response.py` & `affixapi-1.1.74/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_identity_response.py` & `affixapi-1.1.74/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_inline_response400.py` & `affixapi-1.1.74/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_inline_response401.py` & `affixapi-1.1.74/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_inline_response409.py` & `affixapi-1.1.74/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_introspect_response.py` & `affixapi-1.1.74/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_location_no_non_null_request.py` & `affixapi-1.1.74/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_location_response.py` & `affixapi-1.1.74/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_management_api.py` & `affixapi-1.1.74/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_message_response.py` & `affixapi-1.1.74/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_mode_request.py` & `affixapi-1.1.74/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_mode_response.py` & `affixapi-1.1.74/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payrun_response.py` & `affixapi-1.1.74/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payruns20230301_response.py` & `affixapi-1.1.74/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslip_response.py` & `affixapi-1.1.74/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslip_response_contributions.py` & `affixapi-1.1.74/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslip_response_deductions.py` & `affixapi-1.1.74/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslip_response_earnings.py` & `affixapi-1.1.74/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslip_response_taxes.py` & `affixapi-1.1.74/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_payslips20230301_response.py` & `affixapi-1.1.74/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_policy_type_response.py` & `affixapi-1.1.74/test/test_policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_provider_request.py` & `affixapi-1.1.74/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_provider_response.py` & `affixapi-1.1.74/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_providers_response.py` & `affixapi-1.1.74/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_scopes_request.py` & `affixapi-1.1.74/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_scopes_response.py` & `affixapi-1.1.74/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_time_off_balance_response.py` & `affixapi-1.1.74/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.74/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.74/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_time_off_entry_response.py` & `affixapi-1.1.74/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_timesheet_response.py` & `affixapi-1.1.74/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_timesheets20230301_response.py` & `affixapi-1.1.74/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_token_request.py` & `affixapi-1.1.74/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_token_response.py` & `affixapi-1.1.74/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_tokens_response.py` & `affixapi-1.1.74/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_work_locations20230301_response.py` & `affixapi-1.1.74/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.72/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.74/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

